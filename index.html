import React, { useState, useEffect } from 'react';

// === EPUB Book Data ===
const BOOK_DATA = {
  title: "F1 速度極限：300km/h 的物理與科技學",
  author: "Gemini 賽車科技編輯部",
  chapters: [
    {
      id: "ch1",
      title: "第一章：速度的殿堂 — 賽車技術演進史",
      subtitle: "從 1950 年的復古鋼管到 2026 年的永續混合動力",
      readTime: "約 5 分鐘",
      content: "一級方程式賽車（Formula 1）不僅僅是一場賽車運動，更是人類工程學與空氣動力學的終極試驗場。自 1950 年銀石賽道舉辦首場世界錦標賽以來，賽車的結構、安全標準與動力核心經歷了翻天覆地的變化。早期的賽車幾乎沒有任何下壓力概念，車手們依靠著脆弱的鋁合金管狀車架與前置引擎，在沒有安全帶的座艙裡挑戰極限。如今的 F1 賽車則是碳纖維一體成型（Monocoque）、高度數位化且整合強大油電混合動力單元的陸地飛行器。",
      hasInteractive: "timeline"
    },
    {
      id: "ch2",
      title: "第二章：科技狂潮 — F1 賽車解構",
      subtitle: "剖析產生 5G 側向重力加速度的鋼鐵猛獸",
      readTime: "約 8 分鐘",
      content: "是什麼讓 F1 賽車能以超過 250 公里的時速在彎道狂奔，而不會飛離地面？答案在於「空氣動力學（Aerodynamics）」與「地效效應（Ground Effect）」。現代 F1 賽車在高速行駛時產生的下壓力（Downforce）相當於其車重車身的三倍，這理論上意味著賽車可以在隧道的頂棚上倒立行駛。本章將解構車身各大關鍵科技元件，讓讀者親自探索各部件的精密設計與運作原理。",
      hasInteractive: "car-explorer"
    },
    {
      id: "ch3",
      title: "第三章：完美單圈 — 賽道策略與遙測物理",
      subtitle: "如何在零點幾秒的剎那間，找到完美的行車線與物理極限",
      readTime: "約 6 分鐘",
      content: "在 F1 中，快與慢的差距僅在毫秒之間。車手在進入彎道時，必須極其精確地控制重力轉移。完美的入彎需要運用「循跡煞車（Trail Braking）」技術：在直道末端全力踩下煞車，隨後隨著方向盤角度增加而逐漸釋放煞車，使前輪保持最大抓地力以對準彎心（Apex）。如果入彎速度過高，前輪抓地力會崩潰導致「轉向不足」；若出彎太急躁踩油門，則會導致後輪空轉「轉向過度」。",
      hasInteractive: "telemetry-sim"
    },
    {
      id: "ch4",
      title: "第四章：零點幾秒的戰役 — 2.0 秒極限進站",
      subtitle: "揭秘幕後英雄：20 名技師如何演繹地表最快的團隊協作",
      readTime: "約 5 分鐘",
      content: "現代 F1 賽事中已禁止途中加油，進站（Pit Stop）的目的純粹是更換輪胎與調整前翼角度。這是一個將時間壓縮到極致的藝術。在短短 2.0 秒內，賽車停妥、抬起、卸下四顆輪胎、換上全新輪胎、鎖緊螺帽並安全釋放。這需要 20 位技師毫無破綻的完美協同配合。任何一個微小的失誤，比如一發氣動板手卡住，都可能讓車手損失數秒，甚至葬送整場比賽的冠軍希望。",
      hasInteractive: "pitstop-game"
    },
    {
      id: "ch5",
      title: "第五章：傳奇挑戰 — F1 戰術戰略模擬考驗",
      subtitle: "考驗你的直覺、知識與極限分析能力",
      readTime: "約 4 分鐘",
      content: "你已經閱讀了 F1 賽車的歷史、空力科技、遙測遙控和進站策略。現在，是時候檢驗你的知識儲備了。一位優秀的車隊策略師（Strategist）必須在幾秒鐘內根據天氣變化、輪胎磨損和安全車（Safety Car）時機做出價值數百萬美元的決定。請接受以下挑戰，看看你是否具備成為圍場頂尖工程師的潛力！",
      hasInteractive: "quiz"
    }
  ],
  timelineData: [
    { year: "1950", era: "古典極速時代", description: "前置引擎，鋼管車架，完全無下壓力設計。安全裝備僅有布製頭盔，極速高但危險性極高。" },
    { year: "1970", era: "地面效應革命", description: "蓮花車隊引入側箱翼面與裙邊，利用白努利定律將賽車「吸」在地面，彎道速度呈爆發式增長。" },
    { year: "1990", era: "電子輔助尖峰", description: "主動式懸吊、循跡控制系統與半自動變速箱大行其道，賽車科技含量達到巔峰，後因安全疑慮遭禁用。" },
    { year: "2014", era: "渦輪混合動力", description: "全面啟用 1.6 升 V6 渦輪增壓引擎搭配 MGU-K 與 MGU-H 雙熱能、動能回收系統，熱效率突破 50% 創歷史紀錄。" },
    { year: "2026", era: "永續新能源藍圖", description: "全新動力規範：取消 MGU-H，大幅提升電力輸出比例至 50%，並全面採用 100% 永續合成環保燃料。" }
  ],
  carParts: {
    frontWing: {
      name: "前翼 (Front Wing)",
      desc: "賽車空氣動力學的第一道關卡。它不僅負責產生前軸下壓力，更重要的是引導後續氣流繞過旋轉的輪胎，減少車身中後段的亂流（Y250 渦流控制）。"
    },
    drs: {
      name: "DRS 減少阻力系統 (Drag Reduction System)",
      desc: "位於尾翼的可動翼片。在指定直道且落後前車 1 秒內時可開啟，使尾翼角度變平，減少約 10-12% 空氣阻力，極速可提升 10-15 km/h，是現代超車利器。"
    },
    powerUnit: {
      name: "混合動力單元 (Power Unit)",
      desc: "由 1.6 升 V6 渦輪增壓引擎與強大電機（MGU-K / 動能回收系統）組成的超高效動力核心。能壓榨出超過 1,000 匹馬力，同時比傳統引擎節能 30% 以上。"
    },
    tires: {
      name: "熱熔競技輪胎 (Pirelli Slick Tires)",
      desc: "無胎紋的光頭胎，提供極致的抓地力。分為軟胎（紅色，快但耗損快）、中性胎（黃色）與硬胎（白色，慢但耐磨），工作溫度高達 100-110°C。"
    },
    halo: {
      name: "Halo 安全防護系統",
      desc: "鈦合金製成的三叉形保護框架，位於車手座艙上方。重僅 9 公斤卻能承受高達 12 噸的衝擊力（約一輛雙層巴士重），多次在嚴重事故中拯救車手生命。"
    }
  },
  quizQuestions: [
    {
      id: "q1",
      question: "當賽道上出展「黃色旗幟（Yellow Flag）」時，代表車手應該如何應對？",
      options: [
        "前方有危險，必須減速、禁止超車，並準備隨時變道或停車",
        "比賽因嚴重事故暫停，必須立刻返回維修區",
        "有慢車在前方，應準備超越",
        "賽道濕滑，提醒車手注意防滑"
      ],
      correct: 0,
      explain: "黃旗代表前方賽道有危險狀況（如賽車打轉、碎片），車手必須明顯減速且嚴禁超車。若為雙黃旗，則須準備隨時停車。"
    },
    {
      id: "q2",
      question: "為什麼 F1 賽車進入維修區（Pit Lane）時，速度會突然降到非常慢（通常為 80 km/h）？",
      options: [
        "為了配合技師進站換胎的節奏",
        "維修區有嚴格的限速規定，超速將面臨重罰或罰秒",
        "輪胎溫度太高，需要利用慢速行駛冷卻",
        "避免大馬力引擎在狹窄空間內因空轉起火"
      ],
      correct: 1,
      explain: "為了維修區內大量技師與工作人員的安全，F1 嚴格規定維修區限速（大部分賽道為 80 km/h，摩納哥等狹窄賽道為 60 km/h），車手必須按下方向盤上的 Pit Limiter 限速鈕，超速會被處以高額罰金或罰秒。"
    },
    {
      id: "q3",
      question: "在濕地賽事中，哪一種輪胎配方在排水性能最強、適合暴雨環境？",
      options: [
        "半雨胎 (Intermediate Tires - 綠色)",
        "全雨胎 (Full Wet Tires - 藍色)",
        "硬地光頭胎 (Hard Tires - 白色)",
        "極軟光頭胎 (Soft Tires - 紅色)"
      ],
      correct: 1,
      explain: "全雨胎（藍色邊條）擁有極深的排水紋路，在時速 300 公里下每秒可排出高達 85 公升的水，適合賽道積水嚴重的暴雨天。"
    }
  ]
};

