# Sugar Releases

## [Unreleased]
### Added
* [#155](https://github.com/satyan/sugar/issues/155) @benohalloran adding Cursors for Cursor Adapters [Pull 312](https://github.com/satyan/sugar/pull/312)


## v1.4
### Added
* [#306](https://github.com/satyan/sugar/pull/306) @Shyish return boolean/integer on delete methods
* [#304](https://github.com/satyan/sugar/pull/304) @benohalloran add support to enum type
* [#197](https://github.com/satyan/sugar/pull/197) @andresteves add suport for bytes[]
* [#293](https://github.com/satyan/sugar/pull/293) @neilw4 support NULL in queries
* [#273](https://github.com/satyan/sugar/pull/273) @dominicwong617 findById support an array of ids
* [#246](https://github.com/satyan/sugar/pull/246) @kwf2030 use sqlite\_master to check whether table already exist
* [#253](https://github.com/satyan/sugar/pull/202) @JeroenMols add bulk delete
* [#285](https://github.com/satyan/sugar/pull/202) @Shyish add listAll with orderBy param
* No need to extend SugarApp - just call SugarContext.init(Context) instead
* [#129](https://github.com/satyan/sugar/pull/129) @satyan support sugar entities using @Table annotations

### Fixed
* [#314](https://github.com/satyan/sugar/pull/314) @abscondment fix StrictMode DexFile
* [#303](https://github.com/satyan/sugar/pull/303) @RossinesP fixed saving row string bug
* [#258](https://github.com/satyan/sugar/pull/258) @nosrak113 change SugarRecord ID to private to not conflit with other libraries
* [#254](https://github.com/satyan/sugar/pull/254) @jivimberg use weak keys to keep track of annotated entities
* [#215](https://github.com/satyan/sugar/issues/215) @jivimberg fix bug persisting relationship
* [#185](https://github.com/satyan/sugar/issues/185) [#243](https://github.com/satyan/sugar/issues/243) @whoshuu fix save and update method
* [#202](https://github.com/satyan/sugar/pull/202) @allieus improve getDomainsClass()
* [#104](https://github.com/satyan/sugar/issues/104) @whoshuu fix nesting "and" and "or"

## v1.4 Beta [[jar](https://github.com/satyan/sugar/releases/download/v1.4_beta/sugar-1.4_beta.jar)]
### Added
* [#112](https://github.com/satyan/sugar/pull/112) @androdevcafe added Unique and NotNull annotations
* [#78](https://github.com/satyan/sugar/pull/78) @HiddenCleverde capability to specify primary key

### Fixed
* [#113](https://github.com/satyan/sugar/pull/113) @whoshuu override findById to support int
* [#106](https://github.com/satyan/sugar/issues/106) @whoshuu add documentation to onTerminate
* [#54](https://github.com/satyan/sugar/issues/54) @whoshuu simplify count interface
* [#43](https://github.com/satyan/sugar/issues/43) @whoshuu return id on save
* [#72](https://github.com/satyan/sugar/issues/72) @whoshuu allow null values to Date and Calendar objects
* [#96](https://github.com/satyan/sugar/issues/96) @whoshuu roboeletric fallback

## v1.3 [[jar](https://github.com/satyan/sugar/releases/download/v1.3/sugar-1.3.jar)]

- Transaction Support
- Bulk Insert of records 
- Encrypted datastore (branch : sugar-cipher using sqlcipher)
- Removed Constructor with context parameter. Needs default constructor now.
- Enhancements to QueryBuilder
- Bug fixes and other improvements.

## v1.2 [[jar](https://github.com/satyan/sugar/releases/download/v1.2/sugar-1.2.jar)]

- package restriction for domain classes.
- metadata caching
- QueryBuilder v1
- Database Migrations
- Provision for Raw queries
- Better and more organized api guide and usage instructions.

## v1.1 [[jar](https://github.com/satyan/sugar/releases/download/v1.1/sugar-1.1.jar)]

- Static api doesn't take context anymore. Hence

```java
Book.findById(context, Book.class, 1);
```

becomes

```java
Book.findById(Book.class, 1);
```

- Some cleanup in the code.