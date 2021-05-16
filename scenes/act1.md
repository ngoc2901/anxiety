# act1

```
SceneSetup.act1();
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO SỢ CỦA CÔ ẤY

n: _BẠN_ LÀ SỰ LO SỢ ĐẤY

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Này! Chúng ta quay lại đây nữa à?

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: THỰC RA, CHƠI LẠI TRÒ NÀY LÀ ĐỂ HỌ VÀO *NGUY HIỂM* NGAY BÂY GIỜ

n: NHANH, CẢNH BÁO HỌ ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe này, chúng ta đang gặp nguy hiểm! Người chơi...

[...sẽ tra tấn chúng ta lần nữa!](#act1_replay_torture)

[...sẽ không tìm thấy được kết cục tiếp!](#act1_replay_alternate)

[...sẽ thấy sự mâu thuẫn giữa cốt chuyện và game!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Họ sẽ khiến chúng ta co lại thành quả bóng và khóc!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Họ sẽ khiến chúng ta phá điện thoại bạn vì đưa bạn vào cơn hoảng loạn!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Họ sẽ khiến chúng ta *KHÔNG* đấm chủ bữa tiệc!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Họ sẽ khiến chúng ta đấm chủ bữa tiệc phản diện đồng cảm!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ít nhất họ không khiến ta nhảy từ mái nhà xuống lần nà--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: HỌ SẼ KHIẾN TA NHẢY TỪ MÁI NHÀ XUỐNG.
{{/if}}

`bb({body:"fear"});`

b: TẤT CẢ NHỮNG CHUYỆN KINH KHỦNG ĐÓ SẼ XẢY RA VỚI TA, VÀ TA SẼ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Đúng, câu chuyện nhìn *chung* là như nhau, nhưng mỗi chương có hai cái kết, cộng với cả những lựa chọn phân nhá--

`bb({body:"fear"});`

b: Người chơi sẽ thất vọng, đóng tab trình duyệt này, xoá phần mềm của chúng ta, và ta sẽ--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Mâu thuẫn- gì ?

`bb({eyes:"normal"});`

b: Cốt chuyện mở rộng là cách bạn *CHỌN* để tạo ra sự hợp tác tốt đẹp với nỗi sợ của bạn,

`bb({eyes:"normal_right"});`

b: Nhưng chơi lại trò chơi sẽ đưa ra câu chuyện như vậy, thể hiện *LỰA CHỌN* của bạn không quan trọng,

`bb({eyes:"narrow_eyebrow"});`

b: Nên thấy được sự mâu thuẫn giữa thông điệp và cơ chế của trò ,

`bb({eyes:"fear"});`

b: Như vậy làm sáng tỏ kết cấu của vũ trụ này,

`bb({body:"fear"});`

b: Và ta sẽ--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

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

h: OK quay lại nhân vật nào.

```
Game.clearText();
```

n4: (ĐỂ SỰ LO ÂU CỦA _BẠN_ BLAH BLAH BLAH GIỐNG VỚI NỖI SỢ CỦA _BẠN_ NHẤT BLAH BLAH BẠN BIẾT RỒI ĐẤY)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ôi tuyệt, sói của tôi đã quay lại. Tuyyyyệt vời.

`hong({eyes:"0_neutral"})`

n: CÔNG VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: TRONG THỰC TẾ, CHIẾC BÁNH KẸP ĐÓ ĐANG ĐẶT *NGUY HIỂM* CHO CẬU ẤY NGAY BÂY GIỜ

n: NHANH, CẢNH BÁO ĐI!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe đây, chúng ta đang gặp nguy hiểm! Nguy hiểm là...

`bb({body:"squeeze"})`

n4: (HÃY THỂ HIỆN SỰ LO ÂU CỦA _BẠN_! CHỌN CÁI GIỐNG NHẤT VỚI NỖI SỢ CỦA _BẠN_ MÁCH BẢO BẠN)

(#act1_normal_choice)

# act1_normal_choice

[Chúng ta lại ăn trưa một mình! Lần nữa!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Chúng ta không năng động lúc ăn!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Bánh trắng đó không tốt cho ta!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Bạn biết rằng cô đơn tương đương với chết sớm như khi ta hút 15 điếu thuốc lá một ngày?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ờ, cảm ơn vì đã trích dẫn nguồn của bạn nhưng--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Vậy nên nếu ta không bắt chuyện với ai đó *ngay bây giờ* ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: BẠN DÙNG *SỢ KHÔNG ĐƯỢC YÊU THƯƠNG*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Lấy máy ra và làm chút việc ngay bây giờ!

`hong({eyes:"0_annoyed"})`

h: Ờ, Mình không thích vụn bánh rơi vào bàn phí--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nếu ta không góp phần của mình cho cơ thể của xã hội thì ta sẽ là kí sinh trùng của xã hội!

b: Cơ thể của xã hội sẽ tới bác sĩ của xã hội để chữa trị để giết kí sinh trùng của xã hội rồi ta sẽ--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: BẠN DÙNG *SỢ TRỞ THÀNH NGƯỜI XẤU*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Hình như thông tin này đã được sửa--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Lúa mì chế biến sẽ đóng đường trong máu nên họ sẽ cắt đi các chi của ta và ta sẽ-

`bb({body:"panic"})`

b: CHẾTTTTTTTTTTTTTTTTT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: BẠN DÙNG *SỢ BỊ HẠI*

(#act1b)

# act1b

n: NÓ RẤT CÓ HIỆU QUẢ

`bb({mouth:"smile", eyes:"smile"});`

b: Thấy chưa, con người? Tôi là sói bảo vệ trung thành của cậu!

`bb({body:"pride_talk"});`

b: Tin vào tâm hồn mình đi! Cảm xúc của bạn luôn có giá trị!

`bb({body:"pride"});`

n: LÀM CHO THANH NĂNG LƯỢNG CỦA CON NGƯỜI XUỐNG KHÔNG

n: DỂ BẢO VỆ NHU CẦU VỀ THỂ CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA HỌ , BẠN CÓ THỂ DÙNG:

n: SỢ *BỊ HẠI* #harm#

n: SỢ *KHÔNG ĐƯỢC YÊU THƯƠNG* #alone#

n: VÀ SỢ *TRỞ THÀNH NGƯỜI XẤU* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (GỢI Ý: SỬ DỤNG LỰA CHỌN ĐÁNH TRÚNG NỖI SỢ SÂU NHẤT, ĐEN TỐI NHẤT CỦA BẠN!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: bạn biết không mình nên xem điện thoại đây

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: BẢO VỆ CON NGƯỜI CỦA BẠN

n: KHỎI THẾ GIỚI. KHỎI NGƯỜI KHÁC. KHỎI CHÍNH HỌ.

n: CHÚC MAY MẮN

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: VÒNG MỘT: *CHIẾN!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. trang Facebook nói là có bữa tiệc lúc cuối tuần này.

`bb({eyes:"uncertain"});`

b: Hình như thằng kỳ lạ đó *luôn* tổ chức bữa tiệc mỗi ngày cuối tuần?

`bb({eyes:"uncertain_right"});`

b: Họ cố gắng lấp cái khoảng trống nào? Họ chắc là hỗn loạn từ bên trong rồi!

`hong({eyes:"surprise"});`

h: Với lại, mình có lời mời?

`bb({eyes:"fear", mouth:"normal"});`

b: Được rồi!

[Nói có, hoặc ta sẽ chết vì cô đơn!](#act1c_loner)

[Nói không, nó có cả đống thuốc độc!](#act1c_drugs)

[Bỏ qua đi, ta sẽ làm bữa tiệc buồn.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Mười lăm điếu thuốc một ngày, con người! Mười lăm!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Sau đó không ai sẽ tới đám tang của ta, họ sẽ vứt than của ta xuống biển, ta sẽ bị ăn bởi cá voi,
{{/if}}

{{if !_.fifteencigs}}
b: và ta sẽ thành PHÂN CÁ VOI!
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
b: Nên đúng ta phải tới bữa tiệc!
{{/if}}

{{if _.parasite}}
b: Chỉ cần mang laptop để ta làm việc, và không trở thành kí sinh trùng của xã hội.
{{/if}}

{{if _.whitebread}}
b: Chỉ cần ít nhất họ không phục vụ BÁNH MÌ TRẮNG
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TRỜI. Nếu nó làm cậu im mồm thì được rồi.

h: Mình sẽ nói có.

{{if _.whalepoop}}
b: Phân cá voi, con người! Phân cá voi!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: hoặc tệ hơn... BÁNH MÌ TRẮNG
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Ta sẽ quá liều vì quá nhiều cần và bánh mì trắng họ sẽ không cho vừa cái xác béo của ta vào lò hoả !
{{/if}}

{{if !_.whitebread}}
b: Ta sẽ quá liều vì quá nhiều thuốc phục vụ tang lễ  sẽ bất ngờ rằng xác của ta *đã* được ướp như thế nào!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Hơn nữa, không thể chơi, ta phải làm việc hoặc ta là kí sinh trùng tồi tệ của xã !
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TRỜI. Nếu nó làm cậu im mồm thì được.

h: Mình sẽ nói không.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tất cả ta làm là khóc ở góc tường về cách cô đơn chết người như hút 15 điếu thuốc.
{{/if}}

{{if _.parasite}}
b: Tất cả ta thay vì làm ở bữa tiệc là lo về làm thế nào để ta năng đọng.
{{/if}}

{{if _.whitebread}}
b: Tất cả ta làm là lo về lựa chọn đồ ăn không bổ dưỡng sẽ giết ta.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: trời mình không hiểu sao.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Nên nếu ta đi ta sẽ làm họ thấy tệ, nhưng nếu ta từ chối lời mời của họ ta vẫn sẽ làm họ thấy tệ!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TẤT CẢ TA LÀM LÀ LÀM HỌ THẤY TỆ, NÊN TA CẦN THẤY TỆ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Nếu nó làm cậu im mồm thì được.

h: Mình sẽ bỏ qua lời .

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Dù sao. Facebook quá nhiều rồi. Mình cần làm gì bình tĩnh hơn, ít gây ra lo âu .

`hong({eyes:"neutral"});`

h: Cái gì mới trên Twitter?

`bb({eyes:"look"});`

[Ôi không, đọc tin tức kinh khủng kia đi!](#act1d_news)

[Ôi không, hình như tweet kia bí mật nói về *ta?*](#act1d_subtweet)

[Này, một GIF về mèo đang uống sữa](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Trời, nó cảm thấy như thế giới đang cháy, đúng không?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Nó cảm thấy như đó tất cả là kết thúc, như mọi thứ chết dần và ta chết và ta không thể làm gì với nó.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Hãy tweet lại tin tức đó!

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

h: Được rồi mình sẽ tweet lại chỉ cần làm ơn im!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Bỏ qua đi, lên Snapchat .

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Nó là một phụ đề! Một phụ đề thầm kín!

`hong({eyes:"annoyed"});`

h: Nó có lẽ là không?

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng chuyện gì nếu họ đều nói sau lưng chúng ta

h: Họ kh--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: TRƯỚC LƯNG CHÚNG TA

`hong({eyes:"sad", mouth:"sad"});`

h: Mình k--

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng *nếu*

h: T--

`bb({eyes:"narrow_eyebrow"});`

b: *nếu*

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

h: được- RỒI, thử lên Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Nó đáng yêu vậy trời, chỉ cần tweet lại nó, mình ng--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HOÁ SỮA VÀ TA LÀ NGƯỜI KHỦNG KHIẾP VÌ THƯỞNG THỨC HÀNH HẠ ĐỘNG VẬT

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

h: được- RỒI, thử lên Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, ảnh từ tối qua. Vậy *đó là* bữa tiệc hàng tuần là thế.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, trông quá đông cho sự lo âu rồi.

h: Có thể mình không nên nói có cho lời mời?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Đổi đáp án? Như là chó?!](#act1e_yes_dontchange)

[Đổi đáp án đi! Nó quá đông!](#act1e_yes_changetono)

{{if _.subtweet}}
[Đúng họ chắc đang phụ đề mình.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Đợi đã ta tweet lại mà không kiểm tra thông tin.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Bạn biết không, bạn có một tư thế xấu?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Họ đang trông đợi chúng tôi đến và bây giờ chúng tôi đang phản bội lòng tin của họ? Bạn có muốn chết một mình không?!

{{if _.fifteencigs}}
b: MƯỜI LĂM. HÀNG HÓA.
{{/if}}

{{if _.whalepoop}}
b: BÁN HÀNG. DỪNG LẠI.
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

h: Im đi, tôi sẽ giữ nó như có!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bạn không biết về người đóng dấu?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Năm 2003, một hộp đêm ở Rhode Island đã xảy ra hỏa hoạn và sự hoảng loạn khiến mọi người kẹt cứng các lối ra nên 100 người bị chết cháy-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: BẠN CÓ MUỐN ĐẾN VỚI CHÚNG TÔI KHÔNG-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG NÓI KHÔNG N-


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

h: Im đi, tôi sẽ thay đổi câu trả lời của tôi thành không! Chúa Trời!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... nó trông cũng vui đó.

h: Có thể mình không nên nói không về lời mời?

`bb({mouth:"normal", eyes:"normal"});`

[Đổi đáp án? Như là chó?!](#act1e_no_dontchange)

[Đổi đáp án đi! Đừng chết một mình!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Đúng họ chắc đang phụ đè mình.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Đợi đã ta tweet lại mà không kiểm tra thông tin.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Bạn biết không, bạn đang có một tư thế xấu?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Mọi người đã tin tưởng vào chúng tôi!

b: ...để họ yên và để họ có một bữa tiệc vui vẻ mà không có một tên ghê tởm {{if _.whitebread}}white-bread-munching{{/if}} khủng khiếp như bạn--


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

h: Im đi, tôi sẽ giữ nó như không!

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

h: Hm... nó trông cũng vui đó.

h: Có lẽ mình không nên bỏ qua lời mời đó?

`bb({mouth:"normal", eyes:"normal"});`

[Tiếp tục bỏ qua, ta vẫn là kẻ phá bữa tiệc.](#act1e_ignore_continue)

[Thật ra, nói có đi.](#act1e_ignore_changetoyes)

[Thật ra, nói không đi.](#act1e_ignore_changetono)

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

b: Chúng  sh--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^ĐỆT^.*

`hong({body:"2_you"});`

h: MẸ.

(...500)

b: cái

(...1500)

`bb({eyes:"wat_2"});`

b: cái gì vậy?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Tôi sẽ nói CÓ với bên đó,

{{if _.act1g=="go"}}
h: KHÔNG phải vì bạn muốn tôi, mà bởi vì *tôi* muốn.
{{/if}}

{{if _.act1g=="dont"}}
h: Chính xác VÌ bạn không muốn tôi.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Bạn KHÔNG kiểm soát tôi.

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

[AHHHH CHÚNG TÔI ĐANG CHẾT](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH MỌI NGƯỜI GHÉT CHÚNG TÔI](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH CHÚNG TÔI LÀ NHỮNG NGƯỜI KHỔNG LỒ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CHÚNG TÔI ĐANG CHẾT AAAAAAHHHHHHH

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

b: AHHHH MỌI NGƯỜI GHÉT CHÚNG TÔI AAAAAAHHHHHHH

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

b: AHHHH CHÚNG TÔI LÀ NHỮNG NGƯỜI KHỔNG LỒ AAAAAAHHHHHHH

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

n: BẠN ĐÃ BẢO VỆ THÀNH CÔNG CÁC NHU CẦU VỀ THỂ CHẤT + XÃ HỘI + SỨC MẠNH CỦA CON NGƯỜI

n: TẠI SAO, HÃY XEM CHÚNG TỐT ĐẸP NHƯ THẾ NÀO!

(...500)

n: BÂY GIỜ NĂNG LƯỢNG CỦA HỌ LÀ KHÔNG CÓ, BẠN CÓ THỂ KIỂM SOÁT TRỰC TIẾP HÀNH ĐỘNG CỦA HỌ

`bb({mouth:"smile", eyes:"normal"});`

n: PICK DI CHUYỂN KẾT THÚC CỦA BẠN

`bb({mouth:"small_lock", eyes:"fear"});`

n: *FINISH THEM*

[{FIGHT: Hãy trừng phạt điện thoại căng thẳng của bạn!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: Cuộn tròn trong một quả bóng và khóc!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Điện thoại của bạn đang mang đến cho bạn một cuộc tấn công hoảng loạn!

`bb({eyes:"anger"})`

b: Zuckerberg và Co đang chiếm đoạt sức khỏe tinh thần của bạn để lấy tiền đầu tư mạo hiểm!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Hãy trừng phạt điện thoại của bạn! Phá hủy nó! Giết nó!
```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT NÓ GIẾT N--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Cả thế giới tràn ngập nguy hiểm!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Làm như armadillo! Cuộn tròn vào một quả bóng để tự vệ!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: CUỘN TRÒN LÊN VÀ KHÓC CUỘN TRÒN LÊN VÀ KHÓC CUỘN TRÒN LÊN VÀ KHÓC CUỘN TRÒN LÊN VÀ KHÓC CUỘN TRÒN LÊN VÀ KHÓC CUỘN TRÒN LÊN VÀ KH--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
