# Trabajo de la Universidad: Clase Vector en C#

Este proyecto representa un trabajo académico de la universidad en el que desarrollamos una clase Vector en JavaScript. Esta clase permite realizar cálculos matemáticos utilizando un array como base y está diseñada para llevar a cabo una variedad de operaciones matemáticas.

Visita la version Web [Clase-Vector](https://clase-vector-vanilla-javascript.vercel.app/)

<div align="center">
  <a href="https://clase-vector-vanilla-javascript.vercel.app/">
    <img src="https://i.ibb.co/xqYrbBH/clase-vector-csharp.png" alt="clase-vector-csharp" border="0">
  </a>
</div>


## Características

La clase Vector en JavaScript incluye las siguientes características y operaciones:

- **Creación de Vectores:** Puedes crear un nuevo objeto Vector vacío e ir cargándolo con elementos, o cargarlo con valores aleatorios en un rango específico.
  
- **Selección de Elementos:** La clase ofrece métodos para seleccionar elementos específicos basados en ciertos criterios, como primos, no primos, buenos valores, etc.

- **Operaciones Matemáticas:** Incluye operaciones matemáticas comunes como suma, resta, producto escalar, magnitud, producto cruz y más.

- **Ordenamiento:** Puedes ordenar el vector tanto de forma ascendente como descendente utilizando varios algoritmos, como el ordenamiento por intercambio y el ordenamiento burbuja.

- **Búsquedas:** Ofrece búsquedas binarias y secuenciales para encontrar elementos específicos en el vector.

- **Operaciones de Conjuntos:** Permite realizar operaciones de conjuntos como intersección, unión y diferencia entre conjuntos representados por vectores.

- **Eliminación de Duplicados:** Puedes eliminar duplicados del vector.

## Metodos de la Clase Vector

- Cargar elemento x elemento
- Cargar
- Descargar
- Cargar serie aritmética
- Cargar serie Fibonacci
- Seleccionar por posición
- Seleccionar primos
- Seleccionar no primos
- Seleccionar buenos
- Promedio
- Máximo
- Frecuencia
- Desviación media
- Desviación estándar
- Búsqueda binaria
- Búsqueda secuencial
- Ordenamiento ascendente
- Ordenamiento descendente
- Unión de conjuntos
- Intersección de conjuntos
- Diferencia de conjuntos A-B
- Diferencia de conjuntos B-A
- Invertir
- Contar elementos de las posiciones submúltiplos
- Buscar elemento mayor de las posiciones múltiplos
- Buscar la media de las posiciones múltiplos
- Verificar si todos los elementos son iguales
- Verificar si el segmento está ordenado
- Insertar vector2 en 1 respecto a una posición
- Eliminar elementos de un segmento
- Duplicar elementos
- Ordenar elementos de un segmento
- Encontrar elemento menos repetido de un segmento
- Encontrar la frecuencia de distribución de un segmento
- Intercalar primos y no primos
- Segmentar par y no par
- Segmentar primos y no primos
- Segmentar capicuas y no capicuas
- Intercalar par y no par
- Intercalar primo y no primo

## Ejemplo: 

```csharp

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Clase Vector

class Vector
    {
        private const int max = 100;
        private int[] v;
        private int n;
        // Constructor de la clase Vector
        public Vector()
        {
            v = new int[max];
            n = 0;
        }

        // metodos que tienen la capacidad de acceder a variables que estan por fuera de ellos
        public void CargarRandom(int n1, int a, int b)
        {
            Random r = new Random();
            n = n1;
            for (int i = 1; i <= n; i++)
                v[i] = r.Next(a, b + 1);
        }

        // Metodo para cargar por elemento
        public void CargarElementoXElemento(int dato)
        {
            n++;
            v[n] = dato;
        }

        // etc...
    }
```

La Clase Vector se apoya de una clase NEnt (numero entero) para funcionar

## Metodos de la clase NEnt

- Cargar
- Descargar
- Invertir
- Numero digitos
- Verificar par
- Verificar primos
- Verificar capicua

## Ejemplo:

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Clase_Vector
{
    class NEnt
    {
        private int valor;

        public NEnt()
        {
            valor = 0;
        }

        public void Cargar(int numero)
        {
            valor = numero;
        }

        public string Descargar()
        {
            return valor.ToString();
        }

        public void Invertir()
        {
            int digito;
            int resultado = 0;
            int numero = valor;
            while (numero > 0)
            {
                digito = numero % 10;
                resultado = resultado * 10 + digito;
                numero /= 10;
            }
            valor = resultado;
        }
        public void Ndigs()
        {
            int numeroDigs = valor.ToString().Length;
            valor = numeroDigs;
        }
        public bool VerificarPar()
        {
            return valor % 2 == 0;
        }
        public bool VerificarPrimo()
        {
            int i, c, r;
            c = 0;
            for(i=1;i<= valor; i++)
            {
                r = valor % i;
                if (r == 0)
                    c++;
            }
            return c == 2;
        }

        public bool VerificarCapicua()
        {
            int capicua = this.valor;
            this.Invertir();
            return capicua == this.valor;
        }
    }
}

```

# Clonar un Repositorio en Visual Studio 2015

Este tutorial te guiará a través del proceso de clonar un repositorio de GitHub en Visual Studio 2015 utilizando la URL proporcionada. Nota: Tambien puedes descargar el archivo .zip y descomprimirlo en tu maquina.

## Requisitos Previos

Antes de comenzar, asegúrate de tener lo siguiente:

- [Visual Studio 2015](https://visualstudio.microsoft.com/vs/older-downloads/) instalado en tu sistema.
- Una cuenta de [GitHub](https://github.com/).
- Git instalado en tu sistema. Puedes descargarlo desde [git-scm.com](https://git-scm.com/).

## Pasos para Clonar el Repositorio 🙌

### Paso 1: Abrir Visual Studio 2015

Abre Visual Studio 2015 en tu sistema.

### Paso 2: Clonar el Repositorio

1. En el menú superior, selecciona "Archivo" y luego "Clonar repositorio".

2. Ingresa la URL del repositorio que deseas clonar: https://github.com/SebastianINF/Clase-Vector-Csharp

3. Haz clic en el botón "Clonar" para iniciar el proceso de clonación.

### Paso 3: Iniciar Sesión en GitHub

Si aún no has iniciado sesión en GitHub, se te pedirá que lo hagas en este paso. Ingresa tus credenciales de GitHub si es necesario.

### Paso 4: Explorar el Repositorio

Una vez que se complete la clonación, el repositorio estará disponible en el explorador de soluciones de Visual Studio 2015. Ahora puedes trabajar en el proyecto localmente.

¡Listo! Has clonado con éxito el repositorio desde GitHub a Visual Studio 2015 y estás listo para comenzar a trabajar en tu proyecto.

### Paso 5: Crear una Pull Request (Opcional)**:

  -Si cuentas con las ganas de seguir aportando a este proyecto puedes realizar una pull request y mandarme tu trabajo y seguir mejorando este Repositorio.
  - Haz cambios en tu código y confirma tus modificaciones localmente.
  - Luego, crea una nueva rama (branch) para tu pull request.
  - Sube tu rama a tu repositorio remoto.
  - Visita el repositorio en GitHub y selecciona la opción "New Pull Request".
  - Sigue las instrucciones en pantalla para crear tu pull request.

  ¡Esperamos que este repositorio te sea de ayuda!
