<script lang="ts">
	import { Bookmark, CircleUser, Ellipsis, Heart, MessageCircle, Send } from 'lucide-svelte';
	import { Separator } from '$lib/components/ui/separator';

</script>

<div class=" ">
	<a href='/' class="mb-3 flex items-center gap-3">
		<CircleUser />
		<div class="">
			<p class="text-sm font-medium">teste</p>
			<p class="text-xs text-muted-foreground">email@gmail.com</p>
		</div>
		<Ellipsis class="ml-auto w-fit" />
	</a>

    <img src='' class='h-[580px] w-full rounded bg-gray-100 object-contain' alt="">


	
	<div class="my-2 flex items-center gap-5">
		<Heart />
		<MessageCircle />
		<Send />

		<Bookmark class="ml-auto" />
	</div>

	<p class="mb-2 text-sm font-medium">100,4480 likes</p>
	<p class="mb-2 text-sm font-medium">
		teste: <span class="font-light">this is the caption</span>
	</p>

	<button class=" mb-2 text-sm capitalize text-muted-foreground">view all 24 comments</button>
	<input
		type="text"
		class="block border-none bg-transparent outline-none placeholder:text-sm"
		placeholder="Add a comment"
	/>
	<Separator class="mt-3" />
</div>
