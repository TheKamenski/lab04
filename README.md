# lab04

# 
```sh
❯ export GITHUB_USERNAME=TheKamenski

❯ export GITHUB_TOKEN=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

                              
❯ cd ${GITHUB_USERNAME}/workspace

❯ pushd .
~/TheKamenski/workspace ~

❯ source scripts/activate
```

```sh
  ~ ❯  source scripts/activate
  ~ ❯ cat > .travis.yml <<EOF
language: cpp
EOF
  ~ ❯ 
  ~ ❯ cat >> .travis.yml <<EOF

script:
- cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
- cmake --build _build
- cmake --build _build --target install
EOF
  ~ ❯ 
  ~ ❯  cat >> .travis.yml <<EOF

addons:
  apt:
    sources:
      - george-edison55-precise-backports
    packages:
      - cmake
      - cmake-data
EOF

```


```sh
  ~ ❯ sudo gem install travis
Fetching net-http-pipeline-1.0.1.gem
Successfully installed net-http-pipeline-1.0.1
Fetching connection_pool-2.4.1.gem
Successfully installed connection_pool-2.4.1
Fetching net-http-persistent-4.0.2.gem
Successfully installed net-http-persistent-4.0.2
Fetching multi_json-1.15.0.gem
Successfully installed multi_json-1.15.0
Fetching ffi-1.16.3.gem
Building native extensions. This could take a while...
ERROR:  Error installing travis:
	ERROR: Failed to build gem native extension.

    current directory: /usr/local/share/gems/gems/ffi-1.16.3/ext/ffi_c
/usr/bin/ruby -I/usr/share/rubygems extconf.rb
mkmf.rb can't find header files for ruby at /usr/share/include/ruby.h

You might have to install separate package for the ruby development
environment, ruby-dev or ruby-devel for example.
extconf failed, exit code 1

Gem files will remain installed in /usr/local/share/gems/gems/ffi-1.16.3 for inspection.
Results logged to /usr/local/lib64/gems/ruby/ffi-1.16.3/gem_make.out


❯ git add .travis.yml
[main 8779727] added CI
 1 file changed, 14 insertions(+)
 create mode 100644 .travis.yml
 
 ❯ git push origin main
Перечисление объектов: 28, готово.
Подсчет объектов: 100% (28/28), готово.
При сжатии изменений используется до 12 потоков
Сжатие объектов: 100% (19/19), готово.
Запись объектов: 100% (28/28), 8.71 КиБ | 4.35 МиБ/с, готово.
Total 28 (delta 4), reused 24 (delta 3), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), done.
To github.com:TheKamenski/tp-lab04.git
 * [new branch]      main -> main

```
