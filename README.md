# ramdom-music
需要mido,random


透過ramdom隨機設定音樂的節奏
以及音符數量、音量等
最後轉成midi檔輸出

       track.append(mido.Message('program_change', program=10, time=0))    program代表使用的樂器
        pitch_list[i] = [random.randint(70, 80) for t2 in range(note_num)] 此為ramdom音量的上下限
        vel_list[i] = [random.randint(50, 80) for t3 in range(note_num)]   此為ramdom音高的上下限


--附midi音色表
音色表
鋼琴

0 Acoustic Grand Piano 大鋼琴（聲學鋼琴）

1 Bright Acoustic Piano 明亮的鋼琴

2 Electric Grand Piano 電鋼琴

3 Honky-tonk Piano 酒吧鋼琴

4 Rhodes Piano 柔和的電鋼琴

5 Chorused Piano 加合唱效果的電鋼琴

6 Harpsichord 羽管鍵琴（撥弦古鋼琴）

7 Clavichord 科拉維科特琴（擊弦古鋼琴）

色彩打擊樂器

8 Celesta 鋼片琴

9 Glockenspiel 鍾琴

10 Music box 八音盒

11 Vibraphone 顫音琴

12 Marimba 馬林巴

13 Xylophone 木琴

14 Tubular Bells 管鐘

15 Dulcimer 大揚琴

風琴

16 Hammond Organ 擊桿風琴

17 Percussive Organ 打擊式風琴

18 Rock Organ 搖滾風琴

19 Church Organ 教堂風琴

20 Reed Organ 簧管風琴

21 Accordian 手風琴

22 Harmonica 口琴

23 Tango Accordian 探戈手風琴

吉他

24 Acoustic Guitar (nylon) 尼龍弦吉他

25 Acoustic Guitar (steel) 鋼弦吉他

26 Electric Guitar (jazz) 爵士電吉他

27 Electric Guitar (clean) 清音電吉他

28 Electric Guitar (muted) 悶音電吉他

29 Overdriven Guitar 加驅動效果的電吉他

30 Distortion Guitar 加失真效果的電吉他

31 Guitar Harmonics 吉他和音

貝司

32 Acoustic Bass 大貝司（聲學貝司）

33 Electric Bass(finger) 電貝司（指彈）

34 Electric Bass (pick) 電貝司（撥片）

35 Fretless Bass 無品貝司

36 Slap Bass 1 掌擊Bass 1

37 Slap Bass 2 掌擊Bass 2

38 Synth Bass 1 電子合成Bass 1

39 Synth Bass 2 電子合成Bass 2

弦樂

40 Violin 小提琴

41 Viola 中提琴

42 Cello 大提琴

43 Contrabass 低音大提琴

44 Tremolo Strings 弦樂群顫音音色

45 Pizzicato Strings 弦樂群撥弦音色

46 Orchestral Harp 豎琴

47 Timpani 定音鼓

合奏/合唱

48 String Ensemble 1 弦樂合奏音色1

49 String Ensemble 2 弦樂合奏音色2

50 Synth Strings 1 合成弦樂合奏音色1

51 Synth Strings 2 合成弦樂合奏音色2

52 Choir Aahs 人聲合唱“啊”

53 Voice Oohs 人聲“嘟”

54 Synth Voice 合成人聲

55 Orchestra Hit 管弦樂敲擊齊奏

銅管

56 Trumpet 小號

57 Trombone 長號

58 Tuba 大號

59 Muted Trumpet 加弱音器小號

60 French Horn 法國號（圓號）

61 Brass Section 銅管組（銅管樂器合奏音色）

62 Synth Brass 1 合成銅管音色1

63 Synth Brass 2 合成銅管音色2

簧管

64 Soprano Sax  高音薩克斯風

65 Alto Sax 次中音薩克斯風

66 Tenor Sax  中音薩克斯風

67 Baritone Sax 低音薩克斯風

68 Oboe 雙簧管

69 English Horn 英國管

70 Bassoon 巴松（大管）

71 Clarinet 單簧管（黑管）

笛

72 Piccolo 短笛

73 Flute 長笛

74 Recorder 豎笛

75 Pan Flute 排簫

76 Bottle Blow [中文名稱暫缺]

77 Shakuhachi 日本尺八

78 Whistle 口哨聲

79 Ocarina   奧卡雷那

合成主音

80 Lead 1 (square)  合成主音1（方波）

81 Lead 2 (sawtooth) 合成主音2（鋸齒波）

82 Lead 3 (caliope lead) 合成主音3

83 Lead 4 (chiff lead) 合成主音4

84 Lead 5 (charang)  合成主音5

85 Lead 6 (voice) 合成主音6（人聲）

86 Lead 7 (fifths) 合成主音7（平行五度）

87 Lead 8 (bass+lead)合成主音8（貝司加主音）

合成音色

88 Pad 1 (new age) 合成音色1（新世紀）

89 Pad 2 (warm)  合成音色2（溫暖）

90 Pad 3 (polysynth)  合成音色3

91 Pad 4 (choir) 合成音色4（合唱）

92 Pad 5 (bowed) 合成音色5

93 Pad 6 (metallic) 合成音色6（金屬聲）

94 Pad 7 (halo)  合成音色7（光環）

95 Pad 8 (sweep) 合成音色8

合成效果

96 FX 1 (rain) 合成效果1雨聲

97 FX 2 (soundtrack) 合成效果2音軌

98 FX 3 (crystal) 合成效果3水晶

99 FX 4 (atmosphere) 合成效果4大氣

100 FX 5 (brightness) 合成效果5明亮

101 FX 6 (goblins) 合成效果6鬼怪

102 FX 7 (echoes)  合成效果7迴聲

103 FX 8 (sci-fi)  合成效果8科幻

民間樂器

104 Sitar 西塔爾（印度）

105 Banjo 班卓琴（美洲）

106 Shamisen  三昧線（日本）

107 Koto 十三弦箏（日本）

108 Kalimba 卡林巴

109 Bagpipe 風笛

110 Fiddle 民族提琴

111 Shanai 山奈

打擊樂器

112 Tinkle Bell 叮噹鈴

113 Agogo [中文名稱暫缺]

114 Steel Drums 鋼鼓

115 Woodblock 木魚

116 Taiko Drum 太鼓

117 Melodic Tom 通通鼓

118 Synth Drum  合成鼓

119 Reverse Cymbal 銅鈸

Sound Effects 聲音效果

120 Guitar Fret Noise 吉他換把雜音

121 Breath Noise 呼吸聲

122 Seashore 海浪聲

123 Bird Tweet 鳥鳴

124 Telephone Ring 電話鈴

125 Helicopter 直升機

126 Applause 鼓掌聲

127 Gunshot 槍聲


以下為產生結果的範例
https://www.midishow.com/zh-tw/midi/ramdom-midi-download-161793

如果你沒有midishow帳號,你可以嘗試使用google雲端來下載
https://drive.google.com/drive/folders/1Q1DieAoV8QD8tQaJxovg4h_Sp-euVonG?usp=sharing
