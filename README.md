# tsconfig-base

![ts-strict](https://img.shields.io/badge/typescript-%F0%9F%92%AA%20strict-blue?style=for-the-badge&logo=typescript)

tsconfig-base

## node

```json
{
  "compilerOptions": {
    "lib": ["es2020"],
    "baseUrl": ".",
    "module": "esnext",
    "moduleResolution": "node",
    "target": "es6",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "pretty": true,
    "noEmit": true,
    "declaration": true,
    "sourceMap": true,
    "outDir": "lib"
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules", "lib", "test"]
}
```

## react17+

```json
{
  "compilerOptions": {
    "lib": ["es2020", "dom"],
    "baseUrl": ".",
    "module": "es2020",
    "moduleResolution": "node",
    "resolveJsonModule": true,
    "jsx": "react-jsx",
    "target": "es6",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "pretty": true,
    "noEmit": true,
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules", "dist", "test"]
}
```
