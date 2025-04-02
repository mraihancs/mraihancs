import React from "react";
import { motion } from "framer-motion";
import { FaGithub, FaLinkedin, FaEnvelope } from "react-icons/fa";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-900 text-white flex flex-col items-center justify-center p-6">
      <motion.h1
        className="text-5xl font-bold"
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1 }}
      >
        Hi, I'm <span className="text-blue-400">Maruf Raihan</span>
      </motion.h1>
      
      <motion.p
        className="mt-4 text-lg text-gray-400"
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5, duration: 1 }}
      >
        A passionate developer crafting beautiful web experiences.
      </motion.p>

      <motion.div
        className="flex space-x-4 mt-6"
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 1, duration: 1 }}
      >
        <a href="https://github.com/yourgithub" target="_blank" rel="noopener noreferrer">
          <FaGithub className="text-3xl hover:text-blue-400 transition duration-300" />
        </a>
        <a href="https://linkedin.com/in/yourlinkedin" target="_blank" rel="noopener noreferrer">
          <FaLinkedin className="text-3xl hover:text-blue-400 transition duration-300" />
        </a>
        <a href="mailto:youremail@example.com">
          <FaEnvelope className="text-3xl hover:text-blue-400 transition duration-300" />
        </a>
      </motion.div>

      <motion.a
        href="#projects"
        className="mt-6 px-6 py-3 bg-blue-500 rounded-lg text-lg font-semibold hover:bg-blue-600 transition duration-300"
        initial={{ scale: 0.9 }}
        animate={{ scale: 1 }}
        transition={{ delay: 1.2, duration: 0.5 }}
      >
        View My Work
      </motion.a>
    </div>
  );
}

