# The Hamler Programming Language

**Hamler** - Haskell-style functional programming language running on Erlang VM. **Hamler** is a strongly-typed language with compile-time typechecking and built-in support for concurrency and distribution.

**Hamler** empowers industries to build the next generation of scalable, reliable, realtime applications, especially for 5G, IoT and edge computing.

## **Why Hamler?**

For almost a decade, we have been developing software systems based on Erlang/OTP, especially our main product [EMQ X](https://github.com/emqx/emqx) - the scalable open-source MQTT broker. So, we have always believed that Erlang is a masterpiece of engineering. With amazing concurrency, distribution and fault tolerance, it is one of the few general-purpose language platforms able to properly handle concurrency and soft realtime.

However, from all the experience writing Erlang, we believe that the following features can help Erlang programmer better adapt to the coming wave of 5G, IoT and edge-programming and attract more people for using BEAM.

- Compile-time type checking and type reference
- ADTs, Function Composition, Type Classes
- More friendly syntax for prosperous communities
- Functor, Applicative and Monad...:)

Now all the features are avaliable in the Hamler programming language.

## **Features**

- Functional programming
- Haskell and ML style
- ADT and Type Checking/Inference
- Functions, higher-order functions
- Currying and partial application
- Pattern matching, and Guards
- List comprehension
- Applicative and Monad
- Advanced module system
- Built-in concurrency

## **Installation**

**Homebrew(macOS)**

```shell
brew tap hamler-lang/hamler
brew install hamler
```

**Build from source code(macOS)**

0. Install Erlang

   ```shell
   brew install erlang@22
   ```

1. Install Stack

   Stack tutoriall https://docs.haskellstack.org/en/stable/install_and_upgrade/

2. Clone hamler from the git repo

   ```shell
   git clone https://github.com/hamler-lang/hamler.git
   ```

3. Install hamler

   ```shell
   cd hamler
   make
   make install
   ```

## **Try the interpreter**

```shell
hamler repl

> -- List, range and enums
> [1,2,3]
> [1..10]
> ['a'..'z']

> -- erlang style maps
> import Data.Map as Map
> -- New map
> m = #{"foo" => "bar", "bar" => "foo"}
> -- Match Map
> #{"foo" := a, "bar" := b} = m
> -- get, put
> Map.get "foo" m -- a = "bar"
> Map.get "bar" m -- b = "foo"
> m1 = Map.put "key" "val"
> -- keys, values
> keys = Map.keys m
> values = Map.values m
```

## **Create a project**

```shell
mkdir demo-project
cd demo-project
hamler init
make
make run
```

### **Documentation**

- [Cheatsheet](https://github.com/hamler-lang/documentation/blob/master/Cheatsheet.md)
- [Guide](https://github.com/hamler-lang/documentation/blob/master/guides/00_TableOfContents.md)

## **Community, discussion and supports**

You can reach the **Hamler** community and core team via the following channels:

- [Slack - emqx/hamler-lang](https://slack-invite.emqx.io/)
- [Twitter - @hamlerlang](https://twitter.com/hamlerlang)
- [Reddit - /r/HamlerLang](https://www.reddit.com/r/HamlerLang/)
- [Medium - @hamlerlang](https://medium.com/@hamlerlang)

## **Contributing**

To contribute to **Hamler** project:

- Report issues: submit any bugs, issues to [hamler/issues](https://github.com/hamler-lang/hamler/issues)
- Contribute code: Fork the project, and submit feature requests to [hamler-lang/hamler](https://github.com/hamler-lang/hamler).
- Submit a proposal: Fork the [hamler-wiki](https://github.com/hamler-lang/hamler-wiki) project and submit pull request

## **Core Team**

The Hamler core team comes from [EMQ Technologies Co., Ltd.](https://emqx.io/) now.

- [Feng Lee](https://github.com/emqplus): Designer of Hamler Language
- [Yang M](https://github.com/EMQ-YangM): Implemented Hamler Compiler
- [S Hu](https://github.com/SjWho): Maintainer of the documentations
- [Shawn](https://github.com/terry-xiaoyu): Contributed [rebar3_hamler][rebar3_hamler] plugin
- [Rory Z](https://github.com/zhanghongtong): Contributed [homebrew][homebrew] install package
- [wivwiv](https://github.com/wivwiv): Designer of hamler-lang.org website
- [CrazyWisdom](https://github.com/CrazyWisdom): Maintainer of hamler-lang.org
- [ysfscream](https://github.com/ysfscream): Maintainer of hamler-lang.org
- [juan6666](https://github.com/juan6666)：Designer of Hamler language logo

[homebrew]: https://github.com/hamler-lang/homebrew-hamler
[rebar3_hamler]: https://github.com/hamler-lang/rebar3_hamler

## **About EMQ**

[**EMQ**](https://emqx.io/) is an open source software company providing highly-scalable, real-time messaging and streaming platform for IoT applications in 5G Era.

## **License**

BSD3

