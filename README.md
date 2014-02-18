# Cleditor::Rails


Integrates CLEditor into Rails 3.1+ asset pipeline

Forked for latest (for now) version of source at: http://premiumsoftware.net/cleditor/

Includes "Table Plug-in Version 1.0.3".

Also changed version of this gem to be the same as the CLEditor version.

(Except: Right now we're on 1.4.4.1 because we needed to switch away from the advanced table editor plugin
to the normal one for better IE support)

Also also required small changes to JS and CSS files to fix paths so they point to
asset pipeline.

## Installation

Add this line to your application's Gemfile:

    gem "cleditor-rails", :git => "https://github.com/Promptus/cleditor-rails.git"

And then execute:

    $ bundle

## Usage

1.) Run

    $ rails g cleditor:install

2.) Add this to your application.js
    
    $(document).ready(function() {
        $("textarea").cleditor();
    });

3.) In production.rb
  
    config.assets.compile = true


More configuration options here: http://premiumsoftware.net/cleditor/docs/GettingStarted.html#usage

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
