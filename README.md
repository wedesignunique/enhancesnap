<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Enhance Snap - Free AI Image Enhancer – Improve Photo Quality Online</title>
    <meta name="description" content="Use our free AI photo enhancer to fix blurry or low-quality images instantly. No sign-up needed – upload and download with one click.">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.1/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        }
        .drop-zone {
            border: 2px dashed #4F46E5;
            transition: all 0.3s ease;
        }
        .drop-zone:hover {
            background-color: #EEF2FF;
        }
        .theme-toggle:checked + .toggle-bg:after {
            transform: translateX(100%);
        }
        .theme-toggle:checked + .toggle-bg {
            background-color: #4F46E5;
        }
        .image-comparison {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }
        .comparison-slider {
            position: absolute;
            z-index: 10;
            width: 40px;
            height: 40px;
            background-color: #4F46E5;
            border-radius: 50%;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            cursor: ew-resize;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
        }
        .comparison-slider:after, .comparison-slider:before {
            content: '';
            position: absolute;
            width: 2px;
            height: 24px;
            background-color: white;
            left: 19px;
            top: 8px;
        }
        .comparison-slider:before {
            transform: rotate(90deg);
        }
        .separator {
            position: absolute;
            width: 2px;
            height: 100%;
            background-color: #4F46E5;
            z-index: 5;
            left: 50%;
            transform: translateX(-50%);
        }
        .image-before, .image-after {
            position: absolute;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }
        .image-before {
            left: 0;
            width: 50%;
        }
        .image-after {
            right: 0;
            width: 50%;
        }
        .toggle-bg:after {
            content: '';
            position: absolute;
            top: 2px;
            left: 2px;
            width: 20px;
            height: 20px;
            background-color: white;
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        /* Dark mode styles */
        .dark {
            background-color: #1F2937;
            color: #F3F4F6;
        }
        .dark header {
            background-color: #111827;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.3);
        }
        .dark .bg-white {
            background-color: #111827;
        }
        .dark .text-gray-800, .dark .text-gray-900 {
            color: #F3F4F6;
        }
        .dark .text-gray-600, .dark .text-gray-500, .dark .text-gray-400 {
            color: #D1D5DB;
        }
        .dark .bg-gray-50, .dark .bg-gray-100, .dark .bg-gray-200 {
            background-color: #1F2937;
        }
        .dark .shadow-md, .dark .shadow-lg, .dark .shadow-sm {
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.5);
        }
        .dark .border-gray-300, .dark .border-gray-800 {
            border-color: #374151;
        }
        .dark .drop-zone {
            border-color: #6366F1;
        }
        .dark .drop-zone:hover {
            background-color: #2D3748;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">
    <!-- Header -->
    <header class="bg-white shadow-sm">
        <div class="container mx-auto px-4 py-4 flex items-center justify-between">
            <div class="flex items-center space-x-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
                </svg>
                <h1 class="text-xl font-bold text-indigo-600">Enhance Snap</h1>
            </div>
            <nav class="hidden md:flex space-x-6">
                <a href="#home" class="font-medium hover:text-indigo-600 transition">Home</a>
                <a href="#how-it-works" class="font-medium hover:text-indigo-600 transition">How It Works</a>
                <a href="#faq" class="font-medium hover:text-indigo-600 transition">FAQ</a>
                <a href="#blog" class="font-medium hover:text-indigo-600 transition">Blog</a>
            </nav>
            <div class="flex items-center space-x-4">
                <label class="flex items-center cursor-pointer">
                    <div class="relative">
                        <input type="checkbox" id="theme-toggle" class="theme-toggle sr-only">
                        <div class="toggle-bg block w-10 h-6 rounded-full bg-gray-300 transition relative"></div>
                    </div>
                    <div class="ml-2 text-sm">
                        <i class="fas fa-moon"></i>
                    </div>
                </label>
                <button class="hidden md:block bg-indigo-600 hover:bg-indigo-700 text-white font-medium px-4 py-2 rounded-lg transition">
                    Sign Up Free
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="pt-12 pb-24 px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-12">
                <h1 class="text-4xl md:text-5xl font-bold mb-4 text-gray-900">Transform Blurry Photos into Crystal Clear Images</h1>
                <p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto">
                    Our AI-powered tool enhances your low-quality images instantly. Free, fast, and no sign-up required.
                </p>
            </div>

            <div class="bg-white rounded-xl shadow-lg p-6 md:p-8 mb-12">
                <div id="upload-container" class="drop-zone flex flex-col items-center justify-center border-dashed rounded-lg p-8 md:p-12 text-center cursor-pointer">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 text-indigo-500 mb-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12" />
                    </svg>
                    <h3 class="text-xl font-semibold mb-2">Drag & Drop Your Image Here</h3>
                    <p class="text-gray-500 mb-4">Or click to browse files</p>
                    <p class="text-sm text-gray-400">Supports JPG, PNG, WEBP (Max: 10MB)</p>
                    <input type="file" id="file-input" class="hidden" accept="image/jpeg,image/png,image/webp">
                </div>
                
                <div id="preview-container" class="hidden mt-8">
                    <div class="mb-4">
                        <h3 class="text-lg font-semibold mb-2">Enhancing Your Image...</h3>
                        <div class="relative h-4 bg-gray-200 rounded-full overflow-hidden">
                            <div id="progress-bar" class="absolute top-0 left-0 h-full bg-indigo-600 transition-all duration-300" style="width: 0%"></div>
                        </div>
                    </div>

                    <div class="relative h-[300px] md:h-[400px] bg-gray-100 rounded-lg mb-6 overflow-hidden">
                        <div class="image-comparison h-full">
                            <div class="comparison-slider"></div>
                            <div class="separator"></div>
                            <div class="image-before">
                                <img id="before-image" class="w-full h-full object-contain" alt="Original image">
                            </div>
                            <div class="image-after">
                                <img id="after-image" class="w-full h-full object-contain" alt="Enhanced image">
                            </div>
                        </div>
                    </div>

                    <div class="flex flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-4">
                        <button id="download-btn" class="w-full md:w-auto bg-indigo-600 hover:bg-indigo-700 text-white font-medium px-6 py-3 rounded-lg transition flex items-center justify-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M3 17a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zm3.293-7.707a1 1 0 011.414 0L9 10.586V3a1 1 0 112 0v7.586l1.293-1.293a1 1 0 111.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                            Download Enhanced Image
                        </button>
                        <button id="try-another-btn" class="w-full md:w-auto bg-white border border-gray-300 hover:bg-gray-50 text-gray-700 font-medium px-6 py-3 rounded-lg transition flex items-center justify-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M4 2a1 1 0 011 1v2.101a7.002 7.002 0 0111.601 2.566 1 1 0 11-1.885.666A5.002 5.002 0 005.999 7H9a1 1 0 010 2H4a1 1 0 01-1-1V3a1 1 0 011-1zm.008 9.057a1 1 0 011.276.61A5.002 5.002 0 0014.001 13H11a1 1 0 110-2h5a1 1 0 011 1v5a1 1 0 11-2 0v-2.101a7.002 7.002 0 01-11.601-2.566 1 1 0 01.61-1.276z" clip-rule="evenodd" />
                            </svg>
                            Try Another Image
                        </button>
                    </div>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-12">
                <div class="bg-white rounded-xl shadow-md p-6 flex flex-col items-center text-center">
                    <div class="bg-indigo-100 p-3 rounded-full mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                        </svg>
                    </div>
                    <h3 class="text-lg font-semibold mb-2">Lightning Fast</h3>
                    <p class="text-gray-600">Get enhanced images in seconds, not minutes. Our optimized AI model works at lightning speed.</p>
                </div>
                <div class="bg-white rounded-xl shadow-md p-6 flex flex-col items-center text-center">
                    <div class="bg-indigo-100 p-3 rounded-full mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z" />
                        </svg>
                    </div>
                    <h3 class="text-lg font-semibold mb-2">100% Private</h3>
                    <p class="text-gray-600">Your images are processed securely and never stored on our servers. Your privacy is guaranteed.</p>
                </div>
                <div class="bg-white rounded-xl shadow-md p-6 flex flex-col items-center text-center">
                    <div class="bg-indigo-100 p-3 rounded-full mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
                        </svg>
                    </div>
                    <h3 class="text-lg font-semibold mb-2">Advanced AI</h3>
                    <p class="text-gray-600">Powered by state-of-the-art neural networks that restore details even in severely degraded images.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works Section -->
    <section id="how-it-works" class="py-16 bg-indigo-50 px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-4">How It Works</h2>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">
                    Enhance Snap uses advanced AI models to restore and improve your images in three simple steps.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white rounded-xl shadow-md p-6 relative">
                    <div class="absolute -top-4 -left-4 w-12 h-12 bg-indigo-600 rounded-full text-white flex items-center justify-center text-xl font-bold">1</div>
                    <h3 class="text-xl font-semibold mb-4 mt-2">Upload Your Image</h3>
                    <p class="text-gray-600 mb-4">Drag and drop or browse to upload your low-quality, blurry, or pixelated image.</p>
                    <div class="bg-gray-100 rounded-lg p-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-indigo-500 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-8l-4-4m0 0L8 8m4-4v12" />
                        </svg>
                    </div>
                </div>
                <div class="bg-white rounded-xl shadow-md p-6 relative">
                    <div class="absolute -top-4 -left-4 w-12 h-12 bg-indigo-600 rounded-full text-white flex items-center justify-center text-xl font-bold">2</div>
                    <h3 class="text-xl font-semibold mb-4 mt-2">AI Enhancement</h3>
                    <p class="text-gray-600 mb-4">Our AI algorithms analyze your image and enhance it pixel by pixel to improve quality.</p>
                    <div class="bg-gray-100 rounded-lg p-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-indigo-500 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
                        </svg>
                    </div>
                </div>
                <div class="bg-white rounded-xl shadow-md p-6 relative">
                    <div class="absolute -top-4 -left-4 w-12 h-12 bg-indigo-600 rounded-full text-white flex items-center justify-center text-xl font-bold">3</div>
                    <h3 class="text-xl font-semibold mb-4 mt-2">Download Result</h3>
                    <p class="text-gray-600 mb-4">Instantly download your enhanced, high-resolution image ready for use.</p>
                    <div class="bg-gray-100 rounded-lg p-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10 text-indigo-500 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4" />
                        </svg>
                    </div>
                </div>
            </div>

            <div class="mt-12 bg-white rounded-xl shadow-md overflow-hidden">
                <div class="p-6 md:p-8">
                    <h3 class="text-xl font-semibold mb-4">The Technology Behind Enhance Snap</h3>
                    <p class="text-gray-600 mb-6">
                        Enhance Snap utilizes state-of-the-art deep learning models trained on millions of images. Our AI can:
                    </p>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Increase resolution up to 4x</p>
                        </div>
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Remove blur and motion artifacts</p>
                        </div>
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Reconstruct missing details</p>
                        </div>
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Improve contrast and sharpness</p>
                        </div>
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Reduce JPEG compression artifacts</p>
                        </div>
                        <div class="flex items-start">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500 mt-0.5 mr-2 flex-shrink-0" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <p>Intelligently fix facial features</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section id="faq" class="py-16 px-4">
        <div class="container mx-auto max-w-4xl">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-4">Frequently Asked Questions</h2>
                <p class="text-lg text-gray-600">
                    Got questions? We've got answers.
                </p>
            </div>

            <div class="space-y-4">
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-semibold flex justify-between items-center focus:outline-none">
                        <span>Is Enhance Snap really free to use?</span>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-600" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </button>
                    <div class="px-6 pb-4">
                        <p class="text-gray-600">
                            Yes! Our basic enhancement features are completely free with no hidden costs. We also offer premium options for higher resolution outputs and batch processing.
                        </p>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-semibold flex justify-between items-center focus:outline-none">
                        <span>What file types are supported?</span>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-600" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </button>
                    <div class="px-6 pb-4">
                        <p class="text-gray-600">
                            Enhance Snap supports JPG, PNG, and WEBP image formats. The maximum file size is 10MB for free users.
                        </p>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-semibold flex justify-between items-center focus:outline-none">
                        <span>How do you handle my data and privacy?</span>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-600" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </button>
                    <div class="px-6 pb-4">
                        <p class="text-gray-600">
                            We take privacy seriously. Your images are processed in real-time and are never stored on our servers. We don't collect any personally identifiable information from your uploads.
                        </p>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-semibold flex justify-between items-center focus:outline-none">
                        <span>Can I enhance multiple images at once?</span>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-600" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </button>
                    <div class="px-6 pb-4">
                        <p class="text-gray-600">
                            Batch processing is available with our premium plan. Free users can enhance one image at a time.
                        </p>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-semibold flex justify-between items-center focus:outline-none">
                        <span>What AI technology powers Enhance Snap?</span>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-600" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                        </svg>
                    </button>
                    <div class="px-6 pb-4">
                        <p class="text-gray-600">
                            We use state-of-the-art deep learning models including Real-ESRGAN and GFPGAN technologies optimized for speed and quality. These models are specifically trained to intelligently enhance various types of images.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Blog Section -->
    <section id="blog" class="py-16 bg-gray-50 px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-4">Latest From Our Blog</h2>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">
                    Tips, tricks, and insights about image enhancement and photography.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-48 bg-gray-200"></div>
                    <div class="p-6">
                        <p class="text-sm text-indigo-600 font-semibold mb-1">Tips & Tricks</p>
                        <h3 class="font-bold text-xl mb-2">How to Fix Blurry Photos: The Complete Guide</h3>
                        <p class="text-gray-600 mb-4">Learn the top techniques for salvaging blurry images using both software tools and camera settings.</p>
                        <div class="flex items-center">
                            <div class="w-8 h-8 rounded-full bg-gray-300 mr-3"></div>
                            <div>
                                <p class="font-medium">Alex Johnson</p>
                                <p class="text-sm text-gray-500">May 12, 2023 · 5 min read</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-48 bg-gray-200"></div>
                    <div class="p-6">
                        <p class="text-sm text-indigo-600 font-semibold mb-1">Technology</p>
                        <h3 class="font-bold text-xl mb-2">The Science Behind AI Image Enhancement</h3>
                        <p class="text-gray-600 mb-4">Discover how neural networks are revolutionizing image upscaling and restoration technology.</p>
                        <div class="flex items-center">
                            <div class="w-8 h-8 rounded-full bg-gray-300 mr-3"></div>
                            <div>
                                <p class="font-medium">Maria Chen</p>
                                <p class="text-sm text-gray-500">April 28, 2023 · 8 min read</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="h-48 bg-gray-200"></div>
                    <div class="p-6">
                        <p class="text-sm text-indigo-600 font-semibold mb-1">Tutorials</p>
                        <h3 class="font-bold text-xl mb-2">Restoring Old Family Photos: Step by Step</h3>
                        <p class="text-gray-600 mb-4">A comprehensive guide to bringing your damaged or faded family photographs back to life.</p>
                        <div class="flex items-center">
                            <div class="w-8 h-8 rounded-full bg-gray-300 mr-3"></div>
                            <div>
                                <p class="font-medium">James Wilson</p>
                                <p class="text-sm text-gray-500">April 15, 2023 · 6 min read</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="text-center mt-10">
                <button class="bg-white hover:bg-gray-50 text-indigo-600 font-medium px-6 py-3 rounded-lg border border-indigo-200 shadow-sm transition inline-flex items-center">
                    View All Articles
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-2" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                    </svg>
                </button>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="py-16 bg-gradient-to-r from-indigo-600 to-indigo-800 text-white px-4">
        <div class="container mx-auto max-w-4xl text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-6">Ready to Transform Your Images?</h2>
            <p class="text-xl mb-8 text-indigo-100">
                Join thousands of users who enhance their photos with Enhance Snap every day.
            </p>
            <div class="flex flex-col md:flex-row items-center justify-center space-y-4 md:space-y-0 md:space-x-4">
                <a href="#home" class="bg-white text-indigo-700 hover:bg-indigo-50 font-medium px-8 py-3 rounded-lg shadow-lg transition">
                    Enhance Your Image Now
                </a>
                <a href="#premium" class="bg-transparent hover:bg-indigo-700 border-2 border-white font-medium px-8 py-3 rounded-lg transition">
                    Explore Premium Features
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12 px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <div>
                    <div class="flex items-center space-x-2 mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-indigo-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
                        </svg>
                        <h3 class="text-xl font-bold text-indigo-400">Enhance Snap</h3>
                    </div>
                    <p class="text-gray-400">
                        The ultimate AI image enhancement tool. Transform blurry, low-quality images into crystal clear pictures instantly.
                    </p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Product</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Features</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Pricing</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">API</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Integrations</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Resources</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Documentation</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Tutorials</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Support</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Company</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Careers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Privacy Policy</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Terms of Service</a></li>
                    </ul>
                </div>
            </div>
            <div class="pt-8 border-t border-gray-800 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 mb-4 md:mb-0">© 2023 Enhance Snap. All rights reserved.</p>
                <div class="flex space-x-4">
                    <a href="#" class="text-gray-400 hover:text-white transition">
                        <i class="fab fa-twitter text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition">
                        <i class="fab fa-facebook-f text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition">
                        <i class="fab fa-instagram text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition">
                        <i class="fab fa-github text-xl"></i>
                    </a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // DOM Elements
        const uploadContainer = document.getElementById('upload-container');
        const fileInput = document.getElementById('file-input');
        const previewContainer = document.getElementById('preview-container');
        const progressBar = document.getElementById('progress-bar');
        const beforeImage = document.getElementById('before-image');
        const afterImage = document.getElementById('after-image');
        const downloadBtn = document.getElementById('download-btn');
        const tryAnotherBtn = document.getElementById('try-another-btn');
        const themeToggle = document.getElementById('theme-toggle');
        
        // Variables to store file information
        let uploadedFile = null;
        let uploadedFileName = '';
        let uploadedFileType = '';
        let enhancedImageData = '';
        
        // Theme Toggle functionality
        themeToggle.addEventListener('change', () => {
            document.body.classList.toggle('dark');
        });
        
        // Event Listeners
        uploadContainer.addEventListener('click', () => fileInput.click());
        uploadContainer.addEventListener('dragover', (e) => {
            e.preventDefault();
            uploadContainer.classList.add('bg-indigo-50');
        });
        uploadContainer.addEventListener('dragleave', () => {
            uploadContainer.classList.remove('bg-indigo-50');
        });
        uploadContainer.addEventListener('drop', (e) => {
            e.preventDefault();
            uploadContainer.classList.remove('bg-indigo-50');
            if (e.dataTransfer.files.length) {
                handleFile(e.dataTransfer.files[0]);
            }
        });
        fileInput.addEventListener('change', () => {
            if (fileInput.files.length) {
                handleFile(fileInput.files[0]);
            }
        });
        
        tryAnotherBtn.addEventListener('click', () => {
            previewContainer.classList.add('hidden');
            uploadContainer.classList.remove('hidden');
            fileInput.value = '';
            uploadedFile = null;
            uploadedFileName = '';
            uploadedFileType = '';
            enhancedImageData = '';
        });
        
        downloadBtn.addEventListener('click', () => {
            if (enhancedImageData) {
                const link = document.createElement('a');
                link.href = enhancedImageData;
                
                // Maintain the original file extension
                const dotIndex = uploadedFileName.lastIndexOf('.');
                const extension = dotIndex > 0 ? uploadedFileName.substring(dotIndex) : '.png';
                
                // Create the enhanced file name
                const nameWithoutExt = uploadedFileName.substring(0, dotIndex > 0 ? dotIndex : uploadedFileName.length);
                const enhancedName = nameWithoutExt + '-enhanced' + extension;
                
                link.download = enhancedName;
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
            }
        });
        
        // Functions
        function handleFile(file) {
            if (!file.type.match('image.*')) {
                alert('Please upload an image file (JPG, PNG, or WEBP)');
                return;
            }
            
            uploadedFile = file;
            uploadedFileName = file.name;
            uploadedFileType = file.type;
            
            const reader = new FileReader();
            reader.onload = (e) => {
                beforeImage.src = e.target.result;
                uploadContainer.classList.add('hidden');
                previewContainer.classList.remove('hidden');
                
                // Simulate processing with actual enhancement
                simulateProcessing(e.target.result);
            };
            reader.readAsDataURL(file);
        }
        
        function simulateProcessing(imageData) {
            let progress = 0;
            const interval = setInterval(() => {
                progress += 5;
                progressBar.style.width = `${progress}%`;
                
                if (progress >= 100) {
                    clearInterval(interval);
                    // Actually enhance the image
                    enhanceImage(imageData);
                }
            }, 100);
        }
        
        function enhanceImage(imageData) {
            // Create an Image element to hold the image
            const img = new Image();
            img.onload = function() {
                // Create a canvas to process the image
                const canvas = document.createElement('canvas');
                const ctx = canvas.getContext('2d');
                
                // Set the canvas dimensions to match the image
                canvas.width = img.width;
                canvas.height = img.height;
                
                // Draw the original image on the canvas
                ctx.drawImage(img, 0, 0);
                
                // Get the image data from the canvas
                const imgData = ctx.getImageData(0, 0, canvas.width, canvas.height);
                const data = imgData.data;
                
                // Apply image enhancements
                // 1. Increase brightness and contrast
                for (let i = 0; i < data.length; i += 4) {
                    // Brightness increase
                    data[i] = Math.min(255, data[i] * 1.1);     // Red
                    data[i+1] = Math.min(255, data[i+1] * 1.1); // Green
                    data[i+2] = Math.min(255, data[i+2] * 1.1); // Blue
                    
                    // Contrast enhancement
                    data[i] = Math.min(255, Math.max(0, (data[i] - 128) * 1.2 + 128));
                    data[i+1] = Math.min(255, Math.max(0, (data[i+1] - 128) * 1.2 + 128));
                    data[i+2] = Math.min(255, Math.max(0, (data[i+2] - 128) * 1.2 + 128));
                }
                
                // Apply a sharpening filter
                const sharpenKernel = [
                    0, -1, 0,
                    -1, 5, -1,
                    0, -1, 0
                ];
                
                // Create a new ImageData object for the sharpened image
                const sharpenedData = ctx.createImageData(canvas.width, canvas.height);
                
                // Apply a simple convolution for sharpening
                for (let y = 1; y < canvas.height - 1; y++) {
                    for (let x = 1; x < canvas.width - 1; x++) {
                        const centerPixel = (y * canvas.width + x) * 4;
                        
                        // For each RGB channel
                        for (let c = 0; c < 3; c++) {
                            let sum = 0;
                            
                            // Apply kernel
                            for (let ky = -1; ky <= 1; ky++) {
                                for (let kx = -1; kx <= 1; kx++) {
                                    const kernel = sharpenKernel[(ky + 1) * 3 + (kx + 1)];
                                    const pixelPos = ((y + ky) * canvas.width + (x + kx)) * 4;
                                    sum += data[pixelPos + c] * kernel;
                                }
                            }
                            
                            // Set the sharpened pixel value
                            sharpenedData.data[centerPixel + c] = Math.min(255, Math.max(0, sum));
                        }
                        
                        // Keep alpha channel unchanged
                        sharpenedData.data[centerPixel + 3] = data[centerPixel + 3];
                    }
                }
                
                // Fix the border pixels that were skipped
                for (let y = 0; y < canvas.height; y++) {
                    for (let x = 0; x < canvas.width; x++) {
                        // If we're at a border
                        if (y === 0 || y === canvas.height - 1 || x === 0 || x === canvas.width - 1) {
                            const pos = (y * canvas.width + x) * 4;
                            sharpenedData.data[pos] = data[pos];
                            sharpenedData.data[pos + 1] = data[pos + 1];
                            sharpenedData.data[pos + 2] = data[pos + 2];
                            sharpenedData.data[pos + 3] = data[pos + 3];
                        }
                    }
                }
                
                // Put the enhanced image data back on the canvas
                ctx.putImageData(sharpenedData, 0, 0);
                
                // Convert the canvas to an image URL
                enhancedImageData = canvas.toDataURL(uploadedFileType);
                
                // Set the after image
                afterImage.src = enhancedImageData;
                
                // Initialize the comparison slider
                initComparisonSlider();
            };
            
            img.src = imageData;
        }
        
        function initComparisonSlider() {
            const slider = document.querySelector('.comparison-slider');
            const beforeDiv = document.querySelector('.image-before');
            const separator = document.querySelector('.separator');
            
            let isDragging = false;
            
            const getPercentage = (pageX) => {
                const container = slider.parentElement;
                const rect = container.getBoundingClientRect();
                const x = pageX - rect.left;
                let percent = (x / rect.width) * 100;
                percent = Math.max(0, Math.min(100, percent));
                return percent;
            };
            
            const updateSlider = (percentage) => {
                beforeDiv.style.width = `${percentage}%`;
                slider.style.left = `${percentage}%`;
                separator.style.left = `${percentage}%`;
            };
            
            slider.addEventListener('mousedown', () => {
                isDragging = true;
            });
            
            document.addEventListener('mouseup', () => {
                isDragging = false;
            });
            
            document.addEventListener('mousemove', (e) => {
                if (!isDragging) return;
                const percentage = getPercentage(e.pageX);
                updateSlider(percentage);
            });
            
            // For touch devices
            slider.addEventListener('touchstart', () => {
                isDragging = true;
            });
            
            document.addEventListener('touchend', () => {
                isDragging = false;
            });
            
            document.addEventListener('touchmove', (e) => {
                if (!isDragging) return;
                const percentage = getPercentage(e.touches[0].pageX);
                updateSlider(percentage);
            });
        }
        
        // FAQ Toggles
        document.querySelectorAll('#faq button').forEach(button => {
            button.addEventListener('click', () => {
                const content = button.nextElementSibling;
                content.style.display = content.style.display === 'block' ? 'none' : 'block';
                
                const icon = button.querySelector('svg');
                icon.style.transform = content.style.display === 'block' ? 'rotate(180deg)' : 'rotate(0)';
            });
        });
    </script>
</body>
</html>
