"use client";
import { useState } from "react";

export default function Home() {
  const [form, setForm] = useState({ name: "", message: "" });

  const handleSend = (e) => {
    e.preventDefault();
    const msg = `Namaste Sir, Mai ${form.name} bol raha hu. ${form.message} - Education Branch`;
    window.open(`https://wa.me/916200646899?text=${encodeURIComponent(msg)}`, "_blank");
  };

  return (
    <main className="min-h-screen bg-gray-50">
      <header className="bg-blue-800 text-white p-4 text-center">
        <h1 className="text-3xl font-bold">Education Branch</h1>
        <p className="text-blue-200">BY Aftab Alam - बिहार शिक्षा की आवाज</p>
      </header>

      <div className="bg-yellow-400 text-center py-2 text-sm font-bold animate-pulse">
        🔔 बिहार Latest: BSEB 10th/12th Result 2026 | OFSS Admission | Bihar Scholarship | Free Notes
      </div>

      <section className="max-w-6xl mx-auto p-6">
        <h2 className="text-2xl font-bold text-center mb-6">बिहार के सभी शिक्षा अपडेट</h2>
        
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          {/* BSEB */}
          <div className="bg-white rounded-xl shadow p-5 border-l-4 border-blue-700">
            <h3 className="font-bold text-blue-800">📚 बिहार बोर्ड (BSEB)</h3>
            <ul className="text-sm mt-3 space-y-2 text-gray-700">
              <li>• 10th Result 2026</li>
              <li>• 12th Result 2026 - Arts, Science, Commerce</li>
              <li>• Matric / Inter Admit Card</li>
              <li>• Model Paper & Time Table</li>
              <li>• OFSS 11th Admission 2026</li>
            </ul>
          </div>

          {/* University */}
          <div className="bg-white rounded-xl shadow p-5 border-l-4 border-green-600">
            <h3 className="font-bold text-green-800">🎓 बिहार यूनिवर्सिटी</h3>
            <ul className="text-sm mt-3 space-y-2 text-gray-700">
              <li>• Patna University Result</li>
              <li>• LNMU, PPU, BNMU, Munger University</li>
              <li>• Magadh, BRA Bihar University</li>
              <li>• Part 1, 2, 3 Result & Admission</li>
              <li>• B.Ed, D.El.Ed Updates</li>
            </ul>
          </div>

          {/* Scholarship & Jobs */}
          <div className="bg-white rounded-xl shadow p-5 border-l-4 border-red-600">
            <h3 className="font-bold text-red-800">💰 स्कॉलरशिप और योजना</h3>
            <ul className="text-sm mt-3 space-y-2 text-gray-700">
              <li>• Bihar Post Matric Scholarship</li>
              <li>• Kanya Utthan Yojana</li>
              <li>• Medhasoft Scholarship</li>
              <li>• Bihar Student Credit Card</li>
              <li>• रोजगार समाचार</li>
            </ul>
          </div>
        </div>

        {/* Notes Section */}
        <div className="mt-8 bg-white rounded-xl shadow p-6">
          <h3 className="font-bold text-xl text-center">📝 बिहार बोर्ड के फ्री नोट्स</h3>
          <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mt-4 text-sm text-center">
            <div className="bg-blue-50 p-3 rounded-lg">Class 9-10 Notes</div>
            <div className="bg-green-50 p-3 rounded-lg">Class 11-12 Notes</div>
            <div className="bg-yellow-50 p-3 rounded-lg">GK / GS PDF</div>
            <div className="bg-purple-50 p-3 rounded-lg">Previous Year Papers</div>
          </div>
        </div>

        {/* Contact Form */}
        <div className="mt-8 grid md:grid-cols-2 gap-6">
          <div className="bg-blue-900 text-white p-6 rounded-xl">
            <h3 className="text-xl font-bold">संपर्क करें</h3>
            <p className="mt-2">Education Branch BY Aftab Alam</p>
            <p className="mt-4 text-2xl font
