
<script lang="ts">
  import Chat from '../components/Chat.svelte';
</script>

<div class="page-shell">
  <main class="container">
    <section class="hero" aria-labelledby="page-title">
      <h1 id="page-title">
        AMAZON <span class="title-highlight">4 U</span>
      </h1>

      <p class="tagline">
     Ready to explore the world of Amazon selling in Germany?

Whether you're starting from scratch or planning your next big move, AMAZON 4 U helps you navigate the essentials — from finding product opportunities and understanding FBA to calculating fees and avoiding costly beginner mistakes.

      </p>

      <h3>Your idea. Your ambition. Your next opportunity.</h3>

      <img
        class="avatar"
        src="/jeff.png"
        alt="Jeff Bezos"
        width="210"
        height="210"
      />

      <p class="status-badge" aria-label="Jeff is available to chat">
        <span aria-hidden="true">●</span>
       online
      </p>

    </section>

    <section id="chat" class="chat-section" aria-label="Chat with Lorelyn">
      <Chat />
    </section> 

    <aside class="ai-disclosure" aria-label="AI and privacy notice">
      <span class="disclosure-icon" aria-hidden="true">✦</span>

      <p>
        Fulfillment by Amazon (FBA) is a service that lets sellers outsource their entire order fulfillment
process to Amazon. Instead of packing and shipping products yourself, Amazon handles everything:
      </p>
    </aside>

    <section class="about-section" aria-labelledby="about-heading">
      <h2 id="about-heading">Amazon New Seller Incentives: Unlock Your Potential 🚀</h2>

<p>
  Ready to grow your Amazon business? Eligible new sellers can unlock
  incentives worth up to €47,250. This is the maximum potential value,
  not a guaranteed payout. Benefits are earned progressively by completing
  qualifying actions and meeting Amazon's eligibility requirements.
</p>

<p>
  The biggest opportunity is the <strong>New Brand Bonus</strong>, which
  accounts for the majority of the potential value and requires enrolment
  in Amazon Brand Registry.
</p>

<p>
  <strong>Start smart. Build your brand. Maximize your eligible benefits.</strong>
</p>

      <div class="topic-list" aria-label="Suggested discussion topics">
        <span>Amazon Entry Strategy</span>
        
        <span>Brand</span>
        <span>Entry Strategy</span>
        <span>Flat file</span>
        <span>The Complete
History of Amazon</span>
      </div>
    </section>
  </main>

 <footer class="footer">
    <p class="technology-credit">Created with SvelteKit and deployed on Google Firebase</p>

    <nav class="footer-links" aria-label="Footer navigation">
      <a href="/privacy">Datenschutz</a>
     
    </nav>

    <p class="creator-credit">
      © {new Date().getFullYear()} | Built by
      <a
        href="https://uspekhi.web.app"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Visit USPEKHI Web Development"
      >
        USPEKHI
      </a>
    </p>
  </footer>
</div>

