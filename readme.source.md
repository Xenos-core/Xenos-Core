```aura width=860 height=260
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', width: '100%', height: '100%', background: '#07090c', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter', border: '1px solid rgba(52,211,153,0.18)' }}>
  <style>{`
    @keyframes drift-a { 0%, 100% { transform: translate(0px, 0px); opacity: 0.85; } 50% { transform: translate(60px, -20px); opacity: 1; } }
    @keyframes drift-b { 0%, 100% { transform: translate(0px, 0px); opacity: 0.7; } 50% { transform: translate(-70px, 18px); opacity: 0.95; } }
    @keyframes drift-c { 0%, 100% { transform: translate(0px, 0px); opacity: 0.6; } 50% { transform: translate(40px, 24px); opacity: 0.9; } }
    #o1 { animation: drift-a 10s ease-in-out infinite; }
    #o2 { animation: drift-b 13s ease-in-out infinite; }
    #o3 { animation: drift-c 9s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="260" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="r1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(16,185,129,0.55)" />
        <stop offset="70%" stopColor="rgba(16,185,129,0)" />
      </radialGradient>
      <radialGradient id="r2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.45)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
      <radialGradient id="r3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(99,102,241,0.35)" />
        <stop offset="70%" stopColor="rgba(99,102,241,0)" />
      </radialGradient>
      <pattern id="grid" width="28" height="28" patternUnits="userSpaceOnUse">
        <path d="M 28 0 L 0 0 0 28" fill="none" stroke="rgba(255,255,255,0.035)" strokeWidth="1" />
      </pattern>
    </defs>
    <rect width="860" height="260" fill="url(#grid)" />
    <ellipse id="o1" cx="120" cy="250" rx="280" ry="180" fill="url(#r1)" />
    <ellipse id="o2" cx="760" cy="30" rx="260" ry="170" fill="url(#r2)" />
    <ellipse id="o3" cx="560" cy="270" rx="220" ry="140" fill="url(#r3)" />
  </svg>

  <div style={{ position: 'absolute', left: 52, top: 66, width: 128, height: 128, borderRadius: 64, background: 'linear-gradient(135deg, #34d399, #22d3ee)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
    <img src=".github/aura/avatar.png" width={118} height={118} style={{ borderRadius: 59 }} />
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 214 }}>
    <div style={{ display: 'flex', fontSize: 14, color: '#34d399', letterSpacing: 4, fontWeight: 600 }}>HI, I'M</div>
    <div style={{ display: 'flex', fontSize: 52, fontWeight: 800, color: '#ffffff', letterSpacing: -2, lineHeight: 1.05, marginTop: 4 }}>Alireza</div>
    <div style={{ display: 'flex', fontSize: 17, color: 'rgba(226,232,240,0.72)', marginTop: 10 }}>Java developer building fast, Folia-safe Minecraft plugins</div>
    <div style={{ display: 'flex', gap: 8, marginTop: 18 }}>
      <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 12, color: '#a7f3d0', background: 'rgba(52,211,153,0.10)', border: '1px solid rgba(52,211,153,0.30)' }}>Paper</span>
      <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 12, color: '#a5f3fc', background: 'rgba(34,211,238,0.10)', border: '1px solid rgba(34,211,238,0.30)' }}>Folia</span>
      <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 12, color: '#c7d2fe', background: 'rgba(99,102,241,0.12)', border: '1px solid rgba(99,102,241,0.32)' }}>Velocity</span>
      <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 12, color: 'rgba(255,255,255,0.7)', background: 'rgba(255,255,255,0.05)', border: '1px solid rgba(255,255,255,0.12)' }}>Java 21</span>
    </div>
  </div>
