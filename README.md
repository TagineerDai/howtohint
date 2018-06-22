# doc
**HowToHint** in Read the Docs.

#### View the doc

```bash
sudo pip3 install sphinx sphinx-autobuild
git clone https://github.com/TagineerDai/howtohint.git
cd howtohint/docs
sphinx-autobuild . _build/html
```
Open `_build/html/hint_main.html` with [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VSCode.