# Rust Pac-Man

这是一个使用 Rust 编程语言和 [Piston](https://www.piston.rs/) 游戏引擎实现的经典吃豆人（Pac-Man）游戏。
## ✨ 项目特色

- **纯粹的 Rust 实现**: 完全使用 Rust 语言编写，展示了 Rust 在游戏开发中的应用。
- **经典游戏复刻**: 忠实再现了吃豆人的核心玩法，包括吃豆、躲避鬼魂、能量豆反击等。
- **清晰的架构**: 采用了模型-视图-控制器 (MVC) 的思想，将游戏逻辑、渲染和用户输入清晰地分离开来：
    - **`src/pacman.rs`**: 核心游戏逻辑，管理吃豆人、鬼魂的状态和游戏规则。
    - **`src/view.rs`**: 负责所有图形的渲染，包括地图、角色、UI 等。
    - **`src/controler.rs`**: 处理键盘输入和游戏循环的事件。
- **模块化设计**: 代码被组织在不同的模块中，例如 `pacman` 模块下还有 `map` 和 `ghost` 子模块，便于理解和维护。
- **基于 Piston 引擎**: 使用了成熟的 Piston 游戏引擎来处理窗口、事件循环和 2D 图形渲染。

## 🚀 如何运行

在开始之前，请确保您已经安装了 Rust 工具链和 C++ 构建工具。

1.  **克隆或下载项目**

2.  **进入项目根目录**:
    ```bash
    cd path/to/rust-pacman-master
    ```

3.  **运行游戏**:
    我们推荐使用 `release` 模式来获得最佳性能。
    ```bash
    cargo run --release --bin pac
    ```

## 🎮 操作指南

-   **移动**:
    -   使用 **方向键** (`↑`, `↓`, `←`, `→`)
    -   或使用 **Vim 键位** (`K`, `J`, `H`, `L`)
-   **暂停/继续**: 按 `P` 键
-   **退出游戏**: 按 `Q` 键

## 🛠️ 技术栈

-   **语言**: [Rust](https://www.rust-lang.org/) (Edition 2018)
-   **游戏引擎**: [Piston](https://www.piston.rs/)
-   **渲染后端**: [OpenGL](https://www.opengl.org/)
-   **主要依赖**:
    -   `piston_window`
    -   `opengl_graphics`
    -   `glutin_window`
    -   `rand`

希望这份 `README.md` 能更好地帮助您和他人了解这个项目！
