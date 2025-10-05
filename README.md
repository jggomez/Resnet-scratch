# Implementaciones de Micro ResNet y Squeeze-and-Excitation desde Cero

Este repositorio contiene una serie de *notebooks* de Jupyter que exploran la implementación y el entrenamiento de varias arquitecturas de redes residuales (ResNet) simplificadas o "micro", construidas completamente **desde cero** utilizando bibliotecas fundamentales como PyTorch para entender la arquitectura interna.

-----

## 📂 Contenido del Repositorio

El repositorio se organiza en los siguientes *notebooks*, cada uno enfocado en una implementación específica:

### 1\. 🏗️ `Deep_Learning_Micro_Resnet.ipynb`

Este *notebook* sienta las bases, mostrando la construcción y el entrenamiento de una **Micro ResNet básica**.

  * **Objetivo Principal:** Entender el concepto fundamental del **bloque residual** (*residual block*) y su implementación para mitigar el problema del *vanishing gradient* en redes profundas.
  * **Arquitectura:** Implementación de la ruta de identidad (*identity shortcut*) y las capas convolucionales básicas para una ResNet superficial.

-----

### 2\. 🚀 `Deep_Learning_Resnet_34.ipynb`

Una extensión del *notebook* anterior, aquí se implementa una arquitectura más profunda, similar en principio a la conocida **ResNet-34**.

  * **Objetivo Principal:** Construir y apilar **múltiples bloques residuales** (bloque básico de dos capas) para crear una red más profunda, gestionando el *downsampling* mediante *strides* o bloques de proyección.
  * **Arquitectura:** Diseño de un modelo con 34 capas, explorando las diferentes etapas de la red y la transición entre ellas.

-----

### 3\. 👑 `Deep_Learning_SE_Resnet_50.ipynb`

Este *notebook* introduce una complejidad adicional: la implementación del **Bloque *Bottleneck*** (usado en ResNet-50) junto con el mecanismo de atención **Squeeze-and-Excitation (SE)**.

  * **Objetivo Principal:**
    1.  Implementar el **Bloque *Bottleneck*** (1x1, 3x3, 1x1) que reduce la complejidad computacional.
    2.  Integrar el módulo **Squeeze-and-Excitation**, que permite a la red realizar una recalibración adaptativa de los canales de *features* (atención a nivel de canal).
  * **Arquitectura:** Construcción de una red de 50 capas con los bloques *bottleneck* y el módulo SE integrado en cada bloque residual.

-----

## 🤝 Contribuciones

Si tienes sugerencias, correcciones o deseas proponer una extensión, ¡eres bienvenido! Por favor, abre un *Issue* o envía un *Pull Request*.

-----

## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)
