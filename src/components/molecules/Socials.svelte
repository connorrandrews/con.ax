<script>
	import Social from '../atoms/Social.svelte';
	import { user } from '../../util/discord';
</script>

<div class="socials-container">
	<Social icon="github" tip="connorrandrews" link="https://github.com/connorrandrews" />
	<Social icon="discord" tip={user.username} link={`https://discord.com/users/${user.id}`} />
	<Social icon="email" tip="con@con.ax" link="mailto:con@con.ax" />
	<Social icon="kofi" tip="affan" link="https://ko-fi.com/connorrandrews" />
</div>

<style>
	.socials-container {
		display: flex;
		gap: 0.75rem;
	}
</style>
