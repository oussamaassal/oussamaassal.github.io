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

  .feature-container {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: space-between;
  gap: 20px;
  margin-bottom: 40px;
  flex-wrap: wrap;
}

.feature-description {
  flex: 1 1 60%;
  min-width: 300px;
}

.feature-preview {
  flex: 1 1 35%;
  min-width: 200px;
}

.feature-preview img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  border: 1px solid #ccc;
}

</style>

<div class="tab-container">
  <button class="tab-button active" onclick="showTab('sprout')">Sprout & Spell</button>
  <button class="tab-button" onclick="showTab('space')">Space Engineer</button>
  <button class="tab-button" onclick="showTab('vr')">VR Climb</button>
  <button class="tab-button" onclick="showTab('arduino')">Arduino Memory Game</button>
  <button class="tab-button" onclick="showTab('sdl')">SDL 2D Game</button>

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
    <img src="/assets/images/git.png" alt="Git" title="Git" width="190" height="190" />
  </div>

  <p>A procedurally generated dungeon crawler with scalable multiplayer systems, intelligent AI, and network-synced environments. Built using Unity and Netcode for GameObjects.</p>
  <p>🔗 <a href="https://gitlab.com/DoomHEADSHOT/sproutfps" target="_blank">View on Gitlab</a></p>

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
    <img src="/assets/images/strapi.png" alt="strapi" title="strapi" width="456" height="110" />
    <img src="/assets/images/git.png" alt="Git" title="Git" width="190" height="190" />
  </div>

  <p>A sci-fi survival game featuring Souls-like combat mechanics, advanced AI behavior, and seamless multiplayer integration — all developed in Unity.</p>
  <p>🔗 <a href="https://gitlab.com/DoomHEADSHOT/spaceengineer" target="_blank">View on Gitlab</a></p>

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
    <img src="/assets/images/git.png" alt="Git" title="Git" width="190" height="190" />

  </div>

  <p>Physics-based VR climbing game using OpenXR. Smash falling obstacles with a hammer, only if you swing it hard enough!</p>
  <p>🔗 <a href="https://gitlab.com/DoomHEADSHOT/vr_climb" target="_blank">View on Gitlab</a></p>

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

<div id="arduino" class="tab-content">
  <h3>🧠 Arduino-Based Memory Game</h3>

  <h4>🛠 Tools Used</h4>
  <div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: center; margin-bottom: 1rem;">
    <img src="/assets/images/arduino.png" alt="Arduino" title="Arduino" width="144" height="88" />
    <img src="/assets/images/Qt.png" alt="Qt" title="Qt" width="174" height="174" />
    <img src="/assets/images/mySQL.png" alt="MySQL" title="MySQL" width="180" height="150" />
    <img src="/assets/images/C++.png" alt="C++" title="C++" width="180" height="180" />
    <img src="/assets/images/C.png" alt="C" title="C" width="180" height="180" />
    <img src="/assets/images/git.png" alt="Git" title="Git" width="190" height="190" />

  </div>

  <p>A mini memory game inspired by the sequence test on HumanBenchmark.com. Built using Arduino and Qt for touchscreen and database interaction.</p>
  <p>🔗 <a href="https://github.com/yourusername/arduino-memory-game" target="_blank">View on GitHub</a></p>

  <h4>🔹 Dynamic Memory Management</h4>
  <p>Allocated and deallocated memory dynamically during each game session to support varying levels of gameplay difficulty.</p>

  <h4>🔹 Scoring System & Database</h4>
  <p>Implemented a scoring system and connected it to a MySQL database via Qt to persist player scores.</p>

  <h4>🔹 LCD Touchscreen Calibration</h4>
  <p>Calibrated an LCD touchscreen to detect input accurately for responsive gameplay experience.</p>

  <video controls width="500" src="/assets/videos/memoryGame.mp4">Your browser does not support the video tag.</video>
</div>

