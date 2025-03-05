## Components

Os componentes são a parte principal do react, eles podem ser bem simples ou bem complexos, podemos criar componentes do zero, deriva-los a partir de outros componentes ou agrupa-los em um novo componente.

Componentes se assemelham bastante com funções, algumas das diferenças são:
- O nome de um componente sempre começa com letra maiúscula seguindo o padrão PascalCase;
- Componentes sempre retornam elementos visuais (JSX);

#### Componente simples

```javascript
const MyButton = () => {
  return(
    <button>Click me</button>
  );
}
```

#### Componente composto

```javascript
const MyForm = () => {
  return(
    <>
      <form>
        <label>Nome</label>
        <input type="text" placeholder="Digite seu nome" />
        <label>Email</label>
        <input type="email" placeholder="Digite seu email" />
        <MyButton />
      </form>
    </>
  );
}
```

Assim como uma função o componente também pode receber paramêtros, mas nos componentes são chamados de propriedades:

```javascript
const MyButton = ({label}) => {
  return(
    <button>{label}</button>
  );
}

// chamada
<MyButton label="Enviar" />
// o resultado esperado é que o botão seja exibido com o texto "Enviar" nele
```

Um componente pode receber não só paramêtros simples, mas elementos visuais também:

```javascript
const MyList = ({children}) => {
  return(
    <ul>
      {children}
    </ul>
  );
}

// chamada
<MyList>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</MyList>
// o resultado esperado é uma lista não ordenada com tres items
```
