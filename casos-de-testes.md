# Casos de Teste – SauceDemo

## CT01 - Login com sucesso

**Pré-condição:** Usuário cadastrado  
**Passos:**
1. Acessar https://www.saucedemo.com/  
2. Preencher usuário: `standard_user`  
3. Preencher senha: `secret_sauce`  
4. Clicar em "Login"  

**Resultado esperado:**  
Usuário deve ser redirecionado para a página de produtos

---

## CT02 - Login com senha inválida

**Pré-condição:** Usuário cadastrado  
**Passos:**
1. Acessar https://www.saucedemo.com/  
2. Preencher usuário: `standard_user`  
3. Preencher senha: `senha_errada`  
4. Clicar em "Login"  

**Resultado esperado:**  
Mensagem de erro informando senha inválida

---

## CT03 - Login com campos vazios

**Pré-condição:** Nenhuma  
**Passos:**
1. Acessar https://www.saucedemo.com/  
2. Deixar campos de usuário e senha vazios  
3. Clicar em "Login"  

**Resultado esperado:**  
Mensagem de erro solicitando preenchimento dos campos

---

## CT04 - Login com usuário bloqueado

**Pré-condição:** Usuário bloqueado (`locked_out_user`)  
**Passos:**
1. Acessar https://www.saucedemo.com/  
2. Preencher usuário: `locked_out_user`  
3. Preencher senha: `secret_sauce`  
4. Clicar em "Login"  

**Resultado esperado:**  
Mensagem informando que o usuário está bloqueado

---

## CT05 - Adicionar produto ao carrinho

**Pré-condição:** Estar logado  
**Passos:**
1. Clicar no botão "Add to cart" do primeiro produto  
2. Clicar no ícone do carrinho  

**Resultado esperado:**  
Produto adicionado aparece no carrinho

---

## CT06 - Remover produto do carrinho

**Pré-condição:** Ter pelo menos 1 produto no carrinho  
**Passos:**
1. Acessar o carrinho  
2. Clicar em "Remove" no produto  

**Resultado esperado:**  
Produto é removido do carrinho

---

## CT07 - Validar preço total

**Pré-condição:** Ter produtos no carrinho  
**Passos:**
1. Acessar o carrinho  
2. Verificar preço de cada produto  
3. Verificar preço total  

**Resultado esperado:**  
Preço total corresponde à soma dos produtos

---

## CT08 - Preencher informações e finalizar compra

**Pré-condição:** Ter produtos no carrinho  
**Passos:**
1. Clicar em "Checkout"  
2. Preencher Nome, Sobrenome e CEP  
3. Clicar em "Continue"  
4. Clicar em "Finish"  

**Resultado esperado:**  
Mensagem de confirmação da compra exibida

---

## CT09 - Validar mensagem de sucesso

**Pré-condição:** Finalizar compra  
**Passos:**
1. Conferir mensagem exibida após finalizar compra  

**Resultado esperado:**  
Mensagem de sucesso: "THANK YOU FOR YOUR ORDER"
