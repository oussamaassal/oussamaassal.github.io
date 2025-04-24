## 🚀 Projects

<style>
  .tab-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 10px;
  }

  .tab-button {
    padding: 8px 16px;
    border: 1px solid #444;
    background-color: #1e1e1e;
    color: #ccc;
    cursor: pointer;
    border-radius: 4px;
    transition: background-color 0.2s ease, color 0.2s ease;
  }

  .tab-button:hover {
    background-color: #333;
    color: #fff;
  }

  .tab-button.active {
    background-color: #4caf50; /* muted green */
    color: #fff;
    border-color: #4caf50;
  }

  .tab-content {
    display: none;
    margin-top: 1rem;
  }

  .tab-content.active {
    display: block;
  }
</style>

<div class="tab-container">
  <button class="tab-button active" onclick="showTab('sprout')">Sprout & Spell</button>
  <button class="tab-button" onclick="showTab('space')">Space Engineer</button>
  <button class="tab-button" onclick="showTab('vr')">VR Climb</button>
</div>

<div id="sprout" class="tab-content">
  <h3>🧙 Sprout & Spell</h3>

  <h4>🛠 Tools Used</h4>
  <div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: center; margin-bottom: 1rem;">
    <img src="/assets/images/Unity6.png" alt="Unity6" title="Unity6" width="180" height="100" />
    <img src="/assets/images/csharp.png" alt="C#" title="C#" width="100" height="100" />
    <img src="/assets/images/netcode.png" alt="Netcode for GameObjects" title="Netcode for GameObjects" width="300" height="100" />
    <img src="/assets/images/Maya.png" alt="Maya" title="Maya" width="100" height="100" />
    <img src="/assets/images/audacity.png" alt="Audacity" title="Audacity" width="400" height="100" />
    <img src="/assets/images/krita.png" alt="krita" title="krita" width="290" height="100" />
  </div>

  <p>A procedurally generated dungeon crawler with scalable multiplayer systems, intelligent AI, and network-synced environments. Built using Unity and Netcode for GameObjects.</p>
  <p>🔗 <a href="https://github.com/yourusername/sprout-spell" target="_blank">View on GitHub</a></p>

  <h4>🔹 Procedural Room Generation</h4>
  <p>Rooms are generated with just the X and Z axis using <code>Graphics.DrawMeshInstanced</code>. A decorations grid system populates each room with assets that feel naturally placed without looking random.</p>
  <img src="/assets/images/roomGenerator.gif" alt="Procedural Room Generation" width="1000" />

  <h4>🔹 Procedural Dungeon Generation</h4>
  <p>Five-step dungeon generation process:</p>
  <ol>
    <li>🧱 Random room placement with optional buffer to prevent overlap.</li>
    <img src="/assets/images/dungeon1.png" alt="Procedural Dungeon Generation" width="500" />
    <li>📐 Delaunay triangulation using Bowyer-Watson algorithm.</li>
    <img src="/assets/images/dungeon2.png" alt="Procedural Dungeon Generation" width="500" />
    <li>🌲 Minimum Spanning Tree (MST) with Prim’s algorithm for guaranteed connectivity.</li>
    <img src="/assets/images/dungeon3.png" alt="Procedural Dungeon Generation" width="500" />
    <li>🔄 Optional cycle creation with 12.5% extra edge inclusion.</li>
    <img src="/assets/images/dungeon4.png" alt="Procedural Dungeon Generation" width="500" />
    <li>🧭 A* pathfinding for hallway creation that adapts to terrain and layout.</li>
    <img src="/assets/images/dungeon5.gif" alt="Procedural Dungeon Generation" width="500" />
  </ol>

  <h4>🔹 Advanced AI Behavior</h4>
  <p>Expanded on <em>Space Engineer</em>'s AI system. Enemies now locate and pick up items around the map, adding them to their loot tables. They can also interact with world objects like doors and switches.</p>


  <h4>🔹 Multiplayer Networking</h4>
  <p>Built with <strong>Netcode for GameObjects</strong>:</p>
  <ul>
    <li>🌍 Synced procedural dungeon generation via seed sharing.</li>
    <li>🎭 Synced player and enemy animations.</li>
    <li>🧑‍🤝‍🧑 Fully multiplayer-ready AI interactions and combat systems.</li>
  </ul>
</div>

