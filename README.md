import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Github, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-900 text-white p-10">
      <div className="max-w-4xl mx-auto text-center">
        <h1 className="text-4xl font-bold mb-4">Valentin Tran</h1>
        <p className="text-lg text-gray-400 mb-6">
          Data Analyst passionné par les jeux vidéo et la data science
        </p>
        <div className="flex justify-center space-x-4 mb-6">
          <Button variant="outline">
            <a href="https://github.com/ValentinTran" target="_blank" rel="noopener noreferrer">
              <Github className="mr-2" /> GitHub
            </a>
          </Button>
          <Button variant="outline">
            <a href="https://www.linkedin.com/in/valentin-tran" target="_blank" rel="noopener noreferrer">
              <Linkedin className="mr-2" /> LinkedIn
            </a>
          </Button>
        </div>
        <h2 className="text-2xl font-semibold mb-4">Expériences</h2>
        <Card className="bg-gray-800 p-4 mb-4">
          <CardContent>
            <h3 className="text-xl font-medium">Data Analyst - GRDF</h3>
            <p className="text-gray-400 text-sm">Mai 2023 - Septembre 2024</p>
            <p className="text-gray-300 mt-2">
              Création de tableaux de bord avec Tableau et MicroStrategy, développement d'une application mobile low-code, analyse et traitement de données sur Dataiku.
            </p>
          </CardContent>
        </Card>
        <Card className="bg-gray-800 p-4 mb-4">
          <CardContent>
            <h3 className="text-xl font-medium">Stage BI - Sisley Paris</h3>
            <p className="text-gray-400 text-sm">Janvier 2023 - Mai 2023</p>
            <p className="text-gray-300 mt-2">
              Développement d'un script Python de recommandation de produits cosmétiques, création de tableaux de bord sur Tableau.
            </p>
          </CardContent>
        </Card>
        <h2 className="text-2xl font-semibold mt-6 mb-4">Compétences</h2>
        <div className="grid grid-cols-2 md:grid-cols-3 gap-4">
          <span className="bg-gray-700 px-4 py-2 rounded">Python</span>
          <span className="bg-gray-700 px-4 py-2 rounded">SQL</span>
          <span className="bg-gray-700 px-4 py-2 rounded">Tableau</span>
          <span className="bg-gray-700 px-4 py-2 rounded">Power BI</span>
          <span className="bg-gray-700 px-4 py-2 rounded">Dataiku</span>
          <span className="bg-gray-700 px-4 py-2 rounded">MicroStrategy</span>
        </div>
      </div>
    </div>
  );
}
