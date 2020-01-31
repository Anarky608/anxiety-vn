# act1

```
SceneSetup.act1();
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI

n: _BẠN_ LÀ SỰ LO ÂU

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Này! Chúng ta lại quay lại đây à?

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: SỰ THẬT LÀ, CHƠI LẠI TRÒ CHƠI NÀY ĐANG KHIẾN CÔ ẤY GẶP NGUY HIỂM NGAY BÂY GIỜ

n: NHANH LÊN, CẢNH BÁO CÔ ẤY ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Bạn ơi! Nghe này, chúng ta đang gặp nguy hiểm! Người chơi...

[...sẽ hành hạ chúng ta một lần nữa!](#act1_replay_torture)

[...sẽ không thể tìm ra một kết thúc thay thế!](#act1_replay_alternate)

[...sẽ thấy sự mâu thuẫn giữa lối chơi và cốt truyện!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Họ sẽ bắt chúng ta cuộn tròn như quả bóng và khóc!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Họ sẽ bắt chúng ta phá điện thoại của bạn vì đưa bạn vào cơn hoảng loạn!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Họ sẽ làm chúng ta *KHÔNG* đấm chủ bữa tiệc!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Họ sẽ bắt chúng ta đấm vào mặt chủ nhóm đồng cảm phản ác!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ít nhất chúng ta không phải nhảy mái nhà lần n--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: HỌ SẼ BẮT CHÚNG TA NHẢY KHỎI MÁI NHÀ.
{{/if}}

`bb({body:"fear"});`

b: TẤT CẢ NHỮNG ĐIỀU KHỦNG KHIÊP MỚI NÀY SẼ XẢY ĐẾN VỚI CHÚNG TA, VÀ CHÚNG TA SẼ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Vâng, câu chuyện nhìn *chung* là như nhau, nhưng mỗi chương có hai kết thúc, cộng với tất cả các lựa chọn đối thoại phân nhán--

`bb({body:"fear"});`

b: Người chơi sẽ thất vọng, đóng tab trình duyệt này, xóa phần mềm của chúng ta, và sau đó chúng ta sẽ--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Một điều ty tiện-gì đây?

`bb({eyes:"normal"});`

b: Cốt truyện mở rộng là cách bạn *CHỌN* để tạo ra sự hợp tác lành mạnh với nỗi sợ của bạn,

`bb({eyes:"normal_right"});`

b: Nhưng chơi lại trò chơi sẽ cho ra cùng một câu chuyện, nghĩa là *LỰA CHỌN* của bạn không còn quan trọng,

`bb({eyes:"narrow_eyebrow"});`

b: Cho thấy sự mâu thuẫn giữa thông điệp và cơ chế của trò chơi,

`bb({eyes:"fear"});`

b: Do đó làm sáng tỏ kết cấu của câu chuyện này,

`bb({body:"fear"});`

b: Và chúng ta sẽ--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTTT
   
```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Được rồi quay trở lại với nhân vật nào.

```
Game.clearText();
```

n4: (HÃY _ĐỂ_ SỰ LO ÂU CỦA BẠN BLA BLA BLA GIỐNG VỚI NỖI SỢ CỦA BẠN BLA BLA BẠN BIẾT RỒI ĐẤY)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Tuyệt, sói của tôi quay lại rồi. Tuyệệệệệệệệệt.                                   

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: THỰC TẾ LÀ, CHIẾC BÁNH KẸP ĐÓ ĐANG ĐƯA CÔ ẤY VÀO NGUY HIỂM

n: NHANH LÊN, CẢNH BÁO CÔ ẤY ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Bạn ơi! Nghe này, chúng ta đang gặp nguy hiểm! Mối nguy hiểm là...

`bb({body:"squeeze"})`

n4: (HÃY THỂ HIỆN SỰ LO ÂU CỦA _BẠN_. CHỌN CÁI GIỐNG VỚI CÁI MÀ NỖI SỢ MÁCH BẢO _BẠN_)