<div id="space" class="tab-content">
  <h3>🚀 Space Engineer</h3>

  <h4>🛠 Tools Used</h4>
  <div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: center; margin-bottom: 1rem;">
    <img src="/assets/images/Unity.png" alt="Unity" title="Unity" width="150" height="150" />
    <img src="/assets/images/csharp.png" alt="C#" title="C#" width="100" height="100" />
    <img src="/assets/images/Mirror.jpg" alt="Mirror" title="Mirror" width="180" height="120" />
    <img src="/assets/images/Maya.png" alt="Maya" title="Maya" width="100" height="100" />
    <img src="/assets/images/audacity.png" alt="Audacity" title="Audacity" width="400" height="100" />
    <img src="/assets/images/krita.png" alt="krita" title="krita" width="290" height="100" />
  </div>

  <p>A sci-fi survival game featuring Souls-like combat mechanics, advanced AI behavior, and seamless multiplayer integration — all developed in Unity.</p>
  <p>🔗 <a href="https://github.com/yourusername/space-engineer" target="_blank">View on GitHub</a></p>

  <h4>🔹 Player Movement & Combat</h4>
  <p>Implemented a Souls-like system with rolling, dodging, jumping, light/heavy attacks, and fluid combo transitions.</p>

  <h4>🔹 Advanced Animation System</h4>
  <p>Randomized animations, directional hit reactions, upper/lower body blending, and left/right hand-specific attacks.</p>

  <h4>🔹 RPG Stat Scaling</h4>
  <p>Integrated stamina, health, and damage scaling systems based on player stats.</p>

  <h4>🔹 Immersive Effects</h4>
  <p>Used hit angle-based VFX and randomized sound effects for more dynamic and visceral feedback during combat.</p>

  <h4>🔹 Interactions & Items</h4>
  <p>Players can interact with world objects and pickups for resources, weapons, or mission objectives.</p>

  <h4>🔹 Ranged & Melee Weapons</h4>
  <p>Laser guns, hammers, wrenches, and unarmed combat are all supported with unique attack styles.</p>

  <h4>🔹 AI State Machine</h4>
  <p>Custom AI system with Idle, Pursue, Combat Stance, and Attack states, including navigation and target prioritization.</p>

  <h4>🔹 Multiplayer Support</h4>
  <p>Used Mirror for fully networked combat, co-op, and exploration. Players can host sessions, join via code, or browse open lobbies.</p>

  <h4>🔹 Backend & Auth System</h4>
  <p>Connected Unity to Strapi backend. Players can sign up or log in with Discord, Patreon, Twitch, or email via OAuth and UnityWebView.</p>

  <h4>🔹 Save System</h4>
  <p>Created a JSON-based game save and load system to persist progress between sessions.</p>
</div>

<div id="vr" class="tab-content">
  <h3>🧗 VR Climber</h3>

  <h4>🛠 Tools Used</h4>
  <div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: center; margin-bottom: 1rem;">
    <img src="/assets/images/Unity6.png" alt="Unity6" title="Unity6" width="180" height="100" />
    <img src="/assets/images/csharp.png" alt="C#" title="C#" width="100" height="100" />
    <img src="/assets/images/openXR.png" alt="OpenXR" title="OpenXR" width="190" height="100" />
    <img src="/assets/images/Maya.png" alt="Maya" title="Maya" width="100" height="100" />
    <img src="/assets/images/audacity.png" alt="Audacity" title="Audacity" width="400" height="100" />
    <img src="/assets/images/krita.png" alt="krita" title="krita" width="290" height="100" />
  </div>

  <p>Physics-based VR climbing game using OpenXR. Smash falling obstacles with a hammer, only if you swing it hard enough!</p>
  <p>🔗 <a href="https://github.com/yourusername/vr-climber" target="_blank">View on GitHub</a></p>

  <h4>🔹 Climbing Mechanic</h4>
  <p>Grab specific objects using VR controllers and pull yourself up to climb realistically.</p>

  <h4>🔹 Hand Animations</h4>
  <p>Implemented animated VR hands that react to grip and movement.</p>

  <h4>🔹 Physics-Based Weapons</h4>
  <p>Created tools that break falling objects—only when swung fast enough to trigger impact-based destruction.</p>

  <h4>🔹 Jumping Mechanic</h4>
  <p>Players can jump by pushing themselves off while climbing, allowing for tight-space maneuvers and parkour-style movement.</p>

  <h4>🔹 Environment Setup</h4>
  <p>Designed and optimized the 3D environment layout for immersive VR exploration.</p>
</div>

<script>
  function showTab(tabId) {
    document.querySelectorAll('.tab-button').forEach(btn => btn.classList.remove('active'));
    document.querySelectorAll('.tab-content').forEach(div => div.classList.remove('active'));
    document.querySelectorAll(`[onclick*="${tabId}"]`).forEach(btn => btn.classList.add('active'));
    document.getElementById(tabId).classList.add('active');
  }
</script>
