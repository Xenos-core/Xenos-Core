```aura width=860 height=200
<div style={{ width: '100%', height: '100%', display: 'flex', alignItems: 'center', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="172" cy="230" rx="258" ry="190" fill="url(#ra)" />
    <ellipse id="gb" cx="473" cy="240" rx="223" ry="160" fill="url(#rb)" />
    <ellipse id="gc" cx="344" cy="235" rx="172" ry="140" fill="url(#rc)" />
    <ellipse id="gd" cx="731" cy="230" rx="154" ry="130" fill="url(#rd)" />
    <ellipse id="ge" cx="602" cy="220" rx="120" ry="110" fill="url(#re)" />
  </svg>
  <div style={{ position: 'absolute', left: 48, top: 52, width: 96, height: 96, borderRadius: 48, background: 'linear-gradient(135deg, #10b981, #22d3ee)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
    <img src=".github/aura/avatar.png" width={88} height={88} style={{ borderRadius: 44 }} />
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 168, gap: 8 }}>
    <div style={{ display: 'flex', fontSize: 38, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1 }}>Alireza</div>
    <div style={{ display: 'flex', fontSize: 15, color: 'rgba(167,243,208,0.8)', letterSpacing: '0.3px' }}>Java developer · Paper, Folia and Velocity plugins · Based in Iran</div>
    <div style={{ display: 'flex', gap: 8, marginTop: 6 }}>
      {['Java 21', 'Paper', 'Folia', 'Velocity'].map(function(tag) {
        return <div key={tag} style={{ display: 'flex', padding: '4px 12px', borderRadius: 20, background: 'rgba(16,185,129,0.16)', border: '1px solid rgba(52,211,153,0.34)', color: 'rgba(209,250,229,0.88)', fontSize: 12, fontWeight: 600 }}>{tag}</div>;
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=140
(function() {
  var s = (github && github.stats) || {};
  var u = (github && github.user) || {};
  var stats = [
    { label: 'Repos', value: String(s.totalRepos || 0), color: '#34d399' },
    { label: 'Stars', value: String(s.totalStars || 0), color: '#22d3ee' },
    { label: 'Commits', value: String(s.totalCommits || 0), color: '#a3e635' },
    { label: 'Followers', value: String(s.followers || u.followers || 0), color: '#60a5fa' },
  ];
  return (
    <div style={{ width: '100%', height: '100%', display: 'flex', alignItems: 'center', justifyContent: 'center', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="172" cy="170" rx="258" ry="133" fill="url(#ra)" />
    <ellipse id="gb" cx="473" cy="180" rx="223" ry="112" fill="url(#rb)" />
    <ellipse id="gc" cx="344" cy="175" rx="172" ry="98" fill="url(#rc)" />
    <ellipse id="gd" cx="731" cy="170" rx="154" ry="91" fill="url(#rd)" />
    <ellipse id="ge" cx="602" cy="160" rx="120" ry="77" fill="url(#re)" />
  </svg>
      {stats.map(function(st, i) {
        return (
          <div key={st.label} style={{ flexGrow: 1, display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', padding: '16px 8px', gap: 5, borderRight: i < stats.length - 1 ? '1px solid rgba(255,255,255,0.06)' : 'none' }}>
            <div style={{ display: 'flex', fontSize: 30, fontWeight: 800, color: st.color, lineHeight: 1 }}>{st.value}</div>
            <div style={{ display: 'flex', fontSize: 11, color: 'rgba(209,250,229,0.45)', fontWeight: 600, letterSpacing: '1.5px' }}>{st.label.toUpperCase()}</div>
          </div>
        );
      })}
    </div>
  );
})()
```

```aura width=405 height=164 link="https://github.com/Xenos-core/BluCooldown" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', padding: 24, background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="405" height="164" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="81" cy="194" rx="121" ry="155" fill="url(#ra)" />
    <ellipse id="gb" cx="222" cy="204" rx="105" ry="131" fill="url(#rb)" />
    <ellipse id="gc" cx="162" cy="199" rx="81" ry="114" fill="url(#rc)" />
    <ellipse id="gd" cx="344" cy="194" rx="72" ry="106" fill="url(#rd)" />
    <ellipse id="ge" cx="283" cy="184" rx="56" ry="90" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 10, fontWeight: 700, color: 'rgba(209,250,229,0.45)', letterSpacing: '3px' }}>FEATURED</div>
  <div style={{ display: 'flex', fontSize: 22, fontWeight: 800, color: '#ffffff', marginTop: 8 }}>BluCooldown</div>
  <div style={{ display: 'flex', fontSize: 13, color: 'rgba(226,232,240,0.7)', marginTop: 6, lineHeight: 1.45 }}>Lightweight, configurable item cooldowns for Paper and Folia servers.</div>
  <div style={{ display: 'flex', fontSize: 11, fontWeight: 700, color: '#34d399', marginTop: 'auto', letterSpacing: '1px' }}>JAVA 21 · MC 1.21+</div>
</div>
```

