# macOS



## mac

- 鼠标：系统设置 - 鼠标 - 自然滚动
- 桌面：系统设置 - 桌面与程序坞 - 根据最近使用情况自动重新排列空间
- 小组件：系统设置 - 桌面与程序坞 - 小组件 - 调暗桌面小组件
- 终端：`xcode-select --install`
  - 苹果官方命令行开发者工具(一个包含 `git`, `clang`, `make` 等的工具包)
  - 比完整的 Xcode 小很多
- 修改终端主机名
  - `sudo scutil --set HostName 你想要的名字`



## chrome

- https://www.google.cn/chrome/index.html

## github desktop

- https://desktop.github.com/download/

## typora 0.11.18

- https://github.com/wyf9661/typora-free?tab=readme-ov-file

## ollama

- https://ollama.com
  - `ollama --version`
  - `ollama list`
  - `ollama pull <模型名>`
  - `ollama run <模型名>`
  - `ollama rm <模型名>`
- https://ollama.com/library

|      | Models              | Size  | Input       | Context | Annotation |
| ---- | ------------------- | ----- | ----------- | ------- | ---------- |
| ✅    | qwen3.6:35b         | 24GB  | Text, Image | 256K    |            |
|      | qwen3.5:9b          | 6.6GB | Text, Image | 256K    |            |
|      | qwen3.5:35b         | 24GB  | Text, Image | 256K    |            |
|      | deepseek-r1:8b      | 5.2GB | Text        | 128K    |            |
| ✅    | deepseek-r1:32b     | 20GB  | Text        | 128K    |            |
|      | gemma4:e2b          | 7.2GB | Text, Image | 128K    |            |
| ✅    | gemma4:31b          | 20GB  | Text, Image | 128K    |            |
| ✅    | x/flux2-klein:9b    | 12GB  | Text        | -       | 文生图     |
| ✅    | x/z-image-turbo:fp8 | 13GB  | Text        | -       | 文生图     |

## vscode

- https://code.visualstudio.com

## homebrew

- https://brew.sh

  - `brew -v`

- **nvm**

  - 安装 nvm：`brew install nvm`

  - 创建 nvm 目录：`mkdir -p ~/.nvm`

  - 创建 .zshrc 文件 ：`touch ~/.zshrc`

  - 配置环境变量，写入 .zshrc
  
    - ```bash
      export NVM_DIR="$HOME/.nvm"
      [ -s "$(brew --prefix nvm)/nvm.sh" ] && \. "$(brew --prefix nvm)/nvm.sh"
      [ -s "$(brew --prefix nvm)/etc/bash_completion.d/nvm" ] && \. "$(brew --prefix nvm)/etc/bash_completion.d/nvm"
      ```

  - 使配置生效：`source ~/.zshrc`
  
  - 验证安装：`nvm --version`

## nvm

```bash
# 国内镜像加速（淘宝镜像）
export NVM_NODEJS_ORG_MIRROR=https://npmmirror.com/mirrors/node

# 查看当前使用的 Node.js 版本
nvm current

# 安装 Node.js 的最新 LTS（长期支持）版本
nvm install --lts
```

把镜像配置添加到 `~/.zshrc` 中：

```bash
echo 'export NVM_NODEJS_ORG_MIRROR=https://npmmirror.com/mirrors/node' >> ~/.zshrc
source ~/.zshrc
```

## vpn

- https://github.com/yanue/V2rayU/releases/tag/v4.2.8

## comfyui

- https://comfy.org/zh-cn/download

## claude-code

- 需要 Node.js 18.0 或更高版本，以及 Git 2.39 或更高版本。
- 使用 NPM 安装
  - `npm install -g @anthropic-ai/claude-code`
- 官网：https://claude.com/product/claude-code
  - macOS：`curl -fsSL https://claude.ai/install.sh | bash`
- macOS 通过 homebrew 安装
  - `brew install --cask claude-code`
- 验证安装
  - `claude --version`
- 启动 Claude Code：进入你的项目目录，然后运行 `claude` 命令即可启动
- 方舟 Coding Plan
  - https://www.volcengine.com/docs/82379/1928262?lang=zh#77277ce0

## 百度翻译

- https://fanyi.baidu.com/appdownload/download.html
- 截图翻译快捷键：
  - `shift` ➕ `option` ➕ `a`

