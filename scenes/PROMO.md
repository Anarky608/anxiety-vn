# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Trước khi chúng ta bắt đầu, *bạn* muốn đọc như thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Bây giờ, hãy bắt đầu câu chuyện của chúng ta...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT CON NGƯỜI

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

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI

n: _BẠN_ LÀ SỰ LO ÂU

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Không. Không, không, không nghe. Mình sẽ kiểm tra điện thoại.
```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gasp! Bạn lại cuốn cuộc sống của bạn đi trên Twitter! Lần nữa!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ừ mình không hiểu tại sao mình không ngồi và lắng nghe những suy nghĩ của mình thường xuyên hơn

`hong({eyes:"neutral"});`

n: NHANH LÊN, CẢNH BẢO CÔ ẤY VỀ MỘT *NGUY HIỂM*

```
bb({eyes:"look"});
```

[Ôi không, nhìn vào tin tức kinh khủng đó đi!](#act1d_news)

[Ôi không, bài tweet đó nói về bí mật giữa chúng ta à?](#act1d_subtweet)

[Này, một GIF về một con mèo uống sữa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Thật dễ thương, mình--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG TIÊU HÓA ĐƯỢC SỮA VÀ CHÚNG TA LÀ NHỮNG CON NGƯỜI TỒI TỆ VÌ NGƯỢC ĐÃI ĐỘNG VẬT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```

