<svg xmlns="http://www.w3.org/2000/svg" width="1000" height="300" viewBox="0 0 1000 300" role="img" aria-label="yangyin18 terminal">
  <defs>
    <linearGradient id="g1" gradientUnits="userSpaceOnUse" x1="0" y1="0" x2="1000" y2="0">
      <stop offset="0%" stop-color="#6366f1"><animate attributeName="offset" values="0%;35%" dur="6s" repeatCount="indefinite"/></stop>
      <stop offset="20%" stop-color="#8b5cf6"><animate attributeName="offset" values="20%;55%" dur="6s" repeatCount="indefinite"/></stop>
      <stop offset="40%" stop-color="#0ea5e9"><animate attributeName="offset" values="40%;75%" dur="6s" repeatCount="indefinite"/></stop>
      <stop offset="60%" stop-color="#6366f1"><animate attributeName="offset" values="60%;100%" dur="6s" repeatCount="indefinite"/></stop>
      <stop offset="100%" stop-color="#8b5cf6"><animate attributeName="offset" values="100%;135%" dur="6s" repeatCount="indefinite"/></stop>
    </linearGradient>

    <filter id="blur" x="-80%" y="-80%" width="260%" height="260%">
      <feGaussianBlur stdDeviation="50"/>
    </filter>

    <clipPath id="cp0">
      <rect x="100" y="55" width="0" height="60">
        <animate attributeName="width" values="0;150" dur="1.1s" fill="freeze"/>
      </rect>
    </clipPath>
  </defs>

  <!-- 背景辉光 -->
  <g filter="url(#blur)">
    <circle cx="220" cy="150" r="120" fill="#6366f1" opacity="0.20">
      <animateTransform attributeName="transform" type="translate" values="0 0;70 -40;0 0" dur="14s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.20;0.30;0.20" dur="14s" repeatCount="indefinite"/>
    </circle>
    <circle cx="780" cy="140" r="130" fill="#8b5cf6" opacity="0.18">
      <animateTransform attributeName="transform" type="translate" values="0 0;-80 30;0 0" dur="16s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.18;0.28;0.18" dur="16s" repeatCount="indefinite"/>
    </circle>
    <circle cx="500" cy="270" r="110" fill="#0ea5e9" opacity="0.14">
      <animateTransform attributeName="transform" type="translate" values="0 0;50 40;0 0" dur="18s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.14;0.22;0.14" dur="18s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- 两侧星尘 -->
  <g fill="#cbd5e1">
    <circle cx="25" cy="120" r="2.2">
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -40" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.8;0" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="975" cy="90" r="2">
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -44" dur="7s" begin="1s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.8;0" dur="7s" begin="1s" repeatCount="indefinite"/>
    </circle>
    <circle cx="25" cy="200" r="1.8">
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -36" dur="9s" begin="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.7;0" dur="9s" begin="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="975" cy="170" r="2.2">
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -40" dur="7.5s" begin="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.8;0" dur="7.5s" begin="3s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- 终端窗口 -->
  <rect x="40" y="15" width="920" height="270" rx="16" fill="rgba(148,163,184,0.05)" stroke="#475569" stroke-opacity="0.3" stroke-width="2"/>
  <circle cx="78" cy="42" r="6.5" fill="#f87171" opacity="0.85"/>
  <circle cx="106" cy="42" r="6.5" fill="#fbbf24" opacity="0.85"/>
  <circle cx="134" cy="42" r="6.5" fill="#34d399" opacity="0.85"/>

  <!-- 命令:whoami 逐个打出 -->
  <g clip-path="url(#cp0)">
    <text x="110" y="95" font-family="Consolas, Monaco, monospace" font-size="26" fill="#22c55e">$</text>
    <text x="134" y="95" font-family="Consolas, Monaco, monospace" font-size="26" fill="#94a3b8">whoami</text>
  </g>

  <!-- 输出:用户名滑入 -->
  <text x="110" y="178" font-family="Consolas, Monaco, monospace" font-size="70" font-weight="bold" fill="url(#g1)" opacity="0">
    <animate attributeName="opacity" values="0;1" dur="0.5s" begin="1.4s" fill="freeze"/>
    <animateTransform attributeName="transform" type="translate" values="-40 0;0 0" dur="0.6s" begin="1.4s" fill="freeze"/>
  </text>

  <!-- 注释式简介循环 -->
  <text x="110" y="238" font-family="Consolas, Monaco, monospace" font-size="24" fill="#94a3b8" opacity="0">
    <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.02;0.32;0.44;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    # software engineer
  </text>
  <text x="110" y="238" font-family="Consolas, Monaco, monospace" font-size="24" fill="#94a3b8" opacity="0">
    <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.34;0.36;0.66;0.78;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    # python · java · c++
  </text>
  <text x="110" y="238" font-family="Consolas, Monaco, monospace" font-size="24" fill="#94a3b8" opacity="0">
    <animate attributeName="opacity" values="0;0;1;1;0" keyTimes="0;0.68;0.7;0.95;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    # ai &amp; automation
  </text>

  <!-- 底部提示符 + 闪烁光标 -->
  <text x="110" y="272" font-family="Consolas, Monaco, monospace" font-size="24" fill="#22c55e">$</text>
  <text x="134" y="272" font-family="Consolas, Monaco, monospace" font-size="24" fill="#22c55e">
    <animate attributeName="opacity" values="1;0;1" keyTimes="0;0.5;1" dur="1.1s" repeatCount="indefinite"/>
    █
  </text>
</svg>
