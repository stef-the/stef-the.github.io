<script>
	let tick = 0;
	let helloVar = 'Hello';
	const hello = [
		'Hello',
		'Bonjour',
		'Hallo',
		'Hola',
		'Hallå',
		'Selam',
		'你好',
		'こんにちは',
		'Привет',
		'Kumusta',
		'Ciao',
		'Olá',
		'Ahlan',
		'Halløj'
	];

	let svgFill = '#d1d5db';

	const helloFont = [];

	setInterval(() => {
		helloVar = hello[Math.floor(Math.random() * hello.length)];
	}, 1500);
</script>

<main id="main" class="font-sans bg-gray-200 h-screen overflow-hidden">
	<div class="relative grid place-content-center h-screen">
		<a href="#two" class="z-10">
			<div
				class="absolute transition text-gray-800 grid place-content-center mt-8 w-96 h-96 cursor-pointer rounded-md"
				on:click={() => {
					document.getElementById('main')?.classList.add('h-max');
					document.getElementById('main')?.classList.remove('h-screen');
					console.log('overflow turned on');
				}}
				on:mouseenter={() => {
					svgFill = '#1f2937';
					document.getElementById('svgContainer')?.classList.add('translate-y-2');
					document.getElementById('hello')?.classList.add('-translate-y-4');
				}}
				on:mouseleave={() => {
					svgFill = '#d1d5db';
					document.getElementById('svgContainer')?.classList.remove('translate-y-2');
					document.getElementById('hello')?.classList.remove('-translate-y-4');
				}}
			>
				<h1 id="hello" class="text-6xl cursor-inherit text-inherit transition">
					{helloVar}
				</h1>
				<div id="svgContainer" class="transition flex justify-center">
					<svg
						version="1.1"
						id="downArrow"
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
						viewBox="0 0 20.633 20.633"
						style="enable-background:new 0 0 20.633 20.633;"
						xml:space="preserve"
						width="40"
					>
						<g>
							<path
								id="downArrowPath"
								fill={svgFill}
								d="M10.79,15.617l9.648-9.646c0.133-0.131,0.195-0.301,0.195-0.473s-0.062-0.344-0.195-0.473l-0.012-0.012
                    c-0.125-0.127-0.295-0.195-0.472-0.195h-4.682c-0.18,0-0.348,0.068-0.473,0.195l-4.48,4.479l-4.48-4.479
                    C5.711,4.886,5.54,4.818,5.366,4.818H0.684c-0.182,0-0.349,0.068-0.475,0.195L0.196,5.025C0.068,5.148,0,5.322,0,5.498
                    c0,0.176,0.068,0.348,0.196,0.473l9.648,9.646C10.108,15.88,10.53,15.88,10.79,15.617z"
							/>
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
							<g />
						</g>
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
						<g />
					</svg>
				</div>
			</div>
		</a>
		<svg
			version="1.1"
			id="Layer_1"
			xmlns="http://www.w3.org/2000/svg"
			xmlns:xlink="http://www.w3.org/1999/xlink"
			x="0px"
			y="0px"
			viewBox="0 0 371.62 371.62"
			style="enable-background:new 0 0 371.62 371.62;"
			xml:space="preserve"
            height="384"
            class="z-0"
		>
			<g>
				<path
					style="fill:#d1d5db"
					d="M62.513,153.087c-0.009-0.525-0.02-1.049-0.02-1.575c0-50.155,40.659-90.814,90.814-90.814
		c43.222,0,79.388,30.196,88.562,70.643c8.555-4.789,18.409-7.531,28.91-7.531c32.766,0,59.328,26.562,59.328,59.328
		c0,1.339-0.06,2.664-0.148,3.981c24.325,9.03,41.661,32.444,41.661,59.911c0,35.286-28.605,63.892-63.892,63.892H79.865
		C35.757,310.921,0,275.164,0,231.056C0,192.907,26.749,161.011,62.513,153.087z"
				/>
			</g>
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
			<g />
		</svg>
	</div>
	<div id="two" class="grid place-content-center h-screen">height</div>
</main>
