# frozen_string_literal: true

source "https://rubygems.org"

# === DÁN ĐÚNG NHỮNG DÒNG NÀY ĐỂ KHÔNG CẦN TẢI ONLINE NỮA ===
# Phiên bản GitHub Pages mới nhất (cập nhật tháng 12/2025)
GITHUB_PAGES_VERSIONS = {
  "jekyll"                       => "3.10.0",
  "github-pages"                 => "232",
  "jekyll-sass-converter"        => "1.5.2",
  "kramdown"                     => "2.4.0",
  "kramdown-parser-gfm"          => "1.1.0",
  "jekyll-commonmark-ghpages"    => "0.5.1",
  "liquid"                       => "4.0.4",
  "rouge"                        => "3.30.0",
  "jekyll-theme-minimal"         => "0.2.0"   # Theme bạn đang dùng
}.freeze

# === Các gem chính ===
gem "github-pages", GITHUB_PAGES_VERSIONS["github-pages"]
gem "jekyll", GITHUB_PAGES_VERSIONS["jekyll"]
gem "jekyll-theme-minimal", GITHUB_PAGES_VERSIONS["jekyll-theme-minimal"]

# === Các plugin thường dùng trong repo này (đều có trong github-pages rồi) ===
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
end

# Windows & JRuby fixes (giữ nguyên để tránh lỗi trên Windows)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
  gem "wdm", "~> 0.1.1" if Gem.win_platform?
end