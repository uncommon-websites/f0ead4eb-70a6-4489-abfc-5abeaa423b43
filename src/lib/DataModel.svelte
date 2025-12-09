<script lang="ts">
	import { User, Briefcase, Building2, Plus, MoreHorizontal } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20">
	<div class="text-center max-w-3xl mx-auto mb-20">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Complete lifecycle coverage. <span class="text-gray-500 font-sans text-xl font-normal block mt-4">Build covers every stage of development across all major asset classes. From site selection to exit, we automate the workflows that matter.</span>
		</h2>
		<button class="mt-8 px-4 py-2 bg-white border border-gray-200 rounded-full text-sm font-medium hover:border-gray-300 transition-colors">
			Explore workflows
		</button>
	</div>

	<!-- Data Model Visual -->
	<div class="relative bg-gray-50/50 rounded-xl p-10 md:p-20 border border-gray-100 overflow-hidden">
		<!-- Background Grid -->
		<div class="absolute inset-0" style="background-image: radial-gradient(#e5e7eb 1px, transparent 1px); background-size: 20px 20px; opacity: 0.5;"></div>

		<!-- Top Filters -->
		<div class="flex justify-center gap-2 mb-16 relative z-10">
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Data Centers</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Industrial</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Multifamily</button>
			<button class="px-3 py-1 bg-white border border-gray-200 rounded-full text-xs font-medium shadow-sm">Office</button>
		</div>

		<!-- Objects Diagram -->
		<div class="relative max-w-4xl mx-auto h-[500px]">
			<!-- Connecting Lines (SVG) -->
			<svg class="absolute inset-0 w-full h-full pointer-events-none z-0">
				<!-- User to Person -->
				<path d="M 200 150 C 200 200, 250 250, 300 300" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
				<!-- Person to Deal -->
				<path d="M 450 300 C 500 250, 550 200, 600 150" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
				<!-- Person to Add Object -->
				<path d="M 450 350 C 500 350, 550 350, 600 350" fill="none" stroke="#e5e7eb" stroke-width="2" stroke-dasharray="4 4" />
			</svg>

			<!-- Site Selection Object -->
			<div class="absolute top-10 left-10 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded bg-green-100 flex items-center justify-center text-green-600">
							<User size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Site Selection</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Workflow</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">#</div>
						<span>Site ID</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">@</div>
						<span>Buy-box score</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">Aa</div>
						<span>Zoning status</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 8 More Attributes</div>
				</div>
			</div>

			<!-- Permitting Object -->
			<div class="absolute top-10 right-10 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded bg-purple-100 flex items-center justify-center text-purple-600">
							<Briefcase size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Permitting</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Workflow</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">Aa</div>
						<span>Permit type</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">□</div>
						<span>Jurisdiction</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">≡</div>
						<span>Status</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 6 More Attributes</div>
				</div>
			</div>

			<!-- Acquisitions Object (Center) -->
			<div class="absolute top-60 left-1/2 -translate-x-full -ml-4 w-64 bg-white rounded-lg border border-gray-200 shadow-sm z-10">
				<div class="p-3 border-b border-gray-100 flex items-center justify-between bg-gray-50/50 rounded-t-lg">
					<div class="flex items-center gap-2">
						<div class="w-6 h-6 rounded bg-blue-100 flex items-center justify-center text-blue-600">
							<User size={14} />
						</div>
						<span class="text-sm font-semibold text-gray-900">Acquisitions</span>
					</div>
					<span class="text-[10px] text-gray-400 bg-gray-100 px-1.5 py-0.5 rounded">Workflow</span>
				</div>
				<div class="p-3 space-y-2">
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">Aa</div>
						<span>Property name</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">@</div>
						<span>Valuation</span>
					</div>
					<div class="flex items-center gap-2 text-xs text-gray-600">
						<div class="w-4 h-4 flex items-center justify-center text-gray-400">🏢</div>
						<span>Asset class</span>
					</div>
					<div class="text-[10px] text-gray-400 pl-6">+ 10 More Attributes</div>
				</div>
			</div>

			<!-- Add Workflow (Placeholder) -->
			<div class="absolute top-60 left-1/2 ml-4 w-64 h-40 border-2 border-dashed border-gray-300 rounded-lg flex items-center justify-center bg-gray-50/30 z-10">
				<div class="flex items-center gap-2 text-gray-500 font-medium text-sm">
					<Plus size={16} /> Add workflow
				</div>
			</div>
		</div>

		<!-- Table View at Bottom -->
		<div class="mt-10 bg-white border border-gray-200 rounded-lg shadow-sm overflow-hidden max-w-4xl mx-auto">
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-100 bg-gray-50 text-[11px] font-medium text-gray-500">
				<div class="flex items-center gap-2"><User size={12} /> Site</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">#</div> Site ID</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">Aa</div> Asset class</div>
				<div class="flex items-center gap-2"><div class="w-3 h-3 flex items-center justify-center">@</div> Stage</div>
			</div>
			<!-- Row 1 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-900 flex items-center justify-center text-white text-[8px]">DC</div> Dallas TX Site</div>
				<div class="font-mono text-gray-500 text-[10px]">DC-2024-TX-001</div>
				<div><span class="bg-blue-100 text-blue-700 px-1.5 py-0.5 rounded text-[10px]">Data Center</span></div>
				<div><span class="text-green-600">Permitting</span></div>
			</div>
			<!-- Row 2 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-900 flex items-center justify-center text-white text-[8px]">IN</div> Newark NJ Warehouse</div>
				<div class="font-mono text-gray-500 text-[10px]">IN-2024-NJ-012</div>
				<div><span class="bg-purple-100 text-purple-700 px-1.5 py-0.5 rounded text-[10px]">Industrial</span></div>
				<div><span class="text-blue-600">Site Selection</span></div>
			</div>
			<!-- Row 3 -->
			<div class="grid grid-cols-4 gap-4 p-3 border-b border-gray-50 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-900 flex items-center justify-center text-white text-[8px]">MF</div> San Jose CA Complex</div>
				<div class="font-mono text-gray-500 text-[10px]">MF-2024-CA-008</div>
				<div><span class="bg-orange-100 text-orange-700 px-1.5 py-0.5 rounded text-[10px]">Multifamily</span></div>
				<div><span class="text-purple-600">Acquisitions</span></div>
			</div>
			<!-- Row 4 -->
			<div class="grid grid-cols-4 gap-4 p-3 text-xs hover:bg-gray-50">
				<div class="flex items-center gap-2"><div class="w-5 h-5 rounded bg-gray-900 flex items-center justify-center text-white text-[8px]">OF</div> Manhattan NYC Tower</div>
				<div class="font-mono text-gray-500 text-[10px]">OF-2024-NY-003</div>
				<div><span class="bg-green-100 text-green-700 px-1.5 py-0.5 rounded text-[10px]">Office</span></div>
				<div><span class="text-gray-600">Design</span></div>
			</div>
		</div>
	</div>
</section>
