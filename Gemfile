source "https://rubygems.org"

gem "jekyll", "~> 4.3"

# Pinned to the sassc-based converter: avoids the sass-embedded/protobuf
# native gem, which fails to load on dev/pre-release Ruby builds. We ship
# plain CSS, so this has no effect on output.
gem "jekyll-sass-converter", "~> 2.0"

# Standard-library gems that Ruby 3.4 dropped from defaults but Jekyll/Liquid
# still require. No-ops on the CI Ruby (3.3), required on newer Rubies.
gem "bigdecimal"
gem "csv"
gem "base64"
gem "logger"

# SEO / discoverability: emits <title>, meta description, Open Graph, Twitter
# Card and JSON-LD tags ({% seo %}); generates sitemap.xml and feed.xml.
group :jekyll_plugins do
  gem "jekyll-seo-tag", "~> 2.8"
  gem "jekyll-sitemap", "~> 1.4"
  gem "jekyll-feed", "~> 0.17"
end
