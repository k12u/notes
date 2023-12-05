# terraform import コマンドの引数指定がめんどい

モジュールを使っているときに、import するコマンドラインはそれなりに複雑になる。

terraform plan すると `module.name.resource.resource_type.resource.name` 形式の出力が得られるので簡単に import のコマンドラインに使える。