export default function App() {
  // === UI & Book Reader States ===
  const [currentChapterIndex, setCurrentChapterIndex] = useState(0);
  const [theme, setTheme] = useState('dark'); // 'dark' | 'light' | 'sepia'
  const [fontSize, setFontSize] = useState('md'); // 'sm' | 'md' | 'lg' | 'xl'
  const [showTOC, setShowTOC] = useState(true);
  const [bookmarks, setBookmarks] = useState([]);
  const [showHelp, setShowHelp] = useState(false);

  // === Chapter 1: Timeline State ===
  const [activeTimelineIndex, setActiveTimelineIndex] = useState(3); // Default to 2014

  // === Chapter 2: Car Explorer State ===
  const [selectedCarPart, setSelectedCarPart] = useState('frontWing');

  // === Chapter 3: Telemetry Sim States ===
  const [entrySpeed, setEntrySpeed] = useState(120); // km/h
  const [telemetryResult, setTelemetryResult] = useState({
    status: "完美過彎",
    color: "text-green-400",
    bg: "border-green-500",
    apexG: "3.8 G",
    throttle: 100,
    brake: 0,
    optimal: true
  });

  // Calculate telemetry behavior on slider change
  useEffect(() => {
    let status = "完美過彎";
    let color = "text-green-400";
    let bg = "border-green-500/30";
    let apexG = "3.8 G";
    let optimal = true;

    if (entrySpeed < 90) {
      status = "速度過慢：無法產生足夠空氣下壓力，抓地效率低";
      color = "text-yellow-400";
      bg = "border-yellow-500/30";
      apexG = `${(entrySpeed / 30).toFixed(1)} G`;
      optimal = false;
    } else if (entrySpeed > 140) {
      status = "嚴重轉向不足：速度超越物理極限，車輛衝出賽道！";
      color = "text-red-500 font-bold animate-pulse";
      bg = "border-red-500/50 bg-red-950/20";
      apexG = "物理極限崩潰 (Over 5.5 G)";
      optimal = false;
    } else {
      apexG = `${(3.0 + ((entrySpeed - 90) / 50) * 1.8).toFixed(1)} G`;
    }

    setTelemetryResult({ status, color, bg, apexG, entrySpeed, optimal });
  }, [entrySpeed]);

  // === Chapter 4: Pit Stop Minigame States ===
  const [pitStopStep, setPitStopStep] = useState(0); // 0: idle, 1: lift, 2: change, 3: bolt, 4: drop (done)
  const [pitStartTime, setPitStartTime] = useState(null);
  const [pitFinalTime, setPitFinalTime] = useState(null);
  const [pitGameStatus, setPitGameStatus] = useState('idle'); // 'idle' | 'running' | 'success' | 'failed'
  const [pitLogs, setPitLogs] = useState([]);

  const startPitStop = () => {
    setPitStopStep(1);
    setPitStartTime(Date.now());
    setPitFinalTime(null);
    setPitGameStatus('running');
    setPitLogs(["[0.00s] 賽車駛入停妥！開始執行進站！"]);
  };

  const handlePitStep = (step) => {
    if (pitGameStatus !== 'running') return;

    const timeElapsed = ((Date.now() - pitStartTime) / 1000).toFixed(2);
    let logMsg = "";

    if (step === 1 && pitStopStep === 1) {
      logMsg = `[${timeElapsed}s] 前後千斤頂已抬升賽車！`;
      setPitStopStep(2);
    } else if (step === 2 && pitStopStep === 2) {
      logMsg = `[${timeElapsed}s] 4具氣動板手卸下螺栓，舊胎拔除！`;
      setPitStopStep(3);
    } else if (step === 3 && pitStopStep === 3) {
      logMsg = `[${timeElapsed}s] 新輪胎裝上，螺帽已重新鎖緊鎖死！`;
      setPitStopStep(4);
    } else if (step === 4 && pitStopStep === 4) {
      const finalVal = ((Date.now() - pitStartTime) / 1000);
      setPitFinalTime(finalVal);
      setPitStopStep(5);
      setPitGameStatus('success');
      logMsg = `[${finalVal.toFixed(2)}s] 車身放下！發射釋放信號！完美完成！`;
    } else {
      // Wrong sequence
      setPitGameStatus('failed');
      logMsg = `[${timeElapsed}s] 錯誤：步驟順序混亂！技師相撞，進站失敗！`;
    }

    setPitLogs(prev => [...prev, logMsg]);
  };

  const resetPitStop = () => {
    setPitStopStep(0);
    setPitStartTime(null);
    setPitFinalTime(null);
    setPitGameStatus('idle');
    setPitLogs([]);
  };

  // === Chapter 5: Quiz States ===
  const [quizAnswers, setQuizAnswers] = useState({});
  const [quizSubmitted, setQuizSubmitted] = useState(false);
  const [quizScore, setQuizScore] = useState(0);

  const handleSelectQuiz = (qId, optionIdx) => {
    if (quizSubmitted) return;
    setQuizAnswers(prev => ({ ...prev, [qId]: optionIdx }));
  };

  const submitQuiz = () => {
    let score = 0;
    BOOK_DATA.quizQuestions.forEach(q => {
      if (quizAnswers[q.id] === q.correct) {
        score += 1;
      }
    });
    setQuizScore(score);
    setQuizSubmitted(true);
  };

  const resetQuiz = () => {
    setQuizAnswers({});
    setQuizSubmitted(false);
    setQuizScore(0);
  };

  // === Bookmark Handler ===
  const toggleBookmark = (chId) => {
    if (bookmarks.includes(chId)) {
      setBookmarks(prev => prev.filter(id => id !== chId));
    } else {
      setBookmarks(prev => [...prev, chId]);
    }
  };

  // Helper styles based on theme
  const getThemeClass = () => {
    switch (theme) {
      case 'light':
        return {
          bg: 'bg-stone-50 text-stone-900',
          card: 'bg-white border-stone-200 shadow-sm',
          nav: 'bg-stone-100 border-stone-200',
          textMuted: 'text-stone-500',
          activeCh: 'bg-red-50 text-red-600 border-l-4 border-red-600',
          btnSec: 'bg-stone-200 hover:bg-stone-300 text-stone-800'
        };
      case 'sepia':
        return {
          bg: 'bg-[#f4ecd8] text-[#433422]',
          card: 'bg-[#fdf6e3] border-[#e6d8ad] shadow-sm',
          nav: 'bg-[#eadfb9] border-[#e6d8ad]',
          textMuted: 'text-[#846b4e]',
          activeCh: 'bg-[#e2d099] text-[#5c3e16] border-l-4 border-[#8c6239]',
          btnSec: 'bg-[#e5d4a4] hover:bg-[#d9c590] text-[#5c3e16]'
        };
      case 'dark':
      default:
        return {
          bg: 'bg-[#0f1115] text-slate-100',
          card: 'bg-[#161a22] border-slate-800 shadow-xl',
          nav: 'bg-[#1b202c] border-slate-800',
          textMuted: 'text-slate-400',
          activeCh: 'bg-red-950/40 text-red-400 border-l-4 border-red-500',
          btnSec: 'bg-slate-800 hover:bg-slate-700 text-slate-200'
        };
    }
  };

  const themeStyle = getThemeClass();

  // Helper font size classes
  const getFontSizeClass = () => {
    switch (fontSize) {
      case 'sm': return 'text-sm leading-relaxed';
      case 'lg': return 'text-lg leading-relaxed';
      case 'xl': return 'text-xl leading-loose';
      case 'md':
      default:
        return 'text-base leading-relaxed';
    }
  };

  return (
    <div className={`min-h-screen font-sans ${themeStyle.bg} transition-colors duration-300`}>
      
      {/* --- TOP EPUB NAVIGATION BAR --- */}
      <header className={`sticky top-0 z-50 px-4 py-3 border-b flex justify-between items-center ${themeStyle.nav} backdrop-blur-md bg-opacity-95`}>
        <div className="flex items-center gap-3">
          <button 
            onClick={() => setShowTOC(!showTOC)}
            className="p-2 hover:bg-opacity-80 rounded-md transition-colors"
            title="目錄"
          >
            <svg className="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
          <div>
            <h1 className="font-bold text-sm md:text-base tracking-wider text-red-500 flex items-center gap-2">
              <span className="inline-block w-2.5 h-2.5 bg-red-600 rounded-full animate-pulse"></span>
              {BOOK_DATA.title}
            </h1>
            <p className="text-xs opacity-75 hidden md:block">{BOOK_DATA.author}</p>
          </div>
        </div>

        {/* Reader Configuration Widgets */}
        <div className="flex items-center gap-2 md:gap-4">
          
          {/* Font Size Adjuster */}
          <div className="flex items-center border border-current border-opacity-20 rounded-md overflow-hidden bg-black bg-opacity-10">
            <button 
              onClick={() => setFontSize('sm')} 
              className={`px-2 py-1 text-xs font-semibold ${fontSize === 'sm' ? 'bg-red-600 text-white' : 'opacity-60 hover:opacity-100'}`}
            >
              小
            </button>
            <button 
              onClick={() => setFontSize('md')} 
              className={`px-2 py-1 text-xs font-semibold border-x border-current border-opacity-10 ${fontSize === 'md' ? 'bg-red-600 text-white' : 'opacity-60 hover:opacity-100'}`}
            >
              中
            </button>
            <button 
              onClick={() => setFontSize('lg')} 
              className={`px-2 py-1 text-xs font-semibold ${fontSize === 'lg' ? 'bg-red-600 text-white' : 'opacity-60 hover:opacity-100'}`}
            >
              大
            </button>
            <button 
              onClick={() => setFontSize('xl')} 
              className={`px-2 py-1 text-xs font-semibold border-l border-current border-opacity-10 ${fontSize === 'xl' ? 'bg-red-600 text-white' : 'opacity-60 hover:opacity-100'}`}
            >
              特大
            </button>
          </div>

          {/* Theme Selector */}
          <div className="flex items-center gap-1">
            <button 
              onClick={() => setTheme('light')} 
              className={`w-6 h-6 rounded-full border border-stone-300 bg-stone-100 flex items-center justify-center ${theme === 'light' ? 'ring-2 ring-red-500' : ''}`}
              title="經典白晝"
            >
              <span className="text-[10px] text-stone-800 font-bold">L</span>
            </button>
            <button 
              onClick={() => setTheme('sepia')} 
              className={`w-6 h-6 rounded-full border border-[#d6c79a] bg-[#f4ecd8] flex items-center justify-center ${theme === 'sepia' ? 'ring-2 ring-red-500' : ''}`}
              title="暖沙羊皮"
            >
              <span className="text-[10px] text-[#5c3e16] font-bold font-serif">S</span>
            </button>
            <button 
              onClick={() => setTheme('dark')} 
              className={`w-6 h-6 rounded-full border border-slate-700 bg-slate-900 flex items-center justify-center ${theme === 'dark' ? 'ring-2 ring-red-500' : ''}`}
              title="極速黑夜"
            >
              <span className="text-[10px] text-slate-300 font-bold">D</span>
            </button>
          </div>

          {/* Bookmarks Toggle */}
          <button 
            onClick={() => toggleBookmark(BOOK_DATA.chapters[currentChapterIndex].id)}
            className={`p-1.5 rounded-md hover:bg-opacity-20 hover:bg-current transition-colors`}
            title={bookmarks.includes(BOOK_DATA.chapters[currentChapterIndex].id) ? "取消書籤" : "添加書籤"}
          >
            <svg 
              className={`w-5.5 h-5.5 ${bookmarks.includes(BOOK_DATA.chapters[currentChapterIndex].id) ? 'fill-red-500 text-red-500' : 'text-current'}`} 
              fill="none" 
              viewBox="0 0 24 24" 
              stroke="currentColor"
            >
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M5 5a2 2 0 012-2h10a2 2 0 012 2v16l-7-3.5L5 21V5z" />
            </svg>
          </button>
          
          {/* Help Info Dialog button */}
          <button 
            onClick={() => setShowHelp(true)}
            className="p-1.5 rounded-full hover:bg-opacity-20 hover:bg-current transition-colors"
          >
            <svg className="w-5.5 h-5.5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
          </button>
        </div>
      </header>

      {/* --- MAIN INTERACTIVE CONTAINER --- */}
      <div className="flex flex-col md:flex-row min-h-[calc(100vh-65px)]">
        
        {/* --- LEFT SIDE: TABLE OF CONTENTS (TOC) --- */}
        {showTOC && (
          <aside className={`w-full md:w-80 p-4 border-r md:sticky md:top-[65px] h-fit md:h-[calc(100vh-65px)] overflow-y-auto ${themeStyle.nav} transition-all duration-300`}>
            <div className="flex justify-between items-center mb-6">
              <h2 className="font-bold text-xs uppercase tracking-wider text-red-500">電子書目錄</h2>
              <span className="text-xs opacity-60 font-mono">5 Chapters</span>
            </div>
            <nav className="space-y-2">
              {BOOK_DATA.chapters.map((ch, idx) => {
                const isActive = idx === currentChapterIndex;
                const isBookmarked = bookmarks.includes(ch.id);
                return (
                  <button
                    key={ch.id}
                    onClick={() => {
                      setCurrentChapterIndex(idx);
                      // On mobile, auto-close TOC upon chapter selection
                      if (window.innerWidth < 768) {
                        setShowTOC(false);
                      }
                    }}
                    className={`w-full text-left p-3 rounded-lg transition-all flex justify-between items-start ${
                      isActive ? themeStyle.activeCh : 'hover:bg-black hover:bg-opacity-5'
                    }`}
                  >
                    <div className="flex-1 pr-2">
                      <div className="flex items-center gap-1.5">
                        <span className="text-xs font-mono opacity-60">0{idx + 1}</span>
                        <h3 className="font-semibold text-sm line-clamp-1">{ch.title.split('：')[1]}</h3>
                      </div>
                      <p className="text-xs opacity-70 mt-1 line-clamp-1">{ch.subtitle}</p>
                    </div>
                    <div className="flex items-center gap-1">
                      {isBookmarked && (
                        <span className="text-red-500" title="已標記書籤">★</span>
                      )}
                      <span className="text-[10px] px-1.5 py-0.5 rounded bg-black bg-opacity-20 font-mono scale-90">
                        {ch.readTime}
                      </span>
                    </div>
                  </button>
                );
              })}
            </nav>

            <div className="mt-8 pt-6 border-t border-current border-opacity-10">
              <h4 className="text-xs font-bold uppercase tracking-wider text-red-500 mb-3">當前閱讀進度</h4>
              <div className="w-full bg-slate-700 h-2 rounded-full overflow-hidden">
                <div 
                  className="bg-red-600 h-full transition-all duration-500"
                  style={{ width: `${((currentChapterIndex + 1) / BOOK_DATA.chapters.length) * 100}%` }}
                ></div>
              </div>
              <div className="flex justify-between text-xs mt-2 opacity-60 font-mono">
                <span>章節 {currentChapterIndex + 1} / {BOOK_DATA.chapters.length}</span>
                <span>{Math.round(((currentChapterIndex + 1) / BOOK_DATA.chapters.length) * 100)}%</span>
              </div>
            </div>

            {/* Quick F1 Mini Rules Cheat-sheet */}
            <div className={`mt-6 p-3 rounded-lg text-xs border border-dashed border-current border-opacity-20 bg-black bg-opacity-5`}>
              <h5 className="font-bold text-red-500 mb-1">🏁 F1 速學指南</h5>
              <p className="opacity-80">
                F1 賽車極速一般介於 340-360 km/h，彎道重力加速度最高可達 5.5G，整車連同車手最低重量需達到 798 公斤。
              </p>
            </div>
          </aside>
        )}

        {/* --- CENTER CONTENT & INTERACTIVE COMPONENT --- */}
        <main className="flex-1 p-4 md:p-8 flex flex-col justify-between max-w-4xl mx-auto">
          
          {/* Chapter Heading */}
          <article className="space-y-6">
            <header className="border-b border-current border-opacity-10 pb-4">
              <div className="flex items-center justify-between mb-2">
                <span className="text-xs font-bold uppercase tracking-widest text-red-500 font-mono">
                  Chapter {currentChapterIndex + 1}
                </span>
                {bookmarks.includes(BOOK_DATA.chapters[currentChapterIndex].id) && (
                  <span className="text-xs bg-red-600 text-white px-2 py-0.5 rounded font-bold animate-pulse flex items-center gap-1">
                    🔖 已加入書籤
                  </span>
                )}
              </div>
              <h2 className="text-2xl md:text-3xl font-extrabold tracking-tight">{BOOK_DATA.chapters[currentChapterIndex].title}</h2>
              <p className={`text-sm md:text-base italic font-medium mt-1 ${themeStyle.textMuted}`}>
                {BOOK_DATA.chapters[currentChapterIndex].subtitle}
              </p>
            </header>

            {/* Simulated EPUB Content Box */}
            <section className={`prose max-w-none ${getFontSizeClass()}`}>
              <p className="text-justify leading-relaxed indent-8">
                {BOOK_DATA.chapters[currentChapterIndex].content}
              </p>
            </section>

            {/* --- CHAPTER SPECIFIC INTERACTIVE WIDGET --- */}
            <div className={`mt-8 p-4 md:p-6 rounded-xl border ${themeStyle.card} transition-all duration-300`}>
              <div className="flex items-center gap-2 mb-4">
                <span className="bg-red-600 text-white text-[10px] font-bold px-2 py-0.5 rounded uppercase tracking-wider animate-pulse">
                  動態互動
                </span>
                <h4 className="font-bold text-sm tracking-wide uppercase text-red-500">
                  {currentChapterIndex === 0 && "F1 賽車編年史互動滑桿"}
                  {currentChapterIndex === 1 && "F1 賽車動力學 3D 感解構面板"}
                  {currentChapterIndex === 2 && "轉向不足與遙測模擬器"}
                  {currentChapterIndex === 3 && "地表最速進站（Pit Stop）模擬考驗"}
                  {currentChapterIndex === 4 && "F1 圍場策略戰術模擬考試"}
                </h4>
              </div>

              {/* 1. TIMELINE INTERACTIVE */}
              {currentChapterIndex === 0 && (
                <div className="space-y-4">
                  <p className="text-xs opacity-75 mb-3">拖動滑桿，直觀查看不同時代賽車結構和安全理念的巨變：</p>
                  
                  {/* Interactive Slider */}
                  <div className="px-4 py-2">
                    <input 
                      type="range" 
                      min="0" 
                      max={BOOK_DATA.timelineData.length - 1} 
                      value={activeTimelineIndex}
                      onChange={(e) => setActiveTimelineIndex(parseInt(e.target.value))}
                      className="w-full accent-red-600 h-2 bg-slate-700 rounded-lg appearance-none cursor-pointer"
                    />
                    <div className="flex justify-between text-xs font-bold font-mono mt-2 px-1">
                      {BOOK_DATA.timelineData.map((t, idx) => (
                        <button 
                          key={t.year} 
                          onClick={() => setActiveTimelineIndex(idx)}
                          className={`transition-colors ${idx === activeTimelineIndex ? 'text-red-500 scale-110 font-extrabold' : 'opacity-60'}`}
                        >
                          {t.year}
                        </button>
                      ))}
                    </div>
                  </div>

                  {/* Active Info Display */}
                  <div className="p-4 rounded-lg bg-black bg-opacity-20 border border-current border-opacity-10 mt-4">
                    <div className="flex justify-between items-center mb-2">
                      <span className="text-lg font-bold text-red-500 font-mono">{BOOK_DATA.timelineData[activeTimelineIndex].year} 年</span>
                      <span className="text-xs px-2 py-0.5 rounded bg-red-600/20 text-red-400 border border-red-500/30">{BOOK_DATA.timelineData[activeTimelineIndex].era}</span>
                    </div>
                    <p className="text-sm leading-relaxed">{BOOK_DATA.timelineData[activeTimelineIndex].description}</p>
                  </div>
                </div>
              )}

              {/* 2. CAR EXPLORER INTERACTIVE */}
              {currentChapterIndex === 1 && (
                <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                  {/* Stylized Side Profile SVG of F1 Car */}
                  <div className="flex flex-col justify-center items-center p-2 bg-black/30 rounded-lg border border-slate-800">
                    <svg className="w-full max-w-sm h-auto" viewBox="0 0 400 180" fill="none" xmlns="http://www.w3.org/2000/svg">
                      {/* Grid Line Backing */}
                      <g stroke="#ffffff" strokeOpacity="0.05" strokeWidth="1">
                        <line x1="0" y1="30" x2="400" y2="30" />
                        <line x1="0" y1="60" x2="400" y2="60" />
                        <line x1="0" y1="90" x2="400" y2="90" />
                        <line x1="0" y1="120" x2="400" y2="120" />
                        <line x1="0" y1="150" x2="400" y2="150" />
                        <line x1="80" y1="0" x2="80" y2="180" />
                        <line x1="160" y1="0" x2="160" y2="180" />
                        <line x1="240" y1="0" x2="240" y2="180" />
                        <line x1="320" y1="0" x2="320" y2="180" />
                      </g>

                      {/* Asphalt track representation */}
                      <rect x="10" y="148" width="380" height="4" fill="#3b3b3b" rx="2" />
                      
                      {/* Main F1 Chassis Body */}
                      <path d="M 60,115 L 120,115 L 140,85 L 210,85 L 280,105 L 340,105 L 340,118 L 60,118 Z" fill="#64748b" opacity="0.4"/>
                      <path d="M 120,115 C 150,90 200,80 250,90 C 290,100 320,115 340,115 L 340,118 L 120,118 Z" fill="red" opacity="0.7" />
                      
                      {/* Front Wing Hotspot (Left Side of SVG, representing nose) */}
                      <path 
                        d="M 30,115 L 90,115 L 85,128 L 30,128 Z" 
                        fill={selectedCarPart === 'frontWing' ? '#ef4444' : '#475569'} 
                        className="cursor-pointer transition-colors duration-200 hover:fill-red-500"
                        onClick={() => setSelectedCarPart('frontWing')}
                        stroke={selectedCarPart === 'frontWing' ? '#ffffff' : 'none'}
                        strokeWidth="1.5"
                      />
                      {/* Front Wing Flaps */}
                      <path d="M 35,108 L 65,114 L 35,114 Z" fill="#1e293b" />

                      {/* Halo Hotspot (Cockpit area) */}
                      <path 
                        d="M 175,82 C 185,62 210,62 215,82 L 205,82 C 200,72 188,72 185,82 Z" 
                        fill={selectedCarPart === 'halo' ? '#ef4444' : '#475569'} 
                        className="cursor-pointer transition-colors duration-200 hover:fill-red-500"
                        onClick={() => setSelectedCarPart('halo')}
                        stroke={selectedCarPart === 'halo' ? '#ffffff' : 'none'}
                        strokeWidth="1.5"
                      />
                      {/* Driver Helmet representation inside Halo */}
                      <circle cx="195" cy="88" r="8" fill="#eab308" />

                      {/* Power Unit Core Hotspot */}
                      <rect 
                        x="225" y="85" width="45" height="30" rx="3" 
                        fill={selectedCarPart === 'powerUnit' ? '#ef4444' : '#475569'} 
                        className="cursor-pointer transition-colors duration-200 hover:fill-red-500"
                        onClick={() => setSelectedCarPart('powerUnit')}
                        stroke={selectedCarPart === 'powerUnit' ? '#ffffff' : 'none'}
                        strokeWidth="1.5"
                      />

                      {/* DRS / Rear Wing Hotspot */}
                      <path 
                        d="M 330,70 L 375,70 L 365,115 L 330,115 Z" 
                        fill={selectedCarPart === 'drs' ? '#ef4444' : '#475569'} 
                        className="cursor-pointer transition-colors duration-200 hover:fill-red-500"
                        onClick={() => setSelectedCarPart('drs')}
                        stroke={selectedCarPart === 'drs' ? '#ffffff' : 'none'}
                        strokeWidth="1.5"
                      />
                      {/* DRS flap open simulation */}
                      <line x1="335" y1="78" x2="368" y2="78" stroke={selectedCarPart === 'drs' ? '#ffffff' : '#94a3b8'} strokeWidth="3" />

                      {/* Tires Hotspots */}
                      {/* Front Tire */}
                      <circle 
                        cx="100" cy="120" r="28" 
                        fill={selectedCarPart === 'tires' ? '#ef4444' : '#1e293b'} 
                        className="cursor-pointer transition-all duration-200 hover:opacity-90"
                        onClick={() => setSelectedCarPart('tires')}
                        stroke={selectedCarPart === 'tires' ? '#ffffff' : '#475569'}
                        strokeWidth="2.5"
                      />
                      <circle cx="100" cy="120" r="12" fill="#0f172a" />
                      <circle cx="100" cy="120" r="23" stroke="#eab308" strokeWidth="1.5" strokeDasharray="3 3" title="黃色中性胎配方" />

                      {/* Rear Tire */}
                      <circle 
                        cx="305" cy="118" r="30" 
                        fill={selectedCarPart === 'tires' ? '#ef4444' : '#1e293b'} 
                        className="cursor-pointer transition-all duration-200 hover:opacity-90"
                        onClick={() => setSelectedCarPart('tires')}
                        stroke={selectedCarPart === 'tires' ? '#ffffff' : '#475569'}
                        strokeWidth="2.5"
                      />
                      <circle cx="305" cy="118" r="13" fill="#0f172a" />
                      <circle cx="305" cy="118" r="25" stroke="#eab308" strokeWidth="1.5" strokeDasharray="3 3" />

                      {/* Overlay Labels */}
                      <text x="35" y="150" fill="#ffffff" fontSize="10" fontWeight="bold">前翼</text>
                      <text x="180" y="52" fill="#ffffff" fontSize="10" fontWeight="bold">HALO</text>
                      <text x="228" y="77" fill="#ffffff" fontSize="10" fontWeight="bold">動力</text>
                      <text x="345" y="60" fill="#ffffff" fontSize="10" fontWeight="bold">DRS</text>
                      <text x="290" y="165" fill="#ffffff" fontSize="10" fontWeight="bold">Pirelli 輪胎</text>
                    </svg>
                    <span className="text-[10px] opacity-50 mt-1">💡 點擊車身的高亮部件進行深度探索</span>
                  </div>

                  {/* Description Box */}
                  <div className="flex flex-col justify-between p-4 bg-black bg-opacity-20 rounded-lg border border-current border-opacity-10">
                    <div>
                      <h5 className="font-extrabold text-base text-red-500 border-b border-red-500 border-opacity-20 pb-2 mb-3">
                        {BOOK_DATA.carParts[selectedCarPart].name}
                      </h5>
                      <p className="text-sm leading-relaxed">
                        {BOOK_DATA.carParts[selectedCarPart].desc}
                      </p>
                    </div>
                    
                    <div className="mt-4 pt-3 border-t border-current border-opacity-10 flex gap-2">
                      {Object.keys(BOOK_DATA.carParts).map((partKey) => (
                        <button
                          key={partKey}
                          onClick={() => setSelectedCarPart(partKey)}
                          className={`text-xs px-2.5 py-1 rounded transition-colors ${
                            selectedCarPart === partKey 
                              ? 'bg-red-600 text-white font-bold' 
                              : 'bg-black bg-opacity-20 hover:bg-opacity-40'
                          }`}
                        >
                          {BOOK_DATA.carParts[partKey].name.split(' ')[0]}
                        </button>
                      ))}
                    </div>
                  </div>
                </div>
              )}

              {/* 3. TELEMETRY WIDGET */}
              {currentChapterIndex === 2 && (
                <div className="space-y-4">
                  <p className="text-xs opacity-75">
                    這是一處難度極高的 90 度中速直角彎。請左右拉動「入彎速度」，調整賽車的入彎動能：
                  </p>

                  <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
                    {/* Simulator Settings */}
                    <div className="p-4 bg-black bg-opacity-30 rounded-lg border border-slate-800 space-y-4">
                      <div>
                        <label className="text-xs font-bold block mb-1">設定入彎車速 (Entry Speed):</label>
                        <div className="flex items-center gap-3">
                          <input 
                            type="range" 
                            min="70" 
                            max="170" 
                            step="5"
                            value={entrySpeed}
                            onChange={(e) => setEntrySpeed(parseInt(e.target.value))}
                            className="flex-1 accent-red-600"
                          />
                          <span className="font-mono font-bold text-red-500 text-lg w-18 text-right">{entrySpeed} <span className="text-xs">km/h</span></span>
                        </div>
                      </div>

                      <div className="space-y-2 border-t border-slate-800 pt-3">
                        <div className="flex justify-between text-xs">
                          <span>彎心重力加速度 (Lateral G):</span>
                          <span className="font-mono font-bold text-yellow-500">{telemetryResult.apexG}</span>
                        </div>
                        <div className="flex justify-between text-xs">
                          <span>空力下壓力 (Aerodynamics):</span>
                          <span className="font-mono font-bold text-yellow-500">
                            {entrySpeed < 100 ? "偏低 (Low)" : entrySpeed > 140 ? "極高 (Overload)" : "完美 (Optimal)"}
                          </span>
                        </div>
                        <div className="flex justify-between text-xs">
                          <span>出彎油門反應 (Throttle Input):</span>
                          <span className="font-mono font-bold text-yellow-500">
                            {entrySpeed > 140 ? "0% (衝出賽道無法踩油門)" : "100% (全油門加速)"}
                          </span>
                        </div>
                      </div>
                    </div>

                    {/* Interactive Remote Graphic */}
                    <div className="md:col-span-2 p-4 bg-black bg-opacity-40 rounded-lg border border-slate-800 flex flex-col justify-between">
                      <div>
                        <span className="text-xs font-bold text-red-500 block mb-2 font-mono">LIVE TELEMETRY (即時遙測)</span>
                        <div className={`p-3 rounded border ${telemetryResult.bg} transition-all duration-300`}>
                          <h6 className="font-bold text-sm mb-1">物理狀態回饋：</h6>
                          <p className={`text-sm ${telemetryResult.color}`}>{telemetryResult.status}</p>
                        </div>
                      </div>

                      {/* Dynamic Visual Graph (Telemetry Speed Line Simulator) */}
                      <div className="h-28 mt-4 relative border-l border-b border-slate-700 font-mono text-[10px]">
                        <span className="absolute -top-3 left-1 text-slate-500">180kph</span>
                        <span className="absolute bottom-1 right-1 text-slate-500">時間 →</span>
                        
                        {/* Reference Line */}
                        <div className="absolute w-full border-t border-dashed border-green-500/20 top-1/2"></div>
                        
                        {/* Interactive Curve drawing (SVG) */}
                        <svg className="w-full h-full absolute inset-0" preserveAspectRatio="none" viewBox="0 0 100 100">
                          {/* Speed curve */}
                          <path 
                            d={`M 0,20 Q 25,${100 - (entrySpeed/1.8)} 50,${100 - (entrySpeed/2.2)} T 100,20`} 
                            fill="none" 
                            stroke={entrySpeed > 140 ? "#ef4444" : "#10b981"} 
                            strokeWidth="3.5" 
                            className="transition-all duration-300"
                          />
                          {/* Braking marker bar */}
                          <line x1="25" y1="90" x2="25" y2="10" stroke="#f97316" strokeWidth="1" strokeDasharray="2 2" />
                          {/* Apex marker */}
                          <circle cx="50" cy={100 - (entrySpeed/2.2)} r="4.5" fill="#ef4444" className="transition-all duration-300" />
                        </svg>

                        <div className="absolute top-2 right-2 flex gap-3 text-[10px]">
                          <span className="flex items-center gap-1"><span className="w-2 h-2 rounded bg-green-500"></span>時速遙測</span>
                          <span className="flex items-center gap-1"><span className="w-2 h-2 rounded bg-orange-500"></span>煞車點</span>
                          <span className="flex items-center gap-1"><span className="w-2 h-2 rounded bg-red-500"></span>彎心點</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              )}

              {/* 4. PIT STOP GAME */}
              {currentChapterIndex === 3 && (
                <div className="space-y-4">
                  <p className="text-xs opacity-75">
                    模擬考驗：你將扮演車隊總協調技師，依照標準流程，在最短時間內精準觸發四項機械動作。任何錯誤都將導致翻車事故！
                  </p>

                  <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                    {/* Game Dashboard */}
                    <div className="p-4 bg-black bg-opacity-30 rounded-lg border border-slate-800 flex flex-col justify-between">
                      <div>
                        <div className="flex justify-between items-center mb-4">
                          <span className="text-xs font-bold uppercase text-slate-400">進站系統監測</span>
                          <span className={`px-2 py-0.5 rounded text-xs font-bold font-mono ${
                            pitGameStatus === 'running' ? 'bg-amber-600 animate-pulse text-white' :
                            pitGameStatus === 'success' ? 'bg-green-600 text-white' :
                            pitGameStatus === 'failed' ? 'bg-red-600 text-white' : 'bg-slate-700 text-slate-300'
                          }`}>
                            {pitGameStatus === 'idle' && "準備就緒"}
                            {pitGameStatus === 'running' && "進站搶修中"}
                            {pitGameStatus === 'success' && "完美進站"}
                            {pitGameStatus === 'failed' && "失誤砸鍋"}
                          </span>
                        </div>

                        {/* Visual Step indicators */}
                        <div className="grid grid-cols-4 gap-2 mb-4 text-center">
                          {[
                            { name: "1. 升千斤頂", stepVal: 1 },
                            { name: "2. 拆卸螺栓", stepVal: 2 },
                            { name: "3. 鎖緊新胎", stepVal: 3 },
                            { name: "4. 放下賽車", stepVal: 4 }
                          ].map((s) => (
                            <div 
                              key={s.stepVal} 
                              className={`p-2 rounded text-xs transition-all ${
                                pitStopStep >= s.stepVal ? 'bg-green-600/30 border border-green-500 text-green-400 font-extrabold scale-105' : 'bg-slate-800 text-slate-400 opacity-60'
                              }`}
                            >
                              {s.name}
                            </div>
                          ))}
                        </div>
                      </div>

                      {/* Interactive Buttons */}
                      <div className="space-y-2 mt-4">
                        {pitGameStatus === 'idle' && (
                          <button 
                            onClick={startPitStop}
                            className="w-full bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-4 rounded-lg shadow-lg active:scale-95 transition-transform"
                          >
                            🟢 開始挑戰！賽車駛入！
                          </button>
                        )}

                        {pitGameStatus === 'running' && (
                          <div className="grid grid-cols-2 gap-2">
                            <button 
                              onClick={() => handlePitStep(1)}
                              className={`py-3 px-2 font-bold text-xs rounded transition-all ${
                                pitStopStep === 1 ? 'bg-amber-500 text-black animate-bounce' : 'bg-slate-700 opacity-50'
                              }`}
                            >
                              ⚙️ 1. 抬起車身
                            </button>
                            <button 
                              onClick={() => handlePitStep(2)}
                              className={`py-3 px-2 font-bold text-xs rounded transition-all ${
                                pitStopStep === 2 ? 'bg-amber-500 text-black animate-bounce' : 'bg-slate-700 opacity-50'
                              }`}
                            >
                              🔧 2. 拔除舊輪胎
                            </button>
                            <button 
                              onClick={() => handlePitStep(3)}
                              className={`py-3 px-2 font-bold text-xs rounded transition-all ${
                                pitStopStep === 3 ? 'bg-amber-500 text-black animate-bounce' : 'bg-slate-700 opacity-50'
                              }`}
                            >
                              🔩 3. 鎖緊全新輪胎
                            </button>
                            <button 
                              onClick={() => handlePitStep(4)}
                              className={`py-3 px-2 font-bold text-xs rounded transition-all ${
                                pitStopStep === 4 ? 'bg-amber-500 text-black animate-bounce' : 'bg-slate-700 opacity-50'
                              }`}
                            >
                              🏁 4. 安全放下賽車
                            </button>
                          </div>
                        )}

                        {(pitGameStatus === 'success' || pitGameStatus === 'failed') && (
                          <button 
                            onClick={resetPitStop}
                            className="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-lg transition-colors"
                          >
                            🔄 重試挑戰
                          </button>
                        )}
                      </div>
                    </div>

                    {/* Console / Log display */}
                    <div className="p-4 bg-black bg-opacity-50 rounded-lg border border-slate-800 flex flex-col justify-between min-h-48">
                      <div>
                        <span className="text-xs font-bold text-slate-500 block mb-2 font-mono">🔧 WORKSHOP LOGS (工作日誌)</span>
                        <div className="space-y-1 font-mono text-[11px] h-36 overflow-y-auto">
                          {pitLogs.length === 0 ? (
                            <p className="text-slate-500 italic">等待賽車駛入 Pit Area...</p>
                          ) : (
                            pitLogs.map((log, index) => (
                              <p key={index} className={log.includes('錯誤') ? 'text-red-400 font-bold' : log.includes('完美') ? 'text-green-400 font-bold' : 'text-slate-300'}>
                                {log}
                              </p>
                            ))
                          )}
                        </div>
                      </div>

                      {pitFinalTime && (
                        <div className="border-t border-slate-800 pt-2 mt-2 flex justify-between items-center">
                          <span className="text-xs text-slate-400">最終用時:</span>
                          <span className={`text-xl font-mono font-extrabold ${pitFinalTime <= 2.2 ? 'text-green-400' : 'text-yellow-400'}`}>
                            {pitFinalTime.toFixed(3)} 秒
                          </span>
                        </div>
                      )}
                    </div>
                  </div>
                </div>
              )}

              {/* 5. QUIZ CHALLENGE */}
              {currentChapterIndex === 4 && (
                <div className="space-y-6">
                  {!quizSubmitted ? (
                    <div className="space-y-4">
                      {BOOK_DATA.quizQuestions.map((q, idx) => (
                        <div key={q.id} className="p-4 bg-black bg-opacity-20 rounded-lg border border-current border-opacity-10">
                          <h5 className="font-bold text-sm mb-3 text-slate-100 flex gap-2">
                            <span className="text-red-500 font-mono">Q{idx + 1}.</span> {q.question}
                          </h5>
                          <div className="space-y-2">
                            {q.options.map((opt, oIdx) => (
                              <button
                                key={oIdx}
                                onClick={() => handleSelectQuiz(q.id, oIdx)}
                                className={`w-full text-left text-xs p-3 rounded-lg transition-all border ${
                                  quizAnswers[q.id] === oIdx
                                    ? 'bg-red-600/20 border-red-500 text-red-400 font-bold'
                                    : 'bg-black bg-opacity-20 hover:bg-opacity-40 border-transparent text-slate-300'
                                }`}
                              >
                                {opt}
                              </button>
                            ))}
                          </div>
                        </div>
                      ))}

                      <button
                        onClick={submitQuiz}
                        disabled={Object.keys(quizAnswers).length < BOOK_DATA.quizQuestions.length}
                        className={`w-full py-3 rounded-lg font-bold transition-all shadow-lg text-sm ${
                          Object.keys(quizAnswers).length === BOOK_DATA.quizQuestions.length
                            ? 'bg-red-600 hover:bg-red-700 text-white cursor-pointer active:scale-95'
                            : 'bg-slate-800 text-slate-500 cursor-not-allowed'
                        }`}
                      >
                        📊 提交答案（必須回答所有問題）
                      </button>
                    </div>
                  ) : (
                    <div className="space-y-4 text-center py-6">
                      <div className="inline-block p-4 rounded-full bg-red-600/10 border-2 border-red-500 mb-2">
                        <span className="text-3xl font-mono font-extrabold text-red-500">
                          {quizScore} / {BOOK_DATA.quizQuestions.length}
                        </span>
                      </div>
                      <h5 className="font-extrabold text-lg text-red-500">
                        {quizScore === BOOK_DATA.quizQuestions.length ? "👑 F1 圍場戰術大師！" : "🏁 具備潛力，繼續努力學習！"}
                      </h5>
                      <p className="text-xs opacity-75 max-w-md mx-auto">
                        你在賽車技術、賽道安全旗號以及維修區策略上取得了優異的成績。
                      </p>

                      <div className="text-left space-y-4 mt-6">
                        <h6 className="font-bold text-sm border-b border-current border-opacity-10 pb-1 text-red-500">📖 本章詳盡解析：</h6>
                        {BOOK_DATA.quizQuestions.map((q, idx) => (
                          <div key={q.id} className="p-3 bg-black bg-opacity-30 rounded-lg text-xs space-y-1">
                            <p className="font-bold text-slate-200">Q{idx+1}: {q.question}</p>
                            <p className="text-slate-400 font-mono">
                              正確答案：<span className="text-green-400 font-bold">{q.options[q.correct]}</span>
                            </p>
                            <p className="text-slate-400 italic bg-black bg-opacity-20 p-2 rounded mt-1 border-l-2 border-yellow-500">
                              {q.explain}
                            </p>
                          </div>
                        ))}
                      </div>

                      <button
                        onClick={resetQuiz}
                        className="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-lg mt-4 transition-colors text-xs"
                      >
                        🔄 重置考卷
                      </button>
                    </div>
                  )}
                </div>
              )}

            </div>
          </article>

          {/* --- EPUB FOOTER CONTROLS --- */}
          <footer className="mt-12 pt-6 border-t border-current border-opacity-10 flex justify-between items-center">
            <button
              onClick={() => {
                if (currentChapterIndex > 0) {
                  setCurrentChapterIndex(currentChapterIndex - 1);
                }
              }}
              disabled={currentChapterIndex === 0}
              className={`px-4 py-2 rounded-lg text-sm font-bold flex items-center gap-2 transition-all ${
                currentChapterIndex === 0
                  ? 'opacity-30 cursor-not-allowed'
                  : themeStyle.btnSec
              }`}
            >
              ← 上一章
            </button>

            <span className="text-xs opacity-60 font-mono">
              第 {currentChapterIndex + 1} 章 / 共 {BOOK_DATA.chapters.length} 章
            </span>

            <button
              onClick={() => {
                if (currentChapterIndex < BOOK_DATA.chapters.length - 1) {
                  setCurrentChapterIndex(currentChapterIndex + 1);
                }
              }}
              disabled={currentChapterIndex === BOOK_DATA.chapters.length - 1}
              className={`px-4 py-2 rounded-lg text-sm font-bold flex items-center gap-2 transition-all ${
                currentChapterIndex === BOOK_DATA.chapters.length - 1
                  ? 'opacity-30 cursor-not-allowed'
                  : 'bg-red-600 hover:bg-red-700 text-white'
              }`}
            >
              下一章 →
            </button>
          </footer>
        </main>
      </div>

      {/* --- OVERLAY: HELP DIALOG --- */}
      {showHelp && (
        <div className="fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center p-4 z-50 backdrop-blur-sm">
          <div className="bg-slate-900 border border-slate-800 text-slate-100 p-6 rounded-xl max-w-md w-full shadow-2xl relative">
            <button 
              onClick={() => setShowHelp(false)}
              className="absolute top-4 right-4 text-slate-400 hover:text-white"
            >
              <svg className="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>

            <h3 className="text-lg font-extrabold text-red-500 mb-3 border-b border-slate-800 pb-2">🏁 F1 互動電子書操作說明</h3>
            <div className="space-y-3 text-sm leading-relaxed text-slate-300">
              <p>歡迎閱讀這本專為 F1 愛好者打造的精緻 EPUB 互動電子書：</p>
              <ul className="list-disc list-inside space-y-1.5 pl-2 text-xs">
                <li><strong className="text-white">頂部控制面板</strong>：自由切換「極速黑夜」、「塞道暖陽」等背景配色、調節字體大小或點擊「書籤鍵」標記精彩內容。</li>
                <li><strong className="text-white">側欄目錄 (TOC)</strong>：可點擊隨時切換 5 大核心科技章節，隨時掌握全書閱讀進度。</li>
                <li><strong className="text-white">互動組件</strong>：各章末端配置極速互動。您可以控制入彎遙測、親自進行 2 秒極限 Pit Stop、或解剖車身、考驗您的戰術知識！</li>
              </ul>
              <p className="text-xs text-slate-500 mt-4 italic">
                技術提示：當前讀取的所有進度與模擬均在沙盒端即時運算，提供完美的流暢感與高傳真遙測反饋。
              </p>
            </div>
          </div>
        </div>
      )}

    </div>
  );
}