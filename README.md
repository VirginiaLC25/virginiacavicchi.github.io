# virginiacavicchi.github.io
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Your Name] — PhD Student in [Your Field]</title>
    <meta name="description" content="Academic personal webpage of [Your Name], PhD Student in [Your Field] at [University Name].">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter (Sans) & Merriweather (Serif) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Merriweather:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
    
    <!-- Font Awesome for Academic & Social Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- Academicons for Google Scholar & CV icons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">

    <!-- Tailwind Configuration -->
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'system-ui', '-apple-system', 'sans-serif'],
                        serif: ['Merriweather', 'Georgia', 'serif'],
                    },
                    colors: {
                        accent: {
                            light: '#1d4ed8', // Crisp Academic Blue (Light Mode)
                            dark: '#60a5fa',  // Soft Sky Blue (Dark Mode)
                        }
                    }
                }
            }
        }
    </script>

    <!-- Initial Theme Script (Prevents Flash of Unstyled Content) -->
    <script>
        if (localStorage.theme === 'dark' || (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            document.documentElement.classList.add('dark');
        } else {
            document.documentElement.classList.remove('dark');
        }
    </script>
</head>
<body class="bg-stone-50 text-slate-800 dark:bg-slate-950 dark:text-slate-200 font-sans antialiased transition-colors duration-200 selection:bg-blue-100 selection:text-blue-900 dark:selection:bg-blue-900 dark:selection:text-blue-100">

    <!-- Top Navigation Bar -->
    <header class="sticky top-0 z-40 w-full backdrop-blur-md bg-stone-50/85 dark:bg-slate-950/85 border-b border-slate-200/80 dark:border-slate-800/80">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <!-- Brand / Name -->
            <a href="#" class="font-serif font-bold text-lg tracking-tight text-slate-900 dark:text-white hover:text-accent-light dark:hover:text-accent-dark transition-colors">
                [Your Name]
            </a>

            <!-- Desktop Navigation Links -->
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-slate-600 dark:text-slate-300">
                <a href="#about" class="hover:text-accent-light dark:hover:text-accent-dark transition-colors">About</a>
                <a href="#news" class="hover:text-accent-light dark:hover:text-accent-dark transition-colors">News</a>
                <a href="#publications" class="hover:text-accent-light dark:hover:text-accent-dark transition-colors">Publications</a>
                <a href="#teaching" class="hover:text-accent-light dark:hover:text-accent-dark transition-colors">Teaching &amp; Service</a>
                
                <!-- Theme Toggle Button -->
                <button id="theme-toggle" aria-label="Toggle Dark Mode" class="p-2 rounded-lg text-slate-500 hover:text-slate-900 dark:text-slate-400 dark:hover:text-white hover:bg-slate-200/60 dark:hover:bg-slate-800 transition-colors">
                    <i id="theme-icon-dark" class="fas fa-moon hidden"></i>
                    <i id="theme-icon-light" class="fas fa-sun hidden"></i>
                </button>
            </nav>

            <!-- Mobile Controls (Theme Toggle + Hamburger Menu) -->
            <div class="flex items-center space-x-2 md:hidden">
                <button id="theme-toggle-mobile" aria-label="Toggle Dark Mode" class="p-2.5 rounded-lg text-slate-500 hover:text-slate-900 dark:text-slate-400 dark:hover:text-white hover:bg-slate-200/60 dark:hover:bg-slate-800 transition-colors">
                    <i id="theme-icon-dark-mobile" class="fas fa-moon hidden"></i>
                    <i id="theme-icon-light-mobile" class="fas fa-sun hidden"></i>
                </button>
                <button id="mobile-menu-btn" aria-label="Open Menu" aria-expanded="false" class="p-2.5 rounded-lg text-slate-600 dark:text-slate-300 hover:bg-slate-200/60 dark:hover:bg-slate-800 transition-colors">
                    <i class="fas fa-bars text-lg"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Dropdown Navigation -->
        <div id="mobile-menu" class="hidden md:hidden border-b border-slate-200 dark:border-slate-800 bg-stone-50 dark:bg-slate-950 px-4 pt-2 pb-4 space-y-1">
            <a href="#about" class="mobile-link block px-3 py-2.5 rounded-lg text-base font-medium text-slate-700 dark:text-slate-200 hover:bg-slate-200/60 dark:hover:bg-slate-800">About</a>
            <a href="#news" class="mobile-link block px-3 py-2.5 rounded-lg text-base font-medium text-slate-700 dark:text-slate-200 hover:bg-slate-200/60 dark:hover:bg-slate-800">News</a>
            <a href="#publications" class="mobile-link block px-3 py-2.5 rounded-lg text-base font-medium text-slate-700 dark:text-slate-200 hover:bg-slate-200/60 dark:hover:bg-slate-800">Publications</a>
            <a href="#teaching" class="mobile-link block px-3 py-2.5 rounded-lg text-base font-medium text-slate-700 dark:text-slate-200 hover:bg-slate-200/60 dark:hover:bg-slate-800">Teaching &amp; Service</a>
        </div>
    </header>

    <!-- Main Container: Sidebar + Content Grid -->
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 py-10 md:py-16">
        <div class="grid grid-cols-1 md:grid-cols-12 gap-10 lg:gap-12">
            
            <!-- LEFT SIDEBAR: Profile Info & Academic Links -->
            <aside class="md:col-span-4 lg:col-span-4">
                <div class="md:sticky md:top-24 flex flex-col items-center md:items-start text-center md:text-left">
                    
                    <!-- Circular Profile Photo -->
                    <!-- TIP: Replace the src URL with 'assets/profile.jpg' after uploading your photo to your GitHub repo -->
                    <div class="w-40 h-40 sm:w-44 sm:h-44 rounded-full overflow-hidden ring-4 ring-white dark:ring-slate-800 shadow-md mb-5 bg-slate-200 dark:bg-slate-800">
                        <img 
                            src="https://placehold.co/400x400/e2e8f0/475569?text=Your+Photo" 
                            onerror="this.onerror=null; this.src='https://placehold.co/400x400/cbd5e1/334155?text=Profile';"
                            alt="[Your Name] Profile Photo" 
                            class="w-full h-full object-cover"
                        >
                    </div>

                    <!-- Name & Academic Title -->
                    <h1 class="font-serif text-2xl sm:text-3xl font-bold text-slate-900 dark:text-white tracking-tight">
                        [Your Name]
                    </h1>
                    <p class="mt-1.5 text-base font-medium text-accent-light dark:text-accent-dark">
                        PhD Student in [Your Field]
                    </p>

                    <!-- Affiliation & Lab -->
                    <div class="mt-3 space-y-1 text-sm text-slate-600 dark:text-slate-400">
                        <p class="flex items-center justify-center md:justify-start gap-2">
                            <i class="fas fa-university w-4 text-center text-slate-400"></i>
                            <span><a href="[Lab Website URL]" class="hover:underline text-slate-700 dark:text-slate-300">[Your Research Lab]</a></span>
                        </p>
                        <p class="flex items-center justify-center md:justify-start gap-2">
                            <i class="fas fa-map-marker-alt w-4 text-center text-slate-400"></i>
                            <span>[University Name], [City]</span>
                        </p>
                        <p class="flex items-center justify-center md:justify-start gap-2">
                            <i class="fas fa-envelope w-4 text-center text-slate-400"></i>
                            <a href="mailto:[your.email@university.edu]" class="hover:text-accent-light dark:hover:text-accent-dark transition-colors">
                                [your.email@university.edu]
                            </a>
                        </p>
                    </div>

                    <!-- Academic & Social Links -->
                    <div class="mt-6 flex flex-wrap justify-center md:justify-start gap-2.5">
                        <!-- Google Scholar -->
                        <a href="[Google Scholar URL]" target="_blank" rel="noopener noreferrer" aria-label="Google Scholar" title="Google Scholar"
                           class="p-2.5 rounded-lg bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 text-slate-700 dark:text-slate-300 hover:border-accent-light dark:hover:border-accent-dark hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-all">
                            <i class="ai ai-google-scholar text-lg"></i>
                        </a>
                        <!-- GitHub -->
                        <a href="[GitHub Profile URL]" target="_blank" rel="noopener noreferrer" aria-label="GitHub" title="GitHub"
                           class="p-2.5 rounded-lg bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 text-slate-700 dark:text-slate-300 hover:border-accent-light dark:hover:border-accent-dark hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-all">
                            <i class="fab fa-github text-lg"></i>
                        </a>
                        <!-- Twitter / X -->
                        <a href="[Twitter/X Profile URL]" target="_blank" rel="noopener noreferrer" aria-label="Twitter / X" title="Twitter / X"
                           class="p-2.5 rounded-lg bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 text-slate-700 dark:text-slate-300 hover:border-accent-light dark:hover:border-accent-dark hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-all">
                            <i class="fab fa-x-twitter text-lg"></i>
                        </a>
                        <!-- LinkedIn (Optional) -->
                        <a href="[LinkedIn URL]" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn" title="LinkedIn"
                           class="p-2.5 rounded-lg bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 text-slate-700 dark:text-slate-300 hover:border-accent-light dark:hover:border-accent-dark hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-all">
                            <i class="fab fa-linkedin-in text-lg"></i>
                        </a>
                        <!-- Curriculum Vitae (PDF) -->
                        <a href="[assets/cv.pdf]" target="_blank" rel="noopener noreferrer"
                           class="inline-flex items-center gap-1.5 px-3.5 py-2 rounded-lg bg-slate-900 dark:bg-slate-100 text-white dark:text-slate-900 text-sm font-medium hover:bg-accent-light dark:hover:bg-accent-dark dark:hover:text-slate-950 shadow-sm transition-colors">
                            <i class="ai ai-cv text-base"></i>
                            <span>CV (PDF)</span>
                        </a>
                    </div>
                </div>
            </aside>

            <!-- RIGHT MAIN CONTENT -->
            <main class="md:col-span-8 lg:col-span-8 space-y-14">

                <!-- 1. ABOUT ME SECTION -->
                <section id="about" class="scroll-mt-24">
                    <h2 class="font-serif text-xl sm:text-2xl font-bold text-slate-900 dark:text-white pb-2 border-b border-slate-200 dark:border-slate-800">
                        About Me
                    </h2>
                    <div class="mt-4 space-y-4 text-slate-700 dark:text-slate-300 leading-relaxed text-[15.5px]">
                        <p>
                            I am a [Year, e.g., third-year] PhD student in the <a href="[Department URL]" class="text-accent-light dark:text-accent-dark hover:underline">[Department Name]</a> at <a href="[University URL]" class="text-accent-light dark:text-accent-dark hover:underline">[University Name]</a>, where I am fortunate to be advised by <a href="[Advisor URL]" class="text-accent-light dark:text-accent-dark hover:underline">Prof. [Advisor Name]</a>.
                        </p>
                        <p>
                            My research focuses on <strong>[Primary Research Area]</strong>, <strong>[Secondary Research Area]</strong>, and <strong>[Third Research Area]</strong>. Specifically, I am interested in developing [brief 1-sentence description of your core methodology, theoretical focus, or real-world impact].
                        </p>
                        <p>
                            Previously, I received my [M.S. / B.S.] in [Previous Major] from [Previous University], where I worked with [Previous Advisor/Group] on [Previous Topic].
                        </p>
                    </div>

                    <!-- Research Interests Tags -->
                    <div class="mt-5">
                        <h3 class="text-xs font-semibold uppercase tracking-wider text-slate-500 dark:text-slate-400 mb-2.5">
                            Research Interests
                        </h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 rounded-full text-xs font-medium bg-slate-200/70 dark:bg-slate-800/80 text-slate-700 dark:text-slate-300">
                                [Research Interest 1]
                            </span>
                            <span class="px-3 py-1 rounded-full text-xs font-medium bg-slate-200/70 dark:bg-slate-800/80 text-slate-700 dark:text-slate-300">
                                [Research Interest 2]
                            </span>
                            <span class="px-3 py-1 rounded-full text-xs font-medium bg-slate-200/70 dark:bg-slate-800/80 text-slate-700 dark:text-slate-300">
                                [Research Interest 3]
                            </span>
                            <span class="px-3 py-1 rounded-full text-xs font-medium bg-slate-200/70 dark:bg-slate-800/80 text-slate-700 dark:text-slate-300">
                                [Research Interest 4]
                            </span>
                        </div>
                    </div>
                </section>

                <!-- 2. NEWS / UPDATES TIMELINE -->
                <section id="news" class="scroll-mt-24">
                    <h2 class="font-serif text-xl sm:text-2xl font-bold text-slate-900 dark:text-white pb-2 border-b border-slate-200 dark:border-slate-800">
                        News &amp; Updates
                    </h2>
                    <ul class="mt-4 space-y-3 text-sm sm:text-[15px] text-slate-700 dark:text-slate-300">
                        <li class="flex flex-col sm:flex-row sm:items-baseline gap-1 sm:gap-4">
                            <span class="font-mono text-xs font-semibold text-slate-500 dark:text-slate-400 shrink-0 w-24">
                                [Nov 2026]
                            </span>
                            <span>
                                Our paper <em>"[Paper Title]"</em> was accepted at <strong>[Conference/Journal Name 2026]</strong>!
                            </span>
                        </li>
                        <li class="flex flex-col sm:flex-row sm:items-baseline gap-1 sm:gap-4">
                            <span class="font-mono text-xs font-semibold text-slate-500 dark:text-slate-400 shrink-0 w-24">
                                [Aug 2026]
                            </span>
                            <span>
                                Presented our work on [Topic] at the [Workshop/Symposium Name] in [City, Country].
                            </span>
                        </li>
                        <li class="flex flex-col sm:flex-row sm:items-baseline gap-1 sm:gap-4">
                            <span class="font-mono text-xs font-semibold text-slate-500 dark:text-slate-400 shrink-0 w-24">
                                [May 2026]
                            </span>
                            <span>
                                Started a summer research internship at <strong>[Company / National Lab]</strong> working with [Mentor Name].
                            </span>
                        </li>
                        <li class="flex flex-col sm:flex-row sm:items-baseline gap-1 sm:gap-4">
                            <span class="font-mono text-xs font-semibold text-slate-500 dark:text-slate-400 shrink-0 w-24">
                                [Sep 2025]
                            </span>
                            <span>
                                Passed my PhD qualifying exam!
                            </span>
                        </li>
                    </ul>
                </section>

                <!-- 3. PUBLICATIONS SECTION -->
                <section id="publications" class="scroll-mt-24">
                    <div class="flex items-baseline justify-between pb-2 border-b border-slate-200 dark:border-slate-800">
                        <h2 class="font-serif text-xl sm:text-2xl font-bold text-slate-900 dark:text-white">
                            Publications
                        </h2>
                        <span class="text-xs text-slate-500 dark:text-slate-400">
                            (* indicates equal contribution)
                        </span>
                    </div>

                    <div class="mt-6 space-y-7">
                        
                        <!-- Publication Item 1 -->
                        <article class="group">
                            <h3 class="font-semibold text-base sm:text-[17px] text-slate-900 dark:text-white leading-snug">
                                [Title of Your Most Recent Paper: A Subtitle Explaining the Core Contribution]
                            </h3>
                            <p class="mt-1 text-sm text-slate-600 dark:text-slate-300">
                                <strong class="font-semibold text-slate-900 dark:text-white underline decoration-slate-300 dark:decoration-slate-600 underline-offset-2">[Your Name]</strong>*, [Co-author Two]*, [Co-author Three], [Advisor Name]
                            </p>
                            <p class="mt-0.5 text-sm italic text-slate-500 dark:text-slate-400">
                                [Conference or Journal Name (e.g., NeurIPS / ACL / Nature)], [2026]
                                <span class="not-italic ml-2 inline-flex items-center px-2 py-0.5 rounded text-xs font-medium bg-amber-100 text-amber-800 dark:bg-amber-900/40 dark:text-amber-300">
                                    Spotlight / Best Paper Award
                                </span>
                            </p>

                            <!-- Action Pill Buttons -->
                            <div class="mt-2.5 flex flex-wrap items-center gap-2">
                                <a href="[Link to PDF]" target="_blank" rel="noopener noreferrer"
                                   class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors">
                                    <i class="far fa-file-pdf"></i> PDF
                                </a>
                                <a href="[Link to GitHub Repo]" target="_blank" rel="noopener noreferrer"
                                   class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors">
                                    <i class="fab fa-github"></i> Code
                                </a>
                                <a href="[Link to Project Page]" target="_blank" rel="noopener noreferrer"
                                   class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors">
                                    <i class="fas fa-globe"></i> Project Page
                                </a>
                                <button type="button" onclick="toggleBibtex('bib-1')" aria-expanded="false" aria-controls="bib-1"
                                        class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors cursor-pointer">
                                    <i class="fas fa-quote-right"></i> BibTeX
                                </button>
                            </div>

                            <!-- Collapsible BibTeX Box -->
                            <div id="bib-1" class="hidden mt-3 relative rounded-lg bg-slate-100 dark:bg-slate-900 border border-slate-200 dark:border-slate-800 p-3.5">
                                <button type="button" onclick="copyBibtex('bib-1-code', this)"
                                        class="absolute top-2.5 right-2.5 px-2.5 py-1 rounded-md text-xs font-medium bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 text-slate-600 dark:text-slate-300 hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-colors">
                                    <i class="far fa-copy mr-1"></i>Copy
                                </button>
                                <pre id="bib-1-code" class="text-xs font-mono text-slate-700 dark:text-slate-300 overflow-x-auto pr-16 leading-relaxed">@inproceedings{yourlastname2026title,
  title     = {[Title of Your Most Recent Paper: A Subtitle Explaining the Core Contribution]},
  author    = {[Your Lastname, Your Firstname] and [Coauthor, Two] and [Advisor, Name]},
  booktitle = {[Conference or Journal Name]},
  year      = {2026}
}</pre>
                            </div>
                        </article>

                        <!-- Publication Item 2 -->
                        <article class="group">
                            <h3 class="font-semibold text-base sm:text-[17px] text-slate-900 dark:text-white leading-snug">
                                [Second Paper Title: Exploring Methods in Your Domain]
                            </h3>
                            <p class="mt-1 text-sm text-slate-600 dark:text-slate-300">
                                [First Author], <strong class="font-semibold text-slate-900 dark:text-white underline decoration-slate-300 dark:decoration-slate-600 underline-offset-2">[Your Name]</strong>, [Advisor Name]
                            </p>
                            <p class="mt-0.5 text-sm italic text-slate-500 dark:text-slate-400">
                                [Journal or Workshop Name], [2025]
                            </p>

                            <!-- Action Pill Buttons -->
                            <div class="mt-2.5 flex flex-wrap items-center gap-2">
                                <a href="[Link to PDF]" target="_blank" rel="noopener noreferrer"
                                   class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors">
                                    <i class="far fa-file-pdf"></i> PDF
                                </a>
                                <a href="[Link to GitHub Repo]" target="_blank" rel="noopener noreferrer"
                                   class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors">
                                    <i class="fab fa-github"></i> Code
                                </a>
                                <button type="button" onclick="toggleBibtex('bib-2')" aria-expanded="false" aria-controls="bib-2"
                                        class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full text-xs font-medium border border-slate-300 dark:border-slate-700 text-slate-700 dark:text-slate-200 hover:border-accent-light hover:text-accent-light dark:hover:border-accent-dark dark:hover:text-accent-dark transition-colors cursor-pointer">
                                    <i class="fas fa-quote-right"></i> BibTeX
                                </button>
                            </div>

                            <!-- Collapsible BibTeX Box -->
                            <div id="bib-2" class="hidden mt-3 relative rounded-lg bg-slate-100 dark:bg-slate-900 border border-slate-200 dark:border-slate-800 p-3.5">
                                <button type="button" onclick="copyBibtex('bib-2-code', this)"
                                        class="absolute top-2.5 right-2.5 px-2.5 py-1 rounded-md text-xs font-medium bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 text-slate-600 dark:text-slate-300 hover:text-accent-light dark:hover:text-accent-dark shadow-sm transition-colors">
                                    <i class="far fa-copy mr-1"></i>Copy
                                </button>
                                <pre id="bib-2-code" class="text-xs font-mono text-slate-700 dark:text-slate-300 overflow-x-auto pr-16 leading-relaxed">@article{firstauthor2025second,
  title   = {[Second Paper Title: Exploring Methods in Your Domain]},
  author  = {[First, Author] and [Your Lastname, Your Firstname] and [Advisor, Name]},
  journal = {[Journal or Workshop Name]},
  year    = {2025}
}</pre>
                            </div>
                        </article>

                    </div>
                </section>

                <!-- 4. TEACHING, SERVICE & SELECTED PROJECTS -->
                <section id="teaching" class="scroll-mt-24">
                    <h2 class="font-serif text-xl sm:text-2xl font-bold text-slate-900 dark:text-white pb-2 border-b border-slate-200 dark:border-slate-800">
                        Teaching, Service &amp; Projects
                    </h2>

                    <div class="mt-5 grid grid-cols-1 sm:grid-cols-2 gap-6">
                        
                        <!-- Teaching Experience -->
                        <div class="p-4 rounded-xl bg-white dark:bg-slate-900/60 border border-slate-200/80 dark:border-slate-800">
                            <h3 class="font-semibold text-base text-slate-900 dark:text-white flex items-center gap-2">
                                <i class="fas fa-chalkboard-teacher text-accent-light dark:text-accent-dark text-sm"></i>
                                Teaching
                            </h3>
                            <ul class="mt-3 space-y-2.5 text-sm text-slate-600 dark:text-slate-300">
                                <li>
                                    <div class="font-medium text-slate-800 dark:text-slate-200">[CS 101: Introduction to Field]</div>
                                    <div class="text-xs text-slate-500 dark:text-slate-400">Head Teaching Assistant &bull; [Fall 2025]</div>
                                </li>
                                <li>
                                    <div class="font-medium text-slate-800 dark:text-slate-200">[CS 402: Advanced Topics in Field]</div>
                                    <div class="text-xs text-slate-500 dark:text-slate-400">Teaching Assistant &bull; [Spring 2025]</div>
                                </li>
                            </ul>
                        </div>

                        <!-- Academic Service -->
                        <div class="p-4 rounded-xl bg-white dark:bg-slate-900/60 border border-slate-200/80 dark:border-slate-800">
                            <h3 class="font-semibold text-base text-slate-900 dark:text-white flex items-center gap-2">
                                <i class="fas fa-award text-accent-light dark:text-accent-dark text-sm"></i>
                                Academic Service
                            </h3>
                            <ul class="mt-3 space-y-2.5 text-sm text-slate-600 dark:text-slate-300">
                                <li>
                                    <div class="font-medium text-slate-800 dark:text-slate-200">Reviewer</div>
                                    <div class="text-xs text-slate-500 dark:text-slate-400">[Conference A 2026], [Conference B 2025]</div>
                                </li>
                                <li>
                                    <div class="font-medium text-slate-800 dark:text-slate-200">Organizer</div>
                                    <div class="text-xs text-slate-500 dark:text-slate-400">[University Reading Group / Workshop]</div>
                                </li>
                            </ul>
                        </div>

                    </div>

                    <!-- Open-Source / Side Projects -->
                    <div class="mt-6">
                        <h3 class="text-xs font-semibold uppercase tracking-wider text-slate-500 dark:text-slate-400 mb-3">
                            Selected Open-Source &amp; Research Software
                        </h3>
                        <div class="space-y-3">
                            <div class="p-4 rounded-xl bg-white dark:bg-slate-900/60 border border-slate-200/80 dark:border-slate-800 flex flex-col sm:flex-row sm:items-center justify-between gap-3">
                                <div>
                                    <a href="[Project GitHub URL]" target="_blank" rel="noopener noreferrer" class="font-semibold text-sm text-slate-900 dark:text-white hover:text-accent-light dark:hover:text-accent-dark transition-colors">
                                        [Project-Name-Toolkit] <i class="fas fa-arrow-up-right-from-square text-[11px] ml-1 opacity-70"></i>
                                    </a>
                                    <p class="text-xs sm:text-sm text-slate-600 dark:text-slate-400 mt-0.5">
                                        [A lightweight Python/PyTorch library for benchmarking models in your research area.]
                                    </p>
                                </div>
                                <span class="self-start sm:self-center shrink-0 px-2.5 py-1 rounded-md text-xs font-mono bg-slate-100 dark:bg-slate-800 text-slate-600 dark:text-slate-300">
                                    Python &bull; MIT
                                </span>
                            </div>
                        </div>
                    </div>
                </section>

            </main>
        </div>
    </div>

    <!-- Minimal Academic Footer -->
    <footer class="border-t border-slate-200/80 dark:border-slate-800/80 py-8 mt-12">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs text-slate-500 dark:text-slate-400">
            <p>&copy; <span id="current-year">2026</span> [Your Name]. All rights reserved.</p>
            <p>Last updated: [November 2026] &bull; Hosted on GitHub Pages</p>
        </div>
    </footer>

    <!-- Minimal Vanilla JavaScript for Interactivity -->
    <script>
        // 1. Set Current Year in Footer
        document.getElementById('current-year').textContent = new Date().getFullYear();

        // 2. Dark / Light Mode Toggle Logic
        const themeToggleBtns = [
            document.getElementById('theme-toggle'),
            document.getElementById('theme-toggle-mobile')
        ];

        function updateThemeIcons() {
            const isDark = document.documentElement.classList.contains('dark');
            document.getElementById('theme-icon-light').classList.toggle('hidden', !isDark);
            document.getElementById('theme-icon-dark').classList.toggle('hidden', isDark);
            document.getElementById('theme-icon-light-mobile').classList.toggle('hidden', !isDark);
            document.getElementById('theme-icon-dark-mobile').classList.toggle('hidden', isDark);
        }

        // Initialize icons on load
        updateThemeIcons();

        themeToggleBtns.forEach(btn => {
            if (!btn) return;
            btn.addEventListener('click', () => {
                const isDark = document.documentElement.classList.toggle('dark');
                localStorage.theme = isDark ? 'dark' : 'light';
                updateThemeIcons();
            });
        });

        // 3. Mobile Navigation Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        mobileMenuBtn.addEventListener('click', () => {
            const isExpanded = mobileMenu.classList.toggle('hidden');
            mobileMenuBtn.setAttribute('aria-expanded', !isExpanded);
        });

        // Close mobile menu when a navigation link is clicked
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                mobileMenuBtn.setAttribute('aria-expanded', 'false');
            });
        });

        // 4. Toggle BibTeX Citation Box
        function toggleBibtex(id) {
            const bibBox = document.getElementById(id);
            const triggerBtn = document.querySelector(`[aria-controls="${id}"]`);
            if (!bibBox) return;

            const isHidden = bibBox.classList.toggle('hidden');
            if (triggerBtn) {
                triggerBtn.setAttribute('aria-expanded', !isHidden);
            }
        }

        // 5. Copy BibTeX to Clipboard (Compatible with iFrames & GitHub Pages)
        function copyBibtex(codeElementId, buttonElement) {
            const codeEl = document.getElementById(codeElementId);
            if (!codeEl) return;

            const textToCopy = codeEl.textContent;
            const tempTextArea = document.createElement('textarea');
            tempTextArea.value = textToCopy;
            tempTextArea.style.position = 'fixed';
            tempTextArea.style.opacity = '0';
            document.body.appendChild(tempTextArea);
            tempTextArea.select();

            try {
                document.execCommand('copy');
                const originalHTML = buttonElement.innerHTML;
                buttonElement.innerHTML = '<i class="fas fa-check text-emerald-600 dark:text-emerald-400 mr-1"></i>Copied!';
                setTimeout(() => {
                    buttonElement.innerHTML = originalHTML;
                }, 2000);
            } catch (err) {
                console.error('Failed to copy BibTeX:', err);
            } finally {
                document.body.removeChild(tempTextArea);
            }
        }
    </script>
</body>
</html>
