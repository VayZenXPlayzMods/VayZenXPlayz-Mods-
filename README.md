# VayZenXPlayz-Mods-
<!DOCTYPE html>
<html lang="en" class="h-full">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VayZenXPlayz | Core Mod Distribution Network</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        slate: {
                            950: '#0b0f17',
                            900: '#111827',
                            800: '#1f2937',
                            700: '#374151',
                            400: '#9ca3af',
                            300: '#d1d5db'
                        },
                        accent: {
                            cyan: '#06b6d4',
                            cyanHover: '#0891b2',
                            emerald: '#10b981',
                            emeraldHover: '#059669'
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Modernized custom viewport optimization scrollbar */
        ::-webkit-scrollbar { width: 6px; height: 6px; }
        ::-webkit-scrollbar-track { background: #0b0f17; }
        ::-webkit-scrollbar-thumb { background: #374151; border-radius: 9999px; }
        ::-webkit-scrollbar-thumb:hover { background: #06b6d4; }
    </style>
</head>
<body class="h-full bg-slate-950 text-slate-300 antialiased font-sans selection:bg-accent-cyan/30 selection:text-white">

    <div class="min-h-screen flex flex-col justify-between">
        
        <header class="sticky top-0 z-50 backdrop-blur-xl bg-slate-950/75 border-b border-slate-900/80 px-8 py-3 flex justify-between items-center">
            <div class="flex items-center gap-12">
                <div class="flex items-center gap-3 select-none">
                    <div class="w-8 h-8 rounded-lg bg-gradient-to-tr from-accent-cyan to-indigo-500 flex items-center justify-center text-white font-black text-sm shadow-md shadow-accent-cyan/10">V</div>
                    <h1 class="text-base font-bold tracking-tight text-white">
                        VayZenXPlayz <span class="text-accent-cyan font-mono text-xs font-semibold tracking-wider ml-1 px-1.5 py-0.5 rounded bg-accent-cyan/10 border border-accent-cyan/20">NET</span>
                    </h1>
                </div>
                <nav class="hidden lg:flex items-center gap-8 text-xs font-semibold tracking-wide uppercase text-slate-400">
                    <a href="#" class="text-white border-b-2 border-accent-cyan py-4 -mb-4 transition-colors">Directory Node</a>
                    <a href="#" class="hover:text-white transition-colors py-1">Edge Analytics</a>
                    <a href="#" class="hover:text-white transition-colors py-1">Security Ledger</a>
                </nav>
            </div>
            
            <div class="flex items-center gap-4">
                <button class="text-xs font-bold tracking-wide uppercase text-slate-300 hover:text-white transition-colors">
                    Access Portal
                </button>
                <button class="text-xs font-bold tracking-wide uppercase text-white bg-accent-cyan px-4 py-2 rounded-md hover:bg-accent-cyanHover shadow-lg shadow-accent-cyan/10 transition-all flex items-center gap-2">
                    <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 4v16m8-8H4"/></svg>
                    Push Package
                </button>
            </div>
        </header>

        <main class="flex-grow max-w-7xl w-full mx-auto px-8 py-10">
            
            <div class="mb-8 bg-gradient-to-b from-slate-900 to-slate-950 border border-slate-900 rounded-xl p-8 flex flex-col md:flex-row justify-between items-start md:items-center gap-6 shadow-sm">
                <div class="space-y-2">
                    <div class="flex items-center gap-2 text-[10px] font-mono tracking-widest text-accent-cyan font-bold uppercase">
                        <span class="w-2 h-2 rounded-full bg-accent-emerald animate-pulse"></span> Systems Active
                    </div>
                    <h2 class="text-2xl font-bold text-white tracking-tight">Global Mod Registry Node</h2>
                    <p class="text-xs text-slate-400 max-w-xl leading-relaxed">Cryptographically signed package distributions optimized for instantaneous execution across container layers. Query, deploy, and inspect modules below.</p>
                </div>
                <div class="grid grid-cols-2 gap-4 w-full md:w-auto">
                    <div class="bg-slate-900/50 border border-slate-900 rounded-lg px-4 py-3 min-w-[140px]">
                        <span class="text-[10px] text-slate-400 font-mono tracking-wider uppercase block">Network Bandwidth</span>
                        <span class="text-sm font-bold text-white block mt-1">41.8 Gbps</span>
                    </div>
                    <div class="bg-slate-900/50 border border-slate-900 rounded-lg px-4 py-3 min-w-[140px]">
                        <span class="text-[10px] text-slate-400 font-mono tracking-wider uppercase block">Cache Delivery</span>
                        <span class="text-sm font-bold text-accent-cyan block mt-1">99.4% HIT</span>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row gap-4 justify-between items-start md:items-center mb-8 pb-4 border-b border-slate-900">
                <div class="flex items-center gap-1.5 bg-slate-900/60 p-1 rounded-md border border-slate-900 text-xs font-bold">
                    <button id="btn-all" onclick="filterCategory('all')" class="bg-slate-800 text-white px-3 py-1 rounded shadow-sm transition-all">All Objects</button>
                    <button id="btn-vehicle" onclick="filterCategory('vehicle')" class="text-slate-400 hover:text-white px-3 py-1 rounded transition-all">Vehicles</button>
                    <button id="btn-environment" onclick="filterCategory('environment')" class="text-slate-400 hover:text-white px-3 py-1 rounded transition-all">Environments</button>
                </div>
                
                <div class="relative w-full md:w-72">
                    <span class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none text-slate-400">
                        <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
                    </span>
                    <input 
                        type="text" 
                        id="search-input"
                        onkeyup="searchGrid()"
                        placeholder="Filter index strings..." 
                        class="w-full bg-slate-900 border border-slate-900 rounded-md pl-9 pr-4 py-1.5 text-xs text-white placeholder-slate-400 focus:outline-none focus:border-accent-cyan focus:ring-1 focus:ring-accent-cyan transition-all"
                    />
                </div>
            </div>

            <div id="mod-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                
                <div data-category="vehicle" class="mod-card group bg-slate-900/40 border border-slate-900 rounded-xl overflow-hidden hover:border-slate-800 transition-all duration-200 flex flex-col justify-between">
                    <div class="p-6 space-y-4">
                        <div class="flex justify-between items-center">
                            <span class="text-[9px] font-mono uppercase tracking-widest text-accent-cyan font-bold bg-accent-cyan/10 px-2 py-0.5 rounded border border-accent-cyan/10">Vehicle Core</span>
                            <span class="text-[10px] font-mono text-slate-400 bg-slate-900 px-1.5 py-0.5 rounded border border-slate-800">v2.4.1</span>
                        </div>
                        <div class="space-y-1">
                            <h3 class="mod-title font-bold text-white text-base group-hover:text-accent-cyan transition-colors truncate">Scania S730 Heavy Hauler Engine</h3>
                            <p class="text-[11px] text-slate-400">Maintained by: <span class="text-slate-300">SimWorks Studio</span></p>
                        </div>
                        <p class="text-xs text-slate-400 leading-relaxed line-clamp-3">High-fidelity binary payload containing optimized damper structures, accurate transmission ratios, and uncompressed texture maps.</p>
                    </div>
                    <div class="px-6 pb-6 pt-4 border-t border-slate-900 bg-slate-900/20 flex items-center justify-between">
                        <div class="flex gap-4 text-[11px] font-mono text-slate-400">
                            <span>📥 48.2K</span>
                            <span>⭐ 4.9</span>
                        </div>
                        <button class="text-[10px] font-bold tracking-wider uppercase text-white bg-accent-emerald px-3 py-1.5 rounded hover:bg-accent-emeraldHover transition-colors">Fetch Node</button>
                    </div>
                </div>

                <div data-category="environment" class="mod-card group bg-slate-900/40 border border-slate-900 rounded-xl overflow-hidden hover:border-slate-800 transition-all duration-200 flex flex-col justify-between">
                    <div class="p-6 space-y-4">
                        <div class="flex justify-between items-center">
                            <span class="text-[9px] font-mono uppercase tracking-widest text-indigo-400 font-bold bg-indigo-500/10 px-2 py-0.5 rounded border border-indigo-500/10">Environment Matrix</span>
                            <span class="text-[10px] font-mono text-slate-400 bg-slate-900 px-1.5 py-0.5 rounded border border-slate-800">v1.0.0</span>
                        </div>
                        <div class="space-y-1">
                            <h3 class="mod-title font-bold text-white text-base group-hover:text-accent-cyan transition-colors truncate">Alpine Ridge Mud Array Generation</h3>
                            <p class="text-[11px] text-slate-400">Maintained by: <span class="text-slate-300">TerrainMaster</span></p>
                        </div>
                        <p class="text-xs text-slate-400 leading-relaxed line-clamp-3">Dynamic topography layers executing custom multi-threaded physics generation loops for progressive surface deformations.</p>
                    </div>
                    <div class="px-6 pb-6 pt-4 border-t border-slate-900 bg-slate-900/20 flex items-center justify-between">
                        <div class="flex gap-4 text-[11px] font-mono text-slate-400">
                            <span>📥 12.9K</span>
                            <span>⭐ 4.7</span>
                        </div>
                        <button class="text-[10px] font-bold tracking-wider uppercase text-white bg-accent-emerald px-3 py-1.5 rounded hover:bg-accent-emeraldHover transition-colors">Fetch Node</button>
                    </div>
                </div>

            </div>
        </main>

        <footer class="border-t border-slate-900 bg-slate-950 px-8 py-6 flex flex-col md:flex-row justify-between items-center gap-4 max-w-7xl w-full mx-auto text-[11px] text-slate-400 font-mono">
            <p>&copy; 2026 VayZenXPlayz Network Assets. Encryption enabled.</p>
            <div class="flex gap-6">
                <a href="#" class="hover:text-white transition-colors">API Endpoint Specs</a>
                <a href="#" class="hover:text-white transition-colors">Node Telemetry</a>
            </div>
        </footer>

    </div>

    <script>
        let activeCategory = 'all';

        function filterCategory(category) {
            activeCategory = category;
            
            // Manage UI Button State Highlights
            const buttons = ['all', 'vehicle', 'environment'];
            buttons.forEach(btn => {
                const el = document.getElementById(`btn-${btn}`);
                if (btn === category) {
                    el.className = "bg-slate-800 text-white px-3 py-1 rounded shadow-sm transition-all";
                } else {
                    el.className = "text-slate-400 hover:text-white px-3 py-1 rounded transition-all";
                }
            });

            executeFilters();
        }

        function searchGrid() {
            executeFilters();
        }

        function executeFilters() {
            const query = document.getElementById('search-input').value.toLowerCase();
            const cards = document.getElementsByClassName('mod-card');

            for (let card of cards) {
                const cardCategory = card.getAttribute('data-category');
                const title = card.querySelector('.mod-title').textContent.toLowerCase();

                const matchesCategory = (activeCategory === 'all' || cardCategory === activeCategory);
                const matchesQuery = title.includes(query);

                if (matchesCategory && matchesQuery) {
                    card.style.display = "flex";
                } else {
                    card.style.display = "none";
                }
            }
        }
    </script>
</body>
</html>
