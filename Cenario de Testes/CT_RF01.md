## Cenário 01: Inventário de Estoque.

### Caso de Teste 01: . ✅

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT01 | O login será realizado com um nome de usuário e uma senha válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| As credenciais fornecidas (usuário e senha) devem ser válidas. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que estamos na página de login do OrangeHRM              |
| **E** preenchemos "Admin" no campo usuário                        |
| **E** preenchemos "admin123" no campo senha                       |
| **QUANDO** clicarmos no botão "Login"                             |
| **ENTÃO** seremos redirecionados para o Dashboard do sistema      |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O redirecionamento para o Dashboard deve ocorrer corretamente.  |

 https://jam.dev/c/c0a5d518-6dc9-42c4-a020-5c8d3b90074c

---


### Caso de Teste 02: Tentativa de login com senha incorreta. ✅

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT02 | O login falhará quando a senha for inválida.             |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário \"Admin\" deve existir no sistema. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que estamos na página de login do OrangeHRM              |
| **E** preenchemos "Admin" no campo usuário                        |
| **E** preenchemos "senhaerrada" no campo senha                    |
| **QUANDO** clicarmos no botão "Login"                             |
| **ENTÃO** uma mensagem de erro \"Invalid credentials\" será exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A mensagem de erro \"Invalid credentials\" deve ser exibida.    |

https://jam.dev/c/81f2afaa-5cb7-4989-8342-7c3147750097?startFrom=8.83

--- 

### Caso de Teste 03: Tentativa de login com campos em branco. ✅

| ID       | Descrição                                                |
| :------- | :------------------------------------------------------- |
| C01-CT03 | O login falhará quando os campos obrigatórios estiverem em branco. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Nenhuma. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que estamos na página de login do OrangeHRM              |
| **E** deixamos os campos de usuário e senha em branco             |
| **QUANDO** clicarmos no botão "Login"                             |
| **ENTÃO** deve ser exibida a mensagem \"Required\" em ambos os campos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

https://jam.dev/c/49893c43-7c01-40c0-af25-1f079f9c4031