(#act1_normal_choice)

# act1_normal_choice

[Chúng ta đang ăn bữa trưa một mình! Một lần nữa!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Chúng ta không thể làm việc khi ăn!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Bánh mì trắng không tốt cho chúng ta!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Bạn có biết sự cô đơn có thể dẫn đến cái chết nhanh như khi ta hút 15 điếu thuốc lá một ngày?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ừm, rất cảm ơn lời trích dẫn của bạn nhưng--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Điều đó có nghĩa là nếu *ngay bây giờ* chúng ta không đi chơi với ai đó chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTTT
   
```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: BẠN ĐÃ DÙNG *NỖI SỢ BỊ BỎ RƠI*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Lấy laptop ra và làm chút việc ngay bây giờ đi!

`hong({eyes:"0_annoyed"})`

h: Ừm, mình không muốn vụn bánh rơi vào bàn ph--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nếu chúng ta không đóng góp gì cho xã hội thì chúng ta chỉ là một con kí sinh trùng xã hội thôi!

b: Xã hội sẽ tìm được liều thuốc để tiêu diệt những kí sinh trùng xã hội và rồi chúng ta sẽ--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CHẾTTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: BẠN ĐÃ SỬ DUNG *NỖI SỢ TRỞ THÀNH NGƯỜI XẤU*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Hình như những thông tin này đã được sao ché-

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Lúa mì qua chế biến sẽ làm tăng lượng đường trong máu của chúng ta, vì vậy họ sẽ cắt các chi của chúng ta và chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: BẠN ĐÃ SỬ DỤNG *NỖI SỢ BỊ TỔN THƯƠNG*

(#act1b)

# act1b

n: NÓ SIÊU HIỆU QUẢ

`bb({mouth:"smile", eyes:"smile"});`

b: Bạn thấy chưa? Tôi là con sói bảo vệ trung thành của bạn

`bb({body:"pride_talk"});`

b: Tin tưởng bản thân bạn đi! Cảm xúc của bạn luôn có giá trị!

`bb({body:"pride"});`

n: THANH NĂNG LƯỢNG CON NGƯỜI CỦA BẠN BỊ ĐƯA VỀ KHÔNG

n: ĐỂ BẢO VỆ NHU CẦU VẬT CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA BẠN, BẠN CÓ THỂ DÙNG:

n: NỖI SỢ *BỊ TỔN THƯƠNG* #harm#

n: NỖI SỢ *BỊ BỎ RƠI* #alone#

n: VÀ NỖI SỢ *TRỞ THÀNH NGƯỜI XẤU* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (PRO-TIP: CHỌN LỰA CHỌN ĐỘNG ĐẾN NỖI SỢ SÂU NHẤT, ĐEN TỐI NHẤT TRONG CON NGƯỜI BẠN!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: có lẽ đã đến lúc mình kiểm tra điện thoại của mình rồi.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: BẢO VỆ CON NGƯỜI CỦA BẠN.

n: KHỎI THẾ GIỚI. KHỎI NGƯỜI KHÁC. KHỎI CHÍNH HỌ.

n: CHÚC MAY MẮN

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: VÒNG MỘT: *CHIẾN ĐẤU!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Facebook nói là có một bữa tiệc diễn ra vào cuối tuần này.

`bb({eyes:"uncertain"});`

b: Trang web kì lạ đó lúc nào cũng tổ chức một bữa tiệc vào ngày cuối tuần à?

`bb({eyes:"uncertain_right"});`

b: Họ đang cố lấp đầy những khoảng trống nào vậy? Chắc họ đang bị gì đó từ bên trong rồi!

`hong({eyes:"surprise"});`

h: Và, mình có một lời mời?

`bb({eyes:"fear", mouth:"normal"});`

b: Vậy thì tốt!

[Chấp nhận đi, hoặc chúng ta sẽ chết vì cô đơn!](#act1c_loner)

[Đừng đi, nó có vẻ mờ ám!](#act1c_drugs)

[Mặc kệ đi, chúng ta chỉ làm bữa tiệc chán hơn thôi.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Mười lăm điếu thuốc lá một ngày đấy! Mười lăm!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Sau đó sẽ chẳng có ai đến dự đám tang của chúng ta, họ sẽ đổ tro của chúng ta xuống đại dương, cá voi sẽ ăn nó,
{{/if}}

{{if !_.fifteencigs}}
b: và chúng ta sẽ trở thành PHÂN CÁ VOI!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Thế nên chúng ta nên đến bữa tiệc đó!
{{/if}}

{{if _.parasite}}
b: Chỉ cần mang laptop theo để làm việc, và chúng ta sẽ không bị coi là những con ký sinh trùng xã hội.
{{/if}}

{{if _.whitebread}}
b: Chỉ cần họ không bày ra BÁNH MÌ TRẮNG là được
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: CHÚA ƠI. Nếu nó làm cậu im lặng, tốt thôi.

h: Mình sẽ đồng ý.

{{if _.whalepoop}}
b: Phân cá voi! Phân cá voi!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: hoặc thứ gì đó tệ hơn... BÁNH MÌ TRẮNG
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Chúng ta sẽ dùng quá liều hàng đá và bánh mì trắng và họ sẽ không thể nhét xác chết to béo của chúng ta vào lò hỏa táng!
{{/if}}

{{if !_.whitebread}}
b: Chúng ta sẽ dùng thuốc quá liều và người phục vụ lễ tang sẽ không biết vì sao cơ thể chúng ta lại bị ướp xác trước!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Còn nếu như không đến bữa tiệc, chúng ta sẽ phải làm việc hoặc chúng ta sẽ trở thành những con ký sinh trùng xã hội khủng khiếp!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: CHÚA ƠI. Nếu nó làm cậu im lặng, tốt thôi.

h: Mình sẽ từ chối.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tất cả những gì chúng ta làm là khóc về việc cô đơn chết người giống như hút 15 điếu thuốc một ngày à.
{{/if}}

{{if _.parasite}}
b: All we ever do at parties is worry about how we should be productive instead.
{{/if}}

{{if _.whitebread}}
b: All we ever do is worry about how the unhealthy food options are going to kill us.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: gee i wonder why.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: So if we go we'll make them feel bad, but if we reject their invite we'll also make them feel bad!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ALL WE DO IS MAKE PEOPLE FEEL BAD, SO WE SHOULD FEEL BAD

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. If it'll make you shut up, fine.

h: I'll ignore the invite.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Anyway. Facebook's too much. I need something calmer, less anxiety-producing.

`hong({eyes:"neutral"});`

h: What's new on Twitter?

`bb({eyes:"look"});`

[Oh no, look at that horrible news story!](#act1d_news)

[Oh no, is that tweet secretly about *us?*](#act1d_subtweet)

[Hey, a GIF of a cat drinking milk](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: God, it feels like the world's burning, isn't it?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: It feels like it's all ending, like everything's dying and we're doomed and there's nothing we can do about it.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Let's retweet that story!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Okay I'll retweet it just please be quiet!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Screw it, let's look at Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: It's a subtweet! A sneaky, sneaky subtweet!

`hong({eyes:"annoyed"});`

h: It's probably not?

`bb({eyes:"narrow", mouth:"small"});`

b: but what if they're all talking behind our back

h: They're n--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: IN FRONT OF OUR BACK

`hong({eyes:"sad", mouth:"sad"});`

h: I d--

`bb({eyes:"narrow", mouth:"small"});`

b: but *what if*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *what if*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, gonna try Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh ya that's cute, just retweeted it, I thi--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: CATS CAN'T DIGEST MILK AND WE'RE TERRIBLE PEOPLE FOR ENJOYING ANIMAL ABUSE

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, gonna try Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, photos from yesterday night. So *that's* what those weekly parties are like.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, looks way too crowded for my anxiety.

h: Maybe I shouldn't have said yes to the invite?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Change our answer? Like a jerk?!](#act1e_yes_dontchange)

[Change our answer! It's too crowded!](#act1e_yes_changetono)

{{if _.subtweet}}
[Yeah they were totally subtweeting us.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Wait we retweeted without fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[You know, you've got really bad posture?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: They were counting on us to come and now we're betraying their trust? Do you wanna die alone?!

{{if _.fifteencigs}}
b: FIFTEEN. CIGARETTES.
{{/if}}

{{if _.whalepoop}}
b: WHALE. POOP.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll keep it as yes!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Don't you know about human stampedes?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: In 2003 a Rhode Island nightclub had a fire and the panic made people jam the exits so 100 people burned to death-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: DO YOU WANT THAT TO HAPPEN TO US-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll change my answer to no! God!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... that looks really fun.

h: Maybe I shouldn't have said no to the invite?

`bb({mouth:"normal", eyes:"normal"});`

[Change our answer? Like a jerk?!](#act1e_no_dontchange)

[Change our answer! Don't die alone!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Yeah they were totally subtweeting us.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Wait we retweeted without fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[You know, you've got really bad posture?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Everybody was counting on us!

b: ...to leave them alone and let them have a nice party without a horrible disgusting {{if _.whitebread}}white-bread-munching{{/if}} creep like u--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll keep it as no!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chronic loneliness increases our cortisol levels as well as risk for cardiovascular disease and stroke!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: FIFTEEN. CIGARETTES.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll change my answer to yes! God!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: All our problematic tweets have come back to roost!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: We're gonna get called out and cancelled and dragged with a rope on horseback down the information superhighway!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Why are you like this?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: We're spreading disinformation! We're destroying trust in a free press!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: We're the reason fascism will arise from the rubble of democracy!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Why are you like this?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Do you want to have a pretzel for a spine?! Stop hunching over your screen!

```
bb({body:"meta"});
```

b: That means you too.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Why are you like this?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... that looks really fun.

h: Maybe I shouldn't have ignored the invite?

`bb({mouth:"normal", eyes:"normal"});`

[Keep ignoring, we're still party poopers.](#act1e_ignore_continue)

[Actually, say yes.](#act1e_ignore_changetoyes)

[Actually, say no.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: It's kinda rude to keep ignoring them though, no?

`bb({eyes:"normal_right"});`

b: Well other people always ignore *us*, so

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: so let's just call it even.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: You're... letting me have fun?

b: Well, I mean, loneliness *can* kill us.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: It's too crowded. Crowds are dangerous.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Whatever. New Tinder notification.

`bb({eyes:"uncertain"})`

b: What, that hookup app?

`hong({eyes:"annoyed"})`

h: It's not a hookup app, it's just a way to meet new peopl--

`bb({eyes:"narrow"})`

b: It's a hookup app.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, I got a match! They look cute!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Please don't ruin this for m--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: DANGER DANGER DANGER DANGER DANGER DANGER

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[We're being *used* by other people.](#act1f_used_by_others)

[We're just *using* other people.](#act1f_using_others)

[YOUR MATCH IS A SERIAL KILLER](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Random hookups may be able to fill the hole down there,

b: but they can never fill the hole...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: in *here*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: The point is WE'RE GOING TO DIE ALONE

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: You think other people's genitals are Pokémon for us to collect?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon theme song)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ I wanna be, the ^slut^ti-est-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Like no one ever was-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Thighs n' ^ass^, voluptuous breast-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ with sweaty ^dick^ and balls!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PERVY-MON! GOTTA CA-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: The point is we're a manipulative creep.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: They'll trap you in a well and force-feed you white bread to fatten you up so they can wear your skin like a suit!
{{/if}}

{{if _.parasite}}
b: They'll bludgeon you with a pomodoro timer and say "YOU SHOULDA BEEN MORE PRODUCTIVE YOU PARASITE"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: They'll tear your flesh to gory confetti, turn your entrails into streamers, and mix your blood into a punch bowl!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: How's THAT for a party invite?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: i'm so sick of this game.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"loneliness will kill us"... {{/if}}
{{if _.parasite}}"we're a society-parasite"... {{/if}}
{{if _.whitebread}}"don't eat that, it'll kill us"... {{/if}}
{{if _.subtweet}}"they're talking behind our back"... {{/if}}
{{if _.badnews}}"the world is burning"... {{/if}}
{{if _.hookuphole}}"we'll die alone"... {{/if}}
{{if _.serialkiller}}"they're a serial killer"... {{/if}}
{{if _.catmilk}}"cats can't digest milk"... {{/if}}
{{if _.pokemon}}a ^crappy^ parody song... {{/if}}

h: i just want to live my life.

h: i just want to be free from all this... pain.

`bb({eyes:"look_sad"});`

b: Hey... human...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: It'll be okay.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: As your loyal guard-wolf, I'll always keep an eye out for danger, and do my best to keep you safe.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: I promise.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Last app. Instagram. What you got?

`hong({eyes:"sad"});`

h: It's... more party pictures.

`hong({mouth:"sad"});`

h: Everyone looks so happy. Free from worry. Free from anxiety.

`hong({mouth:"anger"});`

h: God, why can't I be like them? Why can't I just be *normal?*

`bb({eyes:"normal_right"});`

b: Speaking of parties, about this weekend's invite. Here's my FINAL decision:

`bb({eyes:"normal"});`

[We should go.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[We should not go.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: We sh--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^FUCK^.*

`hong({body:"2_you"});`

h: YOU.

(...500)

b: w

(...1500)

`bb({eyes:"wat_2"});`

b: wha?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: I'm going to say YES to that party,

{{if _.act1g=="go"}}
h: NOT because you want me to, but because *I* want to.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisely BECAUSE you don't want me to.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: You're NOT in control of me.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Now excuse me while I eat this delicious sandwich in ^goddamn^ peace.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH WE'RE GONNA DIE](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH EVERYONE HATES US](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH WE'RE HORRIBLE PEOPLE](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH WE'RE GONNA DIE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH EVERYONE HATES US AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH WE'RE HORRIBLE PEOPLE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULATIONS

(...500)

n: YOU'VE SUCCESSFULLY PROTECTED YOUR HUMAN'S PHYSICAL + SOCIAL + MORAL NEEDS

n: WHY, LOOK HOW GRATEFUL THEY ARE!

(...500)

n: NOW THAT THEIR ENERGY IS ZERO, YOU CAN DIRECTLY CONTROL THEIR ACTIONS

`bb({mouth:"smile", eyes:"normal"});`

n: PICK YOUR ENDING MOVE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *FINISH THEM*

[{FIGHT: Punish your stressful phone!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: Curl up in a ball and cry!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Your phone was giving you a panic attack!

`bb({eyes:"anger"})`

b: Zuckerberg and Co are hijacking your mental health for venture capitalist money!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punish your phone! Destroy it! Kill it!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL I--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: The whole world is filled with danger!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Do like the armadillo! Curl up into a ball for self-defense!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CR-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`


