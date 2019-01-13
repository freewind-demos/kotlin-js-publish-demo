Kotlin JS Publish Demo
======================

这个例子没有完成，以下命令报错：

```
cd generated
npm install
npm run start
```

其它的也没有好好检查。等再用到kotlin-js的时候，再来完善这个demo。

---

Kotlin-Js project, also publish to jcenter/bintray and npm.

Modify names when copy this project
-----------------------------------

- `README.md`
- `build.gradle`
- `generated/package.json`

Modify version before publishing
--------------------------------

- `README.md`
- `build.gradle`
- `generated/package.json`

Publish
-------

to maven local:

```
./gradlew install
```

to bintray:

```
./gradlew bintrayUpload
```

to npm:

```
cd generated
npm publish
```

Use
---

To use in `build.gradle`:

```
repositories {
    maven {
        url 'https://dl.bintray.com/freewind/maven/'
    }
}

dependencies {
    compile 'freewind.github.com:kotlin-js-publish-demo:0.1.0'
}
```

Also npm:

```
npm install --save kotlin-js-publish-demo
```

