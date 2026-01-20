<!-- Profile + About (Markdown-safe HTML with animations) -->
<style>
  /* Accessibility: respect reduced motion */
  @media (prefers-reduced-motion: reduce) {
    .rm-avatar,
    .glow-name {
      animation: none !important;
    }
  }

  /* =========================
     Avatar (Circle Frame)
     ========================= */
  .rm-avatar {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    object-fit: cover;
    float: left;
    margin-right: 18px;
    margin-bottom: 12px;

    /* circle frame + glow */
    border: 3px solid rgba(255, 60, 60, 0.9);
    box-shadow:
      0 0 12px rgba(255, 60, 60, 0.55),
      0 0 28px rgba(255, 60, 60, 0.35);

    /* animation */
    animation: avatar-float 3s ease-in-out infinite;
    transition: transform .25s ease, box-shadow .25s ease;
  }

  .rm-avatar:hover {
    transform: scale(1.06);
    box-shadow:
      0 0 18px rgba(255, 80, 80, 0.8),
      0 0 40px rgba(255, 80, 80, 0.55);
  }

  @keyframes avatar-float {
    0%, 100% { transform: translateY(4px); }
    50% { transform: translateY(-4px); }
  }

  /* =========================
     Name Glow (Red)
     ========================= */
  .glow-name {
    font-weight: 700;
    color: #ffecec;
    text-shadow:
      0 0 6px rgba(255, 60, 60, 0.7),
      0 0 14px rgba(255, 60, 60, 0.5),
      0 0 28px rgba(255, 60, 60, 0.35);
    animation: glow-pulse 2.8s ease-in-out infinite;
  }

  @keyframes glow-pulse {
    0%, 100% {
      text-shadow:
        0 0 6px rgba(255, 60, 60, 0.7),
        0 0 14px rgba(255, 60, 60, 0.5),
        0 0 28px rgba(255, 60, 60, 0.35);
    }
    50% {
      text-shadow:
        0 0 10px rgba(255, 90, 90, 0.95),
        0 0 26px rgba(255, 90, 90, 0.7),
        0 0 48px rgba(255, 90, 90, 0.5);
    }
  }
</style>

<img
  class="rm-avatar"
  src="https://avatars.githubusercontent.com/u/160775654?v=4"
  alt="Rainiel Montañez"
/>

<div style="min-width:240px; flex:1;">
  <h2 style="margin:0 0 8px 0;">ABOUT ME</h2>

  <p>
    Hi, I’m <span class="glow-name">Rainiel Montañez</span> — an IT enthusiast, DevOps, Automation, and self-proclaimed Vibe Coder.
  </p>

  <p>
    I enjoy creating apps, websites, and simple tutorials that help others learn and build.
    I like creating new things, learning new things, and exploring how systems work under the hood.
  </p>

  <p>
    While I’m still growing my coding skills, I’m highly skilled at using AI tools to turn ideas
    into functional and practical projects—from automation to experiments and modifications.
  </p>

  <p>
    This website is where I share my work, tutorials, OS experiments, system modifications,
    and the things I continue to learn along the way.
  </p>
</div>
