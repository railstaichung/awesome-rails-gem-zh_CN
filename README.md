# Awesome Rails Gem zh-TW [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
Awesome Rails Gem 中文版

熟悉大牛們寫的 gem，不用重複造輪子，將更多的精力放到更有意義的事情上。

* [目錄](#目錄)
  * [用戶](#用戶)
  * [模型](#模型)
  * [插件](#插件)
  * [API](#api)
  * [郵件](#郵件)
  * [文件上傳](#文件上傳)
  * [搜索](#搜索)
  * [定時任務](#定時任務)
  * [視圖](#視圖)
  * [環境變量](#環境變量)
  * [後臺管理](#後臺管理)
  * [日誌](#日誌)
  * [調試](#調試)
  * [代碼風格](#代碼風格)
  * [測試](#測試)
  * [安全](#安全)
  * [生產](#生產)
  * [錯誤日誌](#錯誤日誌)
  * [資源管道](#資源管道)

## 用戶

### 認證
* [Devise](https://github.com/plataformatec/devise/) - 用於快速構建用戶功能，如：註冊，登陸，個人設置，找回密碼...
* [Knock](https://github.com/nsarno/knock) - 符合 JWT (JSON Web Token) 規範的認證 API
* [Clearance](https://github.com/thoughtbot/clearance) - 基於郵箱密碼認證
* [Devise token auth](https://github.com/lynndylanhurley/devise_token_auth) - 基於 Token 認證的 JSON API

### 授權
* [Pundit](https://github.com/elabs/pundit) - Pundit 提供一系列方法來擴展 Ruby 的基本類和物件導向的設計模式，用以構建簡單、強壯、可伸縮的認證系統
* [cancancan](https://github.com/CanCanCommunity/cancancan) - 擴展 CanCan，可以規定某個用戶擁有哪些資源，所有權限都定義在一個單獨的地方( Ability 類)
* [rolify](https://github.com/RolifyCommunity/rolify) - 角色管理
* [acl9](https://github.com/be9/acl9/) - 基於角色的認證系統，並且提供簡潔的 DSL


### Omniauth
* [omniauth-facebook](https://github.com/mkdynamic/omniauth-facebook)
* [omniauth-google-oauth2](https://github.com/zquestz/omniauth-google-oauth2)
* [omniauth-weibo-oauth2](https://github.com/beenhero/omniauth-weibo-oauth2)
* [omniauth-twitter](https://github.com/arunagw/omniauth-twitter)
* [omniauth-github](https://github.com/intridea/omniauth-github)
* [omniauth-linkedin-oauth2](https://github.com/decioferreira/omniauth-linkedin-oauth2)

## 模型
* [Enumerize](https://github.com/brainspec/enumerize) - 適用枚舉類型的屬性，支持 i18n 、activerecord、mongoid，並可以集成到 Simple Form
* [counter_culture](https://github.com/magnusvk/counter_culture) - 計數緩存
* [custom_counter_cache](https://github.com/cedric/custom_counter_cache) - 簡單的自定義技術緩存，可以在 model間共用
* [Sequenced](https://github.com/djreimer/sequenced) - 管理 排序性 id 的 gem
* [FriendlyId](https://github.com/norman/friendly_id) - URL 友好的 ID
* [AASM](https://github.com/aasm/aasm) - 狀態機
* [PaperTrail](https://github.com/airblade/paper_trail) - 記錄版本、審計用的，記錄數據的變化
* [paranoia](https://github.com/rubysherpas/paranoia) - 假刪除
* [Validates](https://github.com/kaize/validates) - 提供一系列有用的自定義驗證，包括Email, Url, Slug, Money, Ip, AssociationLength, AbsolutePath, UriComponent, Color, Ean
* [globalize](https://github.com/globalize/globalize) - 數據翻譯中的 i18n 庫
* [deep_cloneable](https://github.com/moiristo/deep_cloneable) - 深度拷貝、支持關係拷貝、可選拷貝
* [social_shares](https://github.com/Timrael/social_shares) - 檢查 url 在社交網絡中的共享次數
* [public_activity](https://github.com/chaps-io/public_activity) - 活動追蹤，類似 github的 Public Activity
* [goldiloader](https://github.com/salsify/goldiloader) - activerecode 預加載，用來減少數據庫查詢次數
* Tagging
  * [ActsAsTaggableOn](https://github.com/mbleigh/acts-as-taggable-on) - 打標記
  * [closure_tree](https://github.com/mceachen/closure_tree) - 多層級標記

## 插件
* [Spreadsheet](https://github.com/zdavatz/spreadsheet) - 讀寫 Spreadsheet 文檔
* [Chartkick](https://github.com/ankane/chartkick) - 用一行 ruby 代碼創建漂亮的 js 圖表
* [kaminari](https://github.com/amatsuda/kaminari) - 很火的分頁插件
* [CKEditor](https://github.com/galetahub/ckeditor) - 所見即所得編輯器
* [HTML::Pipeline](https://github.com/jch/html-pipeline) - html 處理器
* [Slack Notifier](https://github.com/stevenosloan/slack-notifier) 給 slack 發通知
* [Rails ERD](https://github.com/voormedia/rails-erd) - 生成實體關係圖
* [Parity](https://github.com/thoughtbot/parity) - 為 heroku 提供 shell 命令
* [Airbrussh](https://github.com/mattbrictson/airbrussh) - 美化 SSHKit 和 Capistrano 的輸出內容

## API
* [Grape](https://github.com/ruby-grape/grape) - 提供 REST-ful APIs
* [ActiveModel::Serializers](https://github.com/rails-api/active_model_serializers) - 通過配置方便生成 JSON
* [Jbuilder](https://github.com/rails/jbuilder) - 提供 DSL 來定義 JSON 結構
* [rest-client](https://github.com/rest-client/rest-client) - HTTP 和 REST 客戶端
* [has_scope](https://github.com/plataformatec/has_scope) - 在 controller 中使用named scopes
* Documentation
  * [Grape Swagger](https://github.com/ruby-grape/grape-swagger) - 為 Grape API 自動生成文檔
  * [Grape Swagger UI](https://github.com/swagger-api/swagger-ui) - Grape Swagger 的界面
  * [apiary](https://apiary.io/) - [收費]團隊協作工具，一起設計、原型、文檔和測試 API
  * [apiblueprint](https://apiblueprint.org) - API 文檔

## 郵件
* [letter_opener](https://github.com/ryanb/letter_opener) - 在瀏覽器中預覽郵件，而不用真實的發送

## 文件上傳
* [Carrierwave](https://github.com/carrierwaveuploader/carrierwave) - 為 Rails, Sinatra 等框架負責文件上傳，很流行
  * [carrierwave_backgrounder](https://github.com/lardawge/carrierwave_backgrounder) - 分流圖片處理、並且在後臺存儲，用 Delayed Job, Resque, Sidekiq 等
  * [CarrierWave Crop](https://github.com/kirtithorat/carrierwave-crop/) - 裁剪上傳的圖片
  * [CarrierWave ImageOptimizer](https://github.com/jtescher/carrierwave-imageoptimizer) - 優化上傳的圖片
* [remotipart](https://github.com/JangoSteve/remotipart) - Rails jQuery 上傳控件
* [MiniMagick](https://github.com/minimagick/minimagick) - ImageMagick/GraphicsMagick 的 ruby 包裝
* [fog](https://github.com/fog/fog) - 雲服務管理
* [refile](https://github.com/refile/refile) - 流行的上傳庫
* [Paperclip](https://github.com/thoughtbot/paperclip) - ActiveRecord 附件管理
* [Dragonfly](http://markevans.github.io/dragonfly) -  on-the-fly 上傳工具

## 搜索
* [ransack](https://github.com/activerecord-hackery/ransack) - 可以創建簡單或複雜的搜索表單
* [elasticsearch-rails](https://github.com/elastic/elasticsearch-rails) - 集成 Elasticsearch
* [Chewy](https://github.com/toptal/chewy) - 高度集成 Elasticsearch
* [Chewy_Kiqqer](https://github.com/averell23/chewy_kiqqer) - [不再維護]
* [pg_search](https://github.com/Casecommons/pg_search) - 充分利用 postgres 的優勢
* [sunspot](https://github.com/sunspot/sunspot) - 與 Solr 集成
* [searchkick](https://github.com/ankane/searchkick) - 集成 Elasticsearch

## 定時任務
* [Whenever](https://github.com/javan/whenever) - 定時任務
* [Resque](https://github.com/resque/resque) - 基於 Redis 的後臺延時處理任務
* [Rufus-Scheduler](https://github.com/jmettraux/rufus-scheduler) - 又一個定時任務
* [Delayed Job](https://github.com/collectiveidea/delayed_job) -  基於數據庫的後臺延時處理任務
* [Sidekiq](https://github.com/mperham/sidekiq) - 後臺延時處理任務
  * [sidetiq](https://github.com/tobiassvn/sidetiq) - Sidekiq 的循環任務
  * [sidekiq-cron](https://github.com/ondrejbartas/sidekiq-cron) - Sidekiq 的又一個循環任務
  * [sidekiq-scheduler](https://github.com/Moove-it/sidekiq-scheduler) -  Sidekiq 的又一個循環任務
* [Sucker Punch](https://github.com/brandonhilkert/sucker_punch) - 後臺延時處理任務，不需要額外進程

## 視圖
* [formtastic](https://github.com/justinfrench/formtastic) - 創建表單的 DSL
* [Simple Form](https://github.com/plataformatec/simple_form) - 更加靈活的表單 DSL
* [Nested Form](https://github.com/ryanb/nested_form) - 級聯的表單 DSL，兼容 Simple Form
* [meta-tags](https://github.com/kpumuk/meta-tags) - SEO 相關的庫
* [active_link_to](https://github.com/comfy/active_link_to) - 根據當前 url 自動加 active 樣式
* [cells](https://github.com/apotonick/cells) - 把公用的 UI 寫到 view models
* [i18n Country Code Select](https://github.com/onomojo/i18n_country_select) - 國家代碼列表
* [Subdivision Select](https://github.com/cllns/subdivision_select) - 二級下拉列表，包括國家、省
* [cocoon](https://github.com/nathanvda/cocoon) - 級聯的表單 DSL

## 環境變量
* [Config](https://github.com/railsconfig/config) - 多環境的 YAML 配置文件
* [Figaro](https://github.com/laserlemon/figaro) - 針對 heroku 的配置辦法
* [dotenv](https://github.com/bkeepers/dotenv) - 將環境變量寫到 .env 文件中
* [opsworks-dotenv](https://github.com/mikamai/opsworks-dotenv) - 用 OpsWorks, Chef 和 Dotenv 配置環境變量

## 後臺管理
* [ActiveAdmin](http://activeadmin.info) - 後臺管理框架
  - [active_skin](https://github.com/rstgroup/active_skin): 為 ActiveAdmin 製作的皮膚
* [RailsAdmin](https://github.com/sferik/rails_admin) - 後臺管理
* [Typus](https://github.com/typus/typus) - 管理界面，讓受信任用戶管理數據
* [administrate](https://github.com/thoughtbot/administrate) - 靈活的後臺管理

## 日誌
* [Impressionist](https://github.com/charlotte-ruby/impressionist) - 記錄頁面訪問情況，還可以為一個訪問記錄幾次
* [Ahoy](https://github.com/ankane/ahoy) - 記錄訪問情況，和事件
* [Lograge](https://github.com/roidrage/lograge) - 改變 rails 默認的日誌，使變得更好

## 調試
* [byebug](https://github.com/deivid-rodriguez/byebug) - 簡單易用，不依賴其他代碼
  * [pry-byebug](https://github.com/deivid-rodriguez/pry-byebug) - 集成 Pry 與 byebug
* [pry-rails](https://github.com/rweng/pry-rails) - 使用 pry 打開 rails console
* [awesome_print](https://github.com/michaeldv/awesome_print) - 將 ruby 對象打印的更加漂亮
* [web-console](https://github.com/rails/web-console) - 把 console 加到 rails 中
* [spring](https://github.com/rails/spring) -  rails 預加載
* [rails-footnotes](https://github.com/josevalim/rails-footnotes) - 將調試信息顯示到腳註
* [g](https://github.com/jugyo/g) - [不更新]
* [terminal-notifier](https://github.com/julienXX/terminal-notifier) - 發送 Mac OS X 通知
* [letter_opener](https://github.com/ryanb/letter_opener) - 在瀏覽器中預覽郵件，而不用真實的發送
* [Better Errors](https://github.com/charliesome/better_errors) - 替代原生的錯誤頁面，更加漂亮有用
* [RailsPanel](https://github.com/dejan/rails_panel) - Chrome 擴展，在瀏覽器上更好的顯示 rails 日誌

## 代碼風格
* [RuboCop](https://github.com/bbatsov/rubocop) - 代碼分析，遵循很多代碼規範
* [Rails Best Practice](https://github.com/railsbp/rails_best_practices) - 檢查代碼質量
* [Metric Fu]( https://github.com/metricfu/metric_fu) - 檢查代碼質量
* [Pronto](https://github.com/mmozuras/pronto) - 自動檢查變化的代碼，與 github 集成

## 測試
* [rspec-rails](https://github.com/rspec/rspec-rails) - 測試框架
* [Capybara](https://github.com/jnicklas/capybara) -模擬真實用戶交互 測試 Web 應用，有這些驅動：
  - [capybara-webkit](https://github.com/thoughtbot/capybara-webkit) - 使用 QtWebkit 的 webkit
  - [selenium-webdriver](https://github.com/vertis/selenium-webdriver) - webdriver 支持
  - [poltergeist](https://github.com/teampoltergeist/poltergeist) - headless WebKit browser，使用 PhantomJS
  - [page-object](https://github.com/cheezy/page-object) - 創建靈活的頁面對象來做 web 測試
* [factory_girl](https://github.com/thoughtbot/factory_girl) - 專門用來構造模擬測試數據的,完美替代Fixture的工具
* [factory_girl_rails](https://github.com/thoughtbot/factory_girl_rails) - factory_girl 集成到 Rails
* [factory_factory_girl](https://github.com/st0012/factory_factory_girl) - 根據命名規則，生成 factory 文件
* [Database Cleaner](https://github.com/DatabaseCleaner/database_cleaner) - 一系列清理數據庫的策略
* [shoulda-matchers](https://github.com/thoughtbot/shoulda-matchers) - 提供很多 matchers 來測試 Rails 的函數
* [ResponseCodeMatchers](https://github.com/r7kamura/response_code_matchers) -  rspec matchers 匹配 http 返回值
* [SimpleCov](https://github.com/colszowka/simplecov) - 代碼測試覆蓋分析工具
* [Timecop](https://github.com/travisjeffery/timecop) - 用來測試時間相關，可以凍結時間、時間旅行
* [VCR](https://github.com/vcr/vcr) - 記錄 http 的返回內容，並在以後的測試中快速準確的重現

### 安全
* [brakeman](https://github.com/presidentbeef/brakeman) - 靜態分析工具，檢查程序的安全缺陷
* [bundle-audit](https://github.com/rubysec/bundler-audit) - 檢查 Bundle 的補丁等級，包括易受攻擊版本和不安全的 gem 源等
* [Secure Headers](https://github.com/twitter/secureheaders) -  自動設置安全相關的 headers

## 生產
* [Capistrano](https://github.com/capistrano/capistrano) - 遠程服務器部署工具
* [Slowpoke](https://github.com/ankane/slowpoke) - Rack::Timeout 的升級版
* [Rack Attack](https://github.com/kickstarter/rack-attack) - 防止惡意攻擊、限制訪問頻率
* [Responders](https://github.com/plataformatec/responders) - 一系列 responders
* [production_rails](https://github.com/ankane/production_rails) - Rails Best practices，一系列 Gem
* [Mina](https://github.com/mina-deploy/mina) -  快速部署、服務器自動化工具

## 錯誤日誌
* [Rollbar](https://github.com/rollbar/rollbar-gem) - 記錄錯誤日誌並彙總到 Rollbar
* [Airbrake](https://github.com/airbrake/airbrake) - 與 Airbrake 集成
* [Errbit](https://github.com/errbit/errbit) - 兼容 Airbrake，開源

## 資源管道
* [Alaska](https://github.com/mavenlink/alaska) - ExecJS 運行時保持與 nodejs 連接，加速 coffeescript 的編譯和部署

## 貢獻

歡迎大家貢獻代碼，請先閱讀 [貢獻指南](contributing.md) 。
