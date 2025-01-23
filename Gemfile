# frozen_string_literal: true

source "https://rubygems.org"

# Тема
gem "jekyll-theme-chirpy", "~> 6.2", ">= 6.2.2"

# Явно указываем сам Jekyll (версия 4.3+)
gem "jekyll", "~> 4.3"

# Для Ruby 3.4+ отдельные библиотеки больше не идут «из коробки»
gem "csv"      # уже добавляли
gem "base64"   # нужно для safe_yaml
gem "logger"   # чтобы предупредить будущие проблемы

group :test do
  gem "html-proofer", "~> 4.4"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

platforms :jruby do
  gem "http_parser.rb", "~> 0.6.0"
end

if RUBY_PLATFORM =~ /linux-musl/
  gem "jekyll-sass-converter", "~> 2.0"
end