```aura width=405 height=164 link="https://github.com/Xenos-core/ZelGRank" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', padding: 24, background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="405" height="164" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="81" cy="194" rx="121" ry="155" fill="url(#ra)" />
    <ellipse id="gb" cx="222" cy="204" rx="105" ry="131" fill="url(#rb)" />
    <ellipse id="gc" cx="162" cy="199" rx="81" ry="114" fill="url(#rc)" />
    <ellipse id="gd" cx="344" cy="194" rx="72" ry="106" fill="url(#rd)" />
    <ellipse id="ge" cx="283" cy="184" rx="56" ry="90" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 10, fontWeight: 700, color: 'rgba(209,250,229,0.45)', letterSpacing: '3px' }}>FEATURED</div>
  <div style={{ display: 'flex', fontSize: 22, fontWeight: 800, color: '#ffffff', marginTop: 8 }}>ZelGRank</div>
  <div style={{ display: 'flex', fontSize: 13, color: 'rgba(226,232,240,0.7)', marginTop: 6, lineHeight: 1.45 }}>LuckPerms rank manager with temp ranks, notifications and a permissions GUI.</div>
  <div style={{ display: 'flex', fontSize: 11, fontWeight: 700, color: '#22d3ee', marginTop: 'auto', letterSpacing: '1px' }}>JAVA · LUCKPERMS API</div>
</div>
```

<br/>

```aura width=268 height=76 link="https://github.com/Xenos-core/Folia-AuraSkills-Update" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 18px', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="268" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="53" cy="106" rx="80" ry="72" fill="url(#ra)" />
    <ellipse id="gb" cx="147" cy="116" rx="69" ry="60" fill="url(#rb)" />
    <ellipse id="gc" cx="107" cy="111" rx="53" ry="53" fill="url(#rc)" />
    <ellipse id="gd" cx="227" cy="106" rx="48" ry="49" fill="url(#rd)" />
    <ellipse id="ge" cx="187" cy="96" rx="37" ry="41" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff' }}>Folia-AuraSkills-Update</div>
  <div style={{ display: 'flex', fontSize: 11, color: 'rgba(167,243,208,0.65)', marginTop: 4 }}>RPG skills, Folia support</div>
</div>
```

```aura width=268 height=76 link="https://github.com/Xenos-core/Folia-lagfixer" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 18px', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="268" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="53" cy="106" rx="80" ry="72" fill="url(#ra)" />
    <ellipse id="gb" cx="147" cy="116" rx="69" ry="60" fill="url(#rb)" />
    <ellipse id="gc" cx="107" cy="111" rx="53" ry="53" fill="url(#rc)" />
    <ellipse id="gd" cx="227" cy="106" rx="48" ry="49" fill="url(#rd)" />
    <ellipse id="ge" cx="187" cy="96" rx="37" ry="41" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff' }}>Folia-lagfixer</div>
  <div style={{ display: 'flex', fontSize: 11, color: 'rgba(167,243,208,0.65)', marginTop: 4 }}>Performance optimizer</div>
</div>
```

```aura width=268 height=76 link="https://github.com/Xenos-core/SvcAdminSpyFolia" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 18px', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="268" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="53" cy="106" rx="80" ry="72" fill="url(#ra)" />
    <ellipse id="gb" cx="147" cy="116" rx="69" ry="60" fill="url(#rb)" />
    <ellipse id="gc" cx="107" cy="111" rx="53" ry="53" fill="url(#rc)" />
    <ellipse id="gd" cx="227" cy="106" rx="48" ry="49" fill="url(#rd)" />
    <ellipse id="ge" cx="187" cy="96" rx="37" ry="41" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff' }}>SvcAdminSpyFolia</div>
  <div style={{ display: 'flex', fontSize: 11, color: 'rgba(167,243,208,0.65)', marginTop: 4 }}>Voice chat moderation</div>
</div>
```

