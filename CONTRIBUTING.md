# 🌾 Contribuindo para a Fazenda Digital

Olá, aventureiro! 👋 Muito obrigado por considerar contribuir para este repositório! Como uma boa fazenda, crescemos com ajuda e dedicação.

## 🌱 Como Contribuir

### 1️⃣ Fork do Repositório
Faça um fork deste repositório para sua conta pessoal.

```bash
git clone https://github.com/SEU_USUARIO/mar-ctrl-z.git
cd mar-ctrl-z
```

### 2️⃣ Crie uma Branch
Crie uma branch para sua contribuição:

```bash
git checkout -b feature/sua-feature
# ou
git checkout -b bugfix/seu-bugfix
```

**Nomes de branch recomendados:**
- `feature/nova-funcionalidade`
- `bugfix/corrige-erro`
- `docs/melhora-documentacao`
- `refactor/melhora-codigo`

### 3️⃣ Faça suas Mudanças
✅ Garantir que o código segue o padrão do projeto  
✅ Adicionar comentários/documentação quando necessário  
✅ Testar suas mudanças  

### 4️⃣ Commit
Use mensagens de commit claras e descritivas:

```bash
git commit -m "feat: adiciona detecção de aves com YOLOv8"
git commit -m "fix: corrige erro de validação em dados"
git commit -m "docs: atualiza README com instruções"
```

**Formato recomendado:**
- `feat:` para novas funcionalidades
- `fix:` para correções
- `docs:` para documentação
- `refactor:` para melhor código
- `test:` para testes

### 5️⃣ Push e Pull Request
```bash
git push origin feature/sua-feature
```

Abra um Pull Request com:
- Descrição clara do que foi mudado
- Referência a issues relacionadas (se houver)
- Screenshots/testes (se aplicável)

---

## 📋 Diretrizes do Código

### Python
```python
# ✅ BOM: Código limpo e bem comentado
def detectar_animais(imagem, modelo):
    """
    Detecta animais em uma imagem usando YOLOv8.
    
    Args:
        imagem: Array numpy da imagem
        modelo: Modelo YOLOv8 carregado
        
    Returns:
        Predições do modelo
    """
    resultados = modelo(imagem)
    return resultados
```

### Padrões
- Use **PEP 8** para Python
- Nomes descritivos para variáveis/funções
- Docstrings em português
- Type hints quando possível

---

## 🐛 Reportando Bugs

Se encontrar um bug, abra uma **Issue** com:
- 📝 Descrição clara do problema
- 🔍 Como reproduzir
- 💻 Ambiente (SO, Python version, etc)
- 📸 Screenshots/logs (se relevante)

---

## 💡 Sugestões de Melhorias

Tem uma ideia? Adoraria ouvir! Abra uma **Discussion** ou **Issue** com sua sugestão.

---

## ⭐ Código de Conduta

Todos devem ser respeitosos e inclusivos. Comportamentos abusivos resultarão em bloqueio.

---

## 🙏 Obrigado!

Sua contribuição faz essa fazenda crescer! Você será mencionado em:
- README como colaborador
- Release notes (se aplicável)
- Nossa lista de agradecimentos

**Feito com 💚 por Marina e colaboradores**

