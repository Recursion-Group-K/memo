# FileTree

```
./
  |- src/
    |- assets/
    |- components/
    |- pages/
    |- router/
    |- store/
    |- models/
    |- utils/
    |- api/
    |- App.vue
    |- main.js
  |- tests/
    |- unit
```

※ 実際のディレクトリのソートはちょっと違うはずです。
## src
アプリケーションのソースコードを管理します。

### src/Assets

css image svg など

### src/Components

ページ内で使う部品を管理するフォルダです。ヘッダーやフッター、サイドバーやもっと細かくボタンコンポーネントなどがあっても問題ないです。
ただし、使わないコンポーネントになってしまった場合は確認をとって削除させていただきます🙏
.vue拡張子

### src/Pages

アプリケーションのページを管理するフォルダです。Conponentsフォルダ内の部品の寄せ集めで作れるのがベストですが、直にhtmlを書いても問題はないです。
.vue拡張子

### src/Rotuer

ルーティングを設定するファイルを管理します。

### src/Store

Vuex Storeを管理します。mutations actions などが肥大化する場合はむモジュール分割しながら管理します。

### src/Models

モデルを管理するページです。 constructorはオブジェクトを引数として受け取ります。

### src/utils

アプリケーション内で使う関数やクラスを管理します。
例: getLocalTime(), 

### src/api
API通信をして受け取ったデータからモデルを作成するラッパー関数やラッパークラスを管理します。

## tests
テストファイルを管理します。jestを使っているので、  拡張子は .spec.js にしてください。

## tests/unit
ユニットテストファイルを管理します。



# ファイル名について
ファイル名の付け方についてチームで共通の認識を持っておかないといけないです。

- .vue拡張子 => 大文字から始まるキャメルケース => Home.vue, SignUp.vue
- .js拡張子 => 小文字から始まるキャメルケース => user.js, superUser.js