```aura width=268 height=76 link="https://github.com/Xenos-core/lastwordsFolia" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 18px', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="268" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="53" cy="106" rx="80" ry="72" fill="url(#ra)" />
    <ellipse id="gb" cx="147" cy="116" rx="69" ry="60" fill="url(#rb)" />
    <ellipse id="gc" cx="107" cy="111" rx="53" ry="53" fill="url(#rc)" />
    <ellipse id="gd" cx="227" cy="106" rx="48" ry="49" fill="url(#rd)" />
    <ellipse id="ge" cx="187" cy="96" rx="37" ry="41" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff' }}>lastwordsFolia</div>
  <div style={{ display: 'flex', fontSize: 11, color: 'rgba(167,243,208,0.65)', marginTop: 4 }}>Folia-compatible fork</div>
</div>
```

```aura width=268 height=76 link="https://github.com/Xenos-core/LimboAPI" inline align=center
<div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 18px', background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="268" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="53" cy="106" rx="80" ry="72" fill="url(#ra)" />
    <ellipse id="gb" cx="147" cy="116" rx="69" ry="60" fill="url(#rb)" />
    <ellipse id="gc" cx="107" cy="111" rx="53" ry="53" fill="url(#rc)" />
    <ellipse id="gd" cx="227" cy="106" rx="48" ry="49" fill="url(#rd)" />
    <ellipse id="ge" cx="187" cy="96" rx="37" ry="41" fill="url(#re)" />
  </svg>
  <div style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff' }}>LimboAPI</div>
  <div style={{ display: 'flex', fontSize: 11, color: 'rgba(167,243,208,0.65)', marginTop: 4 }}>Virtual servers for Velocity</div>
</div>
```

<br/>

