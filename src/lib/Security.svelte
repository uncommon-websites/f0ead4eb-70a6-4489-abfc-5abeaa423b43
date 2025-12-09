<script lang="ts">
	import { ShieldCheck, Lock, FileCheck } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20 border-t border-gray-100">
	<div class="flex flex-col md:flex-row items-center justify-between gap-12">
		<div class="max-w-xl">
			<h2 class="text-3xl font-serif text-gray-900 mb-4">
				Enterprise-grade security. <span class="text-gray-500 font-sans text-lg font-normal">Build is SOC 2 Type II compliant with customer data segmentation and regional data storage options.</span>
			</h2>
			<a href="#" class="inline-block mt-4 text-sm font-medium text-gray-600 hover:text-black border border-gray-200 px-4 py-2 rounded-lg hover:border-gray-300 transition-colors">
				Security details
			</a>
		</div>

		<div class="flex items-center gap-12">
			<div class="flex flex-col items-center gap-2">
				<div class="w-16 h-16 rounded-full border border-gray-200 flex items-center justify-center">
					<ShieldCheck size={32} class="text-gray-900" />
				</div>
				<span class="text-[10px] font-bold tracking-wider text-gray-500">SOC 2 Type II</span>
			</div>
			<div class="flex flex-col items-center gap-2">
				<div class="w-16 h-16 rounded-full border border-gray-200 flex items-center justify-center">
					<Lock size={32} class="text-gray-900" />
				</div>
				<span class="text-[10px] font-bold tracking-wider text-gray-500">GDPR</span>
			</div>
			<div class="flex flex-col items-center gap-2">
				<div class="w-16 h-16 rounded-full border border-gray-200 flex items-center justify-center">
					<FileCheck size={32} class="text-gray-900" />
				</div>
				<span class="text-[10px] font-bold tracking-wider text-gray-500">ISO 27001</span>
			</div>
		</div>
	</div>
</section>
