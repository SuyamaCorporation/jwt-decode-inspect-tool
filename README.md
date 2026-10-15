# JWT Token Decoder & Inspector

## 概要
JWTをテキストエリアにペーストするとheader/payload/signatureをJSONフォーマットで表示し、exp/iatクレームを現在時刻と比較して有効/期限切れを色分け表示する。

## 機能
- JWT 3部構造の色分け表示（赤=header/緑=payload/青=signature）
- header・payloadのBase64URLデコードとJSON表示
- exp（有効期限）の検証と残り時間表示
- iat（発行時刻）・nbf（有効開始時刻）の表示
- 標準クレーム（sub/iss/aud等）のハイライト
- サンプルJWTのロード機能

## 使い方
JWTトークンをテキストエリアに貼り付けると自動的にデコードされます。「Load Sample」でサンプルJWTを読み込めます。本番環境のトークンは貼り付けないでください。
