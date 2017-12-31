# Test

`docker build .`

# Checklist

- [x] ファイルサイズが小くなること
- [x] イメージが更新されても、後続のイメージのキャッシュは有効であること
    - main.go が更新されても foo.txt のコピーはスキップされること