</div>
```

```aura width=120 height=40 link="https://github.com/Xenos-core" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+R2l0SHViPC90aXRsZT48cGF0aCBkPSJNMTIgLjI5N2MtNi42MyAwLTEyIDUuMzczLTEyIDEyIDAgNS4zMDMgMy40MzggOS44IDguMjA1IDExLjM4NS42LjExMy44Mi0uMjU4LjgyLS41NzcgMC0uMjg1LS4wMS0xLjA0LS4wMTUtMi4wNC0zLjMzOC43MjQtNC4wNDItMS42MS00LjA0Mi0xLjYxQzQuNDIyIDE4LjA3IDMuNjMzIDE3LjcgMy42MzMgMTcuN2MtMS4wODctLjc0NC4wODQtLjcyOS4wODQtLjcyOSAxLjIwNS4wODQgMS44MzggMS4yMzYgMS44MzggMS4yMzYgMS4wNyAxLjgzNSAyLjgwOSAxLjMwNSAzLjQ5NS45OTguMTA4LS43NzYuNDE3LTEuMzA1Ljc2LTEuNjA1LTIuNjY1LS4zLTUuNDY2LTEuMzMyLTUuNDY2LTUuOTMgMC0xLjMxLjQ2NS0yLjM4IDEuMjM1LTMuMjItLjEzNS0uMzAzLS41NC0xLjUyMy4xMDUtMy4xNzYgMCAwIDEuMDA1LS4zMjIgMy4zIDEuMjMuOTYtLjI2NyAxLjk4LS4zOTkgMy0uNDA1IDEuMDIuMDA2IDIuMDQuMTM4IDMgLjQwNSAyLjI4LTEuNTUyIDMuMjg1LTEuMjMgMy4yODUtMS4yMy42NDUgMS42NTMuMjQgMi44NzMuMTIgMy4xNzYuNzY1Ljg0IDEuMjMgMS45MSAxLjIzIDMuMjIgMCA0LjYxLTIuODA1IDUuNjI1LTUuNDc1IDUuOTIuNDIuMzYuODEgMS4wOTYuODEgMi4yMiAwIDEuNjA2LS4wMTUgMi44OTYtLjAxNSAzLjI4NiAwIC4zMTUuMjEuNjkuODI1LjU3QzIwLjU2NSAyMi4wOTIgMjQgMTcuNTkyIDI0IDEyLjI5N2MwLTYuNjI3LTUuMzczLTEyLTEyLTEyIi8+PC9zdmc+" text="GitHub" width={120} height={40} iconSize={18} backgroundColor="#0b0f0d" gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0b0f0d' }, { offset: '50%', color: '#34d399' }, { offset: '65%', color: '#22d3ee' }, { offset: '85%', color: '#0b0f0d' }, { offset: '100%', color: '#555555' }]} />
```
```aura width=128 height=40 link="https://www.youtube.com/@RiftFox_YT" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+WW91VHViZTwvdGl0bGU+PHBhdGggZD0iTTIzLjQ5OCA2LjE4NmEzLjAxNiAzLjAxNiAwIDAgMC0yLjEyMi0yLjEzNkMxOS41MDUgMy41NDUgMTIgMy41NDUgMTIgMy41NDVzLTcuNTA1IDAtOS4zNzcuNTA1QTMuMDE3IDMuMDE3IDAgMCAwIC41MDIgNi4xODZDMCA4LjA3IDAgMTIgMCAxMnMwIDMuOTMuNTAyIDUuODE0YTMuMDE2IDMuMDE2IDAgMCAwIDIuMTIyIDIuMTM2YzEuODcxLjUwNSA5LjM3Ni41MDUgOS4zNzYuNTA1czcuNTA1IDAgOS4zNzctLjUwNWEzLjAxNSAzLjAxNSAwIDAgMCAyLjEyMi0yLjEzNkMyNCAxNS45MyAyNCAxMiAyNCAxMnMwLTMuOTMtLjUwMi01LjgxNHpNOS41NDUgMTUuNTY4VjguNDMyTDE1LjgxOCAxMmwtNi4yNzMgMy41Njh6Ii8+PC9zdmc+" text="YouTube" width={128} height={40} iconSize={18} backgroundColor="#0b0f0d" gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0b0f0d' }, { offset: '50%', color: '#34d399' }, { offset: '65%', color: '#22d3ee' }, { offset: '85%', color: '#0b0f0d' }, { offset: '100%', color: '#555555' }]} />
```
```aura width=124 height=40 link="https://www.threads.net/@s1idermn" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+VGhyZWFkczwvdGl0bGU+PHBhdGggZD0iTTEyLjE4NiAyNGgtLjAwN2MtMy41ODEtLjAyNC02LjMzNC0xLjIwNS04LjE4NC0zLjUwOUMyLjM1IDE4LjQ0IDEuNSAxNS41ODYgMS40NzIgMTIuMDF2LS4wMTdjLjAzLTMuNTc5Ljg3OS02LjQzIDIuNTI1LTguNDgyQzUuODQ1IDEuMjA1IDguNi4wMjQgMTIuMTggMGguMDE0YzIuNzQ2LjAyIDUuMDQzLjcyNSA2LjgyNiAyLjA5OCAxLjY3NyAxLjI5IDIuODU4IDMuMTMgMy41MDkgNS40NjdsLTIuMDQuNTY5Yy0xLjEwNC0zLjk2LTMuODk4LTUuOTg0LTguMzA0LTYuMDE1LTIuOTEuMDIyLTUuMTEuOTM2LTYuNTQgMi43MTdDNC4zMDcgNi41MDQgMy42MTYgOC45MTQgMy41ODkgMTJjLjAyNyAzLjA4Ni43MTggNS40OTYgMi4wNTcgNy4xNjQgMS40MyAxLjc4MyAzLjYzMSAyLjY5OCA2LjU0IDIuNzE3IDIuNjIzLS4wMiA0LjM1OC0uNjMxIDUuOC0yLjA0NSAxLjY0Ny0xLjYxMyAxLjYxOC0zLjU5MyAxLjA5LTQuNzk4LS4zMS0uNzEtLjg3My0xLjMtMS42MzQtMS43NS0uMTkyIDEuMzUyLS42MjIgMi40NDYtMS4yODQgMy4yNzItLjg4NiAxLjEwMi0yLjE0IDEuNzA0LTMuNzMgMS43OS0xLjIwMi4wNjUtMi4zNjEtLjIxOC0zLjI1OS0uODAxLTEuMDYzLS42ODktMS42ODUtMS43NC0xLjc1Mi0yLjk2NC0uMDY1LTEuMTkuNDA4LTIuMjg1IDEuMzMtMy4wODIuODgtLjc2IDIuMTE5LTEuMjA3IDMuNTgzLTEuMjkxYTEzLjg1MyAxMy44NTMgMCAwIDEgMy4wMi4xNDJjLS4xMjYtLjc0Mi0uMzc1LTEuMzMyLS43NS0xLjc1Ny0uNTEzLS41ODYtMS4zMDgtLjg4My0yLjM1OS0uODloLS4wMjljLS44NDQgMC0xLjk5Mi4yMzItMi43MjEgMS4zMkw3LjczNCA3Ljg0N2MuOTgtMS40NTQgMi41NjgtMi4yNTYgNC40NzgtMi4yNTZoLjA0NGMzLjE5NC4wMiA1LjA5NyAxLjk3NSA1LjI4NyA1LjM4OC4xMDguMDQ2LjIxNi4wOTQuMzIxLjE0MiAxLjQ5LjcgMi41OCAxLjc2MSAzLjE1NCAzLjA3Ljc5NyAxLjgyLjg3MSA0Ljc5LTEuNTQ4IDcuMTU4LTEuODUgMS44MS00LjA5NCAyLjYyOC03LjI3NyAyLjY1Wm0xLjAwMy0xMS42OWMtLjI0MiAwLS40ODcuMDA3LS43MzkuMDIxLTEuODM2LjEwMy0yLjk4Ljk0Ni0yLjkxNiAyLjE0My4wNjcgMS4yNTYgMS40NTIgMS44MzkgMi43ODQgMS43NjcgMS4yMjQtLjA2NSAyLjgxOC0uNTQzIDMuMDg2LTMuNzFhMTAuNSAxMC41IDAgMCAwLTIuMjE1LS4yMjF6Ii8+PC9zdmc+" text="Threads" width={124} height={40} iconSize={18} backgroundColor="#0b0f0d" gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0b0f0d' }, { offset: '50%', color: '#34d399' }, { offset: '65%', color: '#22d3ee' }, { offset: '85%', color: '#0b0f0d' }, { offset: '100%', color: '#555555' }]} />
```
```aura width=110 height=40 link="mailto:drakon1384000@gmail.com" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+R21haWw8L3RpdGxlPjxwYXRoIGQ9Ik0yNCA1LjQ1N3YxMy45MDljMCAuOTA0LS43MzIgMS42MzYtMS42MzYgMS42MzZoLTMuODE5VjExLjczTDEyIDE2LjY0bC02LjU0NS00LjkxdjkuMjczSDEuNjM2QTEuNjM2IDEuNjM2IDAgMCAxIDAgMTkuMzY2VjUuNDU3YzAtMi4wMjMgMi4zMDktMy4xNzggMy45MjctMS45NjRMNS40NTUgNC42NCAxMiA5LjU0OGw2LjU0NS00LjkxIDEuNTI4LTEuMTQ1QzIxLjY5IDIuMjggMjQgMy40MzQgMjQgNS40NTd6Ii8+PC9zdmc+" text="Email" width={110} height={40} iconSize={18} backgroundColor="#0b0f0d" gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0b0f0d' }, { offset: '50%', color: '#34d399' }, { offset: '65%', color: '#22d3ee' }, { offset: '85%', color: '#0b0f0d' }, { offset: '100%', color: '#555555' }]} />
```

<br/>

I started learning Java to build custom plugins for my own server, [Asia.noxel.fun](https://asia.noxel.fun), and it grew into a focus on multithreaded, Folia-safe server software. I also work with C# and .NET.

- 🌍 Based in Iran · open to work
- 🛠️ Building **NoxelLib**, a shared library for NoxelSMP
- 🧠 Learning PacketEvents and Folia's region-threaded scheduling

## Featured

```aura width=424 height=150 link="https://github.com/Xenos-core/BluCooldown" inline align=center
<div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#0b0f0d', borderRadius: 16, border: '1px solid rgba(52,211,153,0.25)', padding: 24, fontFamily: 'Inter', position: 'relative', overflow: 'hidden' }}>
  <svg width="424" height="150" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="c1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(52,211,153,0.28)" /><stop offset="70%" stopColor="rgba(52,211,153,0)" /></radialGradient></defs>
    <ellipse cx="400" cy="10" rx="170" ry="110" fill="url(#c1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', gap: 10 }}>
    <div style={{ display: 'flex', width: 10, height: 10, borderRadius: 5, background: '#34d399' }} />
    <div style={{ display: 'flex', fontSize: 22, fontWeight: 700, color: '#ffffff' }}>BluCooldown</div>
  </div>
  <div style={{ display: 'flex', fontSize: 14, color: 'rgba(226,232,240,0.7)', marginTop: 10, lineHeight: 1.45 }}>Lightweight, configurable item cooldowns for Paper and Folia servers.</div>
  <div style={{ display: 'flex', fontSize: 12, color: '#34d399', marginTop: 'auto', letterSpacing: 1 }}>JAVA 21 · MC 1.21+</div>
