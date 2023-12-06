# terraform: 強制的に再作成

## 問題
たまに、本来リソースを再作成する必要があるのに、terraform provider の実装のクセにより、 update in-place と判定されて update に失敗する場合がある

## 解決方法
terraform taint [resource.address] すると次回の apply 時に再作成となる。

