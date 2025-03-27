<div style="max-width: 800px; margin: auto; text-align: center; font-family: Arial, sans-serif;">
    <h1>Hi there, I'm [Your Name] 👋</h1>
    <p><strong>Software Engineer</strong> passionate about building scalable web applications and interactive experiences.</p>
    <h2>🚀 Tech Stack</h2>
    <p>HTML, CSS, TailwindCSS, Chakra UI, Material UI, JavaScript, React.js, Next.js, RTK Query, Node.js, Express.js, MongoDB, MySQL, PostgreSQL, Google Integration, Firebase, Azure</p>
    <h2>🌐 Connect with Me</h2>
    <p>
        <a href="https://www.linkedin.com/in/your-profile" target="_blank">LinkedIn</a> |
        <a href="https://twitter.com/your-handle" target="_blank">Twitter</a> |
        <a href="https://github.com/your-username" target="_blank">GitHub</a>
    </p>
    <h2>✨ Interactive Experience</h2>
    <canvas id="threejs-canvas" style="width: 100%; height: 400px; background: black;"></canvas>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script>
        const scene = new THREE.Scene();
        const camera = new THREE.PerspectiveCamera(75, window.innerWidth / 400, 0.1, 1000);
        const renderer = new THREE.WebGLRenderer({ canvas: document.getElementById('threejs-canvas') });
        renderer.setSize(window.innerWidth, 400);
        const geometry = new THREE.TorusKnotGeometry(10, 3, 100, 16);
        const material = new THREE.MeshBasicMaterial({ color: 0xff6347, wireframe: true });
        const torusKnot = new THREE.Mesh(geometry, material);
        scene.add(torusKnot);
        camera.position.z = 50;
        function animate() {
            requestAnimationFrame(animate);
            torusKnot.rotation.x += 0.01;
            torusKnot.rotation.y += 0.01;
            renderer.render(scene, camera);
        }
        animate();
    </script>
</div>
