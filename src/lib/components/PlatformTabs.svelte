<script>
    // No script logic needed for this static recreation yet
</script>

<section class="py-20 bg-white font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">Meet the Oars Platform</span>
        <h2 class="mt-8 text-5xl md:text-7xl font-serif-display text-gray-900 leading-tight">Where consumer <br/> brands win visibility <br/> in AI search</h2>
    </div>
    
    <!-- Tabbed interface image area -->
    <div class="max-w-7xl mx-auto mt-16 px-4">
        <div class="border border-gray-200 rounded-xl overflow-hidden shadow-sm bg-white grid md:grid-cols-12 min-h-[600px]">
             <div class="md:col-span-4 p-8 md:p-12 border-r border-gray-200 flex flex-col justify-center">
                 <h3 class="text-3xl font-serif-display mb-4">Know exactly where you stand in AI search</h3>
                 <p class="text-gray-600 text-base leading-relaxed mb-8">Track your brand's visibility across ChatGPT, Perplexity, Google AI Overviews, and other answer engines. See which competitors are winning citations, identify content gaps, and prioritize optimization opportunities that drive real visibility gains.</p>
                 <div>
                    <button class="text-sm font-bold border-b border-gray-300 pb-0.5 hover:border-gray-900 transition-colors">Learn More -></button>
                 </div>
             </div>
             <div class="md:col-span-8 bg-gray-50 p-8 md:p-12 flex items-center justify-center relative overflow-hidden">
                 <!-- Simplified UI Mockup -->
                 <div class="bg-white shadow-xl rounded-lg w-full h-full border border-gray-200 p-6 relative flex flex-col">
                    <div class="flex gap-2 mb-6 border-b border-gray-100 pb-4">
                        <div class="w-3 h-3 rounded-full bg-red-400"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                        <div class="w-3 h-3 rounded-full bg-green-400"></div>
                        <div class="ml-auto flex gap-2">
                            <div class="h-4 w-32 bg-gray-100 rounded-full"></div>
                        </div>
                    </div>
                    
                    <div class="space-y-6">
                        <!-- Header Stats -->
                        <div class="grid grid-cols-4 gap-4">
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Citations</div>
                                 <div class="text-xl font-bold text-gray-900">847</div>
                                 <div class="text-[10px] text-green-600 font-bold">+24%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Visibility</div>
                                 <div class="text-xl font-bold text-gray-900">68%</div>
                                 <div class="text-[10px] text-green-600 font-bold">+15%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Engines</div>
                                 <div class="text-xl font-bold text-gray-900">5</div>
                                 <div class="text-[10px] text-gray-400 font-bold">Active</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Rank Avg</div>
                                 <div class="text-xl font-bold text-gray-900">2.3</div>
                                 <div class="text-[10px] text-green-600 font-bold">↑ 0.8</div>
                             </div>
                        </div>

                        <!-- Data Table -->
                        <div class="border border-gray-100 rounded-lg overflow-hidden">
                            <div class="bg-gray-50 px-4 py-2 border-b border-gray-100 flex text-[10px] font-bold text-gray-500 uppercase tracking-wider">
                                <div class="w-1/3">Query</div>
                                <div class="w-1/6 text-right">Engine</div>
                                <div class="w-1/6 text-right">Rank</div>
                                <div class="w-1/6 text-right">Citations</div>
                                <div class="w-1/6 text-right">Trend</div>
                            </div>
                            <div class="divide-y divide-gray-50 text-xs">
                                 {#each [
                                     {kw: 'best sustainable sneakers', vol: 'ChatGPT', kd: '#2', cpc: '127', status: '↑ 24%'},
                                     {kw: 'eco-friendly clothing brands', vol: 'Perplexity', kd: '#1', cpc: '203', status: '↑ 18%'},
                                     {kw: 'comfortable work shoes', vol: 'Google AI', kd: '#3', cpc: '89', status: '↑ 12%'},
                                     {kw: 'ethical fashion companies', vol: 'ChatGPT', kd: '#4', cpc: '156', status: '↑ 8%'},
                                     {kw: 'sustainable footwear guide', vol: 'Perplexity', kd: '#2', cpc: '94', status: '↑ 15%'}
                                 ] as item}
                                 <div class="px-4 py-3 flex items-center hover:bg-gray-50 transition-colors">
                                     <div class="w-1/3 font-medium text-gray-900">{item.kw}</div>
                                     <div class="w-1/6 text-right text-gray-600 text-[10px]">{item.vol}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="px-1.5 py-0.5 rounded text-[10px] font-bold {item.kd === '#1' ? 'bg-green-100 text-green-700' : item.kd === '#2' ? 'bg-blue-100 text-blue-700' : 'bg-gray-100 text-gray-700'}">{item.kd}</span>
                                     </div>
                                     <div class="w-1/6 text-right text-gray-600">{item.cpc}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="text-[10px] font-bold text-green-600">{item.status}</span>
                                     </div>
                                 </div>
                                 {/each}
                            </div>
                        </div>
                    </div>
                 </div>
             </div>
        </div>
        
        <!-- Bottom Grid of 3 items -->
        <div class="grid md:grid-cols-3 gap-0 mt-0 border-x border-b border-gray-200 divide-x divide-gray-200 bg-white">
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">1</div>
                <p class="text-xs text-gray-600 leading-relaxed">Monitor your brand's visibility across all major AI answer engines in real-time. Track citation frequency, ranking position, and competitor performance.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">2</div>
                <p class="text-xs text-gray-600 leading-relaxed">Identify high-impact optimization opportunities based on semantic analysis and answer engine behavior patterns.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">3</div>
                <p class="text-xs text-gray-600 leading-relaxed">Optimize content positioning with data-driven recommendations that improve your chances of being cited by AI.</p>
            </div>
        </div>
    </div>
</section>