<style>
  :global(*) {
    box-sizing: border-box;
  }

  :global(html) {
    scroll-behavior: smooth;
  }

  :global(body) {
    min-width: 320px;
    min-height: 100vh;
    min-height: 100svh;
    margin: 0;
    color: #f8fafc;
    font-family:
      'Inter',
      -apple-system,
      BlinkMacSystemFont,
      'Segoe UI',
      sans-serif;
    background:
      radial-gradient(
        circle at 12% 8%,
        rgba(223, 239, 243, 0.12),
        transparent 32rem
      ),
      radial-gradient(
        circle at 90% 88%,
        rgba(217, 225, 238, 0.14),
        transparent 35rem
      ),
      linear-gradient(135deg, #6951d4 0%, #3466d1 48%, #45699b 100%);
  }

  

  .page-shell {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    min-height: 100svh;
  }

  .container {
    width: min(100% - 2rem, 1040px);
    flex: 1;
    margin: 0 auto;
    padding: clamp(2.5rem, 6vw, 5.5rem) 0 2rem;
    text-align: center;
  }

  .hero {
    display: grid;
    justify-items: center;
    gap: 1.25rem;
  }

  h1 {
    max-width: 980px;
    margin: 0;
    color: #f8fafc;
    font-size: clamp(2.5rem, 6.4vw, 5.75rem);
    font-weight: 800;
    line-height: 1.02;
    letter-spacing: -0.055em;
    text-wrap: balance;
  }

  .title-highlight {
    color: #a9dff2;
    text-shadow: 0 0 28px rgba(110, 231, 255, 0.12);
  }

  .tagline {
    max-width: 700px;
    margin: 0.4rem auto 0;
    color: #d5dfef;
    font-size: clamp(1.05rem, 1.6vw, 1.3rem);
    font-weight: 400;
    line-height: 1.7;
    text-wrap: pretty;
  }

  .avatar {
    width: clamp(152px, 18vw, 210px);
    height: clamp(152px, 18vw, 210px);
    display: block;
    margin: 0.75rem auto 0;
    object-fit: cover;
    border: 3px solid #28d7e5;
    border-radius: 50%;
    background-color: #0b0d17;
    box-shadow:
      0 0 0 5px rgba(40, 215, 229, 0.09),
      0 0 28px rgba(40, 215, 229, 0.32);
  }

  .status-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    margin: -0.2rem 0 0;
    padding: 0.4rem 0.75rem;
    border: 1px solid rgba(169, 223, 242, 0.2);
    border-radius: 999px;
    color: #b9c8dc;
    font-size: 0.84rem;
    line-height: 1;
    background: rgba(169, 223, 242, 0.06);
  }

  .status-badge span {
    color: #4ade80;
    font-size: 0.7rem;
    text-shadow: 0 0 8px rgba(74, 222, 128, 0.65);
  }

  .chat-section {
    width: min(100%, 860px);
    margin: clamp(2rem, 5vw, 3.5rem) auto 0;
    overflow: hidden;
    text-align: left;
    border: 1px solid rgba(173, 216, 230, 0.18);
    border-radius: 18px;
    background: rgba(15, 23, 42, 0.58);
    box-shadow:
      0 18px 55px rgba(0, 0, 0, 0.22),
      inset 0 1px 0 rgba(255, 255, 255, 0.04);
    backdrop-filter: blur(14px);
  }

  .ai-disclosure {
    display: flex;
    align-items: flex-start;
    gap: 0.7rem;
    width: min(100%, 860px);
    margin: 1rem auto 0;
    padding: 0.85rem 1rem;
    border: 1px solid rgba(169, 223, 242, 0.14);
    border-radius: 12px;
    color: #b9c8dc;
    font-size: 0.84rem;
    line-height: 1.55;
    text-align: left;
    background: rgba(169, 223, 242, 0.05);
  }

  .ai-disclosure p {
    margin: 0;
  }

  .disclosure-icon {
    margin-top: 0.05rem;
    color: #81e6ee;
    font-size: 1rem;
  }

  .about-section {
    width: min(100%, 760px);
    margin: clamp(3rem, 7vw, 5rem) auto 0;
    padding: 1.75rem;
    border: 1px solid rgba(173, 216, 230, 0.12);
    border-radius: 18px;
    text-align: left;
    background: rgba(255, 255, 255, 0.035);
  }

  .about-section h2 {
    margin: 0;
    color: #f8fafc;
    font-size: clamp(1.35rem, 2.3vw, 1.7rem);
    letter-spacing: -0.02em;
  }

  .about-section p {
    max-width: 680px;
    margin: 0.85rem 0 0;
    color: #c8d4e5;
    line-height: 1.65;
  }

  .topic-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    margin-top: 1.25rem;
  }

  .topic-list span {
    padding: 0.48rem 0.72rem;
    border: 1px solid rgba(169, 223, 242, 0.18);
    border-radius: 999px;
    color: #ccecf5;
    font-size: 0.84rem;
    background: rgba(169, 223, 242, 0.06);
  }

  .footer {
    width: min(100% - 2rem, 1040px);
    margin: 0 auto;
    padding: 2.25rem 0 2.5rem;
    color: #aebbd0;
    font-size: 0.9rem;
    text-align: center;
  }

  .footer p {
    margin: 0;
  }

  .technology-credit {
    color: #91a1b9;
    font-size: 0.8rem;
  }

  .footer-links {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.55rem 1rem;
    margin: 0.85rem 0;
  }

  .footer a {
    color: #b5edf7;
    font-weight: 650;
    text-underline-offset: 3px;
  }

  .footer a:hover {
    color: #ffffff;
  }

  .creator-credit {
    font-size: 0.86rem;
  }

  :global(button:focus-visible),
  :global(a:focus-visible),
  :global(input:focus-visible),
  :global(textarea:focus-visible) {
    outline: 3px solid rgba(110, 231, 255, 0.8);
    outline-offset: 3px;
  }

  @media (max-width: 560px) {
    .container {
      width: min(100% - 1.25rem, 1040px);
      padding-top: clamp(1.5rem, 7svh, 2.25rem);
      padding-bottom: 1.25rem;
    }

    .hero {
      gap: 0.9rem;
    }

    h1 {
      font-size: clamp(2.2rem, 11.5vw, 3.6rem);
      letter-spacing: -0.045em;
    }

    .tagline {
      font-size: clamp(1rem, 4vw, 1.08rem);
      line-height: 1.55;
    }

    .avatar {
      width: clamp(112px, 32vw, 148px);
      height: clamp(112px, 32vw, 148px);
      margin-top: 0.15rem;
    }

    .chat-section {
      margin-top: clamp(1.25rem, 5vw, 2rem);
      border-radius: 14px;
    }

    .ai-disclosure {
      margin-top: 0.75rem;
      font-size: 0.86rem;
    }

    .about-section {
      margin-top: clamp(2rem, 8vw, 3rem);
      padding: 1.1rem;
    }

    .footer {
      width: min(100% - 1.25rem, 1040px);
      padding: 1.5rem 0 calc(1.5rem + env(safe-area-inset-bottom));
    }

    .footer-links a {
      display: inline-flex;
      align-items: center;
      min-height: 44px;
      padding: 0.25rem 0.4rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    :global(*) {
      scroll-behavior: auto !important;
      transition-duration: 0.01ms !important;
      animation-duration: 0.01ms !important;
    }
  }
</style>