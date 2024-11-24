<html>
	<head>
		<!-- <meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1.0" > -->
		<!-- <meta  http-equiv="refresh" content="10" > -->
	<style>
		body {
			<!-- height: 100wh; -->
			overflow: hidden;
			display: flex;
			justify-content: center;
			align-items: end;
			background: #212121;
		}
		header {
			display: flex;
			flex-direction: column;
			align-items: center;
		}
		.antenne {
				height: 3em;
				width: 6.5em;
				background: #9b9ba6;
				border-radius: 100px 100px 0 0;
				display: flex;
				justify-content: center;
		}
		.point {
				height: 0.3em;
				width: 0.7em;
				border-radius: 50px 50px 0 0;
				background: #e90a0d;
				translate: 0 -100%;
				position: relative;
		}
		.laser {
			position: absolute;
			left: 50%;
			translate: -50%;
			width: 0.2em;
			background: #e90a0d;
			bottom: 0;
			animation: shoot 5s linear forwards 2s;
		}
		.parabole {
			width: 12em;
			height: 5em;
			background: #edeef0;
			border-radius: 0 0 50px 50px;
		}
		main {
			display: flex;
			justify-content: center;
			align-items: center;
		}
		.solar-array-container {
			display: flex;
		}
		.solar-array {
			height: 10em;
			width: 15em;
			border: #dcdee2 0.8em solid;
			background: #8ec1d6;
			position: relative;
		}
		.solar-array::before,
		.solar-array::after {
			content: "";
			background: #dcdee2;
			position: absolute;
		}
		.solar-array::before {
			width: 100%;
			height: 0.8em;
			top: 50%;
			translate: 0 -50%;
		}
		.solar-array::after {
			width: 0.8em;
			height: 100%;
			left: 50%;
			translate: -50%;
		}
		.linker-container {
			display: flex;
			flex-direction: column;
			justify-content: space-around;
			height: 11.6em;
			width: 2.2em;
		}
		.link {
			width: 100%;
			height: 0.8em;
			background: #dcdee2;
		}
		.module-container {
			display: flex;
			flex-direction: column;*
			align-items: center;
		}
		.top-module {
			width: 8em;
			height: 0;
			border-width: 0 2em 2em 2em;
			border-style: solid;
			border-color: transparent transparent #b7b9c0;
		}
		.module {
			background: #dcdee2;
			height: 18em;
			width: 12em;
		}
		.bottom-module {
			width: 8em;
			height: 0;
			border-width: 2em 2em 0 2em;
			border-style: solid;
			border-color: #b7b9c0 transparent transparent;
		}
		.satellite{
		margin: 300px 200px 100px 200px;}
		.body {margin: 200px;}
		@keyframes shoot {
			from{
					height: 0;
			}
			to { 
					height: 24em;
			}
		}		
	</style>
	</head>
	
	<body>
		<div class="satellite">
			<header>
				<div class="antenne">
					<div class="point">
						<div class="laser"></div>
					</div>
				</div>
				<div class="parabole"></div>
			</header>
			<main>
				<div class="solar-array-container left">
					<div class="solar-array"></div>
					<div class="linker-container">
						<div class="link"></div>
						<div class="link"></div>
					</div>
				</div>
				<div class="module-container">
					<div class="top-module"></div>
					<div class="module"></div>
					<div class="bottom-module"></div>
				</div>
				<div class="solar-array-container right">
					<div class="linker-container">
						<div class="link"></div>
						<div class="link"></div>
					</div>
					<div class="solar-array"></div>
				</div>	
			</main>
			</div>
	<p>Satllite en orbite</p>		
	</body>
</html>
