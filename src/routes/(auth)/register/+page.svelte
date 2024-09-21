<script lang="ts">
	import { Button } from '$lib/components/ui/button/index';
	import * as Card from '$lib/components/ui/card/index';
	import { Input } from '$lib/components/ui/input/index';
	import { Label } from '$lib/components/ui/label/index';
</script>

<Card.Root class="space-y-4 border-none">
	<Card.Header class="px-0">
		<Card.Title>Create an account</Card.Title>
		<Card.Description>
			LazyBrain is an easy-to-use tool designed to enhance your productivity.
		</Card.Description>
	</Card.Header>

	<Card.Content class="px-0">
		<form>
			<div class="grid w-full items-center gap-6">
				<div class="flex flex-col space-y-3">
					<Label for="username">Username</Label>
					<Input id="username" />
				</div>

				<div class="flex flex-col space-y-3">
					<Label for="email">Email</Label>
					<Input id="email" type="email" />
				</div>

				<div class="flex flex-col space-y-3">
					<Label for="password">Password</Label>
					<Input id="password" type="password" />
				</div>
			</div>
		</form>
	</Card.Content>

	<Card.Footer class="px-0">
		<Button class="w-full">Register</Button>
	</Card.Footer>
</Card.Root>

<div class="text-center">
	<p class="text-sm font-medium leading-none">
		Already have an account? <a href="/login" class="text-primary hover:underline">Login</a>
	</p>
</div>
