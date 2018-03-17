# [Awesome IRC](https://davison.io/awesome-irc/) :speech_balloon: [![](https://img.shields.io/travis/davisonio/awesome-irc.svg?style=flat-square)](https://travis-ci.org/davisonio/awesome-irc) [![](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome [IRC](https://en.wikipedia.org/wiki/Internet_Relay_Chat) resources

<p align="center">
<b><a href="#contents">Contents</a></b>
·
<b><a href="#use">Use</a></b>
·
<b><a href="#authors">Authors</a></b>
·
<b><a href="#license--credits">License & Credits</a></b>
</p>

This is a list of tools, software & other resources related to the Internet Relay Chat (IRC) protocol.

*"IRC: The one protocol that you can never resist"* - [Firrre](https://firrre.com)

![](https://davison.io/assets/img/awesome-irc-logo.png)

## Contents

- [Clients](#clients)
- [Bouncers](#bouncers)
  - [Self-hosted](#self-hosted)
  - [Hosted](#hosted)
- [Daemons](#daemons)
- [Services](#services)
- [Bots](#bots)
- [Frameworks](#frameworks)
  - [Bridges](#bridges)
- [Channels](#channels)
  - [Discovery](#discovery)
  - [Platforms](#platforms)
  - [Programming](#programming)
- [Networks](#networks)
- [Articles](#articles)
- [Guides](#guides)
- [Protocol](#protocol)
- [Miscellaneous](#miscellaneous)

### Clients

*You use these to connect to IRC.*

- [Komanda](http://komanda.io) - designed for people who write code (beta) ([source](https://github.com/mephux/komanda)) `Linux`
- [Textual](https://www.codeux.com/textual/) - very customizable, ZNC integration, iCloud sync ($4.99) ([source](https://github.com/Codeux-Software/Textual)) `macOS`
- [LimeChat](http://limechat.net/mac/) - one window for multiple servers, keyboard shortcuts, fast & stable ([source](https://github.com/psychs/limechat)) `macOS`
- [HexChat](https://hexchat.github.io) - based on XChat, easy to use, spell check & multiple languages ([source](https://github.com/hexchat/hexchat)) `Windows` `macOS` `Linux`
- [Kiwi IRC](https://kiwiirc.com) - a powerful modern IRC messenger for the web ([source](https://github.com/kiwiirc/kiwiirc), [demo](https://kiwiirc.com/nextclient/)) `Web`
- [CIRC](https://flackr.github.io/circ/) - uses the chrome.sockets APIs to connect directly to IRC servers without needing a proxy ([source](https://github.com/flackr/circ)) `Chrome`
- [nirc](https://github.com/cjstewart88/nirc) - simple ([demo](https://nirc.herokuapp.com)) `Web`
- [Quassel](https://quassel-irc.org) - distributed (clients can attach to and detach from a central core that stays permanently online ([source](https://github.com/quassel/quassel)) `Linux` `macOS` `Windows`
- [Yaaic](https://www.yaaic.org) - multi-server/channel support, SASL support, Smooth channel scrolling / swiping ([source](https://github.com/pocmo/Yaaic)) `Android`
- [koko](https://github.com/KokoIRC/koko) - minimalistic design, VIM-like shortcuts and built on electron `Windows` `macOS`
- [relay.js](https://github.com/Fauntleroy/relay.js) - focuses on making IRC less intimidating and easier to use ([demo](http://demo.relayjs.com)) `Web`
- [Circe](https://github.com/jorgenschaefer/circe) - for use in Emacs, sane defaults `Emacs`
- [Smuxi](https://smuxi.im) - user-friendly, based on GNOME / GTK+ ([source](https://github.com/meebey/smuxi)) `Linux` `Windows` `macOS`
- [aIRChat](https://github.com/zsck/aIRChat) - beautiful, modernized, browser-based `Web`
- [KVIrc](http://www.kvirc.net) - free, portable, based on Qt GUI toolkit ([source](https://github.com/kvirc/KVIrc)) `Linux` `macOS` `Windows`
- [Konversation](https://konversation.kde.org) - user-friendly client built on the KDE Platform ([source](https://github.com/KDE/konversation)) `Linux`
- [sic](https://tools.suckless.org/sic/) - **s**imple **I**RC **c**lient - a terminal client in less than 250 lines of C. `Linux`
- [Weechat](https://weechat.org) - Fast, light, and extensible chat client. `Linux` `BSD` `macOS`
  `Windows`

*More? Clients that include bouncers are found [below](#bouncers).*

### Bouncers

*Useful for disconnecting and reconnecting without losing the chat session.*

#### Hosted

- [IRCCloud](https://www.irccloud.com) - group chat for teams, friends, and communities. stay connected, chat from anywhere, and never miss a message. (+client) (£0-£3.50/month)
  - [iOS App](https://github.com/irccloud/ios) - official `Objective-C`
  - [Android App](https://github.com/irccloud/android) - official `Java`
  - [Nimbus](https://github.com/jnordberg/irccloudapp) - standalone client `macOS` `Objective-C`
- [Grove](https://grove.io) - hosted IRC and so much more (+client) ($10-$125/month)
- [Firrre](https://firrre.com) - authorized connections to Free / Libre / Open Source driven IRC Networks (Free)

#### Self-hosted

- [Convos](https://convos.by/) - Always online web IRC client ([source](https://github.com/Nordaaker/convos), [demo](https://demo.convos.by/)) `Perl` `JavaScript` `Web`
- [ZNC](http://wiki.znc.in/ZNC) - most popular. many different plugins ([source](https://github.com/znc/znc))
- [IRCAnywhere](http://ircanywhere.com) - built for teams and gives control + privacy to you (alpha) ([source](https://github.com/ircanywhere/ircanywhere))
- [TapChat](http://tapchatapp.com) - modern IRC ([source](https://github.com/tapchat/tapchat))
  - [Android App](https://github.com/tapchat/tapchat-android) - source only `Java`
- [TheLounge](https://thelounge.chat/) - responsive, self-hosted & support for multiple users ([source](https://github.com/thelounge/thelounge), [demo](https://demo.thelounge.chat)) `JavaScript` `Node.js` `Web`

### Daemons

*Used for running your own IRC server or network.*

- [ircd.js](https://github.com/alexyoung/ircd.js) - server will allow clients to connect, join channels, change topics; basic stuff
- [InspIRCd](http://www.inspircd.org) - modular, stable, written from scratch ([source](https://github.com/inspircd/inspircd))
- [miniircd](https://github.com/jrosdahl/miniircd) - very simple and limited
- [ngIRCd](https://ngircd.barton.de) - portable and lightweight for small or private networks ([source](https://github.com/ngircd/ngircd))
- [Hulk](https://github.com/chrisdone/hulk) - intended for private business use or hobby work `Haskell`
- [Oragono](https://oragono.io/) - modern, experimental server that's portable and designed around specifications ([source](https://github.com/oragono/oragono))
- [charybdis](https://github.com/charybdis-ircd/charybdis) - scalable IRCv3 server

### Services

*Used to provide user accounts and bots like NickServ/ChanServ to your network.*

- [Atheme](https://atheme.github.io) - designed for large networks with high scalability requirements ([source](https://github.com/atheme/atheme))
- [anope](http://anope.org) - designed for flexibility and ease of use ([source](https://github.com/anope/anope))

### Bots

*IRC users which provide services for humans, e.g. integrations or information.*

- [BotBot.me](https://botbot.me) - makes IRC logs awesome ([source](https://github.com/BotBotMe/botbot-bot))
  - [Web interface](https://github.com/BotBotMe/botbot-web) - ([demo](https://botbot.me/freenode/ghost/))
- [Sopel](https://sopel.chat) - tonnes of ready made features, tutorial, fully documented ([source](https://github.com/sopel-irc/sopel)) `Python`
- [phenny](http://inamidst.com/phenny/) - simple, module creation guide ([source](https://github.com/sbp/phenny)) `Python`
- [IRCcat](https://github.com/RJ/irccat) - simplifies messaging from shell scripts `Java`
- [Limnoria](https://github.com/ProgVal/Limnoria) - robust, user friendly, developer friendly `Python`
- [Twitch Plays](https://github.com/aidanrwt/twitch-plays ) - takes input from the chat and presses the corresponding key `Python`
- [Skybot](https://github.com/rmmh/skybot) - main goals are simplicity and power `Python`
- [Jenni](https://github.com/myano/jenni) - `Python`
- [talkbackbot](https://geekchick77.dreamwidth.org/472.html) - responds to configured trigger phrases with quotes from notable women ([source](https://github.com/jessamynsmith/talkbackbot)) `Python`
- [lazybot](https://github.com/Raynes/lazybot) - user-friendly and powerful `Clojure`
- [IRC-BF](https://github.com/SirCmpwn/bf-irc-bot) - `Brainfuck`
- [geordi](https://github.com/Eelis/geordi) - compiles and runs C++ code snippets `C++`
- [CloudBot](https://github.com/CloudBotIRC/CloudBot) - simple, fast, expandable `Python`

### Frameworks

*Helpful to write bots or integrate IRC with applications.*

- [node-irc](https://github.com/martynsmith/node-irc) `JavaScript`
- [Cinch](https://github.com/cinchrb/cinch) - quickly create bots with minimal effort `Ruby`
- [goirc](https://github.com/fluffle/goirc) - event-based, stateful, lacking documentation `Go`
- [Hubot IRC Adapter](https://github.com/nandub/hubot-irc) - the IRC adapter for hubot `JavaScript`
- [go-ircevent](https://github.com/thoj/go-ircevent) - event-based `Go`
- [pyaib](https://github.com/facebook/pyaib) - easy to use framework for writing bots `Python`
- [slate-irc](https://github.com/slate/slate-irc) - plugin system, simple api, arbitrary input stream, debug support `JavaScript`
- [Jerk](https://github.com/gf3/Jerk) - ridiculously simple to set-up and get going `JavaScript`

#### Bridges

*Sends messages back and forth.*

- [slack-irc](https://github.com/ekmartin/slack-irc) - Slack <-> IRC `JavaScript`
- [CamperVan](https://github.com/zerowidth/camper_van) - Campfire <-> IRC `Ruby`
- [BitlBee](https://www.bitlbee.org/main.php/news.r.html) - XMPP, Jabber, Google Talk, MSN Messenger, Yahoo! Messenger, AIM, ICQ, Twitter API, HipChat <-> IRC `C`
- [teleirc](https://github.com/FruitieX/teleirc) - Telegram <-> IRC `JavaScript`
- [toxirc](https://github.com/endoffile78/toxirc) - Tox <-> IRC `C`

### Channels

*IRC channels.*

#### Discovery

- [irc.netsplit.de Search](http://irc.netsplit.de/channels/) - searches 563 different networks
- [mibbit Search](https://search.mibbit.com) - searches networks listed [here](https://search.mibbit.com/networks)
- [KiwiIRC Search](https://kiwiirc.com/search) - searches 318 different networks

#### Platforms

- [##linux](https://freenode.linux.community)@freenode - Linux support and discussion channel ([rules](https://freenode.linux.community/channel-rules/))
- [#ubuntu](https://help.ubuntu.com/community/InternetRelayChat)@freenode - official ubuntu support channel ([rules](https://wiki.ubuntu.com/IRC/Guidelines))

#### Programming

- [#python](https://www.python.org/community/irc/)@freenode - good place for short python questions ([rules](https://www.python.org/psf/codeofconduct/))

### Networks

*A collection of IRC servers is known as a network.*

- [freenode](https://freenode.net) - the largest network, for free and open source software communities ([rules](https://freenode.net/policies))
- [Snoonet](https://snoonet.org) - community of redditors and subreddits ([rules](https://snoonet.org/rules))
- [OFTC](https://oftc.net/) - commnuity for free and open source software communities

### Articles

*Articles and blog posts about IRC.*

- [Please don't use Slack for FOSS projects](https://drewdevault.com/2015/11/01/Please-stop-using-slack.html) - Drew DeVault's Blog
- [IRC Networks Under Systematic Attack From Governments](https://www.quakenet.org/articles/102-press-release-irc-networks-under-systematic-attack-from-governments) - QuakeNet
- [IRC is dead, long live IRC](https://royal.pingdom.com/2012/04/24/irc-is-dead-long-live-irc/) - Royal Pingdom
- [IRC Has Lost 60% Of Its Users Since 2003, But Life As A Robot Is Just Beginning](https://techcrunch.com/2013/01/06/irc-has-lost-60-of-its-users-since-2003-but-life-as-a-robot-is-just-beginning/) - Alex Williams (TechCrunch)

### Guides

*How-to's, documentation and books.*

- [#irchelp](http://www.irchelp.org) - a vast amount of reasonably up-to-date information
- [How to Setup a Secure Private IRC Channel](https://botbot.me/how-to-setup-irc-channel/)
- [BotBot's IRC Cheat Sheet](https://botbot.me/irc-guide/) - well-designed and with many well-answered questions

### Protocol

*Information and resources about the IRC protocol itself.*

- [IRCv3 Working Group](https://ircv3.net) - a group of IRC software authors working to enhance, improve, maintain and standardize the IRC protocol ([source](https://github.com/ircv3/ircv3.github.io))
- [Modern IRC Documents](http://modern.ircdocs.horse/) - an attempt to write an update to the original IRC protocol documentation ([source](https://github.com/ircdocs/modern-irc))
- [IRC Definition Files](http://defs.ircdocs.horse/) - lists of numerics, modes, ISUPPORT tokens and other protocol details ([source](https://github.com/ircdocs/irc-defs))
- [grawity's IRC docs](https://github.com/grawity/irc-docs) - collection of misc IRC protocol documentation
- [Protocol Statistics](http://stats.ircdocs.horse/) - statistics around the server software in use on networks today ([source](https://github.com/ircdocs/irc-stats))
- [IRC Parser Tests](https://github.com/DanielOaks/irc-parser-tests) - a CC0 set of test suites, to ensure IRC message parsers are consistent

### Miscellaneous

*Items which don't fit into the other categories*

- [IRC LC](https://irc.lc) - create a URL that points to a channel on a IRC network

## Use

The best ways to use this list are:

- by browing the [contents](#contents)
- by using <kbd>command</kbd> + <kbd>F</kbd> to search the contents

This list also uses tags to help when searching the contents:

- **Language** - `Python`, `Java`, `C++`, `Go`, `JavaScript`, `Ruby`, `C` etc.
- **Platform** - `Web`, `macOS`, `Windows`, `Linux`, `Chrome` etc.

## Authors

**[Craig Davison](https://davison.io)**

[![](https://img.shields.io/github/followers/davisonio.svg?style=social&label=Follow%20davisonio)](https://github.com/davisonio) [![](https://img.shields.io/twitter/follow/davisonio.svg?style=social)](https://twitter.com/davisonio)

With many thanks to the [contributors](https://github.com/davisonio/awesome-irc/graphs/contributors). :clap:

**Contributions are welcome!** Check out the [Contributing Guidelines](https://github.com/davisonio/awesome-irc/blob/master/CONTRIBUTING.md). :raised_hands:

## License & Credits

Unless otherwise stated:

- Copyright © 2016+ [Craig Davison](https://davison.io). Released under the [CC0 1.0 License](https://creativecommons.org/publicdomain/zero/1.0/).
