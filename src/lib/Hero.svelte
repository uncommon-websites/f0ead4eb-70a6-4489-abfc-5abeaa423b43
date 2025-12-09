<script lang="ts">
	import { ArrowRight, ChevronDown, Search, Bell, CheckSquare, Mail, BarChart2, Zap, Layout, Users, Briefcase, Building2, Plus, MoreHorizontal, Filter, RefreshCw, Download } from 'lucide-svelte';
</script>

<section class="pt-40 pb-20 px-6 text-center max-w-[1400px] mx-auto">
	<a href="#" class="inline-flex items-center gap-2 text-xs font-medium text-gray-500 hover:text-black mb-8 border border-gray-200 rounded-full px-3 py-1 bg-white hover:border-gray-300 transition-colors">
		Backed by Blackstone, Google, Palantir & OpenAI talent
		<ArrowRight size={12} />
	</a>

	<h1 class="text-[56px] leading-[1.1] font-serif tracking-tight text-gray-900 mb-6 max-w-4xl mx-auto">
		Development workflows.<br/>90% faster.
	</h1>

	<p class="text-lg text-gray-500 mb-10 max-w-xl mx-auto text-balance">
		Build automates real estate development workflows through agentic AI verified by industry experts.
	</p>

	<div class="flex items-center justify-center gap-4 mb-20">
		<a href="#" class="bg-black text-white text-sm font-medium px-5 py-2.5 rounded-lg hover:bg-gray-800 transition-colors">
			Get started
		</a>
		<a href="#" class="text-sm font-medium text-gray-600 hover:text-black border border-gray-200 px-5 py-2.5 rounded-lg hover:border-gray-300 transition-colors">
			Book a demo
		</a>
	</div>

	<!-- Dashboard Preview -->
	<div class="relative rounded-xl overflow-hidden shadow-2xl border border-gray-200 bg-white text-left mx-auto max-w-[1200px]">
		<!-- Tabs -->
		<div class="flex border-b border-gray-200 bg-gray-50/50">
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Site Selection</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Permitting</button>
			<button class="px-8 py-3 text-xs font-medium text-black border-b-2 border-black bg-white">Analytics</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Portfolio</button>
		</div>

		<!-- UI Container -->
		<div class="flex h-[600px] bg-white">
			<!-- Sidebar -->
			<div class="w-[240px] border-r border-gray-200 flex flex-col text-[13px] text-gray-600">
				<div class="p-3 flex items-center gap-2 font-medium text-black border-b border-gray-100">
					<div class="w-5 h-5 bg-black rounded flex items-center justify-center text-white text-[10px]">
						<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-3 h-3">
							<path fill-rule="evenodd" clip-rule="evenodd" d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386Z" fill="white"/>
						</svg>
					</div>
					Build Platform
					<ChevronDown size={14} class="ml-auto opacity-50" />
				</div>
				
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Search size={14} /> Quick search
						<div class="ml-auto text-[10px] border border-gray-200 rounded px-1">⌘K</div>
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Bell size={14} /> Notifications
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<CheckSquare size={14} /> Tasks
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Mail size={14} /> Dougie
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 bg-gray-100 text-black font-medium rounded cursor-pointer">
						<BarChart2 size={14} /> Analytics
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Zap size={14} /> Workflows
					</div>
				</div>

				<div class="mt-2 px-4 text-[11px] font-medium text-gray-400">Asset Classes</div>
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Building2 size={14} class="text-blue-500" /> Data Centers
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Users size={14} class="text-green-500" /> Industrial
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Briefcase size={14} class="text-orange-500" /> Multifamily
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Layout size={14} class="text-purple-500" /> Office
					</div>
				</div>
			</div>

			<!-- Main Content -->
			<div class="flex-1 flex flex-col bg-gray-50/30">
				<!-- Header -->
				<div class="h-14 border-b border-gray-200 flex items-center justify-between px-6 bg-white">
					<div class="flex items-center gap-2 text-sm text-gray-500">
						<BarChart2 size={16} />
						<span>Analytics</span>
						<span class="text-gray-300">/</span>
						<span class="text-black font-medium">Portfolio Performance</span>
					</div>
					<div class="flex items-center gap-3">
						<div class="flex -space-x-2">
							<div class="w-6 h-6 rounded-full bg-blue-100 border-2 border-white flex items-center justify-center text-[10px]">DC</div>
							<div class="w-6 h-6 rounded-full bg-green-100 border-2 border-white flex items-center justify-center text-[10px]">JS</div>
						</div>
						<button class="text-xs font-medium text-gray-600 hover:text-black flex items-center gap-1">
							Export
						</button>
					</div>
				</div>

				<!-- Dashboard Content -->
				<div class="p-6 overflow-hidden">
					<div class="mb-6 flex items-center justify-between">
						<div>
							<h2 class="text-lg font-semibold text-gray-900">Portfolio Performance</h2>
							<p class="text-sm text-gray-500">Real-time tracking of development pipeline, deal velocity, and market opportunities.</p>
						</div>
						<div class="flex items-center gap-2">
							<button class="text-xs font-medium text-gray-500 hover:text-black flex items-center gap-1 px-2 py-1">
								<RefreshCw size={12} /> Sync data
							</button>
							<button class="bg-black text-white text-xs font-medium px-3 py-1.5 rounded-md hover:bg-gray-800 flex items-center gap-1">
								<Plus size={12} /> New dashboard
							</button>
						</div>
					</div>

					<div class="grid grid-cols-5 gap-6 h-full">
						<!-- Chart 1: Revenue growth -->
						<div class="col-span-3 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Deal velocity by asset class</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex items-center gap-4 text-[10px] text-gray-500 mb-4">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-200"></div> Q2 2024</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-300"></div> Q3 2024</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-400"></div> Data Centers</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-500"></div> Industrial</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-600"></div> Multifamily</div>
							</div>
							
							<!-- Mock Bar Chart -->
							<div class="relative h-[250px] w-full mt-8">
								<!-- Y Axis Labels -->
								<div class="absolute left-0 top-0 bottom-0 w-8 flex flex-col justify-between text-[10px] text-gray-400 text-right pr-2">
									<span>$ 2.8M</span>
									<span>$ 2.4M</span>
									<span>$ 2.0M</span>
									<span>$ 1.6M</span>
									<span>$ 1.2M</span>
									<span>$ 0.8M</span>
									<span>$ 0.4M</span>
								</div>
								<!-- Bars -->
								<div class="ml-10 h-full flex items-end justify-between px-4 border-l border-b border-gray-100">
									<!-- July -->
									<div class="w-8 flex flex-col gap-0.5 items-center group relative">
										<div class="w-full bg-purple-100 h-8 rounded-t-sm"></div>
										<div class="w-full bg-purple-200 h-12"></div>
										<div class="w-full bg-purple-300 h-16"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">July</div>
									</div>
									<!-- August -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full bg-purple-200 h-10 rounded-t-sm"></div>
										<div class="w-full bg-purple-300 h-16"></div>
										<div class="w-full bg-purple-400 h-24"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">August</div>
										
										<!-- Tooltip Mock -->
										<div class="absolute bottom-full mb-2 left-1/2 -translate-x-1/2 bg-gray-900 text-white text-[10px] px-2 py-1 rounded whitespace-nowrap z-10">
											ARR Contribution <span class="text-green-400 ml-1">+45%</span>
										</div>
										<div class="absolute bottom-full mb-1 left-1/2 -translate-x-1/2 w-0 h-0 border-l-[4px] border-l-transparent border-r-[4px] border-r-transparent border-t-[4px] border-t-gray-900"></div>
									</div>
									<!-- September -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full bg-purple-300 h-14 rounded-t-sm"></div>
										<div class="w-full bg-purple-400 h-20"></div>
										<div class="w-full bg-purple-500 h-32"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">September</div>
									</div>
								</div>
							</div>
						</div>

						<!-- Chart 2: Donut -->
						<div class="col-span-2 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Active projects by stage</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex flex-wrap gap-2 text-[10px] text-gray-500 mb-8">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-pink-500"></div> Site Selection</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-blue-500"></div> Permitting</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-500"></div> Acquisitions</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-orange-400"></div> Design</div>
								<div class="flex items-center gap-1 text-gray-400">+4 more</div>
							</div>

							<!-- Mock Donut Chart -->
							<div class="relative w-48 h-48 mx-auto">
								<svg viewBox="0 0 100 100" class="w-full h-full transform -rotate-90">
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#fce7f3" stroke-width="16" /> <!-- Base -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#ec4899" stroke-width="16" stroke-dasharray="60 251" stroke-dashoffset="0" /> <!-- Pink segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#3b82f6" stroke-width="16" stroke-dasharray="80 251" stroke-dashoffset="-60" /> <!-- Blue segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#a855f7" stroke-width="16" stroke-dasharray="40 251" stroke-dashoffset="-140" /> <!-- Purple segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#fb923c" stroke-width="16" stroke-dasharray="30 251" stroke-dashoffset="-180" /> <!-- Orange segment -->
								</svg>
								<div class="absolute inset-0 flex items-center justify-center flex-col">
									<span class="text-2xl font-bold text-gray-900">Projects</span>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- Logos -->
	<div class="mt-20 flex flex-wrap justify-center items-center gap-12 opacity-60">
		<div class="text-sm font-medium text-gray-500">Trusted by leading institutions</div>
		<div class="flex items-center gap-1 font-bold text-lg">
			<div class="w-8 h-8 bg-black text-white flex items-center justify-center text-xs font-bold">B</div>
			<span>Blackstone</span>
		</div>
		<div class="font-bold text-xl tracking-tight">Heatherwick</div>
		<div class="flex items-center gap-1 font-bold text-lg">
			<div class="w-6 h-6 rounded-full bg-gradient-to-br from-blue-500 to-purple-600"></div>
			<span>Google</span>
		</div>
		<div class="font-bold text-xl tracking-wider">PALANTIR</div>
		<div class="flex items-center gap-1 font-bold text-lg">
			<div class="w-6 h-6 bg-black rounded-full flex items-center justify-center text-white text-[10px]">AI</div>
			<span>OpenAI</span>
		</div>
	</div>
</section>
