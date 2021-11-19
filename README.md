模板主题 https://github.com/showzeng/Minimalism

# 如何本地运行？

环境：ruby 2.7.1p83

jekyll安装：`gem install jekyll bundler`

包导入：`bundle install`

启动：`bundle exec jekyll serve`

问题：

- sass文件报编码错误
  1. 进入路径`{ruby安装路径}\lib\ruby\gems\2.7.0\gems\sass-3.7.4\lib`
  2. 找到文件`sass.rb`
  3. 文件最后添加`Encoding.default_external = Encoding.find('utf-8')`
