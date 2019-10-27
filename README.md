### Spina-CMS
---
https://www.spinacms.com/

https://github.com/SpinaCMS/Spina

```rb
// test/lib/spina/plugin_test.rb

module Spina
  module SpinaTest
    class Engine < ::Rails::Engine
      isolate_namespace ::Spina
      
      config.before_initialize do
        ::Spina::Plugin.register do |plugin|
          plugin.name = 'spina_test'
          plugin.namespace = 'spina_test'
          plugin.settings = {
            test_setting: { wysiwyg: '<div></div>' },
            foobar: :string
          }
        end
      end
    end
  end
end

```

```
```

```
```


