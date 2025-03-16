Hi, I'm Starlong.👋
---

☕ A caffeine-driven developer. 

<br />

<div>
  <details>
    <summary>Technologies</summary>
    <br />
    <img src="https://skillicons.dev/icons?i=js,ts,vue,nuxt,react,vite,webpack,nodejs,pnpm,html,css,sass,tailwind,git,github,vscode,python,express,mongodb,docker&perline=10" />
  </details>
</div>

<div>
  <details>
    <summary>My Stats</summary>
    <br />
    <div align="left">
      <img src="https://streak-stats.demolab.com?user=6starlong&locale=en&mode=daily&theme=onedark&hide_border=false&border_radius=5&order=3" height="180" alt="streak graph"  />
      <img src="https://github-readme-stats.vercel.app/api/top-langs?username=6starlong&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=onedark&hide_border=false&order=2" height="180" alt="languages graph"  />
      <img src="https://github-readme-activity-graph.vercel.app/graph?username=6starlong&radius=16&theme=one-dark&area=true&order=5" height="300" alt="activity-graph graph" />
    </div>
  </details>
</div>

<div>
  <details>
    <summary>Find me on</summary>
    <br />
    <div>
      <a href="mailto:starlong.lu@gmail.com">
        <img src="https://img.shields.io/badge/Email-100000?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
      </a>
      <a href="https://github.com/6starlong">
        <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
      </a>
      <a href="https://starlong.vercel.app">
        <img src="https://img.shields.io/badge/Website-100000?style=for-the-badge&logo=safari&logoColor=white" alt="Website" />
      </a>
    </div>
  </details>
</div>

<br />

```javascript
const coder = {
  caffeine: 0,

  refill() {
    this.caffeine++
    console.log(`☕ 咖啡因水平增加到: ${this.caffeine}`)
    return this
  },

  async code() {
    const states = [
      { emoji: '😴', output: '无法集中注意力...' },
      { emoji: '👨‍💻', output: '专注模式，代码流畅' },
      { emoji: '⚡', output: '灵感爆发，代码如行云流水!' },
      { emoji: '🚀', output: '超神状态，一小时抵一天!' },
      { emoji: '🤯', output: '咖啡因过载，思维混乱...' },
    ]

    // 咖啡因过量警告
    if (this.caffeine > 3) console.log('⚠️ 警告：咖啡因摄入过量!')

    const level = Math.min(states.length - 1, this.caffeine)
    console.log(`🧠 当前咖啡因等级: ${level}`)

    // 咖啡因延迟效应：咖啡因水平越高，响应越快
    await new Promise(r => setTimeout(r, this.caffeine ? 500 / this.caffeine : 2000))

    this.caffeine = Math.max(0, this.caffeine - 1)
    console.log(`⏬ 咖啡因消耗后水平: ${this.caffeine}`)

    const result = `${states[level].emoji} ${states[level].output}`
    console.log(`📝 输出结果: ${result}`)

    return result
  },

  sleep() {
    console.log('💤 休息中...')
    this.caffeine = 0
    return this
  },
}

// 示例
await coder.code() // 无咖啡
await coder.refill().code() // 一杯咖啡
await coder.refill().refill().code() // 两杯咖啡
await coder.refill().refill().refill().code() // 三杯咖啡
await coder.sleep() // 休息
```

![Profile Views](https://komarev.com/ghpvc/?username=6starlong&color=blue&style=flat)
