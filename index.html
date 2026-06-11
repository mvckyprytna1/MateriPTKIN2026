import React, { useState, useEffect, useMemo } from 'react';
import { motion, AnimatePresence } from 'framer-motion';
import { 
  BookOpen, Search, Moon, Sun, ChevronRight, Bookmark, BookmarkCheck, 
  CheckSquare, Square, Maximize, Minimize, ArrowLeft, Clock, Target, 
  AlertTriangle, Lightbulb, Zap, CheckCircle2, Menu, X, Rocket
} from 'lucide-react';

// --- DATA MATERI (Diekstrak dari PDF TOP MASTER UMPTKIN) ---
const MATERIALS = [
  {
    id: "al-quran-hadits",
    title: "Al-Qur'an dan Hadits",
    description: "Pemahaman dasar tentang Al-Qur'an, definisi, nama-nama, dan kemu'jizatan Al-Qur'an.",
    readTime: "15 menit",
    category: "Keislaman",
    chapters: [
      {
        id: "pengertian",
        title: "Pengertian Al-Qur'an",
        content: "Secara etimologi, para ulama berbeda pendapat. Menurut Al-Lihyany, berasal dari kata qara'a (membaca). Menurut Al-Asy'ari, dari lafaz qarna (menggabungkan). Secara terminologi (Subkhi Shalih): Al-Qur'an adalah kitab Allah yang mengandung mu'jizat, diturunkan kepada Nabi Muhammad SAW, ditulis dalam mushaf, disampaikan secara mutawatir, dan bernilai ibadah membacanya.",
        keyPoints: [
          "Al-Qur'an adalah kalam Allah SWT yang diturunkan kepada Nabi Muhammad SAW.",
          "Disampaikan secara mutawatir (berkesinambungan).",
          "Membacanya bernilai ibadah."
        ],
        mustRemember: [
          "Al-Lihyany: Qara'a (Membaca)",
          "Al-Asy'ari: Qarna (Menggabungkan)",
          "Al-Farra: Qara'in (Petunjuk/Indikator)",
          "Az-Zujaj: Al-Qar'u (Kumpulan)"
        ],
        traps: [
          "Jangan tertukar antara pendapat Al-Asy'ari (Qarna) dan Al-Farra (Qara'in). Soal sering menjebak di dua nama ini."
        ],
        examples: [
          {
            question: "Menurut Asy-Syafi'i, kata Al-Qur'an berasal dari...",
            answer: "Isim 'alam (nama khusus), bukan kata bentukan (isytiqaaq) dari kata apapun.",
            explanation: "Asy-Syafi'i berpendapat Al-Qur'an sudah menjadi nama khusus sejak awal, seperti Taurat dan Injil."
          }
        ]
      },
      {
        id: "nama-nama",
        title: "Nama-nama Al-Qur'an",
        content: "Menurut Az-Zarkasyi dan As-Suyuthi dalam kitab Al-Itqan, Al-Qur'an memiliki 55 nama. Namun secara redaksional yang paling populer adalah: Al-Qur'an (Bacaan), Al-Kitab (Yang ditulis), Al-Furqan (Pembeda hak & batil), Az-Zikr (Pemberi peringatan), dan At-Tanzil (Yang diturunkan).",
        keyPoints: [
          "Al-Furqan berarti pembeda antara yang haq dan yang batil.",
          "Az-Zikr berarti pemberi peringatan kepada manusia."
        ],
        mustRemember: [],
        traps: [],
        examples: []
      },
      {
        id: "mukjizat",
        title: "Kemu'jizatan Al-Qur'an (I'jazul Qur'an)",
        content: "Mu'jizat bertujuan melemahkan lawan. Syarat mu'jizat: tidak sanggup dilakukan selain Allah, menyalahi kebiasaan, dijadikan saksi kenabian, dan tak ada yang bisa menandingi. Kemu'jizatan Al-Qur'an meliputi gaya bahasa (uslub) yang indah, keseimbangan kata (contoh: kata Hayat dan Maut sama-sama disebut 145 kali), serta misteri angka 19 (Bismillahirrahmanirrahim terdiri dari 19 huruf).",
        keyPoints: [
          "Mu'jizat Hissi: Dapat ditangkap panca indera (Zaman Nabi Musa, Nabi Isa).",
          "Mu'jizat Ma'nawi: Dicapai dengan akal/rasional, bersifat universal dan abadi (Al-Qur'an)."
        ],
        mustRemember: [
          "Kata Hayat dan Maut = 145 kali.",
          "Kata Dunya dan Akhirat = 115 kali.",
          "Kata Malaikat dan Syetan = 88 kali."
        ],
        traps: [
          "Al-Qur'an adalah Mu'jizat Ma'nawi (rasional), BUKAN Hissi (inderawi)."
        ],
        examples: []
      }
    ]
  },
  {
    id: "fiqih-pembunuhan",
    title: "Fiqih: Pembunuhan & Qishash",
    description: "Materi tentang jenis pembunuhan, hukum qishash, dan khilafah dalam Islam.",
    readTime: "12 menit",
    category: "Keislaman",
    chapters: [
      {
        id: "pembunuhan",
        title: "Macam-macam Pembunuhan",
        content: "Pembunuhan adalah melenyapkan nyawa seseorang sehingga menjadi mati. Terbagi menjadi tiga: Pembunuhan Sengaja (Qatlul 'Amd), Pembunuhan Seperti Sengaja (Qatlul Syibhul 'Amd), dan Pembunuhan Tidak Sengaja (Qatlul Khata').",
        keyPoints: [
          "Sengaja: Menggunakan alat yang lazim untuk membunuh dan terencana.",
          "Seperti Sengaja: Menggunakan alat yang tidak lazim mematikan, tapi korban mati.",
          "Tidak Sengaja: Sama sekali tidak ada niat membunuh (misal: peluru nyasar)."
        ],
        mustRemember: [
          "Qatlul 'Amd = Sengaja",
          "Qatlul Syibhul 'Amd = Seperti Sengaja",
          "Qatlul Khata' = Tidak Sengaja"
        ],
        traps: [
          "Pahami perbedaan 'seperti sengaja' dan 'tidak sengaja'. Memukul orang dengan lidi lalu orangnya mati = Seperti Sengaja (karena ada niat memukul, tapi bukan niat membunuh)."
        ],
        examples: []
      },
      {
        id: "qishash",
        title: "Qishash",
        content: "Qishash adalah hukuman balasan yang seimbang bagi pelaku pembunuhan maupun pengrusakan anggota badan. Syarat qishash: Pembunuh baligh & berakal, bukan orang tua yang dibunuh, pembunuhan sengaja, derajat sama (merdeka dengan merdeka), dan dilakukan pada anggota tubuh yang sama.",
        keyPoints: [
          "Tujuan qishash adalah memberikan pelajaran, melindungi jiwa, dan memelihara ketertiban."
        ],
        mustRemember: [
          "Pembunuh BUKAN orang tua dari yang dibunuh (Orang tua tidak diqishash karena membunuh anaknya, hukumannya ta'zir/diyat)."
        ],
        traps: [],
        examples: []
      }
    ]
  },
  {
    id: "tpa-logika",
    title: "TPA: Logika & Analitis",
    description: "Strategi mengerjakan soal Tes Potensi Akademik (TPA) Logika Silogisme dan Analitis.",
    readTime: "10 menit",
    category: "Tes Potensi Akademik",
    chapters: [
      {
        id: "silogisme",
        title: "Logika Silogisme",
        content: "Soal silogisme meminta kita menganalisa apakah kesimpulan dari dua premis sudah benar. Ingat aturan dasar: Jika Premis Umum (Semua) dan Premis Khusus (Sebagian), maka kesimpulannya pasti KHUSUS (Sebagian). Jika salah satu premis negatif (Tidak/Bukan), maka kesimpulan WAJIB negatif.",
        keyPoints: [
          "Semua A adalah B. Sebagian A adalah C. -> Sebagian C adalah B.",
          "Semua mahasiswa berjas almamater. Andi mahasiswa. -> Andi berjas almamater."
        ],
        mustRemember: [
          "Semua + Sebagian = Sebagian",
          "Positif + Negatif = Negatif"
        ],
        traps: [
          "Hati-hati dengan kata 'mungkin'. Kesimpulan logika harus PASTI, bukan kemungkinan (kecuali premisnya menyatakan kemungkinan)."
        ],
        examples: [
          {
            question: "Semua mamalia bernapas dengan paru-paru. Ikan paus adalah mamalia.",
            answer: "Ikan paus bernapas dengan paru-paru.",
            explanation: "Paus masuk dalam himpunan mamalia, maka ia mewarisi sifat himpunan mamalia."
          }
        ]
      }
    ]
  },
  {
    id: "bahasa-inggris-tenses",
    title: "B. Inggris: Tenses & Grammar",
    description: "Rangkuman Grammar dasar yang sering keluar di soal Bahasa Inggris UM-PTKIN.",
    readTime: "10 menit",
    category: "Bahasa",
    chapters: [
      {
        id: "tenses-dasar",
        title: "Tenses Sering Keluar",
        content: "Fokus pada tenses yang menunjukan urutan kejadian (Past Perfect vs Simple Past) dan pengandaian (Conditional Sentences). Past Perfect (Had + V3) terjadi LEBIH DULU sebelum Simple Past (V2) terjadi.",
        keyPoints: [
          "Present Perfect: S + Have/Has + V3 (Kejadian sudah selesai, efeknya masih ada).",
          "Past Perfect: S + Had + V3 (Kejadian yang sudah selesai SEBELUM kejadian lain di masa lalu)."
        ],
        mustRemember: [
          "Type 1: If + Present, Will + V1",
          "Type 2: If + V2 (Past), Would + V1",
          "Type 3: If + Had V3, Would have + V3"
        ],
        traps: [
          "Dalam Conditional Type 2, to-be untuk semua subject adalah WERE. Contoh: If I WERE you (Bukan If I was you)."
        ],
        examples: [
          {
            question: "When he came last night, the drink ___ run out.",
            answer: "had",
            explanation: "Minuman habis lebih dulu (Past Perfect) sebelum dia datang (Simple Past)."
          }
        ]
      }
    ]
  }
];

