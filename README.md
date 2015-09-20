mktorrent
=========

A Ruby Gem for easily creating .torrent files.

To get started:

    git clone https://github.com/mukaibot/mktorrent.git
    gem build mktorrent.gemspec
    gem install mktorrent

Then in your Ruby code:

    require 'mktorrent'
    t = Torrent.new("http://your.tracker.com")
    t.add_file("path/to/your.file")
    t.add_file("path/to/another.file")
    t.add_directory("path/to/directory")
    t.add_webseed("http://your.webseed.com") # Optional!
    t.defaultdir = "Your Torrent"
    t.write_torrent("Yourtorrent.torrent")

Pull requests are very welcome!
