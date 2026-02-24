<h2>About</h2>
<p>
Hi! I'm Akram, and I specialize in the development of bare-metal software where every cycle and byte is manually managed. My work centers on ruling out abstraction by implementing fundamental subsystems, from memory management to network protocols, directly against the hardware. I maintain control over execution determinism and system performance by building monolithic kernels and 3D engines from scratch.
</p>

<h2>Technical Focus</h2>

<ul>
  <li><b>Systems Programming</b>
    <ul>
      <li>Implementation of a 64-bit graphical operating system and drivers for NVMe + Intel HDA hardware via MMIO and DMA</li>
      <li>Development of Slab and Arena allocators for O(1) memory access and minimal heap fragmentation</li>
    </ul>
  </li>

  <li><b>Performance Optimization</b>
    <ul>
      <li>Low-level optimization for x86-64 using SIMD (AVX/SSE) and bitwise operations</li>
      <li>Application of lock-free atomics and cache-line alignment to maximize throughput in concurrent environments</li>
    </ul>
  </li>

  <li><b>Networking &amp; Protocols</b>
    <ul>
      <li>Engineering custom UDP libraries and stacks with zero-copy I/O and polled drivers</li>
      <li>Bypassing kernel overhead for high-frequency packet processing and packet analysis</li>
    </ul>
  </li>

  <li><b>Applied Mathematics</b>
    <ul>
      <li>Implementation of linear algebra and computational geometry within rendering pipelines and spatial partitioning systems</li>
      <li>Application of discrete mathematics and reinforcement learning (Q-Learning) for simulation and fault-burst mitigation</li>
    </ul>
  </li>
</ul>

<h2>Spotlight</h2>

<p>
<b><a href="https://github.com/akramaba/mira">Mira (Custom x86-64 Monolithic OS)</a></b><br>
A 64-bit monolithic kernel written from scratch to handle high-frequency fault bursts. The architecture relies on a custom O(1) Slab Allocator to ensure deterministic memory access patterns, alongside asynchronous NVMe drivers and a polled UDP stack for zero-copy packet processing.
</p>

<p>
<b><a href="https://github.com/akramaba/tori">Tori (Custom 3D Rendering Engine)</a></b><br>
A high-performance rendering engine with 16-byte aligned SIMD mathematics and hardware cache-line locality. It features a custom Linear Algebra library, Octree spatial partitioning for O(log N) search complexity, and a skeletal animation system with matrix hierarchies.
</p>

<p>
<b><a href="https://github.com/akramaba/geo">Geo (Low-Latency Multiplayer 2D Engine)</a></b><br>
A multiplayer engine optimized for unstable networking environments using a custom server-authoritative UDP protocol. The core loop uses C++20 multithreading to decouple network processing from logic, which minimizes frame-time spikes, while entity and scripting logic are handled via Lua coroutines for non-blocking execution.
</p>
