# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# Chơi! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_TIẾP TỤC_: Bữa tiệc](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_TIẾP TỤC_: Bữa tiệc khác](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_CONTINUE_: Chiếc bánh khác](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# CHƠI LẠI! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[Chọn Chương](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(ghi chú về nội dung)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[I. Chiếc Bánh](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[II. Bữa Tiệc](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[III. Bữa Tiệc Khác](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[III. Bữa Tiệc Khác]()
{{/if}}

{{if window.localStorage.act4}}
[IV. Chiếc Bánh Khác](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[III. Chiếc Bánh Khác]()
{{/if}}

{{if window.localStorage.credits}}
[V. Danh Đề](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[V. Danh Đề]()
{{/if}}

[(màn hình chính)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: Chào mừng! Đây không hẳn là một "trò chơi," đúng hơn là một câu chuyện tương tác. Mong bạn thích đọc nó, sucka!

n3: Vậy trước khi bắt đầu, *bạn* thích đọc thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Tuyệt! Ghi chú: bạn luôn có thể thay đổi lựa chọn với biểu tượng ⚙ bên dưới. Hơn nữa, trò chơi tự động lưu tại mỗi chương!

n3: Bây giờ, hãy bắt đầu câu chuyện của chúng ta...

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT GÁI

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`
