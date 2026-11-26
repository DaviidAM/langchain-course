# LangChain Course

## Configuración Git para Push

Si encuentras problemas con la autenticación al hacer push en HTTPS, sigue estos pasos:

### 1. Cambiar el remote a SSH

```bash
git remote set-url origin git@github.com:DaviidAM/langchain-course.git
```

### 2. Verificar que el remote está configurado correctamente

```bash
git remote -v
```

Deberías ver algo como:
```
origin	git@github.com:DaviidAM/langchain-course.git (fetch)
origin	git@github.com:DaviidAM/langchain-course.git (push)
```

### 3. Hacer push del branch

```bash
git push --set-upstream origin <tu-branch>
```

Reemplaza `<tu-branch>` con el nombre de tu branch actual.

### Notas

- SSH usa claves SSH en lugar de tokens HTTPS, lo que es más seguro y confiable
- Si no tienes configuradas claves SSH, puedes generarlas con `ssh-keygen`
- Una vez configurado, puedes hacer push sin problemas en futuras ocasiones
