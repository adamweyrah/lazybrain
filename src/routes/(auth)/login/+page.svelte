<script lang="ts">
	import { Button } from '$lib/components/ui/button/index';
	import * as Card from '$lib/components/ui/card/index';
	import { Input } from '$lib/components/ui/input/index';
	import { Label } from '$lib/components/ui/label/index';
</script>

<Card.Root class="space-y-4 border-none">
	<Card.Header class="px-0">
		<Card.Title>Login</Card.Title>
		<Card.Description>
			Welcome back to LazyBrain – your simple, powerful tool for boosting productivity.
		</Card.Description>
	</Card.Header>

	<Card.Content class="px-0">
		<form>
			<div class="grid w-full items-center gap-6">
				<div class="flex flex-col space-y-3">
					<Label for="email">Email</Label>
					<Input id="email" type="email" />
				</div>

				<div class="flex flex-col space-y-3">
					<div class="flex items-center justify-between">
						<Label for="password">Password</Label>
						<a href="/reset-password" class="text-primary text-sm hover:underline">
							Forgot password?
						</a>
					</div>
					<Input id="password" type="password" />
				</div>
			</div>
		</form>
	</Card.Content>

	<Card.Footer class="px-0">
		<Button class="w-full">Login</Button>
	</Card.Footer>
</Card.Root>

<div class="text-center">
	<p class="text-sm font-medium leading-none">
		Don&apos;t have an account? <a href="/register" class="text-primary hover:underline">Register</a
		>
	</p>
</div>
