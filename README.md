# ConEmu Dex theme

Awesome color theme for ConEmu.

### Table of contents

* [Install](#install)
* [Usage](#usage)
* [Support this project](#support-this-project)
* [Code of Conduct](#code-of-conduct)
* [License](#license)

### Install

1) Open =ConEmu.xml=. Usually it is at  =~\AppData\Roaming=, where =~= is your home directory (=C:\Users\UserName=).
2) Paste the color scheme at the end of palette settings part. It starts with the following:

#+BEGIN_SRC xml
  <key name="Colors" modified="2018-07-18 09:58:34" build="180626">
    <value name="Count" type="long" data="1"/>
    <key name="Palette1" modified="2018-07-18 09:58:34" build="180626">
#+END_SRC

3) If you do not have any custom color scheme, the xml key is not there. In ConEmu, go to =Settings= -> =Feature= -> =Colors= and generate a custom color theme by click on =Save= button and specify any name. Then =Colors= key will be automatically generated in your =ConEmu.xml=. You can overwrite it when you add new themes.

4) Update the palette number (key name =PaletteX=) accordingly. For example, if you have 1 custom color palette already, it should be =Palette2= for the new one:

#+BEGIN_SRC xml
  <key name="Palette2" modified="2018-07-18 09:58:34" build="180626">
#+END_SRC

5) Make sure to increase the value for key name =Count= under key =Colors= as well. It should equal to the total number of pallets you have:

#+BEGIN_SRC xml
  <value name="Count" type="long" data="2"/>
#+END_SRC

6) For example, the =Colors= part of your modified =ConEmu.xml= should look like this:

#+BEGIN_SRC xml
<key name="Colors" modified="2018-07-18 09:58:34" build="180626">
  <value name="Count" type="long" data="2"/>
  <key name="Palette1" modified="2018-07-18 09:58:34" build="180626">
    <value name="Name" type="string" data="EXISTING COLOR"/>
    <value name="TextColorIdx" type="hex" data="10"/>
    ...
    <value name="ColorTable15" type="dword" data="00e3f6fd"/>
  </key>
  <key name="Palette2" modified="2018-07-18 09:58:34" build="180626">
    <value name="Name" type="string" data="NAME OF THE COLOR YOU ADDED"/>
    <value name="TextColorIdx" type="hex" data="10"/>
    ...
    <value name="ColorTable21" type="dword" data="00e7fdfd"/>
  </key>
</key>
#+END_SRC

### Template
The following is the template for color schemes with the default colors that
you can use. (It is also in =dex-theme.xml=):

#+BEGIN_SRC xml
<key name="Palette1" modified="2018-07-18 09:58:34" build="180626">
  <value name="Name" type="string" data="DeX"/>
  <value name="TextColorIdx" type="hex" data="10"/>
  <value name="BackColorIdx" type="hex" data="10"/>
  <value name="PopTextColorIdx" type="hex" data="10"/>
  <value name="PopBackColorIdx" type="hex" data="10"/>
  <value name="ColorTable00" type="dword" data="002b2521"/>
  <value name="ColorTable01" type="dword" data="00423607"/>
  <value name="ColorTable02" type="dword" data="009cbc1a"/>
  <value name="ColorTable03" type="dword" data="00a48231"/>
  <value name="ColorTable04" type="dword" data="003c4ce7"/>
  <value name="ColorTable05" type="dword" data="00b6369c"/>
  <value name="ColorTable06" type="dword" data="000fc4f1"/>
  <value name="ColorTable07" type="dword" data="00c3beb2"/>
  <value name="ColorTable08" type="dword" data="00a1a193"/>
  <value name="ColorTable09" type="dword" data="00d28b26"/>
  <value name="ColorTable10" type="dword" data="00f2a13b"/>
  <value name="ColorTable11" type="dword" data="0098a12a"/>
  <value name="ColorTable12" type="dword" data="002f32dc"/>
  <value name="ColorTable13" type="dword" data="008236d3"/>
  <value name="ColorTable14" type="dword" data="000089b5"/>
  <value name="ColorTable15" type="dword" data="00e3f6fd"/>
</key>
#+END_SRC

### Support this project

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

If you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the project
 - [![Donate](https://img.shields.io/badge/Donate-Paypal-brightgreen.svg?colorB=259cd2)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YKLGUUB34ASEL)—make one-time donations via PayPal.
 - [![Donate](https://img.shields.io/badge/Donate-Patreon-brightgreen.svg?colorB=f86213)](https://www.patreon.com/alexdevero)—set up monthly donation via Patreon and get interesting news about what I'm doing.
 - <img alt="bitcoin" src="https://img.shields.io/badge/Donate-Bitcoin-brightgreen.svg?colorB=fab915">—send bitcoins or ethereum to this address: `19jHGagJWeVvuNjN3kaBoAszXd9ea9gKzp`.

Thank you!

### Code of Conduct

[Contributor Code of Conduct](code-of-conduct.md). By participating in this project you agree to abide by its terms.

### License

MIT © [Alex Devero](https://alexdevero.com).

<!-- links -->
[Grease the Groove]: https://www.artofmanliness.com/2016/01/20/get-stronger-by-greasing-the-groove/
