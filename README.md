import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Input } from "@/components/ui/input"; import { motion } from "framer-motion"; import { Gift, Star, Trophy, Send } from "lucide-react";

export default function ApostaDeOuro() { return ( <div className="min-h-screen bg-gradient-to-br from-yellow-100 to-yellow-300 flex flex-col items-center p-6"> {/* Header */} <header className="text-center mb-8"> <h1 className="text-4xl font-extrabold text-yellow-800 drop-shadow-md"> Aposta de Ouro ✨ </h1> <p className="text-lg text-yellow-700 mt-2"> Onde os teus sonhos se transformam em vitórias! </p> </header>

{/* Main Promo Section */}
  <motion.div
    initial={{ opacity: 0, y: 30 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ duration: 0.7 }}
    className="w-full max-w-2xl"
  >
    <Card className="rounded-2xl shadow-lg bg-white/90">
      <CardContent className="p-6 text-center">
        <h2 className="text-2xl font-bold text-yellow-800 mb-4">
          🎁 Presentes Incríveis Esperam por Ti!
        </h2>
        <p className="text-yellow-700 mb-4">
          Cria já a tua conta, usa o código promocional
          <span className="font-bold"> AO763176 </span>
          e recebe bónus e prémios exclusivos que vão turbinar as tuas apostas.
        </p>
        <a
          href="https://media.premierbetpartners.com/redirect.aspx?pid=128852&bid=5022"
          target="_blank"
          rel="noopener noreferrer"
        >
          <Button className="bg-yellow-600 hover:bg-yellow-700 text-white text-lg px-6 py-3 rounded-xl">
            Criar Conta Agora 🚀
          </Button>
        </a>
      </CardContent>
    </Card>
  </motion.div>

  {/* Bonus Highlights */}
  <div className="grid grid-cols-1 md:grid-cols-3 gap-6 mt-10 max-w-4xl w-full">
    <motion.div
      whileHover={{ scale: 1.05 }}
      className="bg-white rounded-2xl shadow-md p-6 flex flex-col items-center"
    >
      <Gift className="text-yellow-600 w-10 h-10 mb-3" />
      <h3 className="font-bold text-yellow-800">Carregamento Especial</h3>
      <p className="text-sm text-yellow-700 text-center">
        No teu primeiro carregamento de 2000 Kz recebes 6000 Kz para jogar!
      </p>
    </motion.div>

    <motion.div
      whileHover={{ scale: 1.05 }}
      className="bg-white rounded-2xl shadow-md p-6 flex flex-col items-center"
    >
      <Star className="text-yellow-600 w-10 h-10 mb-3" />
      <h3 className="font-bold text-yellow-800">+50 Giros Grátis</h3>
      <p className="text-sm text-yellow-700 text-center">
        Diverte-te e aumenta as tuas chances de ganhar com giros de presente.
      </p>
    </motion.div>

    <motion.div
      whileHover={{ scale: 1.05 }}
      className="bg-white rounded-2xl shadow-md p-6 flex flex-col items-center"
    >
      <Trophy className="text-yellow-600 w-10 h-10 mb-3" />
      <h3 className="font-bold text-yellow-800">+60 Voos Grátis</h3>
      <p className="text-sm text-yellow-700 text-center">
        Ganhas ainda 60 voos grátis para elevar a tua experiência ao próximo nível.
      </p>
    </motion.div>
  </div>

  {/* Lead Capture Form */}
  <motion.div
    initial={{ opacity: 0, y: 20 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ duration: 0.7 }}
    className="mt-12 w-full max-w-lg"
  >
    <Card className="rounded-2xl shadow-lg bg-white/95">
      <CardContent className="p-6 text-center">
        <h3 className="text-xl font-bold text-yellow-800 mb-3">
          🔔 Mantém-te atualizado com as melhores promoções!
        </h3>
        <p className="text-yellow-700 mb-4">
          Deixa o teu e-mail ou WhatsApp e recebe todas as novidades diretamente.
        </p>
        <form
          action="https://formspree.io/f/xyzabcd" // substitui pelo teu endpoint real do Formspree
          method="POST"
          className="flex flex-col md:flex-row items-center gap-3"
        >
          <Input
            type="text"
            name="contact"
            placeholder="O teu e-mail ou WhatsApp"
            className="flex-1 rounded-xl border-yellow-400"
            required
          />
          <Button
            type="submit"
            className="bg-yellow-600 hover:bg-yellow-700 text-white flex items-center gap-2 rounded-xl px-5 py-2"
          >
            <Send className="w-4 h-4" /> Enviar
          </Button>
        </form>
      </CardContent>
    </Card>
  </motion.div>

  {/* Footer */}
  <footer className="mt-12 text-center text-yellow-800 text-sm">
    © 2025 Aposta de Ouro – Todos os direitos reservados.
  </footer>
</div>

); }

