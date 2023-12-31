# Grace Web Profile

[![Build Status](https://github.com/grace-profiles/web-bootstrap/workflows/Grace%20CI/badge.svg)](https://github.com/grace-profiles/web-bootstrap/actions)

A profile for creating standard Grace web applications, with popular CSS framework **Bootstrap**.

## Grace Version

- Grails **2022.0.0**
- Grails Base Profile **2022.0.0**
- Grails Scaffolding Plugin **5.0.0**
- Grails Fields Plugin **5.0.0**

## Usage

### Build Profile

```
git clone https://github.com/grace-profiles/web-bootstrap.git
cd web-bootstrap
./gradlew publishToMavenLocal
```

### Create App

#### Use Bootstrap CSS

Generated project with default features, included `hibernate5`, `events`, `geb2`, `gsp`, `asset-pipeline`, `fields`, `jquery`, `bootstrap`.

```
grails create-app --profile org.graceframework.profiles:web-bootstrap:2022.0.0-SNAPSHOT org.graceframework.demo.web-bootstrap-demo
cd web-bootstrap-demo
grails run-app
```

#### Use Bootstrap with SASS and NPM

Generated project with features, included `hibernate5`, `events`, `geb2`, `gsp`, `asset-pipeline`, `fields`, `jquery`, `bootstrap-sass`.

```
grails create-app --profile org.graceframework.profiles:web-bootstrap:2022.0.0-SNAPSHOT --features hibernate5,events,geb2,jquery,bootstrap-sass org.grails.demo.web-bootstrap-sass-demo
cd web-bootstrap-sass-demo
npm install
npm run build
grails run-app
```

## What's New

### 2022.0.0-SNAPSHOT

* Update Bootstrap v5.1.3, Popper 2.10.2
* Update jQuery 3.6.0, Bootstrap 4.6.1
* Update Grails Scaffolding and Fields default templates
* Support Bootstrap form component, powerful grid system and responsive layout
* Update Bootstrap Icons v1.8.1

* Support Bootstrap with SASS and NPM
* Support Bootswatch themes
* Add Bootstrap taglib, support paginate and datePicker with more options
* Add messages_zh_CN.properties and messages_zh_TW.properties
* Default main layout support load javascript by convention
* Add Languages menu
* Add Management menu
* Add Themes menu
* Remove unsed css in main.css and grails.css
* Remove unsed skin images
* Feature `popper` is optional now, Use `bootstrap.bundle.js` include it
* Support Bootstrap SASS, Use [DartSass](https://sass-lang.com/dart-sass) in place of [Node Sass](https://sass-lang.com/blog/libsass-is-deprecated)


## Links

- [Grace Framework](https://github.com/graceframework/grace-framework)
- [Grace Web Bootstrap Profile](https://github.com/grace-profiles/web-bootstrap)
- [Bootstrap](https://getbootstrap.com)
- [Bootstrap npm starter](https://github.com/twbs/bootstrap-npm-starter)
- [Bootswatch](https://bootswatch.com)
- [jQuery](https://jquery.com)
- [Popper](https://popper.js.org)