# angular2-jasmine


### Visual Studio 2015 をインストール

Visual Studio Community 2015
https://www.visualstudio.com/downloads/download-visual-studio-vs


### Python をインストール

Python.org 2.7.10
https://www.python.org/downloads/release/python-2710/

Windows x86-64 MSI installer

実行ファイル
python-2.7.10.amd64.msi


### Cygwin-64bitのインストール

Cygwin

https://www.cygwin.com/

インストーラをダウンロードして実行する。
https://www.cygwin.com/setup-x86_64.exe

実行ファイル
setup-x86_64.exe



### Node.js、npmのインストール

Node.js
https://nodejs.org/

インストーラをダウンロードして実行する。
DOWNLOADS > Windows Installer (.msi) 64-bit

実行ファイル
node-v0.12.7-x64.msi

$ node -v
v0.12.7



### Github or GitLab

- レポジトリの作成
- レポジトリのクローン


### プロジェクトをクローン

```
$ cd $HOME/hayakawa/project_fa_2015/develop/projects

$ git clone https://github.com/hayao56/angular2-jasmine.git
$ cd $HOME/hayakawa/project_fa_2015/develop/projects/angular2-jasmine
```


### Gulp のインストール

```
$ npm install -g gulp

C:\Users\g-hayakawa\AppData\Roaming\npm\gulp -> C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\gulp\bin\gulp.js
gulp@3.9.0 C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\gulp
├── pretty-hrtime@1.0.0
├── interpret@0.6.5
├── deprecated@0.0.1
├── archy@1.0.0
├── tildify@1.1.0 (os-homedir@1.0.1)
├── minimist@1.1.2
├── v8flags@2.0.10 (user-home@1.1.1)
├── chalk@1.1.0 (escape-string-regexp@1.0.3, supports-color@2.0.0, ansi-styles@2.1.0, has-ansi@2.0.0, strip-ansi@3.0.0)
├── semver@4.3.6
├── orchestrator@0.3.7 (sequencify@0.0.7, stream-consume@0.1.0, end-of-stream@0.1.5)
├── liftoff@2.1.0 (extend@2.0.1, rechoir@0.6.2, flagged-respawn@0.3.1, resolve@1.1.6, findup-sync@0.2.1)
├── gulp-util@3.0.6 (array-uniq@1.0.2, array-differ@1.0.0, lodash._reevaluate@3.0.0, lodash._reescape@3.0.0, lodash._reinterpolate@3.0.0, beeper@1.1.0, object-assign@3.0.0, replace-ext@0.0.1, vinyl@0.5.0, lodash.template@3.6.2, through2@2.0.0, multipipe@0.1.2, dateformat@1.0.11)
└── vinyl-fs@0.3.13 (graceful-fs@3.0.8, strip-bom@1.0.0, defaults@1.0.2, vinyl@0.4.6, mkdirp@0.5.1, through2@0.6.5, glob-stream@3.1.18, glob-watcher@0.0.6)
```


### Karma x Jasmine

#### What is Karma?

node.jsで作成されたテスト実行環境

#### What is Jasmine?

テストの実処理を行うライブラリ


#### 1. karma コマンドを使う関係上、 -g オプションを付けてインストールします。

```
$ npm install -g karma-cli

C:\Users\g-hayakawa\AppData\Roaming\npm\karma -> C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\karma-cli\bin\karma
karma-cli@0.1.0 C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\karma-cli
└── resolve@1.1.6

```


#### 2. Karma から Jasmine を利用するプラグインをインストール

```
$ npm install --save-dev karma-jasmine

npm WARN peerDependencies The peer dependency jasmine-core@* included from karma-jasmine will no
npm WARN peerDependencies longer be automatically installed to fulfill the peerDependency
npm WARN peerDependencies in npm 3+. Your application will need to depend on it explicitly.
jasmine-core@2.3.4 node_modules\jasmine-core

karma-jasmine@0.3.6 node_modules\karma-jasmine
```


#### 3. テスト実行時に Web ブラウザを起動するためのプラグインをインストール

```
$ npm install --save-dev karma-chrome-launcher

karma-chrome-launcher@0.2.0 node_modules\karma-chrome-launcher
├── fs-access@1.0.0 (null-check@1.0.0)
└── which@1.1.1 (is-absolute@0.1.7)

```
  
  
#### 4. Karma のインストール
```
$ npm install --save-dev karma
```
 

#### 5. Karma を初期化して設定ファイルを作成


gyp ERR! stack Error: Can't find "msbuild.exe". Do you have Microsoft Visual Studio C++ 2008+ installed?



```
$ npm install -g npm

C:\Users\g-hayakawa\AppData\Roaming\npm\npm -> C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\npm\bin\npm-cli.js
npm@2.13.2 C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\npm
```

```
$ npm install -g node-gyp

C:\Users\g-hayakawa\AppData\Roaming\npm\node-gyp -> C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\node-gyp\bin\node-gyp.js
node-gyp@2.0.2 C:\Users\g-hayakawa\AppData\Roaming\npm\node_modules\node-gyp
├── graceful-fs@3.0.8
├── osenv@0.1.3 (os-homedir@1.0.1, os-tmpdir@1.0.1)
├── nopt@3.0.3 (abbrev@1.0.7)
├── which@1.1.1 (is-absolute@0.1.7)
├── minimatch@1.0.0 (sigmund@1.0.1, lru-cache@2.6.5)
├── semver@4.3.6
├── fstream@1.0.7 (inherits@2.0.1)
├── mkdirp@0.5.1 (minimist@0.0.8)
├── path-array@1.0.0 (array-index@0.1.1)
├── tar@1.0.3 (inherits@2.0.1, block-stream@0.0.8)
├── npmlog@1.2.1 (ansi@0.3.0, gauge@1.2.2, are-we-there-yet@1.0.4)
├── glob@4.5.3 (inherits@2.0.1, once@1.3.2, inflight@1.0.4, minimatch@2.0.10)
├── rimraf@2.4.2 (glob@5.0.14)
└── request@2.60.0 (aws-sign2@0.5.0, forever-agent@0.6.1, stringstream@0.0.4, caseless@0.11.0, oauth-sign@0.8.0, tunnel-agent@0.4.1, isstream@0.1.2, json-stringify-safe@5.0.1, extend@3.0.0, node-uuid@1.4.3, combined-stream@1.0.5, qs@4.0.0, mime-types@2.1.3, form-data@1.0.0-rc3, http-signature@0.11.0, bl@1.0.0, tough-cookie@2.0.0, hawk@3.1.0, har-validator@1.8.0)
```
