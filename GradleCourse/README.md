# Projetos Java com Gradle

- `build.gradle` é chamado de BuildScript. Ele que define toda a configuração da build.
  - Escrito utilizando uma *Domain Specific Language* (DSL), que pode ser o **Groovy** ou **Kotlin**;
  - Está relacionado as task que serão executadas.

## Instalação (Via Gradlew)

- `./gradlew`: Verifica se o Gradle está instalado. Caso não esteja, baixa a versão especificada no projeto.
- `./gradlew init`: Gera um novo projeto (do zero);
  - Tipo de projeto;
  - Linguagem;
  - Submódulos;
  - DSL;
  - Framework de Teste;
  - Nome do Projeto;
  - Pacote Source;
- `./gradlew tasks`: Exibe as tasks disponíveis para o projeto (padrões e criadas);
- `./gradlew run`: Executa o projeto em uma aplicação JVM;
- `./gradlew build`: Gera um executável;
- `./gradlew clean`: Remove o diretório de `build` um executável;

## Plugins

- Adicionam novas tasks e novos padrões da DSL ao gradle.
- Funcionam como bibliotecas que se pode adicionar no build.gradle;
- `Application`:
  - Facilita a criação de um **executável** de uma aplicação JVM;
  - Utiliza implicitamente os plugins Java e Distribution;
  - Disponibiliza **diversas tasks** para projetos java;

## Modules

- Configurar o arquivo `settings.gradle`: Os elementos em `include()` serão os módulos;
- Nos arquivos `build.gradle`, importa-se os outros módulos em `dependencies`.

## Tasks Customizadas

- `dependesOn`: Define dependências entre tarefas. Garante que a tarefa dependente seja executada após a tarefa que ela depende.
- `finalizedBy`: Especifica tarefas que devem ser executadas após a conclusão da tarefa atual.
- `mustRunAfter`: Define restrição de ordem entre tarefas ao executar múltiplas tarefas.
