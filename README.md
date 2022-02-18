# Knowledge

## 跨端 GUI 库

### [Dioxus](https://dioxuslabs.com/)
基于 Rust Webview 实现, 语法类 React 风格
```rust
fn app(cx: Scope) -> Element {
    let (count, set_count) = use_state(&cx, || 0);

    cx.render(rsx!(
        h1 { "High-Five counter: {count}" }
        button { onclick: move |_| set_count(count + 1), "Up high!" }
        button { onclick: move |_| set_count(count - 1), "Down low!" }
    ))
}
```

### [Flutter](https://flutter.dev/)
原生 UI 实现, Dart 语言

### [React Native](https://reactnative.dev/)
基于 JS/TS 的 Bridge 实现

### [tauri](https://github.com/tauri-apps/tauri)
Rust 构建桌面程序

## 词法分析

### [pest](https://pest.rs/)
基于 Rust 实现的通用解析器
```pest
alpha = { 'a'..'z' | 'A'..'Z' }
digit = { '0'..'9' }

ident = { (alpha | digit)+ }

ident_list = _{ !digit ~ ident ~ (" " ~ ident)? }
```

### [nom](https://github.com/Geal/nom)
基于 Rust 实现的解析器组合库

### [inkwell](https://github.com/TheDan64/inkwell)
LLVM 的 Rust 封装

## 命令行参数解析工具

### [clap](https://github.com/clap-rs/clap)
基于 Rust 命令行参数解析

## 操作系统

### [v86](https://github.com/copy/v86)
基于 Rust, 浏览器里面虚拟化 x86 操作系统

### [Ventoy](https://github.com/ventoy/Ventoy)
USB boot loader

### [writing-an-os-in-rust](https://github.com/rustcc/writing-an-os-in-rust)
使用 Rust 写操作系统教程

### [rCore-Tutorial-v3](https://github.com/rcore-os/rCore-Tutorial-v3)
Rust 实现 RISC-V 架构操作系统

## 工具

### [rust-csv](https://github.com/BurntSushi/rust-csv)
CSV 解析库

### [htmlq](https://github.com/mgdm/htmlq)
基于 Rust 类似 jq 的 html 选择器
```bash
$ curl --silent https://www.rust-lang.org/ | htmlq '#get-help'
<div class="four columns mt3 mt0-l" id="get-help">
        <h4>Get help!</h4>
        <ul>
          <li><a href="https://doc.rust-lang.org">Documentation</a></li>
          <li><a href="https://users.rust-lang.org">Ask a Question on the Users Forum</a></li>
          <li><a href="http://ping.rust-lang.org">Check Website Status</a></li>
        </ul>
        <div class="languages">
            <label class="hidden" for="language-footer">Language</label>
            <select id="language-footer">
                <option title="English (US)" value="en-US">English (en-US)</option>
<option title="French" value="fr">Français (fr)</option>
<option title="German" value="de">Deutsch (de)</option>

            </select>
        </div>
      </div>
```

### [pdf.js](https://github.com/mozilla/pdf.js)
PDF阅读器

### [hyper](https://github.com/hyperium/hyper)
HTTP 库

### [composing.studio](https://github.com/ekzhang/composing.studio)
基于 TS, 生成可视化五线谱
```
T:Duet in G
T:1. Allegro
C:Fran\ccois Devienne
Z:Transcribed by Frank Nordberg - http://www.musicaviva.com
M:C
L:1/8
Q:136
K:G
V:Flute_1
g4 (fd)(ef)|g2g2a2a2|b4 (ag)(ab)|g2g2d4|
V:Flute_2
(BG)(AB) c4|(Bd)(BG) (FA)(FD)|(GA)(Bc) d2d2|B4 (BA)(GA)|
%
V:Flute_1
g4 (ag)(fe)|(fe)(fg) (ab)(^c'd')|b2g2e2^c2|(e4d4):|
V:Flute_2
(BG)(AB) ^c4|(d^c)(de) (fg)(af)|g2B2G2E2|(G4F4):|

```
### [wechat-format](https://github.com/lyricat/wechat-format)
微信公众号排版工具

### [howler.js](https://github.com/goldfire/howler.js)
音乐播放库

### [starship](https://github.com/starship/starship)
终端美化工具

### [free](https://github.com/freefq/free)
免费 VPN 节点

### [rustdesk](https://github.com/rustdesk/rustdesk)
远程桌面软件
