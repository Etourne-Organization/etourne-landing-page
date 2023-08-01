<script lang="ts">
	import '../css/global.css';
</script>

<svelte:head>
	<title>Etourne</title>
</svelte:head>

<div class="parent">
	<div class="navbar">
		<img src="/logo/e-logo.svg" alt="logo" />
		<a
			class="add-discord-bot-btn"
			href="https://discord.com/api/oauth2/authorize?client_id=981646160798290051&permissions=17869480258752&scope=bot%20applications.commands"
		>
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

		<div class="contact">
			<h2>Got questions?</h2>
			<p>Join Discord Server or email info@noobdev54.com.</p>
		</div>
	</div>

	<div class="footer">
		<p>Copyright © 2023 All Rights Reserved</p>
	</div>
</div>

<style lang="scss">
	.parent {
		min-height: 100vh;
		background-color: var(--secondary-color);

		display: flex;
		flex-direction: column;

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

			.about {
				color: var(--white-color);

				h2 {
					font-size: var(--subheading-font-size);
				}

				p {
					font-size: var(--normal-font-size);
					margin-top: 15px;
					line-height: 25px;
				}
			}

			.contact {
				margin-top: 60px;
				color: var(--white-color);

				h2 {
					font-size: var(--subheading-font-size);
				}

				p {
					font-size: var(--normal-font-size);
					margin-top: 15px;
					line-height: 25px;
				}
			}
		}

		.footer {
			margin-top: 100px;
			justify-self: flex-end;
			padding: 25px 50px;
			color: var(--black-color);
			background-color: #f1f1f1;
		}
	}
</style>