<div id="sdl" class="tab-content">
  <h3>🎮 SDL 1.2 – 2D Platformer Game</h3>

  <h4>🛠 Tools Used</h4>
  <div style="display: flex; flex-wrap: wrap; gap: 12px; align-items: center; margin-bottom: 1rem;">
    <img src="/assets/images/SDL.png" alt="SDL" title="SDL" width="230" height="150" />
    <img src="/assets/images/C.png" alt="C" title="C" width="180" height="180" />
    <img src="/assets/images/git.png" alt="Git" title="Git" width="190" height="190" />
    <img src="/assets/images/gimp.png" alt="Gimp" title="Gimp" width="200" height="190" />
    <img src="/assets/images/audacity.png" alt="Audacity" title="Audacity" width="400" height="100" />
    <img src="/assets/images/photoshop.png" alt="Photoshop" title="Photoshop" width="210" height="210" />
    <img src="/assets/images/ubuntu.png" alt="Ubuntu" title="Ubuntu" width="200" height="190" />
  </div>

  <p>A side-scrolling 2D game built using SDL 1.2. Implemented animations, physics, enemies, and collision detection manually from scratch.</p>
  <p>🔗 <a href="https://github.com/yourusername/sdl2d-platformer" target="_blank">View on GitHub</a></p>

  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Parabolic Jump</h4>
      <p>
        This feature simulates a jump using a quadratic formula, providing a natural arc to the character’s motion.
      </p>
      <pre><code class="language-c">
      void saut_parabolique(personne *pe,background b,SDL_Surface* screen)
      {
          pe->saut_x=pe->saut_x+1;
          SDL_BlitSurface(b.img2, &pe->pos1, b.img, &pe->pos1);
          pe->pos1.y=pe->saut_y-((pe->pente*(pe->saut_x)*(pe->saut_x))+(pe->sommet*pe->saut_x)+pe->max_jump);
          SDL_BlitSurface(pe->tab[pe->num], NULL, b.img, &pe->pos1);
          SDL_Flip(b.img);
      }
      </code></pre>
    </div>
    <div class="feature-preview">
      <img src="/assets/images/parabolic_jump.gif" alt="Jump Preview" />
    </div>
  </div>

  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Quadratic Gravity</h4>
      <p>
        Simulates gravity using a downward parabolic motion for smoother and more realistic fall behavior.
      </p>
      <pre><code class="language-c">
      void gravite_parabolique(personne *pe,background b,SDL_Surface* screen)
      {
          pe->gravite_x=pe->gravite_x+pe->gravite;
          SDL_BlitSurface(b.img2, &pe->pos1, b.img, &pe->pos1);
          pe->pos1.y=pe->gravite_y-((pe->gravite_pente*(pe->gravite_x)*(pe->gravite_x)));
          SDL_BlitSurface(pe->tab[pe->num], NULL, b.img, &pe->pos1);
          SDL_Flip(b.img);
      }
      </code></pre>
    </div>
    <div class="feature-preview">
      <img src="/assets/images/parabolic_gravity.gif" alt="Gravity Preview" />
    </div>
  </div>

  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Animated Obstacle Blocks</h4>
      <p>
        Implements wall-mounted moving blocks that protrude and retract at intervals, challenging the player’s timing and precision.
      </p>
      <pre><code class="language-c">
      void blocks_animation(background* bg,background* p,collision* obstacle,
                            char name[],int x,int y,int w,int h,
                            SDL_Surface* screen,int n,int ms,int diff)
      {
          int now = SDL_GetTicks();
          if (now > p->timer + (ms * p->niveau)) {
              if (p->niveau % (n * 2) == 0) p->pos2.x += p->pos2.w;
              p->pos1.x = x;
              if (p->niveau % (n * 2) != 0)
                  p->pos2.x += (p->mode * p->pos2.w);
              SDL_BlitSurface(bg->img1, &p->pos1, bg->img2, &p->pos1);
              SDL_BlitSurface(p->img, &p->pos2, bg->img2, &p->pos1);
              SDL_BlitSurface(bg->img2, &p->pos1, bg->img, &p->pos1);
              if (p->mode == -1) {
                  p->pos3.x = x + 5;
                  SDL_BlitSurface(p->mask, NULL, bg->mask, &p->pos3);
              } else if (p->mode == 1) {
                  p->pos3.x = x + 5;
                  SDL_BlitSurface(bg->img1, &p->pos3, bg->mask, &p->pos3);
              }
              if (p->niveau % n == 0) {
                  p->pos2.x -= p->pos2.w;
                  p->timer = now - (ms * (p->niveau + 1)) + diff;
                  p->mode *= -1;
              }
              p->niveau++;
          }
      }
      </code></pre>
    </div>
    <div class="feature-preview">
      <img src="/assets/images/block_animation.gif" alt="Block Animation Preview" />
      <img src="/assets/images/block_animation_collision.gif" alt="Block Animation Preview" />
      <img src="/assets/images/block_animation_collision_pillar.gif" alt="Block Animation Preview" />
      <img src="/assets/images/block_animation_collision_ledge.gif" alt="Block Animation Preview" />
    </div>
    
  </div>

    
  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Whack-a-Mole Minigame</h4>
      <p>
        A fun and interactive minigame where players must hit monkeys that pop up randomly from barrels. The game tracks the score based on how many moles are hit within a time limit.
      </p>
      <pre><code class="language-c">
      void monkey_animation(enigme e,monkey* m,SDL_Surface* screen)
      {
          int now=SDL_GetTicks();

                      if(now>m->timer+(50*m->niveau))
                      {
                          m->pos_sprite.x=(m->pos_sprite.x+(m->status*m->pos_sprite.w))%(m->pos_sprite.w*6);
                          m->niveau++;

                          //printf("(niveau=%d x=%d y=%d)",m->niveau*m->status,m->pos_img.x,m->pos_img.y);
                          read_monkey(m);
                          SDL_BlitSurface(e.img1,&m->pos_img,screen,&m->pos_img);
                          SDL_BlitSurface(m->img,&m->pos_sprite,screen,&m->pos_img);    
                          SDL_UpdateRect(screen,m->pos_img.x,m->pos_img.y,m->pos_sprite.w,m->pos_sprite.h);

                          if(m->niveau%6==0 && m->status==1)
                          {
                              m->status=(-1)*m->status;
                          }
                          else if(m->niveau%6==0 && m->status==-1)
                              {
                                  SDL_BlitSurface(e.img1,&m->pos_img,screen,&m->pos_img);
                                  SDL_Flip(screen);
                                  m->status=0;
                                  m->enig_lvl=0;
                              } 
                      }    
      }
  </code></pre>
  </div>
    <div class="feature-preview">
      <img src="/assets/images/Whack-a-monkey.gif" alt="Whack-a-Mole Minigame Preview" />
    </div>
  </div>
  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Split Screen Functionality</h4>
      <p>
        This function splits the screen in half for a multiplayer experience, allowing two characters to be displayed simultaneously on the screen.
      </p>
      <pre><code class="language-c">
      partage_ecran(scrolling *camera1, scrolling *camera2)
      {
          camera1->camera.w = camera1->camera.w / 2;
          camera2->camera.x = 0;
          camera2->camera.w = camera1->camera.w;
          camera2->camera.y = camera1->camera.y;
          camera2->camera.h = camera1->camera.h;
      }
      </code></pre>
    </div>
    <div class="feature-preview">
      <img src="/assets/images/Split_screen.gif" alt="Split Screen Preview" />
    </div>
  </div>

  <div class="feature-container">
    <div class="feature-description">
      <h4>🔹 Collision and Damage Detection</h4>
      <p>
        This function uses a mask background with color detection to determine if the player is colliding with walls or other objects that can cause damage.
      </p>
      <pre><code class="language-c">
      SDL_Color getpixel(background b, SDL_Rect pos)
      {
          SDL_Color color;
          Uint32 col = 0;
          char* pPosition = (char*)b.mask->pixels;
          pPosition += (b.mask->pitch * pos.y);
          pPosition += (b.mask->format->BytesPerPixel * pos.x);
          memcpy(&col, pPosition, b.mask->format->BytesPerPixel);
          SDL_GetRGB(col, b.mask->format, &color.r, &color.g, &color.b);
          return color;
      }
      </code></pre>
    </div>
    <div class="feature-preview">
      <img src="/assets/images/dmg_detection.gif" alt="Collision Detection Preview" />
      <img src="/assets/images/mask.jpg" alt="Background Mask Preview" />
    </div>
  </div>
</div>



<script>
  function showTab(tabId) {
    document.querySelectorAll('.tab-button').forEach(btn => btn.classList.remove('active'));
    document.querySelectorAll('.tab-content').forEach(div => div.classList.remove('active'));
    document.querySelectorAll(`[onclick*="${tabId}"]`).forEach(btn => btn.classList.add('active'));
    document.getElementById(tabId).classList.add('active');
  }
</script>

<!-- Prism CSS for dark theme -->
<link href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/themes/prism-tomorrow.min.css" rel="stylesheet" />

<!-- Prism Core JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js"></script>

<!-- Language Support (e.g., C++, C#, Python) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/components/prism-c.min.js"></script>
