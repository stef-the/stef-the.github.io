<script>
	let tick = 0;
    let helloVar = 'Hello'
    const hello = ['Hello', 'Bonjour', 'Hallo', 'Hola', 'Hallå', 'Selam', '你好', 'こんにちは', 'Привет', 'Kumusta', 'Ciao', 'Olá', 'Ahlan', 'Halløj'];

	setInterval(() => {
		helloVar = hello[Math.floor(Math.random() * hello.length)];;
	}, 1500);
</script>

<main class="font-sans bg-gray-200 h-screen">
    <div class="grid place-content-center h-full">
        <h1 class="text-6xl">{helloVar}</h1>
    </div>
</main>
