# terraform import コマンドの引数指定がめんどい

## 問題
モジュールを使っているときに、import するコマンドラインはそれなりに複雑になる。

## 解決方法
terraform plan すると `module.name.resource.resource_type.resource.name` 形式の出力が得られるので簡単に import のコマンドラインに使える。
