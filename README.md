import React from 'react';
import { Heart, Github, Terminal, ShoppingBag } from 'lucide-react';

const LandingPage = () => {
  const technologies = [
    { name: "HTML", icon: <Terminal className="h-6 w-6" /> },
    { name: "CSS", icon: <Terminal className="h-6 w-6" /> },
    { name: "JavaScript", icon: <Terminal className="h-6 w-6" /> },
    { name: "Tailwind CSS", icon: <Terminal className="h-6 w-6" /> }
  ];

  return (
    <div className="min-h-screen bg-stone-50">
      {/* Hero Section */}
      <div className="relative bg-gradient-to-r from-amber-50 to-stone-50">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24">
          <div className="text-center">
            <h1 className="text-4xl font-bold tracking-tight text-stone-900 sm:text-5xl md:text-6xl">
              <span className="block">Idachi Elite Fashion</span>
              <span className="block text-amber-800 mt-2">Moda Premium en Guatemala</span>
            </h1>
            <p className="mt-6 max-w-2xl mx-auto text-lg text-stone-600">
              Una tienda en línea que importará ropa de diferentes marcas premium para mujeres desde Estados Unidos, 
              ofreciendo estilos exclusivos a precios justos.
            </p>
          </div>
        </div>
      </div>

      {/* Descripción Section */}
      <div className="py-16 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="lg:text-center">
            <h2 className="text-3xl font-bold text-stone-900">Nuestra Visión</h2>
            <p className="mt-4 max-w-2xl mx-auto text-lg text-stone-600">
              Nos convertiremos en la tienda online más atractiva de Guatemala, 
              brindando moda de alta calidad y una experiencia de compra memorable.
            </p>
          </div>
        </div>
      </div>

      {/* Motivación Section */}
      <div className="py-16 bg-amber-50">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="lg:text-center">
            <h2 className="text-3xl font-bold text-stone-900">Nuestra Motivación</h2>
            <div className="mt-6 flex justify-center">
              <Heart className="h-12 w-12 text-amber-700" />
            </div>
            <p className="mt-4 max-w-2xl mx-auto text-lg text-stone-600">
              Idachi Elite Fashion será más que un negocio; simbolizará un sueño de reunión 
              familiar y un nuevo comienzo. Cada prenda que ofreceremos representará un paso 
              más cerca de hacer realidad este sueño.
            </p>
          </div>
        </div>
      </div>

      {/* Tecnologías Section */}
      <div className="py-16 bg-stone-50">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="lg:text-center">
            <h2 className="text-3xl font-bold text-stone-900">Tecnologías</h2>
            <div className="mt-10">
              <div className="grid grid-cols-2 gap-8 md:grid-cols-4">
                {technologies.map((tech, index) => (
                  <div key={index} className="flex flex-col items-center p-6 bg-white rounded-lg shadow-sm hover:shadow-md transition-shadow">
                    <div className="text-amber-700">
                      {tech.icon}
                    </div>
                    <span className="mt-2 text-sm font-medium text-stone-600">{tech.name}</span>
                  </div>
                ))}
              </div>
            </div>
          </div>
        </div>
      </div>

      {/* Instalación Section */}
      <div className="py-16 bg-white">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="lg:text-center">
            <h2 className="text-3xl font-bold text-stone-900">Instalación</h2>
            <div className="mt-6 bg-stone-50 rounded-lg shadow-sm p-6">
              <div className="space-y-4">
                <p className="text-left text-stone-700">Para contribuir al desarrollo del proyecto localmente:</p>
                <div className="bg-stone-800 rounded-lg p-4">
                  <code className="text-sm text-stone-100">
                    git clone https://github.com/tu-usuario/idachi-elite-fashion.git
                  </code>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      {/* Features Section */}
      <div className="py-16 bg-amber-50">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div className="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <ShoppingBag className="h-8 w-8 text-amber-700 mb-4" />
              <h3 className="text-lg font-semibold text-stone-900">Marcas Premium</h3>
              <p className="mt-2 text-stone-600">Seleccionaremos exclusivamente las mejores marcas estadounidenses.</p>
            </div>
            <div className="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <Heart className="h-8 w-8 text-amber-700 mb-4" />
              <h3 className="text-lg font-semibold text-stone-900">Calidad Garantizada</h3>
              <p className="mt-2 text-stone-600">Cada prenda será cuidadosamente seleccionada para ti.</p>
            </div>
            <div className="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <Terminal className="h-8 w-8 text-amber-700 mb-4" />
              <h3 className="text-lg font-semibold text-stone-900">Experiencia Única</h3>
              <p className="mt-2 text-stone-600">Brindaremos una experiencia de compra fácil y segura con atención personalizada.</p>
            </div>
          </div>
        </div>
      </div>

      {/* Footer */}
      <footer className="bg-stone-800 text-stone-200">
        <div className="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:px-8">
          <div className="flex justify-center space-x-6">
            <a href="https://github.com/tu-usuario/idachi-elite-fashion" className="text-stone-400 hover:text-stone-300">
              <Github className="h-6 w-6" />
            </a>
            <ShoppingBag className="h-6 w-6 text-amber-500" />
          </div>
          <div className="mt-8 text-center text-stone-400 text-sm">
            &copy; {new Date().getFullYear()} Idachi Elite Fashion. Todos los derechos reservados.
          </div>
        </div>
      </footer>
    </div>
  );
};

export default LandingPage;