const EXAM_PREP_TIPS = [
  {
    title: "20 Poin Super Wajib Hafal",
    items: [
      "I'jazul Qur'an Ma'nawi = Rasional/Akal (berlaku abadi).",
      "Qatlul 'Amd = Pembunuhan Sengaja.",
      "Mubdal Minhu = Kata yang dijelaskan oleh Badal (B. Arab).",
      "Conditional Type 2 selalu pakai to-be 'WERE'.",
      "Asimilasi = Peleburan budaya baru, budaya lama HILANG.",
      "Akulturasi = Percampuran budaya baru, budaya lama TETAP ADA.",
      "Mobilitas Vertikal Naik = Social Climbing.",
      "Lembaga Crescive = Lembaga yang tumbuh tak sengaja dari adat.",
      "Zaman Neozoikum (Tersier & Kuarter) = Mulai ada manusia (Holosen).",
      "Pithecanthropus Erectus = Manusia Kera Berjalan Tegak (E. Dubois).",
      "VOC berdiri tahun 1602 (Gubjen pertama: Pieter Both).",
      "Inflasi Demand Pull = Inflasi tarikan permintaan.",
      "GNP (Kotor) dikurangi Penyusutan = NNP.",
      "Vektor Skalar = Punya nilai saja (Massa, Panjang, Waktu).",
      "Virus = Bersifat aseluler, parasit obligat, punya DNA atau RNA saja.",
      "Siklus Litik = Menghancurkan sel inang.",
      "Siklus Lisogenik = DNA Virus menempel (profage) tanpa langsung memecah inang.",
      "Ikatan Kovalen = Penggunaan bersama pasangan elektron (Nonlogam + Nonlogam).",
      "Ikatan Ion = Serah terima elektron (Logam + Nonlogam).",
      "D(Determinan) > 0 = Memotong di dua titik berbeda."
    ]
  },
  {
    title: "Istilah Sering Tertukar",
    items: [
      "Asimilasi (Budaya lama hilang) VS Akulturasi (Budaya lama dipertahankan).",
      "Imitasi (Meniru sebagian) VS Identifikasi (Meniru persis/keseluruhan).",
      "Siklus Litik (Inang mati) VS Siklus Lisogenik (Inang tetap hidup bawa DNA virus).",
      "Gaya Sentripetal (Ke arah pusat) VS Gaya Sentrifugal (Menjauhi pusat)."
    ]
  },
  {
    title: "Tips Jawab Ganda",
    items: [
      "TPA Logika: Abaikan realita, fokus hanya pada aturan premis di soal.",
      "B. Inggris Reading: Baca pertanyaan dulu (Scanning), lalu cari keyword di teks.",
      "Pilih jawaban yang ekstrim panjang atau ekstrim pendek jika benar-benar buntu (Pola pembuat soal).",
      "Eliminasi 2 pilihan yang maknanya bersinonim, karena tidak mungkin keduanya benar."
    ]
  }
];