</div>
```
```aura width=424 height=150 link="https://github.com/Xenos-core/ZelGRank" inline align=center
<div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#0b0f0d', borderRadius: 16, border: '1px solid rgba(34,211,238,0.25)', padding: 24, fontFamily: 'Inter', position: 'relative', overflow: 'hidden' }}>
  <svg width="424" height="150" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="c2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.26)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient></defs>
    <ellipse cx="400" cy="10" rx="170" ry="110" fill="url(#c2)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', gap: 10 }}>
    <div style={{ display: 'flex', width: 10, height: 10, borderRadius: 5, background: '#22d3ee' }} />
    <div style={{ display: 'flex', fontSize: 22, fontWeight: 700, color: '#ffffff' }}>ZelGRank</div>
  </div>
  <div style={{ display: 'flex', fontSize: 14, color: 'rgba(226,232,240,0.7)', marginTop: 10, lineHeight: 1.45 }}>LuckPerms rank manager with temp ranks, notifications and a permissions GUI.</div>
  <div style={{ display: 'flex', fontSize: 12, color: '#22d3ee', marginTop: 'auto', letterSpacing: 1 }}>JAVA · LUCKPERMS API</div>
</div>
```

## Folia Ports

Porting established plugins to Folia's multithreaded server:

| Project | What it is |
|---|---|
| [**Folia-AuraSkills-Update**](https://github.com/Xenos-core/Folia-AuraSkills-Update) | RPG skills plugin, maintained with Folia support |
| [**Folia-lagfixer**](https://github.com/Xenos-core/Folia-lagfixer) | Server performance optimizer |
| [**SvcAdminSpyFolia**](https://github.com/Xenos-core/SvcAdminSpyFolia) | Simple Voice Chat moderation add-on |
| [**lastwordsFolia**](https://github.com/Xenos-core/lastwordsFolia) | Folia-compatible fork |
| [**LimboAPI**](https://github.com/Xenos-core/LimboAPI) | Virtual-server API for Velocity-CTD proxies |

## Stack

```aura width=860 height=128
<div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07090c', borderRadius: 16, border: '1px solid rgba(255,255,255,0.08)', padding: '22px 26px', fontFamily: 'Inter' }}>
  <div style={{ display: 'flex', alignItems: 'center', gap: 10 }}>
    <div style={{ display: 'flex', width: 92, fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 3 }}>MAIN</div>
    {['Java', 'Paper API', 'Folia API', 'Velocity API', 'Git', 'Linux'].map(function (t) {
      return <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 13, color: '#d1fae5', background: 'rgba(52,211,153,0.10)', border: '1px solid rgba(52,211,153,0.32)' }}>{t}</span>;
    })}
  </div>
  <div style={{ display: 'flex', alignItems: 'center', gap: 10, marginTop: 16 }}>
    <div style={{ display: 'flex', width: 92, fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 3 }}>ALSO</div>
    {['C# / .NET', 'C++', 'React', 'Node.js', 'Docker', 'WordPress'].map(function (t) {
      return <span style={{ padding: '6px 14px', borderRadius: 100, fontSize: 13, color: 'rgba(255,255,255,0.65)', background: 'rgba(255,255,255,0.04)', border: '1px solid rgba(255,255,255,0.12)' }}>{t}</span>;
    })}
  </div>
</div>
```
