# Projeto de Estágio - Mini-Curso SCORM (Articulate Rise)

Este projeto foi desenvolvido utilizando a ferramenta de autoria **Articulate Rise 360** conforme foi sugerido. O objetivo foi entregar um pacote SCORM 1.2 funcional, responsivo e que atendesse aos requisitos específicos de *tracking* de avaliação (`Passed/Failed` com nota mínima de 60%).

## 1. Arquivos de Entrega

O pacote SCORM final, pronto para importação em qualquer LMS, é o arquivo **ZIP** que acompanha esta documentação.

* **Padrão Utilizado:** SCORM 1.2 (Conforme inspeção no `imsmanifest.xml`)
* **Ferramenta de Autoria:** Articulate Rise 360

---

## 2. Conformidade com Requisitos SCORM (Tracking de Nota)

A funcionalidade da avaliação foi garantida com a seguinte configuração na exportação do Rise:

| **Rastreamento** | `Track using quiz result` | Garante que o LMS utilize a nota do quiz (Lição 2) para o status de sucesso. |
| **Nota de Aprovação** | **60%** |. O curso envia `Passed` se a nota for maior ou igual a 60%, e `Failed` se for menor que 60\%. |
| **Status do Relatório** | `Passed/Failed` | Garante o registro do status de aprovação ou reprovação no LMS, conforme exigido. |
| **Tempo Gasto** | Automático | O Rise envia automaticamente, registrando o tempo do aluno. |

---

## 3. Estrutura do Conteúdo

O curso utiliza um design responsivo nativo e está dividido em 3 lições sequenciais:

1.  **Boas-Vindas e Fundamentos (Tela 1):** Introdução ao SCORM e informações iniciais.
     **recurso multimídia** imagem para enriquecer o design.
2.  **Quiz de Avaliação (Tela 2):** 3 questões de **Múltipla Escolha** para avaliação, com feedback imediato.
3.  **Conclusão (Tela 3):** Mensagem final de encerramento e revisão dos tópicos vistos.

---

## 4. Inspeção e Otimização de Código 

O código gerado foi inspecionado no VS Code para garantir a integridade do pacote:

* O arquivo **`imsmanifest.xml`** foi validado para confirmar a estrutura SCORM 1.2.
* **Correção de CSS:** foram feitas por mim algumas mudanças na estilização do projeto, tornando mais intuitivo as páginas e com uma aparência mais amigável para o consumidor final.