// --- COMPONENTS ---

// 1. Highlight Boxes
const HighlightBox = ({ type, title, children }) => {
  const configs = {
    wajib: {
      color: "bg-emerald-50 dark:bg-emerald-900/30 border-emerald-500 text-emerald-800 dark:text-emerald-200",
      icon: <Zap className="w-5 h-5 text-emerald-500 mt-0.5" />
    },
    jebakan: {
      color: "bg-rose-50 dark:bg-rose-900/30 border-rose-500 text-rose-800 dark:text-rose-200",
      icon: <AlertTriangle className="w-5 h-5 text-rose-500 mt-0.5" />
    },
    contoh: {
      color: "bg-blue-50 dark:bg-blue-900/30 border-blue-500 text-blue-800 dark:text-blue-200",
      icon: <Lightbulb className="w-5 h-5 text-blue-500 mt-0.5" />
    },
    poin: {
      color: "bg-indigo-50 dark:bg-indigo-900/30 border-indigo-500 text-indigo-800 dark:text-indigo-200",
      icon: <Target className="w-5 h-5 text-indigo-500 mt-0.5" />
    }
  };

  const config = configs[type] || configs.poin;

  return (
    <div className={`p-4 my-4 rounded-xl border-l-4 flex gap-3 shadow-sm ${config.color}`}>
      <div>{config.icon}</div>
      <div className="flex-1">
        {title && <h4 className="font-bold mb-1">{title}</h4>}
        <div className="text-sm space-y-2">{children}</div>
      </div>
    </div>
  );
};

