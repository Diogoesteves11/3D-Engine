# 3D Engine

Um motor gráfico 3D básico em C++ com OpenGL/GLUT, criado como projeto académico para a cadeira de Computação Gráfica.

## 🚀 Funcionalidades

- Renderização de malhas 3D com texturas aplicadas  
- Suporte a modelos padrão como cubos, esferas, cilindros, etc.  
- Gestão de câmara (movimentação, rotação, zoom)  
- Controlo de iluminação básica (ex: iluminação Phong ou Gouraud)  
- Velocidade de frame controlável (opções VSync)  
- Scripts de geração de geometria procedural

---

## ⚙️ Requisitos

- C++17  
- OpenGL + GLUT (ou freeGLUT) instalados  
- CMake (versão 3.x ou superior)  
- Possivelmente GLEW/GLAD se necessário para gestão das extensões OpenGL  

---

## 🛠️ Instalação & Build

1. Clone o repositório:
   ```bash
   git clone https://github.com/Diogoesteves11/3D-Engine.git
   cd 3D-Engine


mkdir build && cd build
cmake ..

cmake --build .

# Criar um modelo
./generator ...

# Iniciar o motor com um modelo
./engine configFile.xml

# (Opcional) Desativar VSync (em Linux):
vblank_mode=0 ./3d-engine ../models/meu_modelo.obj

## 📝 Documentação

Veja comentários nos ficheiros em src/ para explicações das principais classes e funções. Ideal para aprender organização de um motor gráfico OpenGL simples.


## 📚 Trabalhos Associados
Relatórios de projeto por fases, disponíveis em docs/ (ex: Fase1.pdf, Fase2.pdf…), detalhando requisitos, desenho da arquitetura, testes, etc.

## 🚀 Funcionalidades

Renderização de malhas 3D com texturas aplicadas

Suporte a modelos padrão como cubos, esferas, cilindros, etc.

Gestão de câmara (movimentação, rotação, zoom)

Controlo de iluminação básica (ex: iluminação Phong ou Gouraud)

Velocidade de frame controlável (opções VSync)

Scripts de geração de geometria procedural


## ⚙️ Requisitos

C++17

OpenGL + GLUT (ou freeGLUT) instalados

CMake (versão 3.x ou superior)

Possivelmente GLEW/GLAD se necessário para gestão das extensões OpenGL


## 🎮 Execução

# Gerar plano
./generate_plane <comprimento> <divisões> <output.3d>

# Gerar esfera
./generate_sphere <raio> <slices> <stacks> <output.obj>

# Executar Motor Gráfico
./engine configFile.xml
