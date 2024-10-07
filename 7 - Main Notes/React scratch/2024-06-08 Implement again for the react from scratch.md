Implement again for the react from scratch
- Configure Code Standard
- Configure commit specification check
- Configure Typescript

# Configure Code standard
- Install Eslint + Prettier to config the code standard
- After config eslint and prettier, we can prevent from conflicting between them by 
	- `eslint-config-prettier`: Overwrite `eslint`its own rule configuration
	- `eslint-plugin-prettier`: `prettier`Used to take over the repair code, that is`eslint --fix`
```
pnpm i eslint-config-prettier eslint-plugin-prettier -D -w
```

# Configure commit specification check
- Install Husky for checking before commit
```
pnpm i husky -D -w
```
- Then we install commitlint to check commit syntax 
```
pnpm i commitlint @commitlint/cli @commitlint/config-conventional -D -w
```

# Configure typescript
Create a file `tsconfig.json`
```
{
    "compileOnSave": true,
    "include": ["./packages/**/*"],
    "compilerOptions": {
        "target": "ESNext",
        "useDefineForClassFields": true,
        "module": "ESNext",
        "lib": ["ESNext", "DOM"],
        "moduleResolution": "Node",
        "strict": true,
        "sourceMap": true,
        "resolveJsonModule": true,
        "isolatedModules": true,
        "esModuleInterop": true,
        "noEmit": true,
        "noUnusedLocals": false,
        "noUnusedParameters": false,
        "noImplicitReturns": false,
        "skipLibCheck": true,
        "baseUrl": "./packages",
        "paths": {
            "hostConfig": ["./react-reconciler/src/hostConfig.ts"]
        }
    }
}
```
