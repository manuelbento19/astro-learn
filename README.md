# 🚀 Astro Learning
Lições aprendidas durante os meus estudo sobre o Framework

## Lições:
1. **Configuração e setup**:
- `npx create astro@latest`
3. **Components**:
- Um componente Astro é composto de duas partes principais: o **Component Script** e o **Component Template**.
3. **Props**:
- O Astro usa um limite de código (`---`) para identificar o script do componente em seu componente Astro
- Um componente Astro pode definir e aceitar adereços. Esses adereços ficam então disponíveis para o modelo de componente para renderização de HTML. Os adereços estão disponíveis no `Astro.props` global em seu script frontmatter.
- Também pode definir props com TypeScript com uma interface do tipo `Props`. O Astro selecionará automaticamente a interface Props em seu frontmatter e fornecerá avisos/erros de tipo. Esses adereços também podem receber valores padrão quando desestruturados de `Astro.props`.
4. **Slots**(On React are knowed as **Children**):
- Ao contrário dos **props**, que são atributos passados ​​para um componente Astro disponíveis para uso em todo o seu componente com `Astro.props`, os slots renderizam elementos HTML filhos onde eles são escritos.
- Um componente Astro também pode ter **slots** nomeados. Isso permite que você passe apenas elementos HTML com o nome do slot correspondente para o local de um `slot`.
- Os slots são nomeados usando o atributo `name`.
- Para injetar conteúdo HTML em um slot específico, use o atributo `slot` em qualquer elemento filho para especificar o nome do slot.
5. **Fallback Content for Slots**:
- Os slots também podem renderizar conteúdo substituto. Quando não há filhos correspondentes passados ​​para um slot, um elemento `<slot/>` renderizará seus próprios filhos de espaço reservado.
6. **File-based routing**:
- Astro aproveita uma estratégia de roteamento chamada **roteamento baseado em arquivo**. Cada arquivo em seu diretório `src/pages/` se torna um endpoint em seu site com base no caminho do arquivo.
7. **Markdown/MDX Pages**:
- Podemos também usar arquivos `.md` e `.mdx` para renderizar páginas.
- A sintaxe do componente Astro é um superconjunto do HTML. Ele foi projetado para ser familiar a qualquer pessoa com experiência em **HTML** ou **JSX**, mas existem algumas diferenças importantes entre os arquivos `.astro` e `.jsx`.
8. **Layouts**:
- Para criar layouts usamos os `slots`
- Em arquivos Md e MDX precisamos importar usando o atributo `layout`.
