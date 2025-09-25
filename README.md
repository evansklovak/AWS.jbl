<p align="center">
  <img src="https://example.com/clitool.svg" alt="clitool" width="200" height="200" />
</p>

<h1 align="center">clitool</h1>

<h4 align="center">
  <a href="https://github.com/clitool">Repository</a> |
  <a href="https://docs.run">Documentation</a> |
  <a href="https://discord.run">Discord</a> |
  <a href="https://roadmap.run">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/clitool/actions"><img src="https://github.com/clitool/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/clitool"><img src="https://badge.fury.io/rb/clitool.svg" alt="Version"></a>
  <a href="https://github.com/clitool/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ debugging assistant for rapid iteration 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install clitool
```

In your `Gemfile`:
```ruby
gem 'clitool'
```

### Run clitool

```bash
clitool --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/clitool.rb`:

```ruby
clitool::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = clitool::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'flot-complete-FCBK' },
  { id: 2, title: 'providers' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [flot-complete-FCBK] and [providers].

