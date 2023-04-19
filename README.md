# blockly.games-hax
basically, I am in some sort of group about lego mindstorms and overall "block" (most simple) programming at my school, and before building the lego mindstorms, you need to complete the entirety of [blockly.games](https://blockly.games). So instead of actually completing some of the hardest levels (only Maze Level 10), I went through the site's JavaScript files and built a few lines that would complete the level automatically when typed into the console.

## instructions
1. open the website
2. select your stage
3. go to your level
4. open the Developer tools and navigate to the console (should be `Ctrl-Shift-C` or `Ctrl-Shift-T`)
5. press on "Run Program" or insert a block/line
6. copy and paste the line corresponding to your stage into the console
7. press Enter (or the key you use to send the command)
8. enjoy the hax

## the hax (commands)
note: The [Puzzle](https://blockly.games/puzzle) stage cannot be bypassed, the [Pond (pond-duck)](https://blockly.games/pond-duck) can be completed but the completion will never be saved anyways, and if you are at one of those "Do whatever you want" levels, you can just stop at Step 5 of the instructions.

- [Puzzle](https://blockly.games/puzzle): come on, it's easy (Cannot be bypassed.)
- [Maze](https://blockly.games/maze): `gm(!0), window.localStorage && (window.localStorage[Rj + T] = ll), setTimeout(Fl, 1E3)`
- [Bird](https://blockly.games/bird): `window.localStorage && (window.localStorage[Dk + U] = km), K.Rb.play("quack", .5), Cm()`
- [Turtle](https://blockly.games/turtle): `window.localStorage && (window.localStorage[Bl + T] = Vm), gk.vd.play("win", .5), on()`
- [Movie](https://blockly.games/movie): `window.localStorage && (window.localStorage[Dl + T] = Xm), oi.xd.play("win", .5), nn()`
- [Music](https://blockly.games/music): `window.localStorage && (window.localStorage[wl + V] = Qm), kn()`
- [Pond Tutor](https://blockly.games/pond-tutor): `window.localStorage && (window.localStorage[Ul + V] = im), vn("splash", 1), vn("boom", 1), Bm()`
- [Pond](https://blockly.games/pond-duck): Cannot be bypassed.

### bonus command because I don't want people to use this to cheat though the whole game
- Check if a student has correctly done every stage: 
```
var i;
document.write('<h2>local storage</h2>');
for (i = 0; i < localStorage.length; i++)   {
  const key = localStorage.key(i);
  const value = localStorage.getItem(key);
  document.write(`<li> <b>${key}</b>: ${value}</li>`);
}
```
