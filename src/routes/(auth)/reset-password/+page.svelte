<script lang="ts">
	import { Button } from '$lib/components/ui/button/index';
	import * as Card from '$lib/components/ui/card/index';
	import { Input } from '$lib/components/ui/input/index';
	import { Label } from '$lib/components/ui/label/index';
</script>

<Card.Root class="space-y-4 border-none">
	<Card.Header class="px-0">
		<Card.Title>Reset Password</Card.Title>
		<Card.Description>
			To reset your password enter the email you used to register an account with LazyBrain
		</Card.Description>
	</Card.Header>

	<Card.Content class="px-0">
		<form>
			<div class="grid w-full items-center gap-6">
				<div class="flex flex-col space-y-3">
					<Label for="email">Email</Label>
					<Input id="email" type="email" />
				</div>
			</div>
		</form>
	</Card.Content>

	<Card.Footer class="px-0">
		<Button class="w-full">Reset Password</Button>
	</Card.Footer>
</Card.Root>

<div class="text-center">
	<p class="text-sm font-medium leading-none">
		<span>Do you remember your password?</span>
		<a href="/login" class="text-primary hover:underline">Login</a>
	</p>
</div>
