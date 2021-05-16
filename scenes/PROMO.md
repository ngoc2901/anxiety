# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[CHƠI!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Vậy trước khi bắt đầu, *bạn* thích đọc như thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Bây giờ, hãy bắt đầu câu chuyện của chúng ta...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT  GÁI

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO SỢ CỦA CÔ ẤY

n: _BẠN_ LÀ SỰ LO SỢ ĐẤY

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Không. Không, không, không nghe. Mình sẽ xem điện thoại.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gasp! Bạn cuốn cuộc sống của bạn đi trên Twitter! Lần nữa!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ừ mình không hiểu sao mình không chỉ cần ngồi và nghe suy nghĩ của mình nhiều hơn.

`hong({eyes:"neutral"});`

n: NHANH, CẢNH BÁO HỌ VỀ *NGUY HIỂM!*

```
bb({eyes:"look"});
```

[Ôi không, đọc tin tức kinh khủng kia!](#act1d_news)

[Ôi không, có phải tweet kia bí mật nói về *mình?*](#act1d_subtweet)

[Này, một GIF về con mèo uông sữa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Nó đáng yêu quá trời, mình--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HOÁ SỮA VÀ VÀ CHÚNG TA LÀ NGƯỜI KINH KHỦNG VÌ THƯỞNG THỨC HÀNH HẠ ĐỘNG VẬT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



