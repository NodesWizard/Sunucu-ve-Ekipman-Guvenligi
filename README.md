<article>
<div class="l">
<div class="l">
<section>
<div class="ia ib ic id ie">
<ul class="">
<li id="6bd9" class="je jf ih jg b jh ji jj jk jl jm jn jo jp jq jr js jt ju jv gi" data-selectable-paragraph="">
<div class="o dy">
<div class="en cf fa fb fc fd fe ff fg fh fi">
<article>
<div class="l">
<div class="l">
<section>
<div>
<div class="jf lt lu lv lw">
<p id="422f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Yaptığımız kurulumlarda&nbsp;<strong class="kf gw">G&uuml;venlik</strong>&nbsp;en &ouml;nemli unsurlardan biridir&hellip;Eğerki g&uuml;venliğiniz zayıf kalırsa bu hem sizin i&ccedil;in hemde&nbsp;<strong class="kf gw">Validat&ouml;r</strong>&nbsp;olduğunuz yer i&ccedil;in sorun olacaktır&hellip; Herhangi bir&nbsp;<strong class="kf gw">g&uuml;venlik zaafiyeti</strong>&nbsp;b&uuml;y&uuml;k hasarlara ve zararlara sebep olabilir&hellip;</p>
<p id="bebe" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">NodesWizard</strong>&nbsp;ekibi olarak&nbsp;<strong class="kf gw">Mainnet</strong>&nbsp;ve&nbsp;<strong class="kf gw">Testnet</strong>&nbsp;kurulumlarımızda aldığımız &ouml;nlemleri sizler i&ccedil;in derledik ;</p>
<p id="3f8f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">1&mdash; Sisteminizin G&uuml;ncel</strong>&nbsp;olması en &ouml;nemli g&uuml;venlik unsularından biridir (Testnet ve Mainnet)</p>
<p id="9f56" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Aşağıdaki&nbsp;<strong class="kf gw">kod</strong>&nbsp;ile sisteminizi g&uuml;ncelleyin</p>
<pre class="te tf tg th ti tj bt tk"><span id="018e" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo apt-get update -y &amp;&amp; sudo apt dist-upgrade -y<br />sudo apt-get autoremove<br />sudo apt-get autoclean</span></pre>
<p id="b628" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">G&uuml;ncellemeleri&nbsp;<strong class="kf gw">otomatik</strong>&nbsp;olarak etkinleştirin .. B&ouml;ylece manuel olarak kontrol etmek zorunda kalmayacaksınız&hellip; Bir onay &ccedil;ıkarsa&nbsp;<strong class="kf gw">yes</strong>&nbsp;diyebilirsiniz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="9165" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo apt-get install unattended-upgrades<br />sudo dpkg-reconfigure -plow unattended-upgrades</span></pre>
<p id="b42a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">2 &mdash; Sudo</strong>&nbsp;ayrıcalıklarına sahip başka bir kullanıcı oluşturun.</p>
<p id="51ea" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">root</strong>&nbsp;olmayan bir hesap kullanmayı alışkanlık haline getirin..<strong class="kf gw">Sunucu</strong>&nbsp;g&uuml;venliğini sağlamak i&ccedil;in sık sık&nbsp;<strong class="kf gw">root</strong>&nbsp;olarak oturum a&ccedil;ılmamalıdır..</p>
<p id="83fd" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">aşağıdaki kod ile yeni bir kullanıcı oluşturun&nbsp;<strong class="kf gw">nodeswizard</strong>&nbsp;yerine istediğiniz isim yazabilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="cdfc" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo useradd -m -s /bin/bash <strong class="tn gw">nodeswizard</strong></span></pre>
<p id="b56f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">daha</strong>&nbsp;sonra bir şifre belirleyin</p>
<pre class="te tf tg th ti tj bt tk"><span id="71c5" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo passwd <strong class="tn gw">nodeswizard</strong></span></pre>
<p id="f658" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">oluşturduğunuz yeni</strong>&nbsp;kullanıcıyı sudo grubuna ekleyin</p>
<pre class="te tf tg th ti tj bt tk"><span id="a00d" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo usermod -aG sudo <strong class="tn gw">nodeswizard</strong></span></pre>
<p id="cd4a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki</strong>&nbsp;kod ile root hesabını devre dışı bırakınız.</p>
<pre class="te tf tg th ti tj bt tk"><span id="3281" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo passwd -l root</span></pre>
<p id="6d5a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">ileride</strong>&nbsp;tekrardan etkinleştirmek isterseniz aşağıdaki kodu kullanabilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="b389" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo passwd -u root</span></pre>
<p id="3fab" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra sunucunuza oluşturduğunuz&nbsp;<strong class="kf gw">yeni kullanıcı adı</strong>&nbsp;ve&nbsp;<strong class="kf gw">şifre</strong>&nbsp;ile giriş yapabilirsiniz..</p>
<p id="c908" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">&ouml;rnek ;</strong></p>
<p id="d378" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">kullanıcı adı :&nbsp;<strong class="kf gw">nodeswizard</strong></p>
<p id="21f9" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">şifre : a<strong class="kf gw">kobaba1598753</strong></p>
<p id="78c2" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">3&mdash;&nbsp;</strong>SSH Anahtarı ile bağlanma (Testnet ve Mainnet)</p>
<p id="722a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Sunucumuza&nbsp;<strong class="kf gw">bağlanırken</strong>&nbsp;ilk alacağımız &ouml;nlem&nbsp;<strong class="kf gw">SSH key</strong>&nbsp;ile bağlanmak olacaktır..Ayrıca&nbsp;<strong class="kf gw">şifre</strong>&nbsp;ile giriş işleminide&nbsp;<strong class="kf gw">devre dışı</strong>&nbsp;bırakacağız..</p>
<ul class="">
<li id="1c07" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">&Ouml;ncelikle&nbsp;<strong class="kf gw">SSH key</strong>imizi oluşturma ile başlıyalım.</li>
</ul>
<p id="6181" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Putygen</strong>&nbsp;ile ilk &ouml;nce key oluşturuyoruz.. işaretlediğimiz yeri&nbsp;<strong class="kf gw">4096&nbsp;</strong>olarak değiştiriyoruz ve&nbsp;<strong class="kf gw">Genarate</strong>&nbsp;diyerek key oluşturma işlemini başlatıyoruz&hellip;Key oluşturma işlemi devam ederken bitene kadar&nbsp;<strong class="kf gw">mouse</strong>&rsquo;nizi sağa sola hareket ettiriniz yoksa&nbsp;<strong class="kf gw">ilerlemez</strong>..</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zc"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/598/1*Cw_3VwcS5T10GkQ6hNGyxw.png" alt="" /></div>
</figure>
<p id="846f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Key</strong>&nbsp;oluştukdan sonra sunucumuzu &ccedil;ok daha g&uuml;venli hale getirmek i&ccedil;in şifre belirliyoruz..Burayı&nbsp;<strong class="kf gw">boş</strong>&nbsp;bırakabilirsiniz ama biz şifre yazmanızı&nbsp;<strong class="kf gw">&ouml;neriyoruz..&nbsp;</strong>Daha sonra<strong class="kf gw">&nbsp;Save Private key&nbsp;</strong>diyip herhangi bir&nbsp;<strong class="kf gw">isim</strong>&nbsp;belirliyoruz ve masa&uuml;st&uuml;ne kaydediyoruz&hellip;</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zd"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/603/1*IzQKmrasxQoauOWf_kKUDw.png" alt="" /></div>
</figure>
<p id="257b" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Şimdi Sunucumuza bağlanıyoruz..Sunucumuza&nbsp;<strong class="kf gw">şifre</strong>&nbsp;ile bağlandıkdan sonra&nbsp;<strong class="kf gw">.ssh</strong>&nbsp;klas&ouml;r&uuml; oluşturuyoruz&hellip;<strong class="kf gw">Eğer</strong>&nbsp;daha &ouml;nceden b&ouml;yle klas&ouml;r&uuml;n&uuml;z varsa diğer adımlardan devam edebilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="985b" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">mkdir .ssh</span></pre>
<p id="90d8" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra&nbsp;<strong class="kf gw">.ssh</strong>&nbsp;klas&ouml;r&uuml;ne giriyoruz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="5c60" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">cd .ssh</span></pre>
<p id="8b67" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra&nbsp;<strong class="kf gw">authorized_keys</strong>&nbsp;adında metin belgesi oluşturuyoruz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="6bde" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">touch authorized_keys</span></pre>
<p id="8b96" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra metin belgesinin i&ccedil;ine giriyoruz ve&nbsp;<strong class="kf gw">puttygen</strong>&nbsp;ile oluşturduğumuz keyi komple yapıştırıyoruz&hellip; boşluk bırakmadan yapıştırmaya &ouml;zen g&ouml;sterin.</p>
<pre class="te tf tg th ti tj bt tk"><span id="ec50" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">nano authorized_keys</span></pre>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv ze"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*3Joeo-yd5zISzL_waZ2A2A.png" alt="" /></div>
</div>
</figure>
<p id="db74" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra&nbsp;<strong class="kf gw">CTRL + X + Y</strong>&nbsp;<strong class="kf gw">Enter&nbsp;</strong>diyerek kaydedip &ccedil;ıkıyoruz&hellip;Şimdi sunucumuza&nbsp;<strong class="kf gw">SSH key</strong>&nbsp;ile bağlanalım..&nbsp;<strong class="kf gw">Kontrol&uuml;</strong>&nbsp;sağladıkdan sonra şifre ile girişi&nbsp;<strong class="kf gw">devre dışı</strong>&nbsp;bırakacağız..Biz&nbsp;<strong class="kf gw">Termius</strong>&nbsp;kullanıyoruz ve &ouml;neriyoruz.. Bu şekilde g&ouml;stereceğiz..Siz&nbsp;<strong class="kf gw">putty</strong>&nbsp;ilede bağlanabilirsiniz.</p>
<p id="6521" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">New</strong>&nbsp;<strong class="kf gw">host</strong>&nbsp;diyoruz.</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zf"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/493/1*JNkxO31dcZQRRpo4-dUUeA.png" alt="" /></div>
</figure>
<p id="9677" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Label</strong>&nbsp;b&ouml;l&uuml;m&uuml;ne herhangi bir isim..&nbsp;<strong class="kf gw">adress</strong>&nbsp;b&ouml;l&uuml;m&uuml;ne sunu ip adresinizi yazıyoruz ..&nbsp;<strong class="kf gw">Username</strong>&nbsp;b&ouml;l&uuml;m&uuml;ne kullanıcı adınızı genelde&nbsp;<strong class="kf gw">root</strong>&nbsp;olur farklı bir isim belirlemediyseniz..Daha sonra&nbsp;<strong class="kf gw">keys</strong>&nbsp;b&ouml;l&uuml;m&uuml;ne tıklayarak&nbsp;<strong class="kf gw">key</strong>&nbsp;bilgilerini gireceğiz..</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zg"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/332/1*e4R9MHqm8Vq8qDZ8xn_gbA.png" alt="" /></div>
</figure>
<p id="5eac" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">ADD KEY</strong>&nbsp;dedikden sonra ;</p>
<p id="8789" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Key name</strong>&nbsp;b&ouml;l&uuml;m&uuml;ne putty&rsquo;de masa&uuml;st&uuml;ne kaydettiğiniz dosya ile aynı isimi yazabilirsiniz..<strong class="kf gw">Passphrase</strong>&nbsp;b&ouml;l&uuml;m&uuml;nde&nbsp;<strong class="kf gw">puttygen</strong>&nbsp;ile key oluştururken&nbsp;<strong class="kf gw">şifre</strong>&nbsp;belirlediyseniz onu yazınız yoksa boş bırakınız..Daha sonrasında&nbsp;<strong class="kf gw">Import from key file</strong>&nbsp;diyerek&nbsp;<strong class="kf gw">puttygen</strong>&nbsp;ile oluşturduğunuz key dosyasını y&uuml;kl&uuml;yoruz..Daha sonra&nbsp;<strong class="kf gw">SAVE</strong>&nbsp;diyoruz ve sunucumuza giriş yapıyoruz..</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zh"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*V-L3IxAsF5jTw8F1OtQQZA.png" alt="" /></div>
</div>
</figure>
<p id="9459" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Ve&nbsp;<strong class="kf gw">sorunsuz</strong>&nbsp;bağlandık .. Şimdi&nbsp;<strong class="kf gw">şifre</strong>&nbsp;ile giriş işlemini kapatıyoruz..</p>
<p id="d2fa" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">sshd_config</strong>&nbsp;dosyasının i&ccedil;ine giriyoruz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="de6d" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo nano /etc/ssh/sshd_config</span></pre>
<p id="bc15" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">En aşşağı iniyoruz&nbsp;<strong class="kf gw">PasswordAuthentication yes&nbsp;</strong>b&ouml;l&uuml;m&uuml;n&uuml;<strong class="kf gw">&nbsp;no&nbsp;</strong>olarak değiştiyoruz&hellip;&nbsp;<strong class="kf gw">CTRL X + Y Enter</strong>&nbsp;diyerek kaydedip &ccedil;ıkıyoruz..Daha sonrasında restart atıyoruz işlem tamamlanmış oluyor..</p>
<pre class="te tf tg th ti tj bt tk"><span id="fedd" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo systemctl restart ssh</span></pre>
<p id="18d5" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">İşimizi garantiye almak i&ccedil;in termiusdan yada farklı bir yerden&nbsp;<strong class="kf gw">şifre ile giriş</strong>&nbsp;yapmayı deniyoruz.. mesela&nbsp;<strong class="kf gw">Putty</strong>&nbsp;ile bağlanmak istediğimde girişe izin vermiyor ve<strong class="kf gw">&nbsp;key</strong>&nbsp;ile bağlanmamızı istiyor&hellip; İlk işlemimiz bu kadardı.</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zi"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/403/1*ybaYb46jFeddOr_CgzNdBg.png" alt="" /></div>
</figure>
<p id="5318" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">4 &mdash; SSH i&ccedil;in İki Fakt&ouml;rl&uuml; Kimlik Doğrulamayı Ayarlayın&nbsp;<strong class="kf gw">Google-Authenticator (</strong>Mainnet<strong class="kf gw">)</strong></p>
<p id="066b" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Sunucunuza<strong class="kf gw">&nbsp;SSH key</strong>&nbsp;ile girişi aktifleştirmeden bu işleme başlmayın.</p>
<p id="9aa2" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">iki fakt&ouml;rl&uuml;</strong>&nbsp;doğrulamayı yapmak size ekstradan g&uuml;venlik katacaktır..Bu işlem biraz uzun s&uuml;rd&uuml;ğ&uuml;nden sadece mainnette yapmak yeterli olacaktır &hellip; Bu işlemi uyguladığınızda&nbsp;<strong class="kf gw">SSH key</strong>&nbsp;ile bağlantı yaparken birde&nbsp;<strong class="kf gw">Google-Authenticator</strong>&nbsp;kod gireceksiniz &hellip; Olurda keyiniz&nbsp;<strong class="kf gw">&ccedil;alınırsa</strong>&nbsp;k&ouml;t&uuml; niyetli kişiler birde bu doğrulamayı ge&ccedil;mek zorunda kalacaklar..</p>
<ul class="">
<li id="6917" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">1</li>
</ul>
<pre class="te tf tg th ti tj bt tk"><span id="6774" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo apt install libpam-google-authenticator -y</span></pre>
<ul class="">
<li id="44dd" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">2</li>
</ul>
<pre class="te tf tg th ti tj bt tk"><span id="d902" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo nano /etc/pam.d/sshd</span></pre>
<p id="6249" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki</strong>&nbsp;satırı en alta bir&nbsp;<strong class="kf gw">boşluk</strong>&nbsp;bırakarak ekleyin</p>
<pre class="te tf tg th ti tj bt tk"><span id="1b91" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph=""># Standard Un*x password updating.<br />@include common-password<br /><strong class="tn gw">auth required pam_google_authenticator.so nullok<br />auth required pam_permit.so<br /></strong><strong class="tn gw">auth required pam_google_authenticator.so</strong></span></pre>
<p id="9cbc" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">daha sonra</strong>&nbsp;aşağıdaki resimdeki satırı bulun&nbsp;<a class="au pt" href="http://twitter.com/include" target="_blank" rel="noopener ugc nofollow"><strong class="kf gw">@include</strong></a><strong class="kf gw">&nbsp;common-auth&nbsp;</strong>başına&nbsp;<strong class="kf gw">#</strong>&nbsp;ekleyin..</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="iu iv zj"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/277/1*9-gEII0p75JHpGj5RWSGgg.png" alt="" /></div>
</figure>
<p id="18b3" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra C<strong class="kf gw">TRL + X + Y Enter</strong>&nbsp;diyerek kaydedip &ccedil;ıkın.</p>
<ul class="">
<li id="1545" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">3</li>
</ul>
<p id="ac1e" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">ilk &ouml;nce</strong>&nbsp;dosyanın yedeğini alıyoruz</p>
<pre class="te tf tg th ti tj bt tk"><span id="3ad2" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo cp /etc/ssh/sshd_config /etc/ssh/sshd_config.bak</span></pre>
<p id="f89f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">daha sonra</strong>&nbsp;aşağıdaki kod ile d&uuml;zenleme yapıyoruz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="a94c" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo nano /etc/ssh/sshd_config</span></pre>
<p id="b341" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">girdikden sonra aşağıdaki&nbsp;<strong class="kf gw">2</strong>&nbsp;satırı bulup&nbsp;<strong class="kf gw">yes</strong>&nbsp;olarak değiştirin</p>
<p id="33bb" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">ChallengeResponseAuthentication yes</strong></p>
<p id="24b0" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">UsePAM yes</strong></p>
<p id="50e0" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra dosyanın en altına inip bir&nbsp;<strong class="kf gw">boşluk</strong>&nbsp;bırakıp aşağıdaki kodu ekliyoruz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="3560" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">AuthenticationMethods publickey,password publickey,keyboard-interactive</span></pre>
<p id="ebbd" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonra C<strong class="kf gw">TRL + X + Y Enter</strong>&nbsp;diyerek kaydedip &ccedil;ıkın.</p>
<ul class="">
<li id="ab50" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">4</li>
</ul>
<pre class="te tf tg th ti tj bt tk"><span id="f1e3" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo systemctl restart sshd.service</span></pre>
<ul class="">
<li id="86ec" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph="">5</li>
</ul>
<p id="8d86" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki kod</strong>&nbsp;ile &ccedil;alıştırma işlemini başlatın ve karşınıza &ccedil;ıkan işleme&nbsp;<strong class="kf gw">y</strong>&nbsp;diyerek devam edin.</p>
<pre class="te tf tg th ti tj bt tk"><span id="24b1" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">google-authenticator</span></pre>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zk"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*T7HM1DeD3ZJl-IKR4eEYuw.png" alt="" /></div>
</div>
</figure>
<p id="6f1d" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Size bir QR kodu ve kurtarma kodları verecek &hellip;&nbsp;<strong class="kf gw">QR kodu&nbsp;</strong>taratıp telefonunuza ekleyin ve kurtarma kodlarınızı&nbsp;<strong class="kf gw">kaydedin</strong>.</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zl"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*8WN_uMyXJZBiLNvLjoms0Q.png" alt="" /></div>
</div>
</figure>
<p id="de5c" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Size</strong>&nbsp;aşağıdaki resimler gibi bazı sorular soracak ne yazmanı gerektiğini resimlerde belirttik.</p>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zm"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*tcgUMFEhP7-89TgEIE6kJw.png" alt="" /></div>
</div>
</figure>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zn"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*gSx6m-eFkV68XVXNYPKAtg.png" alt="" /></div>
</div>
</figure>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zo"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*p43-EdB24Pc9-IItVITWqg.png" alt="" /></div>
</div>
</figure>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zp"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*f_QW_zyVVILQeKTmnKdifg.png" alt="" /></div>
</div>
</figure>
<p id="553b" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Daha sonrasında sunucunuza SSH key ile giriş yaparken 2 adımlı doğrulama&nbsp;<strong class="kf gw">kodu</strong>&nbsp;isteyecektir&hellip; bazen kabul etmeyebiliyor spam yapmayın.. kabul etmez ise kodun yenilenmesini bekleyiniz..</p>
<p id="e395" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">5 &mdash; G&uuml;venli</strong>&nbsp;Paylaşılan Bellek (Testnet-Mainnet)</p>
<p id="9eb3" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Sistemde</strong>&nbsp;kullanılan paylaşılan belliği g&uuml;vence altına almak &ouml;nemlidir ..Siz Farkında olmadan paylaşılan bellek, &ccedil;alışan bir hizmete y&ouml;nelik saldırıda kullanılabilir. Bu nedenle, sistem belleğinin bu b&ouml;l&uuml;m&uuml;n&uuml; sabitleyin.</p>
<pre class="te tf tg th ti tj bt tk"><span id="c4f9" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo nano /etc/fstab</span></pre>
<p id="8e9a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Dosyanın&nbsp;<strong class="kf gw">en altına aşağıdaki satırı</strong>&nbsp;ekleyin ve kaydedin.. Bu, paylaşılan belleği salt okunur moda ayarlar&hellip;&nbsp;<strong class="kf gw">CTRL X + Y Enter</strong>&nbsp;ile kaydedebilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="f8a7" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">tmpfs    /run/shm    tmpfs    ro,noexec,nosuid    0 0</span></pre>
<p id="2fc5" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Daha sonra</strong>&nbsp;sistemi yeniden başlatın ve işlemi tamamlayın.</p>
<pre class="te tf tg th ti tj bt tk"><span id="7c80" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo reboot</span></pre>
<p id="ed76" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">6 &mdash; G&uuml;venlik</strong>&nbsp;Duvarınızı Yapılandırın (Testnet-Mainnet)</p>
<p id="c60e" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Standart&nbsp;<strong class="kf gw">UFW g&uuml;venlik duvarı</strong>, d&uuml;ğ&uuml;m&uuml;n&uuml;ze ağ erişimini kontrol etmek i&ccedil;in kullanılabilir..Herhangi bir&nbsp;<strong class="kf gw">yeni</strong>&nbsp;kurulumda, ufw varsayılan olarak devre dışıdır&hellip;Giden bağlantılara izin verin ..&nbsp;<strong class="kf gw">SSH&nbsp;</strong>ve istediğiniz hari&ccedil; t&uuml;m gelen bağlantıları reddetin..Oturum a&ccedil;ma girişimlerini&nbsp;<strong class="kf gw">sınırlayın</strong>..</p>
<p id="dadc" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">alttaki</strong>&nbsp;kodları sırayla giriniz&hellip;a&ccedil;mak istediğiniz b&ouml;l&uuml;m&uuml;ne&nbsp;<strong class="kf gw">istediğinizi</strong>&nbsp;yazarak a&ccedil;abilirsiniz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="42d9" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo ufw default allow outgoing</span><span id="c828" class="ir tl tm ly tn b dn tr ts tt tu tv tp l tq" data-selectable-paragraph="">sudo ufw default deny incoming</span><span id="327d" class="ir tl tm ly tn b dn tr ts tt tu tv tp l tq" data-selectable-paragraph="">sudo ufw allow ssh/tcp</span><span id="0b4b" class="ir tl tm ly tn b dn tr ts tt tu tv tp l tq" data-selectable-paragraph="">sudo ufw limit ssh/tcp</span><span id="b413" class="ir tl tm ly tn b dn tr ts tt tu tv tp l tq" data-selectable-paragraph="">sudo ufw allow <strong class="tn gw">a&ccedil;mak istediğiniz</strong></span><span id="6d18" class="ir tl tm ly tn b dn tr ts tt tu tv tp l tq" data-selectable-paragraph="">sudo ufw enable</span></pre>
<p id="42ff" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">7 &mdash; Fail2ban&rsquo;ı&nbsp;</strong>y&uuml;kleyin (Testnet-Mainnet)</p>
<p id="26e9" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Fail2ban, g&uuml;nl&uuml;k dosyalarını izleyen ve başarısız bir oturum a&ccedil;ma girişimine karşılık gelen bir&nbsp;<strong class="kf gw">saldırı</strong>&nbsp;&ouml;nleme sistemidir. Belirli bir IP adresinden belirli sayıda başarısız oturum a&ccedil;ma tespit edilirse (belirli bir s&uuml;re i&ccedil;inde),&nbsp;<strong class="kf gw">fail2ban</strong>&nbsp;bu IP adreslerinin erişimini engeller&hellip;</p>
<p id="ac18" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki</strong>&nbsp;kod ile fail2ban&rsquo;ı y&uuml;kl&uuml;yoruz</p>
<pre class="te tf tg th ti tj bt tk"><span id="f65f" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo apt-get install fail2ban -y</span></pre>
<p id="b05d" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">daha sonra</strong>&nbsp;yapılandırma dosyasının i&ccedil;ine girip d&uuml;zenleme işlemi yapıyoruz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="5982" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo nano /etc/fail2ban/jail.local</span></pre>
<p id="6ded" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki satıları</strong>&nbsp;dosyanın i&ccedil;ine ekliyoruz ..&nbsp;<strong class="kf gw">beyaz</strong>&nbsp;listeye almak istediğiniz ip adreslerinizi virg&uuml;l koyarak ekleyebilirsiniz..Daha sonra&nbsp;<strong class="kf gw">CTRL + X +Y Enter&nbsp;</strong>diyerek kaydedip &ccedil;ıkalım.</p>
<pre class="te tf tg th ti tj bt tk"><span id="9015" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">[sshd]<br />enabled = true<br />port = 22<br />filter = sshd<br />logpath = /var/log/auth.log<br />maxretry = 3<br /># whitelisted IP addresses<br />ignoreip = <strong class="tn gw">185.125.26.25</strong>,<strong class="tn gw">259.14.12.11</strong></span></pre>
<p id="3fe2" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Engellenen ip</strong>&nbsp;adreslerini aşağıdaki kod ile g&ouml;rebilirsiniz..</p>
<pre class="te tf tg th ti tj bt tk"><span id="0591" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">iptables -n -L</span></pre>
<p id="79a8" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Aşağıdaki kod</strong>&nbsp;ile istediğiniz ip adresinin engelini kaldırabilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="b5e3" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">fail2ban-client set sshd unbanip <strong class="tn gw">103.1.112.3</strong></span></pre>
<p id="b253" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">fail2ban</strong>&nbsp;kullanmayı bırakmak isterseniz aşağıdaki kod ile ger&ccedil;ekleştirebilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="7158" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">fail2ban-client stop</span></pre>
<p id="14da" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">8 &mdash;Port</strong>&nbsp;Bağlantı Noktalarını Doğrulayın. (Testnet-Mainnet)</p>
<p id="b928" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">G&uuml;venli</strong>&nbsp;bir sunucu sağlamak istiyorsanız, arada bir port ağ bağlantı noktalarını doğrulamanız gerekir. Bu size ağınız hakkında &ouml;nemli bilgiler sağlayacaktır&hellip;</p>
<p id="abb9" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">aşağıdaki kod</strong>&nbsp;ile gerekli kontrollerinizi sağlayabilirsiniz.</p>
<pre class="te tf tg th ti tj bt tk"><span id="2c1f" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">sudo netstat -tulpn</span></pre>
<figure class="te tf tg th ti vp iu iv paragraph-image">
<div class="vq vr dp vs cf vt" tabindex="0" role="button">
<div class="iu iv zq"><img class="cf of vu" role="presentation" src="https://miro.medium.com/max/700/1*010fh9FGHJ0P7tsM1FaH4A.png" alt="" /></div>
</div>
</figure>
<p id="ae18" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">9 &mdash; Bash</strong>&nbsp;ge&ccedil;mişini temizle (Testnet-Mainnet)</p>
<p id="19c3" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Yukarı&nbsp;<strong class="kf gw">ok</strong>&nbsp;tuşuna bastığınızda, hassas veriler i&ccedil;erebilecek &ouml;nceki girdiğiniz komutları g&ouml;rebilirsiniz..&nbsp;<strong class="kf gw">history</strong>&nbsp;komutu ile gemişdeki girdiğiniz komutları g&ouml;rebilirsiniz&hellip;&nbsp;<strong class="kf gw">aşağıdaki kod</strong>&nbsp;ile t&uuml;m ge&ccedil;mişinizi tamamen temizleyeceksiniz ve Yukarı&nbsp;<strong class="kf gw">ok</strong>&nbsp;tuşuna bastığınızda artık eski girdiğiniz komutlar &ccedil;ıkmayacaktır..</p>
<pre class="te tf tg th ti tj bt tk"><span id="5e54" class="ir tl tm ly tn b dn to tp l tq" data-selectable-paragraph="">cat /dev/null &gt; ~/.bash_history &amp;&amp; history -c &amp;&amp; exit</span></pre>
<p id="0510" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">10 &mdash;</strong>&nbsp;Elektrik kesintisi ve internet problemleri (Testnet-Mainnet)</p>
<p id="ba5f" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Elektrik kesintisi&nbsp;</strong>;</p>
<p id="b443" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">NodesWizard</strong>&nbsp;ekibi olarak şuan sağlayıcı kullanıyoruz..<strong class="kf gw">Bu</strong>&nbsp;durumlarda elektirik kesintisi olması imkansızdır ..&nbsp;<strong class="kf gw">Uzak sunucu</strong>&nbsp;ile bağlantı kurduğumuz i&ccedil;in elektrik bizim i&ccedil;in sorun olmayacaktır .. &Ccedil;ok b&uuml;y&uuml;k Sağlayıcılar ile &ccedil;alıştığımız i&ccedil;in bu sağlayıcıların &ccedil;ok y&uuml;ksek donanımları ve g&uuml;&ccedil; kaynakları mevcuttur&hellip;&nbsp;<strong class="kf gw">Kendi donanımlarımızın</strong>&nbsp;elektrik kesintisi olması durumunda&nbsp;<strong class="kf gw">UPS</strong>&nbsp;yani&nbsp;<strong class="kf gw">Kesintisiz G&uuml;&ccedil; Kaynağı&nbsp;</strong>kullanıyoruz..</p>
<p id="f25b" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">internet problemleri (Kişisel ve Sunucu) ;</strong></p>
<ul class="">
<li id="4228" class="vv vw ly kf b mw mx mz na nc vx ng vy nk vz no wa wb wc wd ir" data-selectable-paragraph=""><strong class="kf gw">NodesWizard</strong>&nbsp;ekibi olarak&nbsp;<strong class="kf gw">2 adet</strong>&nbsp;internet sağlayıcısı kullanıyoruz&hellip;internet bağlantımız kesintiye uğradığında yedek internet sağlayıcımız mevcuttur&hellip;Ayrıca&nbsp;<strong class="kf gw">NodesWizard</strong>&nbsp;ekibin Telefon hattındaki kişisel internet paketleri &ccedil;ok y&uuml;ksektir&hellip;&nbsp;<strong class="kf gw">Sizlerede</strong>&nbsp;&ouml;nerimiz yedek bir internetiniz yoksa ve bu işlerle uğraşıyorsanız Telefon Hattınızdaki internet paketinin y&uuml;ksek olmasına &ouml;zen g&ouml;sterin ve yaşayacağınız internet problemleri olursa en k&ouml;t&uuml; ihtimalle bu şekilde bağlanabilirsiniz&hellip;</li>
<li id="27e5" class="vv vw ly kf b mw we mz wf nc wg ng wh nk wi no wa wb wc wd ir" data-selectable-paragraph=""><strong class="kf gw">Sunucunuzda internet&nbsp;</strong>problemleri olursa ve hız konusunda sıkıntı yaşarsanız bu sizin i&ccedil;in b&uuml;y&uuml;k sıkıntılara yol a&ccedil;acaktır&hellip;En basitinden anlatmak gerekirse&nbsp;<strong class="kf gw">blokları</strong>&nbsp;ka&ccedil;ıracaksınız&nbsp;<strong class="kf gw">uptime&nbsp;</strong>s&uuml;reniz d&uuml;ş&uuml;k kalacaktır ve bu y&uuml;zden&nbsp;<strong class="kf gw">hapise</strong>&nbsp;bile d&uuml;şebilirsiniz&hellip;&nbsp;<strong class="kf gw">NodesWizard</strong>&nbsp;ekibinin bu konuda tecr&uuml;besi olduk&ccedil;a y&uuml;ksektir ve ekibimizin en iyi verim aldığı sağlayacı&nbsp;<strong class="kf gw">hetzner&rsquo;dir.. NodesWizard&nbsp;</strong>ekibi test işlemlerine daima devam edecektir ve en iyi verim aldığı yerden hizmet alacaktır..<strong class="kf gw">NodesWizard</strong>&nbsp;ekibinin her zaman&nbsp;<strong class="kf gw">yedek</strong>&nbsp;sağlayıcıları mevcuttur&hellip; Ayrıca &ouml;nem derecesi y&uuml;ksek&nbsp;<strong class="kf gw">Testnet</strong>&nbsp;ve&nbsp;<strong class="kf gw">Mainnet&nbsp;</strong>kurulumlarını&nbsp;<strong class="kf gw">&ouml;zel sunucu</strong>&nbsp;ve&nbsp;<strong class="kf gw">&ouml;zel ip adresi</strong>&nbsp;&uuml;zerine inşa etmelisiniz..&nbsp;<strong class="kf gw">NodesWizard</strong>&nbsp;ekibi olarak bu şekilde işlemler yapıyoruz ve kesinlikle &ouml;neriyoruz..</li>
</ul>
<p id="13a6" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">11 &mdash; Kişisel</strong>&nbsp;Bilgisayar G&uuml;venliği (Testnet-Mainnet)</p>
<p id="d2aa" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">NodesWizard</strong>&nbsp;ekibi olarak&nbsp;<strong class="kf gw">Testnet</strong>&nbsp;ve&nbsp;<strong class="kf gw">Mainnet&nbsp;</strong>işlemleri<strong class="kf gw">&nbsp;</strong>i&ccedil;in ayrı bilgisayar kullanıyoruz&hellip;Herhangi bir&nbsp;<strong class="kf gw">kişisel işlem yapmıyoruz</strong>, dosya a&ccedil;mıyoruz ve indirme işlemi yapmıyoruz&hellip;Kullandığımız Bilgisayarların hepsinde G&uuml;&ccedil;l&uuml; bir şifre kullanıyoruz .. Kullandığımız T&uuml;m&nbsp;<strong class="kf gw">g&uuml;venlik</strong>&nbsp;ve diğer &uuml;r&uuml;nler&nbsp;<strong class="kf gw">Lisanslıdır..</strong></p>
<p id="111a" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">12 &mdash; Alarm</strong>&nbsp;ve Takip Sistemi</p>
<p id="41d1" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">13 &mdash;</p>
<p id="b61c" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Telegram</strong>&nbsp;kanallarımız ;</p>
<p id="d493" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Sohbet :&nbsp;<a class="au pt" href="https://t.me/nodeswizard" target="_blank" rel="noopener ugc nofollow">https://t.me/nodeswizard</a></p>
<p id="40b7" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph="">Duyuru :&nbsp;<a class="au pt" href="https://t.me/nodeswizardduyuru" target="_blank" rel="noopener ugc nofollow">https://t.me/nodeswizardduyuru</a></p>
<p id="2183" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Website</strong>&nbsp;:&nbsp;<a class="au pt" href="https://www.nodeswizard.com/" target="_blank" rel="noopener ugc nofollow">https://www.nodeswizard.com</a></p>
<p id="95fc" class="pw-post-body-paragraph mu mv ly kf b mw mx gy my mz na hc nb nc nd ne nf ng nh ni nj nk nl nm nn no jf ir" data-selectable-paragraph=""><strong class="kf gw">Twitter</strong>&nbsp;:&nbsp;<a class="au pt" href="https://twitter.com/NodesWizard" target="_blank" rel="noopener ugc nofollow">https://twitter.com/NodesWizard</a></p>
</div>
</div>
</section>
</div>
</div>
</article>
</div>
</div>
</li>
</ul>
</div>
</section>
</div>
</div>
</article>
