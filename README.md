## React

React é uma biblioteca para criar pequenas partes de interface que são chamadas de componentes, os componentes podem ser um único elemento customizado ou uma composição:

#### Componente simples

```javascript
const ComponentSimples = () => {
  return(
    <button>Click me</button>
  );
}
```

#### Componente composto

```javascript
const ComponentComposto = () => {
  return(
    <>
      <form>
        <label>Nome</label>
        <input type="text" placeholder="Digite seu nome" />
        <label>Email</label>
        <input type="email" placeholder="Digite seu email" />
        <button>Enviar</button>
      </form>
    </>
  );
}
```

Esses componentes são auto gerenciados, também podem pertencer à um contexto e trocarem informações mutuamente.

### Principais conceitos

- Components
- Hooks
- Contexts
- Routes
- Layouts
