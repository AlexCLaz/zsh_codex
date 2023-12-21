<h1 align="center">⌨️ 🦾 Zsh Open AI</h1>

<p align="center">
    AI in the command line.
</p>

<p align="center">
    <img src='https://github.com/tom-doerr/bins/raw/main/zsh_codex/zc4.gif'>
    <p align="center">
        You just need to write a comment or variable name and the AI will write the corresponding code.
    </p>
</p>


## What is it?

This is a ZSH plugin that enables you to use OpenAI's powerful AI in the command line. OpenAI is the AI that also powers GitHub Copilot.


## How do I install it?
### Manual Installation
1. Install the OpenAI package.
```
pip3 install openai
```

2. Download the ZSH plugin.

```
git clone https://github.com/alexclaz/zsh_openai.git ~/.oh-my-zsh/custom/plugins/zsh_openai
```

3. Add the following to your `.zshrc` file.

Using oh-my-zsh:
```
    plugins=(zsh_openai)
    bindkey '^X' create_completion
```
Without oh-my-zsh:
```
    # in your/custom/path you need to have a "plugins" folder and in there you clone the repository as zsh_openai
    export ZSH_CUSTOM="your/custom/path"
    source "$ZSH_CUSTOM/plugins/zsh_openai/zsh_openai.plugin.zsh"
    bindkey '^X' create_completion
```

4. Create a file called `openaiapirc` in `~/.config` with your ORGANIZATION_ID and SECRET_KEY.

```
[openai]
organization_id = ...
secret_key = ...
```

5. Run `zsh`, start typing and complete it using `^X`!

<p align="center">
    Buy a coffee to the original creator: TomDoerr<br>
    <a href="https://www.buymeacoffee.com/TomDoerr" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
</p>
