# Test

`docker build .`

# Checklist

- [x] 除外されるパスの指定は .dockerignore が置かれたディレクトリからの相対パスであること
    - foo/include/ が除外されないこと
- [x] 先頭に `**` をつければ、ネストしたディレクトリも除外されること
    - foo/nest/ が除外されること
