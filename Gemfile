# frozen_string_literal: true

source "https://rubygems.org"

DECIDIM_VERSION = "0.27"
DECIDIM_BRANCH = "release/#{DECIDIM_VERSION}-stable".freeze

ruby RUBY_VERSION

# Core gems
gem "decidim", "~> #{DECIDIM_VERSION}.0"
gem "decidim-conferences", "~> #{DECIDIM_VERSION}.0"
gem "decidim-initiatives", "~> #{DECIDIM_VERSION}.0"
gem "decidim-templates", "~> #{DECIDIM_VERSION}.0"

# External Decidim gems
gem "decidim-budget_category_voting", git: "https://github.com/alecslupu-pfa/decidim-budget_category_voting.git", branch: DECIDIM_BRANCH
gem "decidim-cache_cleaner"
gem "decidim-category_enhanced", "~> 0.0.1"
gem "decidim-decidim_awesome"
gem "decidim-extended_socio_demographic_authorization_handler", git: "https://github.com/OpenSourcePolitics/decidim-module-extended_socio_demographic_authorization_handler.git",
                                                                branch: DECIDIM_BRANCH
gem "decidim-extra_user_fields", git: "https://github.com/OpenSourcePolitics/decidim-module-extra_user_fields.git", branch: "release/0.27-stable"
gem "decidim-friendly_signup", git: "https://github.com/OpenSourcePolitics/decidim-module-friendly_signup.git"
gem "decidim-gallery", git: "https://github.com/OpenSourcePolitics/decidim-module-gallery.git", branch: "fix/nokogiri_deps"
gem "decidim-homepage_interactive_map", git: "https://github.com/OpenSourcePolitics/decidim-module-homepage_interactive_map.git", branch: DECIDIM_BRANCH
gem "decidim-ludens", git: "https://github.com/OpenSourcePolitics/decidim-ludens.git", branch: DECIDIM_BRANCH
gem "decidim-phone_authorization_handler", git: "https://github.com/OpenSourcePolitics/decidim-module_phone_authorization_handler", branch: "chore/update-initializer"
gem "decidim-spam_detection"
gem "decidim-survey_multiple_answers", git: "https://github.com/OpenSourcePolitics/decidim-module-survey_multiple_answers"
gem "decidim-term_customizer", git: "https://github.com/OpenSourcePolitics/decidim-module-term_customizer.git", branch: "fix/email_with_precompile"

# Omniauth gems
gem "omniauth-france_connect", git: "https://github.com/OpenSourcePolitics/omniauth-france_connect"
gem "omniauth-publik", git: "https://github.com/OpenSourcePolitics/omniauth-publik"

# Default
gem "activejob-uniqueness", require: "active_job/uniqueness/sidekiq_patch"
gem "activerecord-session_store"
gem "aws-sdk-s3", require: false
gem "bootsnap", "~> 1.4"
gem "deepl-rb", require: "deepl"
gem "deface"
gem "dotenv-rails", "~> 2.7"
gem "faker", "~> 2.14"
gem "fog-aws"
gem "foundation_rails_helper", git: "https://github.com/sgruhier/foundation_rails_helper.git"
gem "letter_opener_web", "~> 1.3"
gem "nokogiri", "1.13.4"
gem "omniauth-rails_csrf_protection", "~> 1.0"
gem "puma", ">= 5.5.1"
gem "rack-attack", "~> 6.6"
gem "sys-filesystem"
gem "wicked_pdf", "2.6.3"

group :development do
  gem "listen", "~> 3.1"
  gem "rubocop-faker"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "4.0.4"
end

group :development, :test do
  gem "brakeman", "~> 5.1"
  gem "byebug", "~> 11.0", platform: :mri
  gem "climate_control", "~> 1.2"
  gem "decidim-dev", "~> #{DECIDIM_VERSION}.0"
  gem "parallel_tests"
end

group :production do
  gem "dalli"
  gem "health_check", "~> 3.1"
  gem "lograge"
  gem "sendgrid-ruby"
  gem "sentry-rails"
  gem "sentry-ruby"
  gem "sentry-sidekiq"
  gem "sidekiq", "~> 6.0"
  gem "sidekiq-scheduler", "~> 5.0"
end
