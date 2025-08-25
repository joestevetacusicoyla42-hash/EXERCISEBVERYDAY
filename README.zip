Aquí tienes el **proyecto Next.js + TailwindCSS** para tu web **EXERCISEVERYDAY** con varias páginas. Puedes usarlo directamente en Vercel para tener una URL pública:

---

### 📂 Estructura
```
exerciseveryday/
 ├─ pages/
 │   ├─ index.js          # Inicio
 │   ├─ recomendaciones.js
 │   ├─ alimentacion.js
 │   ├─ calendario.js
 │   ├─ galeria.js
 │   ├─ testimonios.js
 │   └─ contacto.js
 ├─ components/
 │   ├─ Layout.js         # Layout con Navbar y Footer
 │   └─ Navbar.js         # Menú de navegación
 ├─ styles/
 │   └─ globals.css       # Tailwind
 ├─ package.json
 └─ tailwind.config.js
```

---

### 📌 Código principal

#### `pages/_app.js`
```javascript
import '../styles/globals.css'
import Layout from '../components/Layout'

function MyApp({ Component, pageProps }) {
  return (
    <Layout>
      <Component {...pageProps} />
    </Layout>
  )
}

export default MyApp
```

#### `components/Layout.js`
```javascript
import Navbar from "./Navbar";

export default function Layout({ children }) {
  return (
    <div className="min-h-screen flex flex-col bg-gradient-to-b from-green-50 to-white">
      <Navbar />
      <main className="flex-grow container mx-auto p-6">{children}</main>
      <footer className="text-center p-4 text-gray-500">
        © {new Date().getFullYear()} - EXERCISEVERYDAY | Salud, Deporte y Bienestar
      </footer>
    </div>
  );
}
```

#### `components/Navbar.js`
```javascript
import Link from "next/link";

export default function Navbar() {
  return (
    <nav className="bg-green-700 text-white p-4 shadow-lg">
      <ul className="flex justify-center gap-6">
        <li><Link href="/">Inicio</Link></li>
        <li><Link href="/recomendaciones">Recomendaciones</Link></li>
        <li><Link href="/alimentacion">Alimentación</Link></li>
        <li><Link href="/calendario">Calendario</Link></li>
        <li><Link href="/galeria">Galería</Link></li>
        <li><Link href="/testimonios">Testimonios</Link></li>
        <li><Link href="/contacto">Contacto</Link></li>
      </ul>
    </nav>
  );
}
```

---

### 🌍 Ejemplo de páginas

#### `pages/index.js`
```javascript
export default function Home() {
  return (
    <div className="text-center">
      <h1 className="text-5xl font-bold text-green-900 mb-4">EXERCISEVERYDAY</h1>
      <p className="text-lg text-gray-700 mb-6">
        Bienvenido a la comunidad de salud, deporte y bienestar.
      </p>
      <img
        src="https://source.unsplash.com/800x400/?fitness,motivation"
        alt="Motivación"
        className="mx-auto rounded-2xl shadow-lg"
      />
    </div>
  );
}
```

#### `pages/recomendaciones.js`
```javascript
export default function Recomendaciones() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-4">Recomendaciones</h2>
      <p className="text-gray-700 mb-4">
        Encuentra rutinas de ejercicio, consejos de entrenamiento y tips prácticos para mejorar tu rendimiento.
      </p>
      <img
        src="https://source.unsplash.com/600x300/?training"
        alt="Entrenamiento"
        className="rounded-xl shadow-md"
      />
    </div>
  );
}
```

#### `pages/alimentacion.js`
```javascript
export default function Alimentacion() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-4">Alimentación</h2>
      <p className="text-gray-700 mb-4">
        Planes alimenticios, recetas saludables y la importancia de una buena nutrición.
      </p>
      <img
        src="https://source.unsplash.com/600x300/?healthy-food"
        alt="Alimentación"
        className="rounded-xl shadow-md"
      />
    </div>
  );
}
```

#### `pages/calendario.js`
```javascript
import { Calendar } from "@/components/ui/calendar";

export default function Calendario() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-4">Calendario</h2>
      <p className="text-gray-700 mb-4">
        Organiza tus entrenamientos y controla tu progreso.
      </p>
      <Calendar className="border rounded-xl shadow-md" />
    </div>
  );
}
```

#### `pages/galeria.js`
```javascript
export default function Galeria() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-6">Galería Motivacional</h2>
      <div className="grid md:grid-cols-3 gap-6">
        <img src="https://source.unsplash.com/400x300/?running" className="rounded-lg shadow-md" />
        <img src="https://source.unsplash.com/400x300/?gym" className="rounded-lg shadow-md" />
        <img src="https://source.unsplash.com/400x300/?yoga" className="rounded-lg shadow-md" />
      </div>
    </div>
  );
}
```

#### `pages/testimonios.js`
```javascript
export default function Testimonios() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-4">Testimonios</h2>
      <p className="text-gray-700 mb-4">
        Escucha lo que otros deportistas tienen que decir sobre su experiencia.
      </p>
      <blockquote className="border-l-4 border-green-700 pl-4 italic text-gray-600 mb-4">
        “Gracias a EXERCISEVERYDAY logré organizar mi vida y sentirme más saludable.”
      </blockquote>
      <blockquote className="border-l-4 border-green-700 pl-4 italic text-gray-600">
        “La motivación diaria me ayuda a no rendirme.”
      </blockquote>
    </div>
  );
}
```

#### `pages/contacto.js`
```javascript
export default function Contacto() {
  return (
    <div>
      <h2 className="text-3xl font-bold text-green-800 mb-4">Contacto</h2>
      <p className="text-gray-700 mb-6">Envíanos tus dudas o sugerencias.</p>
      <form className="grid gap-4 max-w-md mx-auto">
        <input type="text" placeholder="Nombre" className="border p-2 rounded" />
        <input type="email" placeholder="Correo" className="border p-2 rounded" />
        <textarea placeholder="Mensaje" className="border p-2 rounded"></textarea>
        <button className="bg-green-700 text-white py-2 rounded shadow-md hover:bg-green-800">Enviar</button>
      </form>
    </div>
  );
}
```

---

✅ Con este proyecto, si lo subes a **GitHub** y lo conectas a **Vercel**, obtendrás una URL como:
```
https://exerciseveryday.vercel.app
```

---