// 2. Material Reader View
const MaterialReaderView = ({ material, onBack, isDarkMode }) => {
  const [activeChapter, setActiveChapter] = useState(material.chapters[0]?.id);
  const [isFocusMode, setIsFocusMode] = useState(false);
  const [scrollProgress, setScrollProgress] = useState(0);
  const [isSidebarOpen, setIsSidebarOpen] = useState(false);
  
  // Bookmarks Logic
  const [bookmarks, setBookmarks] = useState(() => {
    return JSON.parse(localStorage.getItem('umptkin_bookmarks') || '[]');
  });

  const toggleBookmark = () => {
    const newBookmarks = bookmarks.includes(material.id)
      ? bookmarks.filter(id => id !== material.id)
      : [...bookmarks, material.id];
    setBookmarks(newBookmarks);
    localStorage.setItem('umptkin_bookmarks', JSON.stringify(newBookmarks));
  };

  // Scroll Progress
  useEffect(() => {
    const handleScroll = () => {
      const totalScroll = document.documentElement.scrollTop;
      const windowHeight = document.documentElement.scrollHeight - document.documentElement.clientHeight;
      const scroll = `${totalScroll / windowHeight}`;
      setScrollProgress(Number(scroll));
    }
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  return (
    <div className="min-h-screen bg-slate-50 dark:bg-slate-950 text-slate-800 dark:text-slate-200 transition-colors duration-300">
      {/* Top Navbar */}
      <nav className="fixed top-0 left-0 right-0 h-16 bg-white/80 dark:bg-slate-900/80 backdrop-blur-md border-b border-slate-200 dark:border-slate-800 flex items-center justify-between px-4 z-50">
        <div className="flex items-center gap-3">
          <button onClick={onBack} className="p-2 hover:bg-slate-100 dark:hover:bg-slate-800 rounded-full transition">
            <ArrowLeft className="w-5 h-5" />
          </button>
          <h1 className="font-bold text-lg hidden sm:block truncate max-w-xs">{material.title}</h1>
          <button 
            className="sm:hidden p-2 hover:bg-slate-100 dark:hover:bg-slate-800 rounded-full"
            onClick={() => setIsSidebarOpen(!isSidebarOpen)}
          >
            <Menu className="w-5 h-5" />
          </button>
        </div>
        
        <div className="flex items-center gap-2">
          <button onClick={toggleBookmark} className="p-2 hover:bg-slate-100 dark:hover:bg-slate-800 rounded-full transition" title="Bookmark">
            {bookmarks.includes(material.id) ? <BookmarkCheck className="w-5 h-5 text-indigo-600" /> : <Bookmark className="w-5 h-5" />}
          </button>
          <button 
            onClick={() => setIsFocusMode(!isFocusMode)} 
            className={`p-2 rounded-full transition ${isFocusMode ? 'bg-indigo-100 text-indigo-600 dark:bg-indigo-900 dark:text-indigo-400' : 'hover:bg-slate-100 dark:hover:bg-slate-800'}`}
            title="Focus Mode"
          >
            {isFocusMode ? <Minimize className="w-5 h-5" /> : <Maximize className="w-5 h-5" />}
          </button>
        </div>
      </nav>

      {/* Progress Bar */}
      <div className="fixed top-16 left-0 right-0 h-1 bg-slate-200 dark:bg-slate-800 z-50">
        <div className="h-full bg-indigo-600 transition-all duration-150" style={{ width: `${scrollProgress * 100}%` }}></div>
      </div>

      <div className="pt-20 pb-24 px-4 max-w-7xl mx-auto flex gap-8">
        {/* Sidebar TOC */}
        <AnimatePresence>
          {(!isFocusMode || isSidebarOpen) && (
            <motion.aside 
              initial={{ x: -300, opacity: 0 }}
              animate={{ x: 0, opacity: 1 }}
              exit={{ x: -300, opacity: 0 }}
              className={`fixed sm:sticky top-24 left-0 h-[calc(100vh-8rem)] w-64 bg-white dark:bg-slate-900 sm:bg-transparent rounded-xl p-4 overflow-y-auto z-40 shadow-xl sm:shadow-none transition-transform ${isSidebarOpen ? 'translate-x-0' : '-translate-x-full sm:translate-x-0'}`}
            >
              <div className="flex justify-between items-center mb-6 sm:hidden">
                <h3 className="font-bold text-slate-500 uppercase text-xs">Daftar Isi</h3>
                <button onClick={() => setIsSidebarOpen(false)}><X className="w-5 h-5"/></button>
              </div>
              <h3 className="font-bold text-slate-500 dark:text-slate-400 uppercase text-xs tracking-wider mb-4 hidden sm:block">Daftar Isi</h3>
              <ul className="space-y-2">
                {material.chapters.map((chap) => (
                  <li key={chap.id}>
                    <button 
                      onClick={() => {
                        setActiveChapter(chap.id);
                        document.getElementById(`chapter-${chap.id}`)?.scrollIntoView({ behavior: 'smooth', block: 'start' });
                        setIsSidebarOpen(false);
                      }}
                      className={`w-full text-left px-3 py-2 rounded-lg text-sm transition-colors ${activeChapter === chap.id ? 'bg-indigo-50 dark:bg-indigo-900/50 text-indigo-700 dark:text-indigo-300 font-medium' : 'text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800'}`}
                    >
                      {chap.title}
                    </button>
                  </li>
                ))}
              </ul>
            </motion.aside>
          )}
        </AnimatePresence>

        {/* Main Content */}
        <main className={`flex-1 transition-all duration-500 ${isFocusMode ? 'max-w-3xl mx-auto' : 'max-w-4xl'}`}>
          <div className="mb-10 text-center sm:text-left">
            <span className="inline-block px-3 py-1 bg-indigo-100 dark:bg-indigo-900/50 text-indigo-800 dark:text-indigo-200 text-xs font-semibold rounded-full mb-3 uppercase tracking-wide">
              {material.category}
            </span>
            <h1 className="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mb-4 leading-tight">{material.title}</h1>
            <p className="text-slate-600 dark:text-slate-400 text-lg">{material.description}</p>
          </div>

          <div className="space-y-16">
            {material.chapters.map((chap) => (
              <section key={chap.id} id={`chapter-${chap.id}`} className="scroll-mt-24">
                <h2 className="text-2xl font-bold border-b-2 border-slate-200 dark:border-slate-800 pb-2 mb-6 text-slate-800 dark:text-slate-100">{chap.title}</h2>
                <div className="prose dark:prose-invert prose-indigo max-w-none prose-p:leading-relaxed prose-p:text-slate-700 dark:prose-p:text-slate-300">
                  <p>{chap.content}</p>
                </div>

                {chap.keyPoints && chap.keyPoints.length > 0 && (
                  <HighlightBox type="poin" title="Poin Penting">
                    <ul className="list-disc list-inside space-y-1 ml-2">
                      {chap.keyPoints.map((pt, i) => <li key={i}>{pt}</li>)}
                    </ul>
                  </HighlightBox>
                )}

                {chap.mustRemember && chap.mustRemember.length > 0 && (
                  <HighlightBox type="wajib" title="Wajib Hafal 🔥">
                    <ul className="list-disc list-inside space-y-1 ml-2">
                      {chap.mustRemember.map((mr, i) => <li key={i} className="font-medium">{mr}</li>)}
                    </ul>
                  </HighlightBox>
                )}

                {chap.traps && chap.traps.length > 0 && (
                  <HighlightBox type="jebakan" title="Awas Jebakan Soal! ⚠️">
                    <ul className="list-disc list-inside space-y-1 ml-2">
                      {chap.traps.map((tr, i) => <li key={i}>{tr}</li>)}
                    </ul>
                  </HighlightBox>
                )}

                {chap.examples && chap.examples.length > 0 && (
                  <div className="mt-8">
                    <h3 className="text-lg font-bold flex items-center gap-2 mb-4 text-slate-800 dark:text-slate-200"><Lightbulb className="w-5 h-5 text-amber-500" /> Contoh Soal</h3>
                    {chap.examples.map((ex, i) => (
                      <div key={i} className="bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-xl p-5 shadow-sm mb-4">
                        <p className="font-medium text-slate-800 dark:text-slate-200 mb-3">Q: {ex.question}</p>
                        <div className="pl-4 border-l-4 border-amber-400 bg-amber-50 dark:bg-amber-900/10 p-3 rounded-r-lg">
                          <p className="font-bold text-amber-800 dark:text-amber-400 mb-1">Jawaban: {ex.answer}</p>
                          <p className="text-sm text-slate-600 dark:text-slate-400">{ex.explanation}</p>
                        </div>
                      </div>
                    ))}
                  </div>
                )}
              </section>
            ))}
          </div>
          
          <div className="mt-16 pt-8 border-t border-slate-200 dark:border-slate-800 flex justify-between">
            <button className="text-slate-500 hover:text-indigo-600 font-medium transition" onClick={() => window.scrollTo({top: 0, behavior: 'smooth'})}>
              ↑ Kembali ke Atas
            </button>
            <button onClick={onBack} className="bg-indigo-600 hover:bg-indigo-700 text-white px-6 py-2 rounded-full font-medium transition shadow-md hover:shadow-lg flex items-center gap-2">
              Selesai Belajar <CheckCircle2 className="w-4 h-4" />
            </button>
          </div>
        </main>
      </div>
    </div>
  );
};


// 3. Exam Prep View (Mode Ujian Besok)
const ExamPrepView = ({ onBack }) => {
  const [checkedItems, setCheckedItems] = useState(() => {
    return JSON.parse(localStorage.getItem('umptkin_checks') || '[]');
  });

  const toggleCheck = (item) => {
    const newChecks = checkedItems.includes(item)
      ? checkedItems.filter(i => i !== item)
      : [...checkedItems, item];
    setCheckedItems(newChecks);
    localStorage.setItem('umptkin_checks', JSON.stringify(newChecks));
  };

  return (
    <div className="min-h-screen bg-slate-50 dark:bg-slate-950 text-slate-800 dark:text-slate-200 transition-colors py-10 px-4">
      <div className="max-w-4xl mx-auto">
        <button onClick={onBack} className="flex items-center gap-2 text-slate-500 hover:text-indigo-600 font-medium mb-8 transition">
          <ArrowLeft className="w-4 h-4" /> Kembali ke Dashboard
        </button>
        
        <div className="text-center mb-12">
          <div className="inline-flex items-center justify-center p-4 bg-rose-100 dark:bg-rose-900/30 rounded-full mb-4">
            <Rocket className="w-10 h-10 text-rose-600 dark:text-rose-400" />
          </div>
          <h1 className="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mb-4">Mode Ujian Besok</h1>
          <p className="text-lg text-slate-600 dark:text-slate-400 max-w-2xl mx-auto">Baca cepat rangkuman pamungkas ini jika ujianmu tinggal menghitung jam. Checklist setiap poin yang sudah kamu kuasai.</p>
        </div>

        <div className="space-y-10">
          {EXAM_PREP_TIPS.map((section, idx) => (
            <div key={idx} className="bg-white dark:bg-slate-900 rounded-2xl shadow-sm border border-slate-200 dark:border-slate-800 overflow-hidden">
              <div className="bg-slate-100 dark:bg-slate-800/50 px-6 py-4 border-b border-slate-200 dark:border-slate-800">
                <h2 className="text-xl font-bold text-slate-800 dark:text-slate-100">{section.title}</h2>
              </div>
              <ul className="divide-y divide-slate-100 dark:divide-slate-800/50">
                {section.items.map((item, i) => (
                  <li key={i} className="px-6 py-4 hover:bg-slate-50 dark:hover:bg-slate-800/20 transition-colors flex items-start gap-4 cursor-pointer" onClick={() => toggleCheck(item)}>
                    <button className="mt-1 focus:outline-none shrink-0">
                      {checkedItems.includes(item) ? (
                        <CheckSquare className="w-5 h-5 text-emerald-500" />
                      ) : (
                        <Square className="w-5 h-5 text-slate-300 dark:text-slate-600" />
                      )}
                    </button>
                    <span className={`text-base ${checkedItems.includes(item) ? 'text-slate-400 dark:text-slate-500 line-through' : 'text-slate-700 dark:text-slate-300'}`}>
                      {item}
                    </span>
                  </li>
                ))}
              </ul>
            </div>
          ))}
        </div>
      </div>
    </div>
  );
};


// 4. Main App Container
export default function App() {
  const [currentView, setCurrentView] = useState('home'); // 'home', 'reader', 'exam-prep'
  const [activeMaterialId, setActiveMaterialId] = useState(null);
  const [searchQuery, setSearchQuery] = useState('');
  const [isDarkMode, setIsDarkMode] = useState(false);

  // Initialize Theme
  useEffect(() => {
    const savedTheme = localStorage.getItem('theme');
    const prefersDark = window.matchMatchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches;
    if (savedTheme === 'dark' || (!savedTheme && prefersDark)) {
      setIsDarkMode(true);
      document.documentElement.classList.add('dark');
    }
  }, []);

  const toggleTheme = () => {
    setIsDarkMode(!isDarkMode);
    if (!isDarkMode) {
      document.documentElement.classList.add('dark');
      localStorage.setItem('theme', 'dark');
    } else {
      document.documentElement.classList.remove('dark');
      localStorage.setItem('theme', 'light');
    }
  };

  const filteredMaterials = useMemo(() => {
    return MATERIALS.filter(m => 
      m.title.toLowerCase().includes(searchQuery.toLowerCase()) || 
      m.category.toLowerCase().includes(searchQuery.toLowerCase()) ||
      m.description.toLowerCase().includes(searchQuery.toLowerCase())
    );
  }, [searchQuery]);

  const openMaterial = (id) => {
    setActiveMaterialId(id);
    setCurrentView('reader');
    window.scrollTo(0,0);
  };

  // Route Handling
  if (currentView === 'reader') {
    const material = MATERIALS.find(m => m.id === activeMaterialId);
    return <MaterialReaderView material={material} onBack={() => setCurrentView('home')} isDarkMode={isDarkMode} />;
  }

  if (currentView === 'exam-prep') {
    return <ExamPrepView onBack={() => setCurrentView('home')} />;
  }

  return (
    <div className="min-h-screen bg-slate-50 dark:bg-slate-950 text-slate-800 dark:text-slate-200 transition-colors duration-300 font-sans">
      
      {/* NAVBAR */}
      <nav className="sticky top-0 z-50 bg-white/80 dark:bg-slate-900/80 backdrop-blur-lg border-b border-slate-200 dark:border-slate-800 px-4 py-3 sm:px-6 lg:px-8">
        <div className="max-w-7xl mx-auto flex justify-between items-center">
          <div className="flex items-center gap-2">
            <div className="bg-indigo-600 text-white p-2 rounded-lg">
              <BookOpen className="w-5 h-5" />
            </div>
            <span className="font-extrabold text-xl tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-indigo-600 to-emerald-500">MateriPTKIN</span>
          </div>
          <button onClick={toggleTheme} className="p-2 rounded-full hover:bg-slate-100 dark:hover:bg-slate-800 transition-colors">
            {isDarkMode ? <Sun className="w-5 h-5 text-amber-400" /> : <Moon className="w-5 h-5 text-slate-600" />}
          </button>
        </div>
      </nav>

      <main className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10">
        
        {/* HERO SECTION */}
        <section className="text-center py-12 md:py-20">
          <motion.h1 
            initial={{ opacity: 0, y: 20 }} animate={{ opacity: 1, y: 0 }}
            className="text-4xl md:text-5xl lg:text-6xl font-extrabold text-slate-900 dark:text-white tracking-tight mb-6"
          >
            Belajar Rapi, Cepat, & Fokus <br className="hidden md:block"/> Hadapi <span className="text-indigo-600 dark:text-indigo-400">UM-PTKIN 2026</span>
          </motion.h1>
          <motion.p 
            initial={{ opacity: 0, y: 20 }} animate={{ opacity: 1, y: 0 }} transition={{ delay: 0.1 }}
            className="text-lg md:text-xl text-slate-600 dark:text-slate-400 mb-10 max-w-2xl mx-auto"
          >
            Materi premium yang disusun dari e-book TOP MASTER UMPTKIN. Dirancang untuk kenyamanan membaca di HP & Laptop tanpa gangguan.
          </motion.p>

          <motion.div 
            initial={{ opacity: 0, y: 20 }} animate={{ opacity: 1, y: 0 }} transition={{ delay: 0.2 }}
            className="flex flex-col sm:flex-row gap-4 justify-center"
          >
            <button 
              onClick={() => {
                document.getElementById('materi-section').scrollIntoView({ behavior: 'smooth' });
              }}
              className="bg-indigo-600 hover:bg-indigo-700 text-white px-8 py-3.5 rounded-full font-bold text-lg transition-all shadow-lg hover:shadow-indigo-500/30 flex items-center justify-center gap-2"
            >
              Mulai Belajar <ChevronRight className="w-5 h-5" />
            </button>
            <button 
              onClick={() => { setCurrentView('exam-prep'); window.scrollTo(0,0); }}
              className="bg-rose-100 hover:bg-rose-200 dark:bg-rose-900/30 dark:hover:bg-rose-900/50 text-rose-700 dark:text-rose-400 border border-rose-200 dark:border-rose-800 px-8 py-3.5 rounded-full font-bold text-lg transition-all flex items-center justify-center gap-2"
            >
              <Rocket className="w-5 h-5" /> Mode Ujian Besok
            </button>
          </motion.div>
        </section>

        {/* SEARCH BAR */}
        <section id="materi-section" className="mb-12 max-w-2xl mx-auto scroll-mt-24">
          <div className="relative group">
            <div className="absolute inset-y-0 left-0 pl-4 flex items-center pointer-events-none">
              <Search className="h-5 w-5 text-slate-400 group-focus-within:text-indigo-500 transition-colors" />
            </div>
            <input
              type="text"
              className="block w-full pl-11 pr-4 py-4 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-2xl text-slate-900 dark:text-slate-100 placeholder-slate-400 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:border-transparent transition-shadow shadow-sm text-lg"
              placeholder="Cari materi (contoh: Silogisme, Fiqih, Tenses...)"
              value={searchQuery}
              onChange={(e) => setSearchQuery(e.target.value)}
            />
          </div>
        </section>

        {/* MATERIAL CARDS */}
        <section>
          {filteredMaterials.length === 0 ? (
            <div className="text-center py-20">
              <div className="inline-block p-4 bg-slate-100 dark:bg-slate-800 rounded-full mb-4">
                <Search className="w-8 h-8 text-slate-400" />
              </div>
              <h3 className="text-xl font-bold text-slate-700 dark:text-slate-300">Materi tidak ditemukan</h3>
              <p className="text-slate-500 dark:text-slate-400">Coba gunakan kata kunci lain.</p>
            </div>
          ) : (
            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
              <AnimatePresence>
                {filteredMaterials.map((m) => (
                  <motion.div
                    layout
                    initial={{ opacity: 0, scale: 0.9 }}
                    animate={{ opacity: 1, scale: 1 }}
                    exit={{ opacity: 0, scale: 0.9 }}
                    transition={{ duration: 0.2 }}
                    key={m.id}
                    className="bg-white dark:bg-slate-900 rounded-2xl p-6 border border-slate-200 dark:border-slate-800 hover:border-indigo-300 dark:hover:border-indigo-700 shadow-sm hover:shadow-xl transition-all cursor-pointer flex flex-col h-full group"
                    onClick={() => openMaterial(m.id)}
                  >
                    <div className="flex justify-between items-start mb-4">
                      <span className="text-xs font-bold uppercase tracking-wider text-indigo-600 dark:text-indigo-400 bg-indigo-50 dark:bg-indigo-900/30 px-3 py-1 rounded-full">
                        {m.category}
                      </span>
                      <div className="flex items-center text-slate-400 text-sm gap-1">
                        <Clock className="w-4 h-4" /> {m.readTime}
                      </div>
                    </div>
                    
                    <h3 className="text-xl font-bold text-slate-900 dark:text-white mb-2 group-hover:text-indigo-600 dark:group-hover:text-indigo-400 transition-colors">
                      {m.title}
                    </h3>
                    <p className="text-slate-600 dark:text-slate-400 text-sm mb-6 flex-1">
                      {m.description}
                    </p>
                    
                    <div className="pt-4 border-t border-slate-100 dark:border-slate-800 flex justify-between items-center text-sm">
                      <span className="font-medium text-slate-500 dark:text-slate-400">{m.chapters.length} Subbab</span>
                      <span className="text-indigo-600 dark:text-indigo-400 font-bold flex items-center gap-1 group-hover:translate-x-1 transition-transform">
                        Mulai <ChevronRight className="w-4 h-4" />
                      </span>
                    </div>
                  </motion.div>
                ))}
              </AnimatePresence>
            </div>
          )}
        </section>

      </main>

      {/* FOOTER */}
      <footer className="border-t border-slate-200 dark:border-slate-800 bg-white dark:bg-slate-950 py-8 mt-20 text-center">
        <p className="text-slate-500 dark:text-slate-400 text-sm">
          &copy; 2026 Materi UM-PTKIN. Dibuat dengan presisi untuk mendukung kesuksesan belajar.
        </p>
      </footer>
    </div>
  );
}
