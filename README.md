# 🏰 **Course IT Tower**
### _A sua torre do conhecimento online!_  
👨‍💻 Desenvolvido por **Lucas Siqueira Torres** e **Gabriel Siqueira Torres**

---

![Banner](https://img.shields.io/badge/STATUS-EM%20DESENVOLVIMENTO-yellow)
![License](https://img.shields.io/badge/Licença-Educacional-blue)
![Build](https://img.shields.io/badge/Build-Passing-brightgreen)


---

## 📘 **Sobre o Projeto**

O **Course IT Tower** é uma plataforma de **Educação a Distância (EAD)** simplificada, onde **instrutores** criam, gerenciam e publicam cursos — e **alunos** se matriculam, assistem às aulas e acompanham seu progresso.  

> 🎯 Nosso objetivo é tornar o aprendizado online mais acessível, intuitivo e interativo.

🧗‍♂️ **Suba os andares da torre do conhecimento — um curso de cada vez!**

---

## 👥 **Perfis de Usuário**

| Perfil | Função Principal |
|:--|:--|
| 🧑‍🏫 **Instrutor** | Cria e gerencia cursos e aulas |
| 🎓 **Aluno** | Matricula-se e acompanha seu progresso |
| 🛠️ **Administrador** | Gerencia usuários e conteúdos da plataforma |

---

## ⚙️ **Lógica de Negócio Principal**

### 📘 Estrutura
- O **Instrutor** cria **Cursos** e adiciona **Aulas** → relação **OneToMany**.  
- O **Aluno** se **matricula** em cursos → relação **ManyToMany** entre `Usuario(Aluno)` e `Curso`, via **Matricula**.

### 📈 Progresso
- A entidade **Matricula** armazena o progresso do aluno.  
- Quando uma **Aula** é concluída, o progresso é atualizado **somente** para aquela matrícula.  
- Apenas o **Instrutor dono** do curso pode editar seu conteúdo.

---

