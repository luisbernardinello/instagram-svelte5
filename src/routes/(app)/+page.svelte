<script lang="ts">
	import PostCard from '$lib/components/PostCard.svelte';
	import Stories from '$lib/components/Stories.svelte';
	import { CircleUser } from 'lucide-svelte';
</script>

<div class="flex flex-col gap-5 lg:flex-row">
	<div class="flex-1 lg:flex-shrink-0">
		<div class="mx-auto w-full max-w-[630px]">
			<Stories />
			<div class="mt-5 space-y-5 px-5 md:px-10">
				<PostCard />
			</div>
		</div>
	</div>

	<div class="hidden px-3 text-sm lg:block lg:w-[300px] xl:w-[319px]">
		<div class="flex items-center gap-3">
			<CircleUser class="size-11" />
			<div>
				<p class="font-medium">teste</p>
				<p class="text-muted-foreground">teste@gmail.com</p>
			</div>
		</div>

		<div class="mb-3 mt-8 flex items-center justify-between">
			<p class="text-muted-foreground capitalize">suggested for you</p>
			<p class="text-xs font-medium">see all</p>
		</div>

		<div class="space-y-4">
			{#each { length: 5 } as _}
				<div class="flex items-center gap-3">
					<CircleUser class="size-11" />
					<div>
						<p class="font-medium">teste</p>
						<p class="text-muted-foreground">teste@gmail.com</p>
					</div>
					<a href="/" class="ml-auto text-xs text-blue-500">follow</a>
				</div>
			{/each}
		</div>
	</div>
</div>
