# Awesome IRC [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> A curated list of awesome [IRC](https://en.wikipedia.org/wiki/Internet_Relay_Chat) resources.

A list of tools, software & other resources related to the Internet Relay Chat (IRC) protocol.

IRC (Internet Relay Chat) is an open source protocol that can be used for multi-user text based communication through channels.

## Contents

<!--lint disable awesome-toc-->
<!--lint disable awesome-list-item-->
<!--lint ignore double-link-->
- [Clients](#clients)
- [Bouncers](#bouncers)
  - [Hosted](#hosted)
  - [Self-hosted](#self-hosted)
- [Daemons](#daemons)
- [Services](#services)
- [Bots](#bots)
- [Frameworks](#frameworks)
  - [Bridges](#bridges)
- [Channels](#channels)
  - [Discovery](#discovery)
  - [Platforms](#platforms)
- [Networks](#networks)
- [Articles](#articles)
- [Guides](#guides)
- [Protocol](#protocol)
- [Miscellaneous](#miscellaneous)

## Clients

*You use these to connect to IRC.*

- [Halloy](https://halloy.chat) - Modern, fast IRC client built with Iced GUI. IRCv3.2, SASL, DCC, and multi-server support. ([source](https://github.com/squidowl/halloy)) `Rust` `Windows` `macOS` `Linux`
- [Textual](https://www.codeux.com/textual/) - Very customizable, ZNC integration, iCloud sync ($4.99). ([source](https://github.com/Codeux-Software/Textual)) `macOS`
- [HexChat](https://hexchat.github.io) - Based on XChat, easy to use, spell check & multiple languages. ([source](https://github.com/hexchat/hexchat)) `Windows` `macOS` `Linux`
- [gamja](https://sr.ht/~emersion/gamja/) - A simple IRC web client. ([source](https://git.sr.ht/~emersion/gamja)) `Web`
- [Kiwi IRC](https://kiwiirc.com) - Powerful modern IRC messenger for the web. ([source](https://github.com/kiwiirc/kiwiirc), [demo](https://kiwiirc.com/nextclient/)) `Web`
- [Quassel](https://quassel-irc.org) - Distributed (clients can attach to and detach from a central core that stays permanently online). ([source](https://github.com/quassel/quassel)) `Linux` `macOS` `Windows`
- [Circe](https://github.com/emacs-circe/circe) - For use in Emacs, sane defaults. `Emacs`
- [KvIRC](https://www.kvirc.net) - Free, portable, based on Qt GUI toolkit. ([source](https://github.com/kvirc/KVIrc)) `Linux` `macOS` `Windows`
- [Konversation](https://konversation.kde.org) - User-friendly client built on the KDE Platform. ([source](https://github.com/KDE/konversation)) `Linux`
- [sic](https://tools.suckless.org/sic/) - **S**imple **I**RC **c**lient - a terminal client in less than 250 lines of C. `Linux`
- [irssi](https://irssi.org) - Terminal client, multi-protocol friendly for module authors, GPLv2. `Linux` `macOS` `Cygwin` `BSD`
- [catgirl](https://git.causal.agency/catgirl/) - TLS-only terminal client with tab-complete, nick coloring, URL detection, and split scrolling. `Linux` `macOS` `BSD`
- [senpai](https://sr.ht/~delthas/senpai/) - Modern terminal client designed to work best with IRC bouncers. CHATHISTORY and SEARCH support. ([source](https://git.sr.ht/~delthas/senpai)) `Go`
- [tiny](https://github.com/osa1/tiny) - Terminal client with nick mention tracking, auto-reconnect, and configurable key bindings. `Rust`
- [kirc](https://github.com/mcpcpc/kirc) - A KISS for IRC, tiny IRC client written in POSIX C99. `Linux`
- [AdiIRC](https://adiirc.com) - Never has a client offered such granular settings for every aspect of the IRC experience. ([features](https://dev.adiirc.com/projects/adiirc/wiki/Features), [screenshots](https://dev.adiirc.com/projects/adiirc/wiki/Screenshots)) `Windows` `WINE`
- [IRC for Android™](https://www.countercultured.net/android/) - Android/Chrome OS client for power users, with ZNC built-ins, notification logic, reliable DCC, keybinds for hardware keyboards, etc. `Android` `ChromeOS`
- [Revolution IRC](https://github.com/MCMrARM/revolution-irc) - Feature-full, actively maintained Android IRC client. `Android`
- [Goguma](https://sr.ht/~emersion/goguma/) - An IRC client for mobile devices, from the creator of soju. `Android` `Linux`

<!--lint ignore double-link-->
*More? Clients that include bouncers are found [below](#bouncers).*

## Bouncers

*Useful for disconnecting and reconnecting without losing the chat session.*

### Hosted

- [IRCCloud](https://www.irccloud.com) - Group chat for teams, friends, and communities. stay connected, chat from anywhere, and never miss a message (+client) (£0-£3.50/month).
  - [iOS App](https://github.com/irccloud/ios) - Official. `Objective-C`
  - [Android App](https://github.com/irccloud/android) - Official. `Java`
  - [Nimbus](https://github.com/jnordberg/irccloudapp) - Standalone client. `macOS` `Objective-C`

### Self-hosted

- [soju](https://soju.im) - A user-friendly IRC bouncer with multi-upstream support and IRCv3 extensions. ([source](https://git.sr.ht/~emersion/soju)) `Go`
- [ZNC](https://wiki.znc.in/ZNC) - Most popular. many different plugins. ([source](https://github.com/znc/znc)) `C++`
- [Convos](https://convos.chat) - Always online web IRC client. ([source](https://github.com/convos-chat/convos)) `Perl` `JavaScript` `Web`
- [TheLounge](https://thelounge.chat) - Responsive, self-hosted & support for multiple users. ([source](https://github.com/thelounge/thelounge), [demo](https://demo.thelounge.chat/)) `JavaScript` `Node.js` `Web`
- [WeeChat](https://weechat.org) - A fast, light and extensible chat client. ([source](https://github.com/weechat/weechat)) `Linux` `macOS` `Windows`
- [pounce](https://git.causal.agency/pounce/) - Multi-client, TLS-only IRC bouncer. By the author of catgirl. `C`

## Daemons

*Used for running your own IRC server or network.*

- [UnrealIRCd](https://www.unrealircd.org) - The most widely deployed IRC server (38% market share). Modular, highly configurable, with advanced security and IRCv3 support. ([source](https://github.com/unrealircd/unrealircd)) `C`
- [InspIRCd](https://www.inspircd.org) - Modular, stable, written from scratch. ([source](https://github.com/inspircd/inspircd)) `C++`
- [Ergo](https://ergo.chat) - Modern server that's portable and designed around specifications (bleeding-edge IRCv3 support). Combines ircd, services, and bouncer. ([source](https://github.com/ergochat/ergo)) `Go`
- [Solanum](https://solanum.chat) - IRCv3 server used by Libera.Chat and OFTC, continuation of Charybdis. ([source](https://github.com/solanum-ircd/solanum)) `C`
- [ngIRCd](https://ngircd.barton.de) - Portable and lightweight for small or private networks. ([source](https://github.com/ngircd/ngircd)) `C`

## Services

*Used to provide user accounts and bots like NickServ/ChanServ to your network.*

- [Atheme](https://atheme.github.io) - Designed for large networks with high scalability requirements. ([source](https://github.com/atheme/atheme))
- [anope](https://www.anope.org) - Designed for flexibility and ease of use. ([source](https://github.com/anope/anope))

## Bots

*IRC users which provide services for humans, e.g. integrations or information.*

- [Eggdrop](https://www.eggheads.org) - Oldest IRC bot still in active development. Feature rich, uses Tcl scripting. ([source](https://github.com/eggheads/eggdrop)) `C`
- [Sopel](https://sopel.chat) - Tonnes of ready made features, tutorial, fully documented. ([source](https://github.com/sopel-irc/sopel)) `Python`
- [Limnoria](https://github.com/ProgVal/Limnoria) - Robust, user friendly, developer friendly. `Python`
- [CloudBot](https://github.com/TotallyNotRobots/CloudBot) - Simple, fast, expandable. `Python`
- [milla](https://github.com/terminaldweller/milla) - LLM-powered bot with Lua scripting support. `Go`
- [wayback](https://github.com/wabarc/wayback) - An archiving tool with an IRC interface integrated with various archiving services.

## Frameworks

*Helpful to write bots or integrate IRC with applications.*

- [irc](https://github.com/aatxe/irc) - A thread-safe and reactive IRC library. `Rust`
- [PircBotX](https://github.com/pircbotx/pircbotx) - Event based IRC Library with a straightforward API (updated fork of [PircBot](http://www.jibble.org/pircbot.php)). `Java`
- [girc](https://github.com/lrstanley/girc) - Flexible IRC library with support for decoding/encoding raw IRC lines. `Go`
- [IRC::Client](https://github.com/lizmat/IRC-Client) - `Perl6` based extendable IRC client framework.

### Bridges

*Sends messages back and forth.*

- [matterbridge](https://github.com/42wim/matterbridge) - IRC ↔ Mattermost ↔ Discord ↔ XMPP ↔ Gitter ↔ Slack ↔ Discord ↔ Telegram ↔ etc. `Go`
- [Heisenbridge](https://github.com/hifi/heisenbridge) - Bouncer-style Matrix IRC bridge. `Python`
- [Appservice-IRC](https://github.com/matrix-org/matrix-appservice-irc) - Gateway and bridge Matrix ↔ IRC. `JavaScript`
- [discord-irc](https://github.com/reactiflux/discord-irc) - Discord ↔ IRC. `JavaScript`
- [dibridge](https://github.com/OpenTTD/dibridge) - Discord ↔ IRC (with puppets). `Python`
- [teleirc](https://github.com/RITlug/teleirc) - Telegram ↔ IRC. `JavaScript`
- [BitlBee](https://www.bitlbee.org/main.php/news.r.html) - XMPP, Jabber, Google Talk, MSN Messenger, Yahoo! Messenger, AIM, ICQ, Twitter API, HipChat ↔ IRC. `C`
- [Biboumi](https://biboumi.louiz.org/) - IRC gateway for XMPP clients. `C`
- [irc-slack](https://github.com/insomniacslk/irc-slack) - Slack ↔ IRC. `Go`
- [matterircd](https://github.com/42wim/matterircd) - Mattermost ↔ IRC, Slack ↔ IRC, Mastodon ↔ IRC. `Go`

## Channels

*IRC channels.*

### Discovery

- [netsplit.de Search](https://netsplit.de/channels/) - Searches 563 different networks.
- [mibbit Search](https://search.mibbit.com) - Searches networks listed [here](https://search.mibbit.com/networks).
- [KiwiIRC Search](https://kiwiirc.com/search) - Searches 318 different networks.

### Platforms

- [#ubuntu](https://wiki.ubuntu.com/IRC/ChannelList)@Libera.Chat - Official Ubuntu support channel. ([rules](https://wiki.ubuntu.com/IRC/Guidelines))

## Networks

*A collection of IRC servers is known as a network.*

- [Libera.Chat](https://libera.chat) - The largest IRC network, mostly focused on free and open source projects.
- [OFTC](https://oftc.net) - Community for free and open source software communities.
- [Snoonet](https://snoonet.org) - Community of redditors and subreddits. ([rules](https://snoonet.org/rules/))
- [EFnet](http://www.efnet.org) - One of the original IRC networks, founded in 1990.
- [DALnet](https://www.dal.net) - Large network with a long history, services-friendly.
- [Rizon](https://rizon.net) - Large general-purpose network popular in the anime and creative communities.
- [LibertaCasa](https://liberta.casa) - Privacy endorsing community serving as a safe and open space for the discussion of various topics.

## Articles

*Articles and blog posts about IRC.*

- [Please don't use Slack for FOSS projects](https://drewdevault.com/2015/11/01/Please-stop-using-slack.html) - Drew DeVault's Blog.
- [IRC Networks Under Systematic Attack From Governments](https://www.quakenet.org/articles/102-press-release-irc-networks-under-systematic-attack-from-governments) - QuakeNet.
- [IRC is dead, long live IRC](https://www.pingdom.com/blog/irc-is-dead-long-live-irc/) - Pingdom.
- [IRC Has Lost 60% Of Its Users Since 2003, But Life As A Robot Is Just Beginning](https://techcrunch.com/2013/01/06/irc-has-lost-60-of-its-users-since-2003-but-life-as-a-robot-is-just-beginning/) - Alex Williams (TechCrunch).

## Guides

*How-to's, documentation and books.*

- [#irchelp](https://www.irchelp.org) - A vast amount of reasonably up-to-date information.

## Protocol

*Information and resources about the IRC protocol itself.*

- [IRCv3 Working Group](https://ircv3.net) - A group of IRC software authors working to enhance, improve, maintain and standardize the IRC protocol. ([source](https://github.com/ircv3/ircv3.github.io))
- [Modern IRC Documents](https://modern.ircdocs.horse) - An attempt to write an update to the original IRC protocol documentation. ([source](https://github.com/ircdocs/modern-irc))
- [IRC Definition Files](https://defs.ircdocs.horse) - Lists of numerics, modes, ISUPPORT tokens and other protocol details. ([source](https://github.com/ircdocs/irc-defs))
- [grawity's IRC docs](https://github.com/grawity/irc-docs) - Collection of misc IRC protocol documentation.
- [Protocol Statistics](https://stats.ircdocs.horse) - Statistics around the server software in use on networks today. ([source](https://github.com/ircdocs/irc-stats))
- [IRC Parser Tests](https://github.com/ircdocs/parser-tests) - A CC0 set of test suites, to ensure IRC message parsers are consistent.
- [DareNET Archives](https://archives.darenet.org) - IRC Archives for old hard to find IRC related software.

## Miscellaneous

*Items that belong on the list but defy classification.*

- [superseriousstats](https://github.com/tommyrot/superseriousstats) - Fast and efficient program to create statistics out of various types of chat logs. `PHP` `Web`
- [img2irc](https://github.com/waveplate/img2irc) - Convert images to halfblock ANSI or IRC, with a bunch of post-processing filters. `Rust`

## Use

The best ways to use this list are:

- By browsing the [contents](#contents)
- By using <kbd>command</kbd> + <kbd>F</kbd> to search the contents

This list also uses tags to help when searching the contents:
- **Language** - `Python`, `Java`, `C++`, `Go`, `JavaScript`, `Ruby`, `C`, `Rust` etc.
- **Platform** - `Web`, `macOS`, `Windows`, `Linux`, `Chrome` etc.

## Credits

By [Craig Davison](https://davison.io) and contributors.
