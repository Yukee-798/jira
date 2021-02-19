### 使用 typescript 创建项目
```bash
$ npx create-react-app jira --template typescript
```
### 修改参照路径
**tsconfig.json**
```diff
{
  "compilerOptions": {
+   // 将默认的参照路径从项目根目录改为 ./src
+   "baseUrl": "./src",
    "target": "es5",
    "lib": [
      "dom",
      "dom.iterable",
      "esnext"
    ],
    "allowJs": true,
    "skipLibCheck": true,
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true,
    "strict": true,
    "forceConsistentCasingInFileNames": true,
    "noFallthroughCasesInSwitch": true,
    "module": "esnext",
    "moduleResolution": "node",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "noEmit": true,
    "jsx": "react-jsx"
  },
  "include": [
    "src"
  ]
}

```

### prettier 规范代码格式