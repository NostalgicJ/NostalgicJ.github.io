# frozen_string_literal: true

source "https://rubygems.org"

# Jekyll 버전을 명시합니다. 4.4.x 버전을 사용하므로 이렇게 지정하면 됩니다.
gem "jekyll", "~> 4.4"

# GitHub Pages의 기본 빌드 시스템을 사용하지 않고,
# 직접 GitHub Actions로 빌드할 것이기 때문에 "github-pages" 젬은 제거하거나 주석 처리해야 합니다.
# gem "github-pages", group: :jekyll_plugins # 이 줄은 삭제하거나 #으로 주석 처리합니다.

# _config.yml에 명시된 모든 플러그인 젬들을 여기에 추가해야 합니다.
# 특히 jekyll-paginate와 jekyll-spaceship은 GitHub Pages가 기본 지원하지 않으므로 필수입니다.
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-paginate" # jekyll-paginate 젬 추가
  gem "jekyll-spaceship" # jekyll-spaceship 젬 추가
end

# Ruby 3.5.0부터 'logger' 경고를 없애려면 이 두 젬을 추가하는 것이 좋습니다.
# 현재 Ruby 3.4.4를 사용 중이시므로 필수적이지는 않지만, 미래를 위해 추가하는 것을 권장합니다.
gem 'bigdecimal'
gem 'logger'
gem 'ostruct'

# `gemspec`은 Jekyll 테마 개발 시 사용됩니다.
# 만약 당신의 프로젝트가 테마 자체가 아니라 일반 Jekyll 사이트라면 이 줄은 필요 없을 수 있습니다.
# 하지만 현재 오류와는 무관하므로 그대로 두셔도 됩니다.
gemspec