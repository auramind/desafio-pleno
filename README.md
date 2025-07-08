## Desafio Técnico – Desenvolvedor Python Pleno

**Sistema de Gerenciamento de Inventário**

### Requisitos Funcionais

1. **Representação de Produtos**

   * O sistema deve ser capaz de representar produtos com as seguintes propriedades mínimas:

     * Identificador único
     * Nome
     * Preço unitário
     * Quantidade em estoque

2. **Gerenciamento de Produtos**

   * Deve ser possível:

     * Adicionar um novo produto ao inventário
     * Consultar um produto a partir de seu identificador
     * Atualizar a quantidade em estoque de um produto existente

3. **Regras de Negócio**

   * A quantidade em estoque não pode ser negativa.
   * Produtos com identificadores duplicados não devem ser adicionados ao inventário.
   * Consultas a produtos inexistentes devem retornar de forma segura (sem crash).

4. **Cálculos e Relatórios**

   * O sistema deve ser capaz de calcular o valor total do inventário (somatório de `preço * quantidade` para cada item).
   * Deve ser possível listar os produtos com estoque abaixo de um valor mínimo informado.

5. **Boas Práticas**

   * O código deve ser orientado a objetos
   * Utilize tipagem estática com type hints
   * Utilize recursos modernos da linguagem (como `@dataclass` ou `property`, se fizer sentido)
   * Evite repetição de código e implemente validações de forma reutilizável

---

### Requisitos Não Funcionais

* O sistema deve funcionar completamente **em memória**, sem dependência de arquivos, bancos de dados ou frameworks web.
* O código deve ser **modular e testável**.
* Não utilize bibliotecas externas (exceto `typing`, `dataclasses`, ou `unittest/pytest` para testes).
* A estrutura do projeto deve ser limpa e organizada.

---

### Diferenciais Técnicos

Os seguintes itens não são obrigatórios, mas serão considerados diferenciais positivos:

* Implementação de testes automatizados
* Validações desacopladas por meio de classes ou funções auxiliares
* Uso de princípios SOLID, especialmente SRP e OCP
* Design extensível (ex: facilitar inclusão futura de categorias, descontos, etc.)
* Logging ou tratamento de exceções com mensagens claras

---

### Entrega

* Envie seu código em um repositório Git (GitHub, GitLab, Bitbucket etc.)
* Adicione um README.md com instruções básicas de execução e testes, se houver