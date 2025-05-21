/* 文件头注释 */
/* CSS 样式文件 */
/* 风格: 白色背景，橘黄和黑色调 */

:root {
    --bg-primary:rgb(255, 255, 255)景色 - 白色 */
    --bg-secondary: #f8f8f8; /* 卡片背景色 - 浅灰色 */
    --bg-tertiary: #eeeeee; /* 次要卡片背景色 - 稍深灰色 */
    --text-primary: #000000; /* 主要文字颜色 - 黑色 */
    --text-secondary: #333333; /* 次要文字颜色 - 深灰色 */
    --accent-primary: #ff8c00; /* 强调色 - 橘黄色 */
    --accent-secondary: #e07b00; /* 次要强调色 - 稍深的橘黄色 */
    --accent-tertiary: #c06a00; /* 第三强调色 */
    --accent-blue: #007bff; /* 保留蓝色作为可能的辅助色，但主要使用橘黄和黑色 */
    --accent-purple: #6610f2; /* 保留紫色作为可能的辅助色 */
    --accent-cyan: #00b4d8; /* 保留青色作为可能的辅助色 */
    --card-padding: 20px;
    --grid-gap: 15px;
}

body {
    font-family: 'SF Pro Display', 'Segoe UI', sans-serif;
    background-color: var(--bg-primary);
    color: var(--text-primary);
    line-height: 1.6;
    font-size: 16px;
    width: 100%;
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px;
}

.grid-container {
    display: grid;
    grid-template-columns: 1fr;
    gap: var(--grid-gap);
}

.main-card {
    grid-column: 1 / -1;
    background-color: var(--bg-secondary);
    padding: var(--card-padding);
    min-height: 200px;
    border: 1px solid var(--bg-tertiary); /* 添加边框增加区分度 */
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* 添加阴影 */
}

.sub-cards-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: var(--grid-gap);
}

.card {
    background-color: var(--bg-tertiary);
    padding: var(--card-padding);
    border: 1px solid #dddddd; /* 添加边框 */
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05); /* 添加阴影 */
}

/* 标题颜色调整 */
h1 {
    color: var(--accent-primary); /* 主标题使用橘黄色 */
}

h2 {
    color: var(--accent-secondary); /* 副标题使用稍深的橘黄色 */
}

h3 {
    color: var(--text-primary); /* 三级标题使用黑色 */
}

/* 媒体查询 */
@media (max-width: 768px) {
    body {
        padding: 10px;
        font-size: 16px;
    }

    .sub-cards-row {
        grid-template-columns: 1fr;
    }

    h1 {
        font-size: 32px;
    }

    h2 {
        font-size: 24px;
    }

    h3 {
        font-size: 20px;
    }
}

/* 文件尾注释 */