```aura width=860 height=190
(function() {
  var cats = [
    { title: 'Main', color: '#34d399', items: ['Java', 'Paper API', 'Folia API', 'Velocity API', 'PacketEvents'] },
    { title: 'Also', color: '#22d3ee', items: ['C# / .NET', 'C++', 'React', 'Node.js'] },
    { title: 'Tools', color: '#a3e635', items: ['Git', 'Linux', 'Docker', 'Gradle', 'Maven'] },
  ];
  return (
    <div style={{ width: '100%', height: '100%', display: 'flex', flexDirection: 'column', padding: '18px 32px', gap: 14, background: '#060a09', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(52,211,153,0.18)' }}>

  <style>{`
    @keyframes f-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes f-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-240px); opacity: 1; } }
    @keyframes f-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(180px); opacity: 0.6; } }
    @keyframes f-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-150px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1; } }
    @keyframes f-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.25); opacity: 0.45; } }
    #ga { animation: f-slow 9s ease-in-out infinite; }
    #gb { animation: f-med 12s ease-in-out infinite; }
    #gc { animation: f-fast 8s ease-in-out infinite; }
    #gd { animation: f-wave 13s ease-in-out infinite; }
    #ge { animation: f-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="190" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ra" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(16,185,129,0.62)" /><stop offset="42%" stopColor="rgba(5,150,105,0.26)" /><stop offset="70%" stopColor="rgba(5,150,105,0)" /></radialGradient>
      <radialGradient id="rb" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="45%" stopColor="rgba(8,145,178,0.2)" /><stop offset="70%" stopColor="rgba(8,145,178,0)" /></radialGradient>
      <radialGradient id="rc" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(20,184,166,0.45)" /><stop offset="70%" stopColor="rgba(20,184,166,0)" /></radialGradient>
      <radialGradient id="rd" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.34)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="re" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(132,204,22,0.30)" /><stop offset="70%" stopColor="rgba(132,204,22,0)" /></radialGradient>
    </defs>
    <ellipse id="ga" cx="172" cy="220" rx="258" ry="180" fill="url(#ra)" />
    <ellipse id="gb" cx="473" cy="230" rx="223" ry="152" fill="url(#rb)" />
    <ellipse id="gc" cx="344" cy="225" rx="172" ry="133" fill="url(#rc)" />
    <ellipse id="gd" cx="731" cy="220" rx="154" ry="123" fill="url(#rd)" />
    <ellipse id="ge" cx="602" cy="210" rx="120" ry="104" fill="url(#re)" />
  </svg>
      <div style={{ display: 'flex', fontSize: 10, fontWeight: 700, color: 'rgba(209,250,229,0.45)', letterSpacing: '3px' }}>TECH STACK</div>
      <div style={{ display: 'flex', flexDirection: 'column', gap: 14 }}>
        {cats.map(function(c) {
          return (
            <div key={c.title} style={{ display: 'flex', alignItems: 'center', gap: 16 }}>
              <div style={{ display: 'flex', fontSize: 10, fontWeight: 700, color: c.color, letterSpacing: '1px', width: 80 }}>{c.title.toUpperCase()}</div>
              <div style={{ display: 'flex', flexWrap: 'wrap', gap: 7 }}>
                {c.items.map(function(it) {
                  return <div key={it} style={{ display: 'flex', padding: '4px 13px', borderRadius: 6, background: c.color + '15', border: '1px solid ' + c.color + '40', color: 'rgba(236,253,245,0.88)', fontSize: 12, fontWeight: 600 }}>{it}</div>;
                })}
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
})()
```

<br/>

```aura width=140 height=44 link="https://asia.noxel.fun" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmZmZmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiLz48cGF0aCBkPSJNMiAxMmgyMCIvPjxwYXRoIGQ9Ik0xMiAyYTE1LjMgMTUuMyAwIDAgMSA0IDEwIDE1LjMgMTUuMyAwIDAgMS00IDEwIDE1LjMgMTUuMyAwIDAgMS00LTEwIDE1LjMgMTUuMyAwIDAgMSA0LTEweiIvPjwvc3ZnPgo=" text="Noxel SMP" backgroundColor="#000000" width={140} height={44} gradientStops={[{ offset: '0%', color: '#34d399' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#6ee7b7' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#10b981' }]} />
```

```aura width=128 height=44 link="https://www.youtube.com/@RiftFox_YT" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+WW91VHViZTwvdGl0bGU+PHBhdGggZD0iTTIzLjQ5OCA2LjE4NmEzLjAxNiAzLjAxNiAwIDAgMC0yLjEyMi0yLjEzNkMxOS41MDUgMy41NDUgMTIgMy41NDUgMTIgMy41NDVzLTcuNTA1IDAtOS4zNzcuNTA1QTMuMDE3IDMuMDE3IDAgMCAwIC41MDIgNi4xODZDMCA4LjA3IDAgMTIgMCAxMnMwIDMuOTMuNTAyIDUuODE0YTMuMDE2IDMuMDE2IDAgMCAwIDIuMTIyIDIuMTM2YzEuODcxLjUwNSA5LjM3Ni41MDUgOS4zNzYuNTA1czcuNTA1IDAgOS4zNzctLjUwNWEzLjAxNSAzLjAxNSAwIDAgMCAyLjEyMi0yLjEzNkMyNCAxNS45MyAyNCAxMiAyNCAxMnMwLTMuOTMtLjUwMi01LjgxNHpNOS41NDUgMTUuNTY4VjguNDMyTDE1LjgxOCAxMmwtNi4yNzMgMy41Njh6Ii8+PC9zdmc+" text="YouTube" backgroundColor="#000000" width={128} height={44} gradientStops={[{ offset: '0%', color: '#f87171' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#fb7185' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#ef4444' }]} />
```

```aura width=124 height=44 link="https://www.threads.net/@s1idermn" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+VGhyZWFkczwvdGl0bGU+PHBhdGggZD0iTTEyLjE4NiAyNGgtLjAwN2MtMy41ODEtLjAyNC02LjMzNC0xLjIwNS04LjE4NC0zLjUwOUMyLjM1IDE4LjQ0IDEuNSAxNS41ODYgMS40NzIgMTIuMDF2LS4wMTdjLjAzLTMuNTc5Ljg3OS02LjQzIDIuNTI1LTguNDgyQzUuODQ1IDEuMjA1IDguNi4wMjQgMTIuMTggMGguMDE0YzIuNzQ2LjAyIDUuMDQzLjcyNSA2LjgyNiAyLjA5OCAxLjY3NyAxLjI5IDIuODU4IDMuMTMgMy41MDkgNS40NjdsLTIuMDQuNTY5Yy0xLjEwNC0zLjk2LTMuODk4LTUuOTg0LTguMzA0LTYuMDE1LTIuOTEuMDIyLTUuMTEuOTM2LTYuNTQgMi43MTdDNC4zMDcgNi41MDQgMy42MTYgOC45MTQgMy41ODkgMTJjLjAyNyAzLjA4Ni43MTggNS40OTYgMi4wNTcgNy4xNjQgMS40MyAxLjc4MyAzLjYzMSAyLjY5OCA2LjU0IDIuNzE3IDIuNjIzLS4wMiA0LjM1OC0uNjMxIDUuOC0yLjA0NSAxLjY0Ny0xLjYxMyAxLjYxOC0zLjU5MyAxLjA5LTQuNzk4LS4zMS0uNzEtLjg3My0xLjMtMS42MzQtMS43NS0uMTkyIDEuMzUyLS42MjIgMi40NDYtMS4yODQgMy4yNzItLjg4NiAxLjEwMi0yLjE0IDEuNzA0LTMuNzMgMS43OS0xLjIwMi4wNjUtMi4zNjEtLjIxOC0zLjI1OS0uODAxLTEuMDYzLS42ODktMS42ODUtMS43NC0xLjc1Mi0yLjk2NC0uMDY1LTEuMTkuNDA4LTIuMjg1IDEuMzMtMy4wODIuODgtLjc2IDIuMTE5LTEuMjA3IDMuNTgzLTEuMjkxYTEzLjg1MyAxMy44NTMgMCAwIDEgMy4wMi4xNDJjLS4xMjYtLjc0Mi0uMzc1LTEuMzMyLS43NS0xLjc1Ny0uNTEzLS41ODYtMS4zMDgtLjg4My0yLjM1OS0uODloLS4wMjljLS44NDQgMC0xLjk5Mi4yMzItMi43MjEgMS4zMkw3LjczNCA3Ljg0N2MuOTgtMS40NTQgMi41NjgtMi4yNTYgNC40NzgtMi4yNTZoLjA0NGMzLjE5NC4wMiA1LjA5NyAxLjk3NSA1LjI4NyA1LjM4OC4xMDguMDQ2LjIxNi4wOTQuMzIxLjE0MiAxLjQ5LjcgMi41OCAxLjc2MSAzLjE1NCAzLjA3Ljc5NyAxLjgyLjg3MSA0Ljc5LTEuNTQ4IDcuMTU4LTEuODUgMS44MS00LjA5NCAyLjYyOC03LjI3NyAyLjY1Wm0xLjAwMy0xMS42OWMtLjI0MiAwLS40ODcuMDA3LS43MzkuMDIxLTEuODM2LjEwMy0yLjk4Ljk0Ni0yLjkxNiAyLjE0My4wNjcgMS4yNTYgMS40NTIgMS44MzkgMi43ODQgMS43NjcgMS4yMjQtLjA2NSAyLjgxOC0uNTQzIDMuMDg2LTMuNzFhMTAuNSAxMC41IDAgMCAwLTIuMjE1LS4yMjF6Ii8+PC9zdmc+" text="Threads" backgroundColor="#000000" width={124} height={44} gradientStops={[{ offset: '0%', color: '#e5e7eb' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#9ca3af' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#f3f4f6' }]} />
```

```aura width=110 height=44 link="mailto:drakon1384000@gmail.com" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+R21haWw8L3RpdGxlPjxwYXRoIGQ9Ik0yNCA1LjQ1N3YxMy45MDljMCAuOTA0LS43MzIgMS42MzYtMS42MzYgMS42MzZoLTMuODE5VjExLjczTDEyIDE2LjY0bC02LjU0NS00LjkxdjkuMjczSDEuNjM2QTEuNjM2IDEuNjM2IDAgMCAxIDAgMTkuMzY2VjUuNDU3YzAtMi4wMjMgMi4zMDktMy4xNzggMy45MjctMS45NjRMNS40NTUgNC42NCAxMiA5LjU0OGw2LjU0NS00LjkxIDEuNTI4LTEuMTQ1QzIxLjY5IDIuMjggMjQgMy40MzQgMjQgNS40NTd6Ii8+PC9zdmc+" text="Email" backgroundColor="#000000" width={110} height={44} gradientStops={[{ offset: '0%', color: '#22d3ee' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#67e8f9' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#06b6d4' }]} />
```

<p align="center"><sub>powered by <a href="https://github.com/collectioneur/readme-aura">readme-aura</a></sub></p>
