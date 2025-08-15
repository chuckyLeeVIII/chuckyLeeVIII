<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>chuckyLeeVIII | Alien Tech Architect</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="https://unpkg.com/@dotlottie/player-component@latest/dist/dotlottie-player.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&family=Exo+2:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&family=Exo+2:wght@300;400;600&display=swap');
    
    body {
      background-color: #0a0a0a;
      background-image: 
        radial-gradient(circle at 25% 25%, rgba(0, 200, 83, 0.1) 0%, transparent 50%),
        radial-gradient(circle at 75% 75%, rgba(234, 74, 170, 0.1) 0%, transparent 50%);
      font-family: 'Exo 2', sans-serif;
      color: #e0e0e0;
    }
    
    .orbitron {
      font-family: 'Orbitron', sans-serif;
    }
    
    .glow-text {
      text-shadow: 0 0 10px rgba(0, 200, 83, 0.7), 0 0 20px rgba(0, 200, 83, 0.4);
    }
    
    .neon-border {
      border: 1px solid rgba(0, 200, 83, 0.3);
      box-shadow: 0 0 15px rgba(0, 200, 83, 0.2), inset 0 0 10px rgba(0, 200, 83, 0.1);
    }
    
    .card-glow {
      box-shadow: 0 0 20px rgba(0, 200, 83, 0.15);
      transition: all 0.3s ease;
    }
    
    .card-glow:hover {
      box-shadow: 0 0 30px rgba(0, 200, 83, 0.25), 0 0 40px rgba(234, 74, 170, 0.15);
      transform: translateY(-5px);
    }
    
    .pulse {
      animation: pulse 2s infinite;
    }
    
    @keyframes pulse {
      0% { opacity: 0.7; }
      50% { opacity: 1; }
      100% { opacity: 0.7; }
    }
    
    .typing-animation {
      overflow: hidden;
      border-right: 2px solid #00C853;
      white-space: nowrap;
      margin: 0 auto;
      letter-spacing: 0.15em;
      animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
    }
    
    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }
    
    @keyframes blink-caret {
      from, to { border-color: transparent }
      50% { border-color: #00C853 }
    }
    
    .floating {
      animation: floating 6s ease-in-out infinite;
    }
    
    @keyframes floating {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0px); }
    }
    
    .grid-pattern {
      background-image: 
        linear-gradient(rgba(0, 200, 83, 0.1) 1px, transparent 1px),
        linear-gradient(90deg, rgba(0, 200, 83, 0.1) 1px, transparent 1px);
      background-size: 50px 50px;
    }
    
    .hover-scale {
      transition: transform 0.3s ease;
    }
    
    .hover-scale:hover {
      transform: scale(1.05);
    }
    
    .progress-bar {
      height: 4px;
      background: rgba(234, 74, 170, 0.3);
      border-radius: 2px;
      overflow: hidden;
    }
    
    .progress-fill {
      height: 100%;
      background: linear-gradient(90deg, #00C853, #EA4AAA);
      border-radius: 2px;
      animation: progress-fill 2s ease-in-out;
    }
    
    @keyframes progress-fill {
      0% { width: 0%; }
      100% { width: 97%; }
    }
  </style>
</head>
<body class="min-h-screen">
  <!-- Animated Background Elements -->
  <div class="fixed inset-0 overflow-hidden pointer-events-none">
    <div class="absolute top-1/4 left-1/4 w-2 h-2 bg-green-400 rounded-full animate-pulse"></div>
    <div class="absolute top-3/4 right-1/4 w-1 h-1 bg-pink-400 rounded-full animate-pulse" style="animation-delay: 1s"></div>
    <div class="absolute bottom-1/4 left-1/3 w-1.5 h-1.5 bg-cyan-400 rounded-full animate-pulse" style="animation-delay: 2s"></div>
    <div class="absolute top-1/2 right-1/3 w-1 h-1 bg-purple-400 rounded-full animate-pulse" style="animation-delay: 0.5s"></div>
  </div>

  <div class="container mx-auto px-4 py-8 relative">
    <!-- Header Section -->
    <header class="text-center mb-12">
      <div class="flex flex-col items-center justify-center mb-6">
        <h1 class="text-5xl md:text-7xl font-black orbitron text-transparent bg-clip-text bg-gradient-to-r from-green-400 via-pink-400 to-cyan-400 glow-text mb-2">
          <span class="typing-animation">chuckyLeeVIII</span>
        </h1>
        <div class="flex items-center space-x-2 mb-4">
          <div class="w-2 h-2 bg-green-400 rounded-full pulse"></div>
          <span class="text-sm text-green-400 font-mono">ALIEN TECH ARCHITECT</span>
          <div class="w-2 h-2 bg-green-400 rounded-full pulse" style="animation-delay: 0.5s"></div>
        </div>
      </div>

      <p class="text-xl md:text-2xl text-gray-300 mb-4 font-light">
        Architect of <span class="text-green-400 font-semibold">Trustless Systems</span> · 
        <span class="text-pink-400 font-semibold">OPSEC</span> Advocate · 
        <span class="text-cyan-400 font-semibold">Protocol</span> Engineer
      </p>
      
      <blockquote class="text-lg md:text-xl italic text-gray-400 max-w-3xl mx-auto border-l-4 border-green-400 pl-6 my-8">
        "My work is my word — <span class="text-green-400 font-bold">100% trustless</span>."
      </blockquote>
    </header>

    <!-- Action Badges -->
    <div class="flex flex-wrap justify-center gap-3 mb-12">
      <a href="https://exdex.cc/" class="hover-scale transform transition-all duration-300">
        <div class="bg-gray-900 px-6 py-3 rounded-full border border-green-400/30 hover:border-green-400 transition-all duration-300 flex items-center space-x-2">
          <svg class="w-5 h-5 text-green-400" fill="currentColor" viewBox="0 0 20 20">
            <path d="M10 12a2 2 0 100-4 2 2 0 000 4z"></path>
            <path fill-rule="evenodd" d="M.458 10C1.732 5.943 5.522 3 10 3s8.268 2.943 9.542 7c-1.274 4.057-5.064 7-9.542 7S1.732 14.057.458 10zM14 10a4 4 0 11-8 0 4 4 0 018 0z" clip-rule="evenodd"></path>
          </svg>
          <span class="text-white font-mono text-sm">exdex.cc</span>
        </div>
      </a>
      
      <a href="https://github.com/sponsors/chuckyLeeVIII" class="hover-scale transform transition-all duration-300">
        <div class="bg-gradient-to-r from-purple-600 to-pink-600 px-6 py-3 rounded-full flex items-center space-x-2">
          <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
            <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path>
          </svg>
          <span class="text-white font-mono text-sm">Sponsor</span>
        </div>
      </a>
      
      <a href="https://buymeacoffee.com/johnsoneriq" class="hover-scale transform transition-all duration-300">
        <div class="bg-gradient-to-r from-yellow-400 to-orange-500 px-6 py-3 rounded-full flex items-center space-x-2">
          <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
            <path d="M3 6a3 3 0 013-3h10a1 1 0 01.8.4l3 4a1 1 0 01.2.6V17a1 1 0 01-1 1H4a1 1 0 01-1-1V6z"></path>
          </svg>
          <span class="text-white font-mono text-sm">Buy Me Coffee</span>
        </div>
      </a>
      
      <div class="bg-gray-900 px-6 py-3 rounded-full border border-cyan-400/30 flex items-center space-x-2">
        <svg class="w-5 h-5 text-cyan-400" fill="currentColor" viewBox="0 0 20 20">
          <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3zM6 8a2 2 0 11-4 0 2 2 0 014 0zM16 18v-3a5.972 5.972 0 00-.75-2.906A3.005 3.005 0 0119 15v3h-3zM4.75 12.094A5.973 5.973 0 004 15v3H1v-3a3 3 0 013.75-2.906z"></path>
        </svg>
        <span class="text-white font-mono text-sm">97th Percentile Python</span>
      </div>
    </div>

    <!-- Featured Work - Alien Tech Showcase -->
    <section class="mb-16">
      <h2 class="text-3xl md:text-4xl font-black orbitron text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-pink-400 text-center mb-12">
        ⚡ ALIEN TECH SHOWCASE
      </h2>
      
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
        <!-- PolyPy - Masterpiece -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-green-400 rounded-full mr-3 pulse"></div>
            <h3 class="text-2xl font-bold text-green-400 orbitron">PolyPy</h3>
          </div>
          <p class="text-gray-300 mb-4">The ultimate Python paradigm shift — universal code generation from structured comments. <span class="text-pink-400">97th percentile Python mastery</span> in action.</p>
          <div class="mb-4">
            <div class="text-sm text-gray-400 mb-2">Python Mastery Level</div>
            <div class="progress-bar">
              <div class="progress-fill"></div>
            </div>
            <div class="text-right text-sm text-green-400 mt-1">97% Expertise</div>
          </div>
          <a href="https://github.com/chuckyLeeVIII/PolyPy--a-master-and-universal-guide-and-proof-of-work-to-polly-py-paradigm" class="inline-block bg-gradient-to-r from-green-600 to-green-700 hover:from-green-500 hover:to-green-600 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            View Quantum Code
          </a>
        </div>

        <!-- Agent_Samantha_Blackwin - Finished -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-cyan-400 rounded-full mr-3"></div>
            <h3 class="text-2xl font-bold text-cyan-400 orbitron">Agent_Samantha</h3>
            <span class="ml-3 bg-green-600 text-white text-xs px-2 py-1 rounded-full font-mono">FINISHED</span>
          </div>
          <p class="text-gray-300 mb-4">Local-first AI/OPSEC system with offline RAG capabilities. The future of private artificial intelligence is here.</p>
          <a href="https://github.com/chuckyLeeVIII/Agent_Samantha_Blackwin" class="inline-block bg-gradient-to-r from-cyan-600 to-cyan-700 hover:from-cyan-500 hover:to-cyan-600 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            Deploy Agent
          </a>
        </div>

        <!-- AirForceOne-100-Trustless -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-pink-400 rounded-full mr-3"></div>
            <h3 class="text-2xl font-bold text-pink-400 orbitron">AirForceOne</h3>
          </div>
          <p class="text-gray-300 mb-4">Trustless bridge/pool/dual-key/arbiter reference implementation. The gold standard for secure cross-chain protocols.</p>
          <a href="https://github.com/chuckyLeeVIII/AirForceOne-100-Trustless" class="inline-block bg-gradient-to-r from-pink-600 to-purple-600 hover:from-pink-500 hover:to-purple-500 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            Secure Protocol
          </a>
        </div>

        <!-- DaBlockV6.0 -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-yellow-400 rounded-full mr-3"></div>
            <h3 class="text-2xl font-bold text-yellow-400 orbitron">DaBlockV6.0</h3>
          </div>
          <p class="text-gray-300 mb-4">Advanced Solidity toolkit with comprehensive tests (Hardhat/Foundry). FamilyCryptoSystem architecture with structured src/ & test/ organization.</p>
          <a href="https://github.com/chuckyLeeVIII/DaBlockV6.0" class="inline-block bg-gradient-to-r from-yellow-600 to-orange-600 hover:from-yellow-500 hover:to-orange-500 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            Solidity Arsenal
          </a>
        </div>

        <!-- AUTO-RBF-BTC-ETH - Satoshi's Unfinished Code -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-orange-400 rounded-full mr-3"></div>
            <h3 class="text-2xl font-bold text-orange-400 orbitron">AUTO-RBF-BTC-ETH</h3>
            <span class="ml-3 bg-orange-600 text-white text-xs px-2 py-1 rounded-full font-mono">SATOSHI'S UNFINISHED</span>
          </div>
          <p class="text-gray-300 mb-4">Reviving and completing Satoshi Nakamoto's vision for automated replace-by-fee protocols across Bitcoin and Ethereum networks.</p>
          <a href="https://github.com/chuckyLeeVIII/AUTO-RBF-BTC-ETH" class="inline-block bg-gradient-to-r from-orange-600 to-red-600 hover:from-orange-500 hover:to-red-500 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            Complete Legacy
          </a>
        </div>

        <!-- ai-hedge-fund -->
        <div class="card-glow bg-gray-900 rounded-2xl p-6 neon-border hover-scale">
          <div class="flex items-center mb-4">
            <div class="w-3 h-3 bg-purple-400 rounded-full mr-3"></div>
            <h3 class="text-2xl font-bold text-purple-400 orbitron">AI Hedge Fund</h3>
          </div>
          <p class="text-gray-300 mb-4">Agentic trading research with CLI/web interfaces. The future of autonomous financial systems powered by advanced AI agents.</p>
          <a href="https://github.com/chuckyLeeVIII/ai-hedge-fund" class="inline-block bg-gradient-to-r from-purple-600 to-indigo-600 hover:from-purple-500 hover:to-indigo-500 text-white px-6 py-2 rounded-full font-mono text-sm transition-all duration-300 transform hover:scale-105">
            Deploy Agents
          </a>
        </div>
      </div>
    </section>

    <!-- Core Principles - Quantum Level -->
    <section class="mb-16">
      <h2 class="text-3xl md:text-4xl font-black orbitron text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-green-400 text-center mb-12">
        🌌 QUANTUM OPERATING PRINCIPLES
      </h2>
      
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="bg-gray-900 p-6 rounded-2xl border border-cyan-400/30 neon-border">
          <div class="flex items-start space-x-3">
            <div class="w-2 h-2 bg-cyan-400 rounded-full mt-2"></div>
            <p class="text-gray-300">Trustless by <span class="text-cyan-400 font-bold">quantum default</span> — remove implicit trust; verify everything at the protocol level</p>
          </div>
        </div>
        
        <div class="bg-gray-900 p-6 rounded-2xl border border-green-400/30 neon-border">
          <div class="flex items-start space-x-3">
            <div class="w-2 h-2 bg-green-400 rounded-full mt-2"></div>
            <p class="text-gray-300">Adversarial design at <span class="text-green-400 font-bold">Planck scale</span> — think like an attacker; ship like a defender with zero trust</p>
          </div>
        </div>
        
        <div class="bg-gray-900 p-6 rounded-2xl border border-pink-400/30 neon-border">
          <div class="flex items-start space-x-3">
            <div class="w-2 h-2 bg-pink-400 rounded-full mt-2"></div>
            <p class="text-gray-300"><span class="text-pink-400 font-bold">Owner sovereignty</span> enforced — user-controlled keys, data, and exits at the quantum level</p>
          </div>
        </div>
        
        <div class="bg-gray-900 p-6 rounded-2xl border border-yellow-400/30 neon-border">
          <div class="flex items-start space-x-3">
            <div class="w-2 h-2 bg-yellow-400 rounded-full mt-2"></div>
            <p class="text-gray-300">Auditability through <span class="text-yellow-400 font-bold">deterministic builds</span> & reproducible deployments — no black boxes</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Tech Stack - Advanced Arsenal -->
    <section class="mb-16">
      <h2 class="text-3xl md:text-4xl font-black orbitron text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-cyan-400 text-center mb-12">
        🛠 ADVANCED TECH ARSENAL
      </h2>
      
      <div class="bg-gray-900 rounded-2xl p-8 neon-border">
        <div class="grid grid-cols-3 md:grid-cols-6 lg:grid-cols-8 gap-6 justify-items-center">
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-green-400 font-mono">Python 97%</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/solidity/FFFFFF" alt="Solidity" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-pink-400 font-mono">Solidity</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/ethereum/3C3C3D" alt="Ethereum" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-purple-400 font-mono">Ethereum</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/bitcoin/F7931A" alt="Bitcoin" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-orange-400 font-mono">Bitcoin</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/react/61DAFB" alt="React" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-cyan-400 font-mono">React</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/typescript/3178C6" alt="TypeScript" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-blue-400 font-mono">TypeScript</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/hardhat/hardhat-original.svg" alt="Hardhat" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-red-400 font-mono">Hardhat</span>
          </div>
          
          <div class="text-center hover-scale transform transition-all duration-300">
            <img src="https://cdn.simpleicons.org/ipfs/65C2CB" alt="IPFS" class="w-12 h-12 mb-2 drop-shadow-lg">
            <span class="text-xs text-green-400 font-mono">IPFS</span>
          </div>
        </div>
        
        <div class="mt-8 text-center">
          <p class="text-gray-400 italic">"The most advanced toolchain for building trustless systems across EVM/BTC/L2 networks"</p>
        </div>
      </div>
    </section>

    <!-- Call to Action -->
    <section class="text-center mb-12">
      <div class="bg-gradient-to-r from-green-900/30 to-purple-900/30 rounded-2xl p-8 border border-green-400/30 neon-border">
        <h2 class="text-2xl md:text-3xl font-black orbitron text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-pink-400 mb-6">
          WORK WITH THE FUTURE
        </h2>
        <p class="text-gray-300 mb-6 max-w-2xl mx-auto">
          Protocol architecture & audits · Agentic/AI contract systems · Custom EVM/BTC/L2 development · OPSEC & zero-trust frameworks. High-impact contracts & strategic consults.
        </p>
        <div class="flex flex-col sm:flex-row justify-center gap-4">
          <a href="https://exdex.cc" class="bg-gradient-to-r from-green-600 to-green-700 hover:from-green-500 hover:to-green-600 text-white px-8 py-3 rounded-full font-bold orbitron transition-all duration-300 transform hover:scale-105 hover:shadow-lg hover:shadow-green-500/25">
            Contact via exdex.cc
          </a>
          <a href="https://github.com/sponsors/chuckyLeeVIII" class="bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-500 hover:to-pink-500 text-white px-8 py-3 rounded-full font-bold orbitron transition-all duration-300 transform hover:scale-105 hover:shadow-lg hover:shadow-purple-500/25">
            Become a Sponsor
          </a>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="text-center text-gray-500 text-sm pt-8 border-t border-gray-800">
      <p>© 2024 chuckyLeeVIII | Alien Tech Architect | <span class="text-green-400">97th Percentile Python Engineer</span></p>
      <p class="mt-2">Building the future of trustless systems, one quantum protocol at a time.</p>
    </footer>
  </div>

  <script>
    // Add typing animation effect
    document.addEventListener('DOMContentLoaded', function() {
      const typingElements = document.querySelectorAll('.typing-animation');
      typingElements.forEach(el => {
        const text = el.textContent;
        el.textContent = '';
        let i = 0;
        const timer = setInterval(() => {
          if (i < text.length) {
            el.textContent += text.charAt(i);
            i++;
          } else {
            clearInterval(timer);
          }
        }, 100);
      });
    });
  </script>
</body>
</html>
