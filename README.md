# lab11

Aquí empieza lab11: una base de Next.js para construir la web y avanzar con cambios pequeños, fáciles de revisar.

## La primera historia

- **Quién:** como desarrollador de lab11.
- **Quiero:** iniciar el repositorio con Next.js, TypeScript, Tailwind CSS y ESLint.
- **Para qué:** tener una aplicación que pueda ejecutar, extender y revisar mediante PR de `develop` hacia `main`.
- **Por qué:** una base compartida y versionada evita empezar cada entorno desde cero y permite rastrear las decisiones desde el primer cambio.

Arrancamos con la pantalla de Create Next App. Las funcionalidades del producto vendrán después.

## La siguiente historia: pnpm

- **Quién:** como desarrollador que trabaja en lab11.
- **Quiero:** usar pnpm como gestor de dependencias del proyecto.
- **Para qué:** instalar las mismas versiones y compartir un flujo de trabajo claro entre entornos.
- **Por qué:** un solo gestor y su lockfile reducen diferencias de instalación y evitan mantener archivos de bloqueo que compiten entre sí.

Pasamos de npm a pnpm. La versión del gestor queda en `package.json` y las versiones resueltas en `pnpm-lock.yaml`.

## Ejecutarlo en local

Necesitas Node.js 20.9 o superior y pnpm 9.0.6. Si tienes Corepack disponible, puedes activar esa versión con `corepack enable` y `corepack prepare pnpm@9.0.6 --activate`.

```bash
pnpm install --frozen-lockfile
pnpm dev
```

Abre [localhost:3000](http://localhost:3000). La página está en `app/page.tsx` y el layout en `app/layout.tsx`.

```bash
pnpm lint   # Revisión con ESLint
pnpm build  # Compilación de producción
pnpm start      # Servir la compilación
```

## Cómo avanzamos

Trabajamos en `develop` y proponemos la integración a `main` mediante PR. Cada PR cuenta su historia con quién, quiero, para qué y por qué. Este README guarda la versión rápida para quien llega al proyecto.
