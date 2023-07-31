<script lang="ts">
	import '../css/global.css';
</script>

<svelte:head>
	<title>Etourne</title>
</svelte:head>

<div class="parent">
	<div class="navbar">
		<img src="/logo/e-logo.svg" alt="logo" />
		<a class="add-discord-bot-btn" href="/">
			<img src="/icons/discord-logo.svg" alt="discord logo" /> Add Discord Bot
		</a>
	</div>
	<div class="hero">
		<h1>Tournament and Event Management Software</h1>
		<h1>With Discord Bot and Web App</h1>
		<div class="coming-soon">
			<p>Web App coming soon</p>
		</div>
	</div>
	<div class="layout">
		<div class="about">
			<h2>How does it work?</h2>
			<p>
				Etourne is a versatile app that simplifies event and tournament
				organization on Discord. With both a Discord bot and a web app, it
				streamlines the creation and management of events, whether for teams
				or individual players. You can set limits for participants and host
				events for any game of your choice. With user-friendly commands and
				buttons, Etourne aims to make event planning simple.
			</p>
		</div>
	</div>
</div>

<style lang="scss">
	.parent {
		min-height: 100vh;
		background-color: var(--secondary-color);

		.navbar {
			background-color: var(--light-secondary-color);
			padding: 30px 50px;

			display: flex;
			justify-content: space-between;

			img {
				width: 35px;
			}

			a {
				background-color: var(--primary-color);
				color: var(--white-color);
				border-radius: 5px;
				padding: 15px 30px;
				text-decoration: none;

				display: flex;
				gap: 20px;
				align-items: center;
				font-size: var(--normal-font-size);
				font-weight: bold;

				&:hover {
					cursor: pointer;
					filter: brightness(0.95);
				}

				&:visited {
					background-color: var(--primary-color);
					color: var(--white-color);
				}
			}
		}

		.hero {
			text-align: center;
			color: var(--white-color);
			padding: 120px;

			display: flex;
			flex-direction: column;
			align-items: center;

			h1 {
				font-size: var(--heading-font-size);
			}

			.coming-soon {
				background-color: var(--primary-color);
				color: var(--white-color);
				border-radius: 5px;
				padding: 10px 30px;
				font-size: var(--normal-font-size);
				margin-top: 30px;
			}
		}

		.layout {
			margin: 0 150px;
		}
	}
</style>
