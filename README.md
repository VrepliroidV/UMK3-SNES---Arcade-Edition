# UMK3 Arcade Edition

A Super Nintendo hack of **Ultimate Mortal Kombat 3** that brings the game closer to the arcade version. It includes everything from Lucas Dext5r's UMK3 Deluxe (MK3 stages, Sheeva, Chameleon, stage fatalities) and uses Nemesis_C's Genesis "UMK3 Arcade" hack as a reference.

UMK3 Deluxe content is used with permission from its author, Lucas Dext5r.

**Download (beta 65):** [UMK3_arcade_edition.zip](https://github.com/VrepliroidV/UMK3-SNES---Arcade-Edition/raw/main/UMK3_arcade_edition.zip). The zip has the IPS patch, an English README and the full changelog in Portuguese (LEIA-ME.txt). No ROM is included.

![Main menu](images/titulo.png) ![Select screen](images/img1_selecao.png)
![Mode select](images/img2_modos.png) ![Tower](images/img3_torre.png)
![Fight](images/img4_luta.png)

## How to apply

| | |
|---|---|
| Apply to | `Ultimate Mortal Kombat 3 (USA).sfc` (4 MB, no header) |
| Original ROM MD5 | `0644da71f79d405a22934daa1474cefc` |
| Patched ROM MD5 | `ca5bb96f92f6cf6a4aff6266de7606f1` |

- The patched ROM is 8 MB (64 Mbit, ExHiROM). Use a patcher that can expand the file: Floating IPS, Lunar IPS, [ROM Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) or UniPatcher.
- If your ROM is 4,194,816 bytes (512-byte header, common in `.smc` files), remove the header first.
- No MSU-1 needed. Tested in Snes9x. Runs on emulators and flashcarts that support 64 Mbit ExHiROM (e.g. FXPak / SD2SNES); flashcarts limited to 32 Mbit will not run it.

## Latest changes (betas 57-65)

- **Beta 65:** fixed the life bar glitch seen on some emulators and flash carts (a colored block over a letter of the name, a broken run meter). The HUD no longer changes a palette color mid-screen; the letters over the red part of a bar are now all white.

- **Beta 64:** BIOGRAPHIES is now an item of the SECRET STUFF screen, right under SOUND TEST, in the big font (it used to be inside KOOLER STUFF).

- **Beta 63:** Ermac's fatality 2 (head punch: Run, Block, Run, Run, HK, close) can now be performed. On the original SNES cart a stray byte between Ermac's HK move list and Human Smoke's (where that shared fatality entry is) made the game read the entry one byte off, so only the one-button fatality cheat could do it.

- **Beta 62:** Motaro and Shao Kahn picked by a player can now fight on any stage (the normal order or the KOMBAT ZONE pick). CPU bosses in the tower still fight on their own stages, as in the arcade.
- **Beta 61:** playable Motaro: landing from a jump has a sound again (the same thud the CPU Motaro uses).
- **Beta 60:** fixed a crash on Liu Kang's fatality (Fwd, Fwd, Down, Down, LK): a Chameleon table entry was written 2 bytes too far, over the start of that fatality's code. It also restores three of Motaro's position values.

- **Beta 59:** fixed the graphics glitch in fights with Motaro and/or Shao Kahn (e.g. Motaro vs Shao Kahn): pink dots on the floor and background, wrong colors on the fighters. In the heaviest frames the end-of-frame work ran out of time and the scanline effects were turned on without being reset, writing random colors into the palettes. They are now reset when that happens, and the sprite graphics sent per frame in a fight are capped a bit lower so it almost never happens.
- **Beta 59:** Bell Tower: fixed occasional frames with the whole screen garbled (e.g. Chameleon vs Jax doing combos). The rope drawing code is about 4x faster.
- **Beta 58:** Liu Kang: after his launcher combo (HP, HP, Back+LP), every later hit did only 1/4 of the damage until the end of the round. Fixed.
- **Beta 57:** The Bridge: the gap under the floor is filled like on the other stages. Jump-in HP + combo now connects on Kitana, Jade and Mileena like on everyone else.

## Highlights

- Arcade-style select screen (7/7/5/5/5) with everyone unlocked: Sheeva, Chameleon, Human Smoke, Motaro and Shao Kahn, each with a slot and portrait. "?" slot = random select.
- Chameleon cycles through every ninja's colors, has one special move from each ninja, his own name, announcer voice, brutality and green blood.
- Motaro and Shao Kahn get big VS-screen art and biographies; Motaro can't be launched or juggled.
- Arcade intro story, redesigned main menu and mode select, CHOOSE YOUR DESTINY tower with the GOD tower.
- Fighter names inside the life bars, as in the arcade.
- Air combos for Kitana, Jade and Mileena.
- **TRAINING mode:** pick both fighters with controller 1, the opponent stands still, infinite health and time, KOMBAT ZONE stage select. START + SELECT exits.
- KOMBAT ZONE stage select, OPTIONS > CREDITS screen, many sound, announcer and graphics fixes, less slowdown in the boss fights.

## Credits

- UMK3 Deluxe: Lucas Dext5r (2022)
- Original MSU-1 patch: Kurrono, Relikk, Conn
- Genesis "UMK3 Arcade" hack (reference): Nemesis_C
- This patch: Repliroid do Futuro (Gabriel Calmon)

---

## Português

Hack de **Ultimate Mortal Kombat 3** para Super Nintendo que deixa o jogo mais perto do arcade. Traz tudo do UMK3 Deluxe do Lucas Dext5r e usa a hack de Mega Drive "UMK3 Arcade" do Nemesis_C como referência.

O conteúdo do UMK3 Deluxe é usado com a permissão do autor, Lucas Dext5r.

**Download (beta 65):** [UMK3_arcade_edition.zip](https://github.com/VrepliroidV/UMK3-SNES---Arcade-Edition/raw/main/UMK3_arcade_edition.zip). O zip tem o patch IPS, um README em inglês e o LEIA-ME.txt com todas as novidades em português. A ROM não vem junto.

Aplique na `Ultimate Mortal Kombat 3 (USA).sfc` original (4 MB, sem cabeçalho, MD5 `0644da71f79d405a22934daa1474cefc`). Depois do patch a ROM fica com 8 MB e MD5 `ca5bb96f92f6cf6a4aff6266de7606f1`.

### Novidades recentes (betas 57-65)

- **Beta 65:** corrigido o glitch das barras de vida em alguns emuladores e flashcarts (bloco colorido em cima de uma letra do nome, barrinha de corrida errada). O HUD não troca mais cor no meio da tela; as letras sobre a parte vermelha da barra ficam todas brancas.

- **Beta 64:** BIOGRAPHIES virou um item da tela SECRET STUFF, logo abaixo do SOUND TEST, com a fonte grande (antes ficava dentro do KOOLER STUFF).

- **Beta 63:** o fatality 2 do Ermac (soco que arranca a cabeça: corrida, defesa, corrida, corrida, chute alto, de perto) agora sai. No cartucho original sobrava 1 byte na lista de golpes dele e o comando nunca era reconhecido.

- **Beta 62:** Motaro e Shao Kahn escolhidos por um jogador agora lutam em qualquer cenário (a ordem normal ou o KOMBAT ZONE). Os chefes da CPU na torre continuam no próprio cenário, como no arcade.
- **Beta 61:** Motaro jogável: o pouso do pulo tem som de novo (o mesmo baque do Motaro da CPU).
- **Beta 60:** corrigido o travamento no fatality do Liu Kang (frente, frente, baixo, baixo, chute fraco).

- **Beta 59:** corrigido o glitch gráfico nas lutas com o Motaro e/ou o Shao Kahn (ex.: Motaro x Shao Kahn): pontos rosa no chão e no fundo, cores erradas nos lutadores.
- **Beta 59:** Bell Tower: corrigidos os quadros com a tela inteira embaralhada (ex.: Chameleon x Jax fazendo combos).
- **Beta 58:** Liu Kang: depois do combo lançador (soco forte, soco forte, trás + soco fraco), os golpes seguintes tiravam só 1/4 do dano até o fim do round. Corrigido.
- **Beta 57:** The Bridge: o vazio embaixo do chão foi preenchido. Pulo + soco forte e combo agora pegam na Kitana, Jade e Mileena como nos outros.
