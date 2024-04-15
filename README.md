# Algo

## Gradle

O **Gradle** é uma ferramenta de automação de compilação versátil e poderosa que pode ser usada para projetos em qualquer linguagem e plataforma. Ele ajuda equipes a construir, automatizar e entregar software de maneira mais eficiente e rápida.

- Capacidades:
  - Realizar tarefas antes, durante e após builds;
  - Rodar unit tests;
  - Colocar JAR ou APK em uma pasta diferente da padrão;
  - Gestão de dependencias do projeto;
  - Fazer builds com multiplos módulos e variações de compilação;
  - Gerar documentação Javadoc;
  - Assinar apks e aab no Android;
- Características:
  - Scripts escritos na linguagem Groovy;
  - Baseado em tasks;
  - Forte sistema de plugins;
  - Open Source;

O Gradlew (Gradle Wrapper) é uma ferramenta específica do Gradle que facilita a execução de tarefas de compilação e gerenciamento de projetos. É um script shell que envolve o Gradle e é utilizado para executar tarefas Gradle sem a necessidade de ter o Gradle.

- Portabilidade: Garante que todos os membros da equipe usem a mesma versão do Gradle, evitando problemas de compatibilidade;
- Automatização: Baixa automaticamente a versão correta do Gradle para o projeto;
- Modularização, também chamado de Multi Projetos;
  - Cada pasta/módulo vai possuir seu build.gradle.

## Maven

O **Apache Maven** é uma ferramenta opensource de automação e gerenciamento de projetos amplamente utilizada no mundo Java.

- Endereça como o software foi construído e suas dependências através do Project Object Model (POM);
- Facilita a compreensão do desenvolvedor;
- Fornece informações de qualidade;

## Comparações

- Gradle: Flexibilidade e Scripts.
  - Construído em cima dos padrões e convenções do Maven, mas usa a linguagem Groovy;
  - Mais flexível e permite maior customização;
  - Permite scripts no arquivo de configuração `build.gradle`;
  - Não possui um repositório central próprio par dependências;
- Maven: Projetos Java tradicionais.
  - Facilita a gestão das bibliotecas (JARS) utilizadas;
  - Define fases (clean, compile, test, package, etc.) para a construção do projeto;
  - `pom.xml` define as propriedades do build, mas não contém scripts;  
- NPM: JavaScript
  - Gerênciamento de pacotes e dependências similar ao Maven;
  - Usa o repositótio NPM para baixar pacotes;
  - Permite árvores de dependências aninhadas;
