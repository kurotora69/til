#rails g controller コントローラー名(複数形) で自動生成されるファイル

生成したファイルに対応したスタイルシート・ヘルパー・JavaScriptのファイル、テスト用ファイルの４つ

※自動生成をしない場合はconfig/application.rb内で設定を変更する

```Ruby:config/application.rb
module アプリ名
  class Application < Rails::Application
    config.load_defaults 6.0
   # 中略
    config.generators do |g|
      g.stylesheets false
      g.javascripts false
      g.helper false
      g.test_framework false
    end
  end
end


