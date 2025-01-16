```
Project Structure:
├── assets
├── author.hbs
├── codefetch
│   └── output.md
├── custom-account.hbs
├── custom-authors.hbs
├── custom-contact.hbs
├── custom-featured.hbs
├── custom-membership.hbs
├── custom-sign-in.hbs
├── custom-sign-up.hbs
├── custom-subscribe.hbs
├── custom-tags.hbs
├── default-custom.hbs
├── default.hbs
├── error.hbs
├── index.hbs
├── locales
│   └── en.json
├── package.json
├── partials
│   ├── featured.hbs
│   ├── footer.hbs
│   ├── footer_icons.hbs
│   ├── header.hbs
│   ├── hero.hbs
│   ├── item.hbs
│   ├── logo.hbs
│   ├── logo_mode.hbs
│   ├── loop.hbs
│   ├── meta.hbs
│   ├── navigation.hbs
│   ├── pagination.hbs
│   ├── related.hbs
│   ├── search.hbs
│   ├── sections.hbs
│   └── widgets.hbs
├── post-card.hbs
├── post.hbs
├── rough-notes.hbs
└── tag.hbs
```

assets/css/screen.css
```
1 | @import url("https://fonts.cdnfonts.com/css/canela-text-trial");
2 | 
3 | /* General settings */
4 | body,
5 | h1,
6 | h2,
7 | h3,
8 | h4,
9 | h5,
10 | h6,
11 | p,
12 | a,
13 | li,
14 | ul,
15 | div,
16 | span,
17 | header,
18 | footer,
19 | main,
20 | section,
21 | blockquote,
22 | article,
23 | aside,
24 | nav,
25 | figure,
26 | figcaption {
27 |     font-family: "Canela Deck Trial", sans-serif !important;
28 | }
29 | 
30 | 
31 | .post-title,
32 | .global-title,
33 | .featured-title,
34 | .post-content h2,
35 | .kg-card,
36 | .kg-header-card,
37 | post-content blockquote p,
38 | .post-content,
39 | .subscribe-title,
40 | .global-content,
41 | .global-main,
42 | article.post-section.is-sidebar,
43 | .post-wrap,
44 | .global-meta-content,
45 | .global-dynamic-color,
46 | .global-button,
47 | h3.subscribe-title {
48 |     font-family: "Canela Deck Trial", sans-serif !important;
49 | }
50 | 
51 | 
52 | 
53 | /* //////////////////////////////////////////////////////////////////////////
54 | 
55 |    Reiro 1.4.0
56 | 
57 |    //////////////////////////////////////////////////////////////////////////
58 | 
59 |    I. Customize
60 |    |
61 |    ├─ Global settings
62 |    ├─ Fonts
63 |    ├─ Colors
64 |    ├─ Light version
65 |    ├─ Sepia version
66 |    ├─ Dark version
67 |    ├─ Secondary logo
68 |    └─ Hiding 'Portal' notifications
69 | 
70 |    II. 3rd party scripts
71 |    |
72 |    ├─ Normalize.css
73 |    └─ lightense-images.js, progress bar
74 | 
75 |    III. Theme
76 |    |
77 |    ├─ 1.Global
78 |    ├─ 2.Header
79 |    ├─ 3.Hero
80 |    ├─ 4.Widgets
81 |    ├─ 5.Featured
82 |    ├─ 6.Loop
83 |    ├─ 7.Special
84 |    ├─ 8.Subscribe form
85 |    ├─ 9.Pagination
86 |    ├─ 10.Search function
87 |    ├─ 11.Post — Header
88 |    ├─ 12.Post — Content
89 |    ├─ 13.Post — Sidebar
90 |    ├─ 14.Post — Share
91 |    ├─ 15.Post — Navigation
92 |    ├─ 16.Post — Comments
93 |    ├─ 17.Author & Tag page
94 |    ├─ 18.Footer
95 |    ├─ 19.Custom — Pages
96 |    ├─ 20.Custom — Error page
97 |    ├─ 21.Custom — Membership page
98 |    ├─ 22.Custom — Account page
99 |    └─ 23.Custom — Authors & Tags page
100 | 
101 |    //////////////////////////////////////////////////////////////////////////
102 | 
103 |    I. Customize
104 | 
105 |    ////////////////////////////////////////////////////////////////////////// */
106 | 
107 | :root {
108 |     /* Global settings
109 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
110 | 
111 |     /* Logo */
112 |     --height-logo-header: 40px;
113 |     --height-logo-footer: 34px;
114 |     --height-logo-mobile-header: 34px;
115 |     --height-logo-mobile-footer: 34px;
116 | 
117 |     /* Global wrapper */
118 |     --max-width-global-wrap: 1360px;
119 | 
120 |     /* Post global wrapper */
121 |     --max-width-content-wrap: 1060px;
122 | 
123 |     /* Post content wrapper */
124 |     --max-width-post-wrap-one: 740px;
125 |     --max-width-post-wrap-two: 600px;
126 | 
127 |     /* Grid gap */
128 |     --grid-gap: 2.4vw;
129 | 
130 |     /* Border-radius */
131 |     --border-radius: 22px;
132 | 
133 |     /* Global margin */
134 |     --margin-wrap-left-right: 5vw;
135 | 
136 |     /* Border */
137 |     --border: 1px solid;
138 | 
139 |     /* Fonts
140 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
141 |     --font-family-system: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
142 |         Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", "Canela Deck Trial",
143 |         sans-serif;
144 | 
145 |     /* Headings, etc. */
146 |     --font-family-one: var(--font-family-system);
147 |     --font-weight-one-light: 300;
148 |     --font-weight-one-bold: 700;
149 | 
150 |     --font-family-two: var(--font-family-system);
151 |     --font-weight-two-bold: 700;
152 | 
153 |     /* Post content, alerts, etc. */
154 |     --font-family-three: var(--font-family-system);
155 |     --font-weight-three-regular: 400;
156 |     --font-weight-three-medium: 500;
157 |     --font-weight-three-bold: 700;
158 | 
159 |     /* Colors
160 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
161 | 
162 |     /* Color of details */
163 |     --ghost-accent-color: #ff4d82;
164 | 
165 |     /* Light version
166 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
167 | 
168 |     /* Fonts */
169 |     --color-font-one: #080b12;
170 |     --color-font-two: #fff;
171 |     --color-font-black: #080b12;
172 |     --color-font-white: #fff;
173 | 
174 |     /* Background & elements */
175 |     --color-one: #f1f1f3;
176 |     --color-two: #e8e8ec;
177 |     --color-three: #080b12;
178 |     --color-four: #fff;
179 |     --color-five: #f8f6f8;
180 |     --color-six: #fff;
181 |     --color-seven: #fff;
182 |     --color-white: #fff;
183 |     --color-black: #080b12;
184 | 
185 |     /* Body */
186 |     --color-body: #fff;
187 | 
188 |     /* Border */
189 |     --color-border-one: #dfe2e6;
190 |     --color-border-two: #959596;
191 | 
192 |     /* Alerts */
193 |     --color-alert-success: #61d6ad;
194 |     --color-alert-error: #ff6c78;
195 | 
196 |     /* Opacity */
197 |     --opacity-one: 0.85;
198 |     --opacity-two: 0.7;
199 |     --opacity-three: rgba(255, 255, 255, 0.2);
200 |     --opacity-four: rgba(0, 0, 0, 0.1);
201 |     --opacity-cover: 0.2;
202 |     --opacity-cover-custom: 0.18;
203 |     --opacity-search: rgba(0, 0, 0, 0.2);
204 | }
205 | 
206 | /* Sepia version
207 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
208 | .sepia-mode {
209 |     --color-font-one: #1e1e1e;
210 |     --color-font-two: #f1efe3;
211 |     --color-font-black: #1e1e1e;
212 |     --color-font-white: #f1efe3;
213 |     --color-one: #e0e0d4;
214 |     --color-two: #d9d7cb;
215 |     --color-three: #1e1e1e;
216 |     --color-four: #f1e7e4;
217 |     --color-five: #e7ddda;
218 |     --color-six: #f1e4e4;
219 |     --color-seven: #f1e4e4;
220 |     --color-white: #f1efe3;
221 |     --color-black: #1e1e1e;
222 |     --color-body: #f9f7f6;
223 |     --color-border-one: #ede7e3;
224 |     --color-border-two: #bda798;
225 |     --opacity-search: rgba(0, 0, 0, 0.3);
226 | }
227 | 
228 | /* Dark version
229 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
230 | .dark-mode {
231 |     --color-font-one: #fafafa;
232 |     --color-font-two: #1a1a1c;
233 |     --color-font-white: #fafafa;
234 |     --color-font-black: #1a1a1c;
235 |     --color-one: #292b30;
236 |     --color-two: #32343a;
237 |     --color-three: #fafafa;
238 |     --color-four: #1a1a1c;
239 |     --color-five: #222226;
240 |     --color-six: #26282b;
241 |     --color-seven: #292b30;
242 |     --color-white: #fafafa;
243 |     --color-black: #1a1a1c;
244 |     --color-body: #1a1a1c;
245 |     --color-border-one: #303237;
246 |     --color-border-two: #5e6265;
247 |     --opacity-one: 0.8;
248 |     --opacity-two: 0.6;
249 |     --opacity-three: rgba(0, 0, 0, 0.06);
250 |     --opacity-four: rgba(0, 0, 0, 0.1);
251 |     --opacity-cover: 0.15;
252 |     --opacity-cover-custom: 0.1;
253 |     --opacity-search: rgba(0, 0, 0, 0.3);
254 | }
255 | 
256 | /* Auto dark version [duplicate dark version]
257 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
258 | @media (prefers-color-scheme: dark) {
259 |     .auto-dark-mode {
260 |         --color-font-one: #fafafa;
261 |         --color-font-two: #1a1a1c;
262 |         --color-font-white: #fafafa;
263 |         --color-font-black: #1a1a1c;
264 |         --color-one: #292b30;
265 |         --color-two: #32343a;
266 |         --color-three: #fafafa;
267 |         --color-four: #1a1a1c;
268 |         --color-five: #222226;
269 |         --color-six: #26282b;
270 |         --color-seven: #292b30;
271 |         --color-white: #fafafa;
272 |         --color-black: #1a1a1c;
273 |         --color-body: #1a1a1c;
274 |         --color-border-one: #303237;
275 |         --color-border-two: #5e6265;
276 |         --opacity-one: 0.8;
277 |         --opacity-two: 0.6;
278 |         --opacity-three: rgba(0, 0, 0, 0.06);
279 |         --opacity-four: rgba(0, 0, 0, 0.1);
280 |         --opacity-cover: 0.15;
281 |         --opacity-cover-custom: 0.1;
282 |         --opacity-search: rgba(0, 0, 0, 0.3);
283 |     }
284 | }
285 | 
286 | /* Secondary logo
287 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
288 | @media (prefers-color-scheme: dark) {
289 |     .auto-dark-mode .is-auto + .is-logo,
290 |     .auto-dark-mode .is-auto + .is-title {
291 |         display: none;
292 |     }
293 | }
294 | 
295 | @media (prefers-color-scheme: light) {
296 |     .auto-dark-mode .is-auto {
297 |         display: none;
298 |     }
299 | }
300 | 
301 | /* Hiding 'Portal' notifications
302 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
303 | iframe[title="portal-notification"] {
304 |     display: none;
305 | }
306 | 
307 | /* //////////////////////////////////////////////////////////////////////////
308 | 
309 |    II. 3rd party scripts
310 | 
311 |    ////////////////////////////////////////////////////////////////////////// */
312 | 
313 | /* Normalize.css
314 |    ––––––––––––––––––––––––––––––––––––––––––––––––––––
315 |    Version : 8.0.1
316 |    Website : necolas.github.io/normalize.css
317 |    Repo    : github.com/necolas/normalize.css
318 |    Author  : Nicolas Gallagher
319 |    License : MIT
320 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
321 | html {
322 |     line-height: 1.15;
323 |     -webkit-text-size-adjust: 100%;
324 | }
325 | 
326 | body {
327 |     margin: 0;
328 | }
329 | 
330 | main {
331 |     display: block;
332 | }
333 | 
334 | h1 {
335 |     font-size: 2em;
336 |     margin: 0.67em 0;
337 | }
338 | 
339 | hr {
340 |     overflow: visible;
341 |     box-sizing: content-box;
342 |     height: 0;
343 | }
344 | 
345 | pre {
346 |     font-family: monospace, monospace;
347 |     font-size: 1em;
348 | }
349 | 
350 | a {
351 |     background-color: transparent;
352 | }
353 | 
354 | abbr[title] {
355 |     text-decoration: underline;
356 |     text-decoration: underline dotted;
357 |     border-bottom: none;
358 | }
359 | 
360 | b,
361 | strong {
362 |     font-weight: bolder;
363 | }
364 | 
365 | code,
366 | kbd,
367 | samp {
368 |     font-family: monospace, monospace;
369 |     font-size: 1em;
370 | }
371 | 
372 | small {
373 |     font-size: 80%;
374 | }
375 | 
376 | sub,
377 | sup {
378 |     font-size: 75%;
379 |     line-height: 0;
380 |     position: relative;
381 |     vertical-align: baseline;
382 | }
383 | 
384 | sub {
385 |     bottom: -0.25em;
386 | }
387 | 
388 | sup {
389 |     top: -0.5em;
390 | }
391 | 
392 | img {
393 |     border-style: none;
394 | }
395 | 
396 | button,
397 | input,
398 | optgroup,
399 | select,
400 | textarea {
401 |     font-family: inherit;
402 |     font-size: 100%;
403 |     line-height: 1.15;
404 |     margin: 0;
405 | }
406 | 
407 | button,
408 | input {
409 |     overflow: visible;
410 | }
411 | 
412 | button,
413 | select {
414 |     text-transform: none;
415 | }
416 | 
417 | button,
418 | [type="button"],
419 | [type="reset"],
420 | [type="submit"] {
421 |     -webkit-appearance: button;
422 | }
423 | 
424 | button::-moz-focus-inner,
425 | [type="button"]::-moz-focus-inner,
426 | [type="reset"]::-moz-focus-inner,
427 | [type="submit"]::-moz-focus-inner {
428 |     padding: 0;
429 |     border-style: none;
430 | }
431 | 
432 | button:-moz-focusring,
433 | [type="button"]:-moz-focusring,
434 | [type="reset"]:-moz-focusring,
435 | [type="submit"]:-moz-focusring {
436 |     outline: 1px dotted ButtonText;
437 | }
438 | 
439 | fieldset {
440 |     padding: 0.35em 0.75em 0.625em;
441 | }
442 | 
443 | legend {
444 |     display: table;
445 |     box-sizing: border-box;
446 |     max-width: 100%;
447 |     padding: 0;
448 |     white-space: normal;
449 |     color: inherit;
450 | }
451 | 
452 | progress {
453 |     vertical-align: baseline;
454 | }
455 | 
456 | textarea {
457 |     overflow: auto;
458 | }
459 | 
460 | [type="checkbox"],
461 | [type="radio"] {
462 |     box-sizing: border-box;
463 |     padding: 0;
464 | }
465 | 
466 | [type="number"]::-webkit-inner-spin-button,
467 | [type="number"]::-webkit-outer-spin-button {
468 |     height: auto;
469 | }
470 | 
471 | [type="search"] {
472 |     outline-offset: -2px;
473 |     -webkit-appearance: textfield;
474 | }
475 | 
476 | [type="search"]::-webkit-search-decoration {
477 |     -webkit-appearance: none;
478 | }
479 | 
480 | ::-webkit-file-upload-button {
481 |     font: inherit;
482 |     -webkit-appearance: button;
483 | }
484 | 
485 | details {
486 |     display: block;
487 | }
488 | 
489 | summary {
490 |     display: list-item;
491 | }
492 | 
493 | template {
494 |     display: none;
495 | }
496 | 
497 | [hidden] {
498 |     display: none;
499 | }
500 | 
501 | /* Custom settings for lightense-images.js, progress bar
502 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
503 | .lightense-backdrop {
504 |     z-index: 99998 !important;
505 |     background-color: var(--color-body) !important;
506 |     -webkit-backdrop-filter: initial !important;
507 |     backdrop-filter: initial !important;
508 | }
509 | 
510 | .lightense-wrap ~ br,
511 | .lightense-wrap ~ small {
512 |     display: none;
513 | }
514 | 
515 | .lightense-wrap img {
516 |     border-radius: 0 !important;
517 | }
518 | 
519 | .post-progress {
520 |     position: fixed;
521 |     z-index: 90;
522 |     top: 0;
523 |     right: 0;
524 |     left: 0;
525 |     width: 100%;
526 |     height: 8px;
527 |     transition: opacity 0.15s ease-out 0.3s;
528 |     border: none;
529 |     outline: none;
530 |     -webkit-appearance: none;
531 |     -moz-appearance: none;
532 |     appearance: none;
533 | }
534 | 
535 | .post-progress:not([value]) {
536 |     display: none;
537 | }
538 | 
539 | .post-progress,
540 | .post-progress[value]::-webkit-progress-bar {
541 |     background-color: transparent;
542 | }
543 | 
544 | .post-progress[value]::-webkit-progress-value {
545 |     background-color: var(--ghost-accent-color);
546 | }
547 | 
548 | .post-progress[value]::-moz-progress-bar {
549 |     background-color: var(--ghost-accent-color);
550 | }
551 | 
552 | .post-progress[value="1"] {
553 |     opacity: 0;
554 | }
555 | 
556 | /* //////////////////////////////////////////////////////////////////////////
557 | 
558 |    III. Theme
559 | 
560 |    ////////////////////////////////////////////////////////////////////////// */
561 | 
562 | /* --------------------------------------------------------------------------
563 |    1.Global
564 |    -------------------------------------------------------------------------- */
565 | html {
566 |     font-size: 70%;
567 | }
568 | 
569 | html,
570 | body {
571 |     -webkit-font-smoothing: antialiased;
572 |     -moz-osx-font-smoothing: grayscale;
573 |     -webkit-tap-highlight-color: transparent;
574 | }
575 | 
576 | body {
577 |     font-family: var(--font-family-three);
578 |     font-size: 2.5rem;
579 |     font-weight: var(--font-weight-three-regular);
580 |     line-height: 1.5;
581 |     word-wrap: break-word;
582 |     word-break: break-word;
583 |     color: var(--color-font-one);
584 |     background-color: var(--color-body);
585 | }
586 | 
587 | /* Post content typography adjustments */
588 | .post-section .post-content {
589 |     font-size: 2rem;
590 |     line-height: 1.5;
591 | }
592 | 
593 | @media (max-width: 768px) {
594 |     .post-section .post-content {
595 |         font-size: 1.8rem;
596 |         line-height: 1.8; /* Increased line-height for better readability */
597 |         margin-bottom: 1.5rem; /* Added margin for breathing space */
598 |     }
599 | 
600 |     .post-section .post-content p {
601 |         margin-bottom: 1.2rem; /* Space between paragraphs */
602 |     }
603 | 
604 |     h1, h2, h3, h4, h5, h6 {
605 |         margin-bottom: 1rem; /* Space below headings */
606 |     }
607 | }
608 | 
609 | @media (max-width: 480px) {
610 |     .post-section .post-content {
611 |         font-size: 1.6rem;
612 |         line-height: 1.7; /* Increased line-height for better readability */
613 |         margin-bottom: 1.5rem; /* Added margin for breathing space */
614 |     }
615 | 
616 |     .post-section .post-content p {
617 |         margin-bottom: 1rem; /* Space between paragraphs */
618 |     }
619 | 
620 |     h1, h2, h3, h4, h5, h6 {
621 |         margin-bottom: 0.8rem; /* Space below headings */
622 |     }
623 | }
624 | 
625 | @media (max-width: 480px) {
626 |     .post-section .post-content {
627 |         font-size: 1.6rem;
628 |         line-height: 1.5;
629 |     }
630 |     
631 |     .post-section .post-content p,
632 |     .post-section .post-content ul,
633 |     .post-section .post-content ol {
634 |         font-size: 1.6rem;
635 |         line-height: 1.5;
636 |         margin-bottom: 1.2rem;
637 |     }
638 | }
639 | 
640 | 
641 | /* Typography
642 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
643 | h1,
644 | h2,
645 | h3,
646 | h4,
647 | h5,
648 | h6,
649 | input,
650 | textarea,
651 | blockquote {
652 |     line-height: 1.3;
653 | }
654 | 
655 | h1,
656 | h2,
657 | h3,
658 | h4,
659 | h5,
660 | h6 {
661 |     font-family: var(--font-family-one);
662 |     font-weight: var(--font-weight-one-bold);
663 |     width: 100%;
664 | }
665 | 
666 | /* Links
667 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
668 | a {
669 |     text-decoration: none;
670 |     color: var(--color-font-one);
671 | }
672 | 
673 | /* Input & textarea
674 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
675 | input,
676 | input:focus,
677 | textarea {
678 |     color: var(--color-font-one);
679 | }
680 | 
681 | input,
682 | textarea {
683 |     font-family: var(--font-family-three);
684 |     border: none;
685 |     border-radius: 0;
686 |     outline: none;
687 |     background-color: transparent;
688 |     box-shadow: none;
689 | }
690 | 
691 | input::-moz-placeholder,
692 | textarea::-moz-placeholder {
693 |     opacity: var(--opacity-two);
694 |     color: var(--color-font-one);
695 | }
696 | 
697 | input::placeholder,
698 | textarea::placeholder {
699 |     opacity: var(--opacity-two);
700 |     color: var(--color-font-one);
701 | }
702 | 
703 | /* Dynamic color
704 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
705 | body:not(.is-white-text) .global-button:not(.no-color),
706 | body:not(.is-white-text) .global-dynamic-color,
707 | body:not(.is-white-text) .global-dynamic-color a,
708 | body:not(.is-white-text) .global-button.is-cta:hover {
709 |     color: var(--color-font-black);
710 | }
711 | 
712 | body:not(.is-white-text)
713 |     .kg-header-card.kg-style-accent:not(.kg-v2)
714 |     .kg-header-card-button {
715 |     color: var(--color-font-white);
716 |     background-color: var(--color-black);
717 | }
718 | 
719 | body:not(.is-white-text) .global-dynamic-color svg,
720 | body:not(.is-white-text) .kg-audio-thumbnail.placeholder svg {
721 |     fill: var(--color-font-black);
722 | }
723 | 
724 | body:not(.is-white-text) .kg-button-card a,
725 | body:not(.is-white-text) .kg-product-card-button,
726 | body:not(.is-white-text) .kg-style-light .kg-header-card-button,
727 | body:not(.is-white-text)
728 |     .kg-header-card.kg-style-accent:not(.kg-v2)
729 |     .kg-header-card-header,
730 | body:not(.is-white-text)
731 |     .kg-header-card.kg-style-accent:not(.kg-v2)
732 |     .kg-header-card-subheader {
733 |     color: var(--color-font-black) !important;
734 | }
735 | 
736 | /* Contrast script - is white */
737 | body.is-white-text .global-button:not(.no-color),
738 | body.is-white-text .global-dynamic-color,
739 | body.is-white-text .global-dynamic-color a,
740 | body.is-white-text .global-button.is-cta:hover {
741 |     color: var(--color-font-white);
742 | }
743 | 
744 | body.is-white-text .global-dynamic-color svg {
745 |     fill: var(--color-font-white);
746 | }
747 | 
748 | body.is-white-text .featured-section.is-accent .item::before {
749 |     background-color: var(--opacity-four);
750 | }
751 | 
752 | @media (max-width: 480px) {
753 |     body.is-white-text .featured-section.is-accent .featured-content {
754 |         background-color: var(--opacity-four);
755 |     }
756 | }
757 | 
758 | /* Logo
759 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
760 | .global-logo.is-header {
761 |     line-height: 0;
762 | }
763 | 
764 | .global-logo img {
765 |     width: auto;
766 |     aspect-ratio: attr(width) / attr(height);
767 | }
768 | 
769 | .global-logo.is-header img {
770 |     height: var(--height-logo-header);
771 | }
772 | 
773 | .global-logo.is-footer img {
774 |     height: var(--height-logo-footer);
775 | }
776 | 
777 | .global-logo .is-title {
778 |     font-family: var(--font-family-one);
779 |     font-weight: var(--font-weight-one-bold);
780 |     line-height: 1.2;
781 |     display: inline-block;
782 |     max-width: 300px;
783 | }
784 | 
785 | .global-logo .is-title {
786 |     font-size: 3rem;
787 | }
788 | 
789 | /* Image
790 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
791 | .global-image {
792 |     display: block;
793 | }
794 | 
795 | .global-image img {
796 |     width: 100%;
797 |     height: 100%;
798 |     -o-object-fit: cover;
799 |     object-fit: cover;
800 | }
801 | 
802 | .global-bg-image {
803 |     background: no-repeat center center/cover;
804 | }
805 | 
806 | /* Image orientation */
807 | .global-image-orientation {
808 |     line-height: 0;
809 |     position: relative;
810 |     width: 100%;
811 |     margin: 0;
812 |     transition: transform 0.3s ease;
813 |     aspect-ratio: 4/2.8;
814 | }
815 | 
816 | .global-image-orientation > img {
817 |     position: absolute;
818 |     top: 0;
819 |     right: 0;
820 |     bottom: 0;
821 |     left: 0;
822 | }
823 | 
824 | .global-image-orientation.is-portrait {
825 |     aspect-ratio: 1/1.2;
826 | }
827 | 
828 | .global-image-orientation.is-panoramic {
829 |     aspect-ratio: 4/2.3;
830 | }
831 | 
832 | .global-image-orientation.is-square {
833 |     aspect-ratio: 1/1;
834 | }
835 | 
836 | .global-image-orientation.is-natural {
837 |     padding-bottom: 0;
838 |     aspect-ratio: initial;
839 | }
840 | 
841 | .global-image-orientation.is-natural > img {
842 |     position: relative;
843 | }
844 | 
845 | @supports not (aspect-ratio: 1/1) {
846 |     .global-image-orientation {
847 |         padding-bottom: 70%;
848 |     }
849 | 
850 |     .global-image-orientation.is-panoramic {
851 |         padding-bottom: 57.5%;
852 |     }
853 | 
854 |     .global-image-orientation.is-square {
855 |         padding-bottom: 100%;
856 |     }
857 | 
858 |     .global-image-orientation.is-portrait {
859 |         padding-bottom: 120%;
860 |     }
861 | }
862 | 
863 | /* Cover
864 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
865 | .global-cover {
866 |     position: absolute;
867 |     z-index: -1;
868 |     top: 0;
869 |     right: 0;
870 |     left: 0;
871 |     height: 45vh;
872 |     background: no-repeat center center/cover;
873 | }
874 | 
875 | .global-cover:not(.is-membership) {
876 |     opacity: var(--opacity-cover);
877 |     -webkit-mask-image: linear-gradient(
878 |         to top,
879 |         transparent,
880 |         rgba(0, 0, 0, 0.013) 8.1%,
881 |         rgba(0, 0, 0, 0.049) 15.5%,
882 |         rgba(0, 0, 0, 0.104) 22.5%,
883 |         rgba(0, 0, 0, 0.175) 29%,
884 |         rgba(0, 0, 0, 0.259) 35.3%,
885 |         rgba(0, 0, 0, 0.352) 41.2%,
886 |         rgba(0, 0, 0, 0.45) 47.1%,
887 |         rgba(0, 0, 0, 0.55) 52.9%,
888 |         rgba(0, 0, 0, 0.648) 58.8%,
889 |         rgba(0, 0, 0, 0.741) 64.7%,
890 |         rgba(0, 0, 0, 0.825) 71%,
891 |         rgba(0, 0, 0, 0.896) 77.5%,
892 |         rgba(0, 0, 0, 0.951) 84.5%,
893 |         rgba(0, 0, 0, 0.987) 91.9%,
894 |         black
895 |     );
896 |     mask-image: linear-gradient(
897 |         to top,
898 |         transparent,
899 |         rgba(0, 0, 0, 0.013) 8.1%,
900 |         rgba(0, 0, 0, 0.049) 15.5%,
901 |         rgba(0, 0, 0, 0.104) 22.5%,
902 |         rgba(0, 0, 0, 0.175) 29%,
903 |         rgba(0, 0, 0, 0.259) 35.3%,
904 |         rgba(0, 0, 0, 0.352) 41.2%,
905 |         rgba(0, 0, 0, 0.45) 47.1%,
906 |         rgba(0, 0, 0, 0.55) 52.9%,
907 |         rgba(0, 0, 0, 0.648) 58.8%,
908 |         rgba(0, 0, 0, 0.741) 64.7%,
909 |         rgba(0, 0, 0, 0.825) 71%,
910 |         rgba(0, 0, 0, 0.896) 77.5%,
911 |         rgba(0, 0, 0, 0.951) 84.5%,
912 |         rgba(0, 0, 0, 0.987) 91.9%,
913 |         black
914 |     );
915 | }
916 | 
917 | .global-cover.is-membership {
918 |     height: 100%;
919 | }
920 | 
921 | .global-cover.is-featured {
922 |     height: 44%;
923 |     max-height: 800px;
924 |     opacity: var(--opacity-cover-custom);
925 | }
926 | 
927 | /* Border radius
928 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
929 | .global-radius {
930 |     overflow: hidden;
931 | }
932 | 
933 | .global-radius,
934 | .global-radius > img {
935 |     border-radius: var(--border-radius);
936 | }
937 | 
938 | /* Title
939 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
940 | .global-title {
941 |     font-size: 5.6rem;
942 |     line-height: 1.2;
943 |     margin: 0;
944 | }
945 | 
946 | /* Subtitle
947 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
948 | .global-subtitle {
949 |     font-size: 1.2rem;
950 |     font-weight: var(--font-weight-three-medium);
951 |     line-height: 1.1;
952 |     display: block;
953 |     margin: 0 0 1em;
954 |     letter-spacing: 1px;
955 |     text-transform: uppercase;
956 | }
957 | 
958 | /* Link overlay
959 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
960 | .global-link {
961 |     position: absolute;
962 |     z-index: 1;
963 |     top: 0;
964 |     right: 0;
965 |     bottom: 0;
966 |     left: 0;
967 | }
968 | 
969 | /* Button
970 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
971 | .global-button,
972 | .global-button.is-cta {
973 |     font-family: var(--font-family-three);
974 |     font-size: 1.8rem;
975 |     font-weight: var(--font-weight-three-medium);
976 |     line-height: 1.3;
977 |     position: relative;
978 |     z-index: 1;
979 |     display: inline-block;
980 |     box-sizing: border-box;
981 |     padding: 0.8em 1.8em;
982 |     cursor: pointer;
983 |     text-align: center;
984 |     text-decoration: none;
985 |     color: var(--color-font-white);
986 |     border: none;
987 |     outline: none;
988 |     background-color: transparent;
989 | }
990 | 
991 | .global-button.is-cta:hover {
992 |     color: var(--color-font-white);
993 | }
994 | 
995 | .global-button,
996 | .global-button.is-cta,
997 | .global-button::before,
998 | .global-button.is-cta::before {
999 |     border-radius: 100px;
1000 | }
1001 | 
1002 | .global-button::before,
1003 | .global-button.is-cta::before {
1004 |     position: absolute;
1005 |     z-index: -1;
1006 |     top: 0;
1007 |     right: 0;
1008 |     bottom: 0;
1009 |     left: 0;
1010 |     content: "";
1011 |     transition: all 0.2s ease;
1012 |     background-color: var(--ghost-accent-color);
1013 | }
1014 | 
1015 | .global-button:hover::before,
1016 | .global-button.is-cta:hover::before {
1017 |     right: -5px;
1018 |     left: -5px;
1019 | }
1020 | 
1021 | /* Excerpt
1022 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1023 | .global-excerpt {
1024 |     font-size: 2.2rem;
1025 |     display: block;
1026 |     max-width: 700px;
1027 |     margin: 2vh 0 0;
1028 |     opacity: var(--opacity-one);
1029 | }
1030 | 
1031 | /* Tags & Visibility label
1032 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1033 | .global-tags {
1034 |     line-height: 0;
1035 |     display: flex;
1036 |     align-items: flex-start;
1037 |     flex-wrap: wrap;
1038 | }
1039 | 
1040 | .global-tags small:last-child,
1041 | .global-tags a:last-child {
1042 |     margin-bottom: 1.3vh;
1043 | }
1044 | 
1045 | .global-tags:empty {
1046 |     display: none;
1047 | }
1048 | 
1049 | .global-tags small {
1050 |     background-color: var(--ghost-accent-color);
1051 | }
1052 | 
1053 | .global-tags a {
1054 |     transition: background-color 0.2s ease;
1055 |     background-color: var(--color-one);
1056 | }
1057 | 
1058 | .global-tags small,
1059 | .global-tags a {
1060 |     font-size: 1.2rem;
1061 |     font-weight: var(--font-weight-three-medium);
1062 |     line-height: 1.2;
1063 |     display: inline-block;
1064 |     margin-right: 6px;
1065 |     margin-bottom: 6px;
1066 |     padding: 6px 12px;
1067 |     border-radius: 100px;
1068 | }
1069 | 
1070 | .global-tags a:hover {
1071 |     background-color: var(--color-two);
1072 | }
1073 | 
1074 | /* Meta
1075 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1076 | .global-meta {
1077 |     font-size: 1.4rem;
1078 |     line-height: 1.4;
1079 |     margin-top: 1em;
1080 | }
1081 | 
1082 | .global-meta-content {
1083 |     opacity: var(--opacity-one);
1084 | }
1085 | 
1086 | .global-meta.is-full-meta {
1087 |     display: flex;
1088 |     flex-wrap: wrap;
1089 |     margin-top: 2.5vh;
1090 | }
1091 | 
1092 | .global-meta.is-full-meta.is-post {
1093 |     margin-top: 0;
1094 | }
1095 | 
1096 | .global-meta > div {
1097 |     align-self: center;
1098 | }
1099 | 
1100 | .global-meta time {
1101 |     display: block;
1102 | }
1103 | 
1104 | .global-meta a:hover {
1105 |     text-decoration: underline;
1106 | }
1107 | 
1108 | .global-meta-wrap {
1109 |     line-height: 0;
1110 |     flex: 0 0 auto;
1111 | }
1112 | 
1113 | .global-meta-avatar {
1114 |     position: relative;
1115 |     display: inline-block;
1116 |     overflow: hidden;
1117 |     width: 46px;
1118 |     height: 46px;
1119 |     margin-right: -14px;
1120 |     transition-timing-function: ease;
1121 |     transition-duration: 0.2s;
1122 |     transition-property: transform, background-color;
1123 |     background-color: var(--color-body);
1124 |     will-change: transform;
1125 | }
1126 | 
1127 | .global-meta-avatar:last-of-type {
1128 |     margin-right: 12px;
1129 | }
1130 | 
1131 | .global-meta-avatar:hover {
1132 |     transform: translateY(-2px);
1133 | }
1134 | 
1135 | .global-meta-avatar:not(.is-image) {
1136 |     z-index: -1;
1137 |     background-color: var(--color-one);
1138 | }
1139 | 
1140 | .global-meta-avatar:nth-child(1) {
1141 |     z-index: 5;
1142 | }
1143 | 
1144 | .global-meta-avatar:nth-child(2) {
1145 |     z-index: 4;
1146 | }
1147 | 
1148 | .global-meta-avatar:nth-child(3) {
1149 |     z-index: 3;
1150 | }
1151 | 
1152 | .global-meta-avatar:nth-child(4) {
1153 |     z-index: 2;
1154 | }
1155 | 
1156 | .global-meta-avatar:nth-child(5) {
1157 |     z-index: 1;
1158 | }
1159 | 
1160 | .global-meta-avatar,
1161 | .global-meta-avatar.is-image {
1162 |     border-radius: 100px;
1163 | }
1164 | 
1165 | .global-meta-avatar img {
1166 |     width: 101%;
1167 |     height: 101%;
1168 | }
1169 | 
1170 | .global-meta-avatar span {
1171 |     font-family: Menlo, Monaco, Consolas, "Liberation Mono", "Courier New",
1172 |         monospace;
1173 |     font-size: 1.4rem;
1174 |     font-weight: normal;
1175 |     line-height: 14px;
1176 |     position: absolute;
1177 |     top: 50%;
1178 |     left: 50%;
1179 |     display: block;
1180 |     overflow: hidden;
1181 |     width: calc(1ch + 4px);
1182 |     transform: translate(-50%, -50%);
1183 |     text-align: center;
1184 |     white-space: nowrap;
1185 |     text-indent: 2px;
1186 |     letter-spacing: 4px;
1187 |     text-transform: uppercase;
1188 |     color: var(--color-font-one);
1189 | }
1190 | 
1191 | /* Alerts
1192 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1193 | .global-alert {
1194 |     font-size: 1.3rem;
1195 |     line-height: 1.4;
1196 |     display: none;
1197 |     max-width: 420px;
1198 |     opacity: var(--opacity-one);
1199 | }
1200 | 
1201 | /* Questions
1202 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1203 | .global-question {
1204 |     font-size: 1.4rem;
1205 |     display: block;
1206 |     margin-top: 5vh;
1207 | }
1208 | 
1209 | .global-question span {
1210 |     opacity: var(--opacity-two);
1211 | }
1212 | 
1213 | .global-question a,
1214 | .global-question.is-cta a {
1215 |     font-weight: var(--font-weight-three-medium);
1216 |     text-decoration: none;
1217 | }
1218 | 
1219 | .global-question a:hover,
1220 | .global-question.is-cta a:hover {
1221 |     color: var(--color-font-one);
1222 |     text-decoration: underline;
1223 | }
1224 | 
1225 | /* Notifications
1226 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1227 | .global-notification div {
1228 |     font-size: 1.5rem;
1229 |     font-weight: var(--font-weight-three-medium);
1230 |     position: fixed;
1231 |     z-index: 100;
1232 |     top: 1.4vh;
1233 |     right: 10px;
1234 |     left: 10px;
1235 |     display: none;
1236 |     visibility: hidden;
1237 |     max-width: 600px;
1238 |     margin: 0 auto;
1239 |     padding: 20px;
1240 |     transform: translateY(-150%);
1241 |     -webkit-animation: slideDownNotification 5s cubic-bezier(0.19, 1, 0.22, 1)
1242 |         forwards;
1243 |     animation: slideDownNotification 5s cubic-bezier(0.19, 1, 0.22, 1) forwards;
1244 |     text-align: center;
1245 |     color: var(--color-font-black);
1246 |     border-radius: 5px;
1247 |     background-color: var(--color-alert-success);
1248 | }
1249 | 
1250 | .global-notification .expired {
1251 |     background-color: var(--color-alert-error);
1252 | }
1253 | 
1254 | .global-notification.is-subscribe .subscribe,
1255 | .global-notification.is-signin .signin,
1256 | .global-notification.is-signup .signup,
1257 | .global-notification.is-update-email .update-email,
1258 | .global-notification.is-expired .expired,
1259 | .global-notification.is-checkout-success .checkout-success {
1260 |     display: block;
1261 | }
1262 | 
1263 | @-webkit-keyframes slideDownNotification {
1264 |     15% {
1265 |         transform: translateY(0);
1266 |     }
1267 | 
1268 |     85% {
1269 |         transform: translateY(0);
1270 |     }
1271 | 
1272 |     100% {
1273 |         visibility: visible;
1274 |     }
1275 | }
1276 | 
1277 | @keyframes slideDownNotification {
1278 |     15% {
1279 |         transform: translateY(0);
1280 |     }
1281 | 
1282 |     85% {
1283 |         transform: translateY(0);
1284 |     }
1285 | 
1286 |     100% {
1287 |         visibility: visible;
1288 |     }
1289 | }
1290 | 
1291 | /* Padding
1292 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1293 | .global-padding {
1294 |     max-width: var(--max-width-global-wrap);
1295 |     margin-right: auto;
1296 |     margin-left: auto;
1297 |     padding-right: var(--margin-wrap-left-right);
1298 |     padding-left: var(--margin-wrap-left-right);
1299 | }
1300 | 
1301 | /* Wrap & Sticky Footer
1302 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1303 | .global-wrap,
1304 | .global-content {
1305 |     min-height: 100vh;
1306 | }
1307 | 
1308 | .global-content {
1309 |     display: flex;
1310 |     flex-direction: column;
1311 |     margin: 0 auto;
1312 | }
1313 | 
1314 | .global-main {
1315 |     flex: 1 0 auto;
1316 |     width: 100%;
1317 |     margin: 0 auto;
1318 | }
1319 | 
1320 | .global-footer {
1321 |     flex-shrink: 0;
1322 | }
1323 | 
1324 | /* RWD — Global settings
1325 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1326 | @media (max-width: 1280px) {
1327 |     .global-title {
1328 |         font-size: 5.2rem;
1329 |     }
1330 | }
1331 | 
1332 | @media (max-width: 1024px) {
1333 |     .global-excerpt {
1334 |         font-size: 2.2rem;
1335 |     }
1336 | 
1337 |     .global-title {
1338 |         font-size: 4.4rem;
1339 |     }
1340 | 
1341 |     .global-meta {
1342 |         margin-top: 8px;
1343 |     }
1344 | 
1345 |     .global-button,
1346 |     .global-button.is-cta {
1347 |         font-size: 1.6rem;
1348 |     }
1349 | }
1350 | 
1351 | @media (max-width: 768px) {
1352 |     .global-excerpt {
1353 |         font-size: 2rem;
1354 |     }
1355 | 
1356 |     .global-radius,
1357 |     .global-radius > img {
1358 |         border-radius: calc(var(--border-radius) / 1.5);
1359 |     }
1360 | 
1361 |     .global-meta-avatar {
1362 |         width: 40px;
1363 |         height: 40px;
1364 |     }
1365 | 
1366 |     .global-meta-avatar span {
1367 |         font-size: 1.2rem;
1368 |         line-height: 12px;
1369 |     }
1370 | }
1371 | 
1372 | @media (max-width: 480px) {
1373 |     .global-logo.is-header {
1374 |         overflow: hidden;
1375 |         margin-top: 10px;
1376 |         margin-bottom: 10px;
1377 |     }
1378 | 
1379 |     .global-logo .is-title {
1380 |         font-size: 2.8rem;
1381 |     }
1382 | 
1383 |     .global-logo.is-header img {
1384 |         height: var(--height-logo-mobile-header);
1385 |     }
1386 | 
1387 |     .global-logo.is-footer img {
1388 |         height: var(--height-logo-mobile-footer);
1389 |     }
1390 | 
1391 |     .global-cover {
1392 |         height: 200px;
1393 |     }
1394 | 
1395 |     .global-cover.is-featured {
1396 |         height: 100px;
1397 |     }
1398 | 
1399 |     .global-title {
1400 |         font-size: 3.6rem;
1401 |     }
1402 | 
1403 |     .global-meta {
1404 |         font-size: 1.3rem;
1405 |         margin-top: 6px;
1406 |     }
1407 | 
1408 |     .global-meta-avatar:last-of-type {
1409 |         margin-right: 10px;
1410 |     }
1411 | }
1412 | 
1413 | /* --------------------------------------------------------------------------
1414 |    2.Header
1415 |    -------------------------------------------------------------------------- */
1416 | .header-wrap {
1417 |     min-height: 60px;
1418 |     padding: 0.5vh 2vw 2vh;
1419 | }
1420 | 
1421 | .header-wrap,
1422 | .header-nav nav > ul {
1423 |     display: flex;
1424 |     align-items: center;
1425 | }
1426 | 
1427 | .header-wrap li,
1428 | .header-wrap a {
1429 |     font-family: var(--font-family-three);
1430 |     font-size: 1.6rem;
1431 |     font-weight: var(--font-weight-three-medium);
1432 |     display: inline-block;
1433 | }
1434 | 
1435 | .header-nav a:hover,
1436 | .header-nav a.is-active {
1437 |     text-decoration: underline;
1438 |     text-decoration-thickness: 1px;
1439 |     text-underline-offset: 3px;
1440 | }
1441 | 
1442 | .header-nav svg {
1443 |     fill: var(--color-font-one);
1444 | }
1445 | 
1446 | /* Logo
1447 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1448 | .header-logo {
1449 |     flex: 0 0 auto;
1450 |     margin: 20px 0.5vw 20px 0;
1451 | }
1452 | 
1453 | /* Navigation
1454 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1455 | .header-nav {
1456 |     position: relative;
1457 |     z-index: 2;
1458 |     flex: 0 1 100%;
1459 | }
1460 | 
1461 | .header-nav nav {
1462 |     display: flex;
1463 | }
1464 | 
1465 | .header-nav nav ul {
1466 |     margin: 0;
1467 |     padding: 0;
1468 |     list-style: none;
1469 |     word-break: normal;
1470 | }
1471 | 
1472 | .header-nav nav li {
1473 |     margin-left: 1.3vw;
1474 | }
1475 | 
1476 | .header-nav nav > ul:first-of-type {
1477 |     align-items: center;
1478 |     flex-basis: auto;
1479 |     flex-grow: 1;
1480 |     justify-content: flex-start;
1481 | }
1482 | 
1483 | .header-nav nav > ul:last-of-type,
1484 | .header-nav nav.is-right > ul:first-of-type {
1485 |     justify-content: flex-end;
1486 | }
1487 | 
1488 | /* Item
1489 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1490 | .header-nav a {
1491 |     line-height: 1.5;
1492 |     margin: 0;
1493 | }
1494 | 
1495 | /* Dropdown
1496 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1497 | .header-nav .is-dropdown {
1498 |     position: relative;
1499 |     -webkit-user-select: none;
1500 |     -moz-user-select: none;
1501 |     user-select: none;
1502 | }
1503 | 
1504 | .header-nav .is-dropdown,
1505 | .header-nav .is-dropdown svg {
1506 |     cursor: pointer;
1507 | }
1508 | 
1509 | .header-nav .is-dropdown ul {
1510 |     position: absolute;
1511 |     z-index: 999;
1512 |     top: 35px;
1513 |     left: -18px;
1514 |     display: none;
1515 |     min-width: 120px;
1516 |     margin: 0;
1517 |     padding: 20px;
1518 |     list-style: none;
1519 |     cursor: default;
1520 |     border-radius: calc(var(--border-radius) / 1.5);
1521 |     background-color: var(--color-six);
1522 |     box-shadow: 0 8px 50px -10px rgba(0, 0, 0, 0.25);
1523 | }
1524 | 
1525 | .header-nav nav.is-right .is-dropdown ul {
1526 |     right: -19px;
1527 |     left: initial;
1528 |     text-align: right;
1529 | }
1530 | 
1531 | .header-nav .is-dropdown.is-active ul,
1532 | .header-nav .is-dropdown ul li {
1533 |     display: block;
1534 | }
1535 | 
1536 | .header-nav .is-dropdown ul li:not(:last-child) {
1537 |     padding-bottom: 8px;
1538 | }
1539 | 
1540 | .header-nav li.is-dropdown li {
1541 |     margin-left: 0;
1542 | }
1543 | 
1544 | .header-nav .is-dropdown svg {
1545 |     width: 19px;
1546 |     margin: 0 0 4px;
1547 | }
1548 | 
1549 | /* Login panel & Search element
1550 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1551 | .header-search.is-desktop + .signin,
1552 | .header-search.is-desktop + .signup,
1553 | .header-search.is-desktop + .account {
1554 |     margin-left: 0.6vw;
1555 | }
1556 | 
1557 | .header-nav .signup a,
1558 | .header-nav .account a {
1559 |     padding: 8px 17px;
1560 |     text-decoration: none;
1561 | }
1562 | 
1563 | .header-nav .account a {
1564 |     color: var(--color-font-two);
1565 | }
1566 | 
1567 | .header-nav .account a::before {
1568 |     background-color: var(--color-three);
1569 | }
1570 | 
1571 | .header-search,
1572 | .header-search.is-mobile svg {
1573 |     display: block;
1574 |     cursor: pointer;
1575 | }
1576 | 
1577 | .header-search svg {
1578 |     width: 15px;
1579 | }
1580 | 
1581 | .header-search:not(.is-mobile) svg {
1582 |     margin-right: 8px;
1583 |     transform: translateY(2px);
1584 | }
1585 | 
1586 | .header-search.is-mobile {
1587 |     display: none;
1588 | }
1589 | 
1590 | .header-search.is-mobile svg {
1591 |     position: absolute;
1592 |     top: 8px;
1593 |     right: 45px;
1594 |     width: 20px;
1595 | }
1596 | 
1597 | /* Toogle
1598 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1599 | .header-toggle,
1600 | .header-checkbox,
1601 | .header-checkbox:checked,
1602 | .header-checkbox:checked ~ nav {
1603 |     display: none;
1604 | }
1605 | 
1606 | .header-toggle,
1607 | .header-toggle > span,
1608 | .header-checkbox:checked ~ nav ul {
1609 |     position: relative;
1610 | }
1611 | 
1612 | .header-toggle .bar,
1613 | .header-checkbox:checked ~ nav {
1614 |     position: absolute;
1615 | }
1616 | 
1617 | .header-toggle {
1618 |     z-index: 99;
1619 |     overflow: visible;
1620 |     width: 29px;
1621 |     height: 29px;
1622 |     margin: 0;
1623 |     cursor: pointer;
1624 |     opacity: 1;
1625 |     border: none;
1626 |     outline: none;
1627 |     background-color: transparent;
1628 |     will-change: transform;
1629 | }
1630 | 
1631 | .header-toggle > span {
1632 |     top: calc(50% + 2px);
1633 | }
1634 | 
1635 | .header-toggle > span,
1636 | .header-toggle .bar {
1637 |     display: block;
1638 |     width: 100%;
1639 | }
1640 | 
1641 | .header-toggle .bar {
1642 |     height: 2px;
1643 |     content: "";
1644 |     transition:
1645 |         transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1),
1646 |         top 0.3s cubic-bezier(0.645, 0.045, 0.355, 1) 0.2s;
1647 |     background-color: var(--color-three);
1648 | }
1649 | 
1650 | .header-toggle .bar:nth-child(1) {
1651 |     top: -11px;
1652 | }
1653 | 
1654 | .header-toggle .bar:nth-child(3) {
1655 |     top: 11px;
1656 | }
1657 | 
1658 | .header-checkbox:checked ~ label .bar {
1659 |     transition:
1660 |         transform 0.3s cubic-bezier(0.645, 0.045, 0.355, 1) 0.3s,
1661 |         top 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
1662 | }
1663 | 
1664 | .header-checkbox:checked ~ label .bar:nth-child(1),
1665 | .header-checkbox:checked ~ label .bar:nth-child(3) {
1666 |     top: 0;
1667 | }
1668 | 
1669 | .header-checkbox:checked ~ label .bar:nth-child(1),
1670 | .header-checkbox:checked ~ label .bar:nth-child(2) {
1671 |     transform: rotate(45deg);
1672 | }
1673 | 
1674 | .header-checkbox:checked ~ label .bar:nth-child(3) {
1675 |     transform: rotate(-45deg);
1676 | }
1677 | 
1678 | .header-checkbox:checked ~ nav {
1679 |     border-radius: var(--border-radius);
1680 |     background-color: var(--color-six);
1681 |     box-shadow: 0 10px 45px -10px rgba(0, 0, 0, 0.4);
1682 | }
1683 | 
1684 | .header-checkbox:checked ~ nav ul {
1685 |     display: block;
1686 |     margin: 0;
1687 |     padding: 0;
1688 |     list-style: none;
1689 | }
1690 | 
1691 | /* RWD — Header
1692 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1693 | @media (max-width: 1024px) {
1694 |     .header-wrap {
1695 |         padding-right: 3vw;
1696 |         padding-left: 3vw;
1697 |     }
1698 | 
1699 |     .header-logo {
1700 |         flex-basis: 80%;
1701 |     }
1702 | 
1703 |     .header-nav {
1704 |         flex-basis: 20%;
1705 |         text-align: right;
1706 |     }
1707 | 
1708 |     .header-nav a {
1709 |         line-height: 1.3;
1710 |         padding: 5px;
1711 |         word-break: break-word;
1712 |     }
1713 | 
1714 |     .header-nav ul > li,
1715 |     .header-search.is-mobile,
1716 |     .header-checkbox:checked ~ nav {
1717 |         display: block;
1718 |     }
1719 | 
1720 |     .header-nav nav ul,
1721 |     .header-nav .is-dropdown span,
1722 |     .header-search:not(.is-mobile) {
1723 |         display: none;
1724 |     }
1725 | 
1726 |     .header-nav .is-dropdown ul {
1727 |         top: 0;
1728 |         left: initial;
1729 |         min-width: initial;
1730 |         box-shadow: none;
1731 |     }
1732 | 
1733 |     .header-nav nav.is-right .is-dropdown ul {
1734 |         right: 0;
1735 |     }
1736 | 
1737 |     .header-nav .is-dropdown ul li:not(:last-child) {
1738 |         padding-bottom: 0;
1739 |     }
1740 | 
1741 |     .header-toggle {
1742 |         display: inline-block;
1743 |     }
1744 | 
1745 |     .header-checkbox:checked ~ nav {
1746 |         top: 43px;
1747 |         right: -16px;
1748 |         width: 170px;
1749 |         padding: 2vh 15px;
1750 |     }
1751 | 
1752 |     .header-checkbox:checked ~ nav ul {
1753 |         width: 100%;
1754 |     }
1755 | 
1756 |     .header-checkbox:checked ~ nav ul ul {
1757 |         padding-left: 0;
1758 |     }
1759 | 
1760 |     .header-nav .signup,
1761 |     .header-nav .account {
1762 |         margin: 0;
1763 |     }
1764 | 
1765 |     .header-nav .signup a,
1766 |     .header-nav .account a {
1767 |         font-size: 1.4rem;
1768 |         margin-top: 8px;
1769 |         padding: 6px 12px;
1770 |     }
1771 | }
1772 | 
1773 | @media (max-width: 768px) {
1774 |     .header-checkbox:checked ~ nav {
1775 |         right: -10px;
1776 |         padding-right: 10px;
1777 |         padding-left: 10px;
1778 |     }
1779 | }
1780 | 
1781 | @media (max-width: 480px) {
1782 |     .header-wrap li,
1783 |     .header-wrap a {
1784 |         font-size: 1.8rem;
1785 |     }
1786 | 
1787 |     .header-wrap {
1788 |         margin-top: 1.6vh;
1789 |         margin-bottom: 3vh;
1790 |         padding-right: var(--margin-wrap-left-right);
1791 |         padding-bottom: 0;
1792 |         padding-left: var(--margin-wrap-left-right);
1793 |     }
1794 | }
1795 | 
1796 | /* --------------------------------------------------------------------------
1797 |    3.Hero
1798 |    -------------------------------------------------------------------------- */
1799 | .hero-wrap {
1800 |     margin-top: 4vh;
1801 |     margin-bottom: 8vh;
1802 | }
1803 | 
1804 | .hero-title {
1805 |     font-weight: var(--font-weight-one-light);
1806 |     max-width: 1020px;
1807 |     margin: 0 auto;
1808 |     text-align: center;
1809 |     letter-spacing: var(--letter-spacing, normal);
1810 | }
1811 | 
1812 | .hero-title span,
1813 | .hero-title strong,
1814 | .hero-title b {
1815 |     font-weight: var(--font-weight-one-bold);
1816 | }
1817 | 
1818 | /* Search
1819 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1820 | .hero-search {
1821 |     display: flex;
1822 |     align-items: center;
1823 |     box-sizing: border-box;
1824 |     width: 100%;
1825 |     max-width: 500px;
1826 |     margin: 5vh auto 0;
1827 |     padding: 6px 6px 6px 26px;
1828 |     cursor: pointer;
1829 |     border-radius: 100px;
1830 |     background-color: var(--color-one);
1831 | }
1832 | 
1833 | .hero-search span:first-of-type {
1834 |     font-size: 1.8rem;
1835 |     line-height: 1.2;
1836 |     overflow: hidden;
1837 |     flex: 1 0 50%;
1838 |     white-space: nowrap;
1839 |     text-overflow: ellipsis;
1840 |     opacity: var(--opacity-two);
1841 | }
1842 | 
1843 | .hero-search span:last-of-type {
1844 |     display: flex;
1845 |     align-items: center;
1846 |     justify-content: center;
1847 |     width: 24px;
1848 |     height: 24px;
1849 |     padding: 10px;
1850 |     border-radius: 100%;
1851 |     background-color: var(--ghost-accent-color);
1852 | }
1853 | 
1854 | .hero-search svg {
1855 |     width: 14px;
1856 | }
1857 | 
1858 | /* Flat */
1859 | .hero-search.is-flat {
1860 |     transition: background-color 0.16s ease;
1861 | }
1862 | 
1863 | .hero-search.is-flat:hover {
1864 |     background-color: var(--color-two);
1865 | }
1866 | 
1867 | /* Linear */
1868 | .hero-search.is-linear {
1869 |     transition: border-color 0.16s ease;
1870 |     border: var(--border) var(--color-border-one);
1871 |     background-color: var(--color-body);
1872 | }
1873 | 
1874 | .hero-search.is-linear:hover {
1875 |     border-color: var(--color-border-two);
1876 | }
1877 | 
1878 | /* Shadow & Accent*/
1879 | .hero-search.is-shadow {
1880 |     transition: all 0.2s ease;
1881 |     background-color: var(--color-seven);
1882 |     box-shadow: 0 11px 50px -10px rgba(0, 0, 0, 0.3);
1883 | }
1884 | 
1885 | .hero-search.is-shadow:hover {
1886 |     transform: translateY(-2px);
1887 |     box-shadow: 0 15px 50px -10px rgba(0, 0, 0, 0.4);
1888 | }
1889 | 
1890 | /* RWD — Hero
1891 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1892 | @media (max-width: 1480px) and (min-width: 1025px) {
1893 |     .hero-title {
1894 |         font-size: 4.6rem;
1895 |     }
1896 | }
1897 | 
1898 | @media (max-width: 1480px) {
1899 |     .hero-wrap {
1900 |         margin-top: 3vh;
1901 |         margin-bottom: 7vh;
1902 |     }
1903 | 
1904 |     .hero-title {
1905 |         max-width: 850px;
1906 |     }
1907 | 
1908 |     .hero-search span:first-of-type {
1909 |         font-size: 1.6rem;
1910 |     }
1911 | }
1912 | 
1913 | @media (max-width: 1280px) {
1914 |     .hero-search {
1915 |         max-width: 400px;
1916 |     }
1917 | 
1918 |     .hero-search span:last-of-type {
1919 |         padding: 8px;
1920 |     }
1921 | }
1922 | 
1923 | @media (max-width: 1024px) and (min-width: 769px) {
1924 |     .hero-title {
1925 |         font-size: 4rem;
1926 |     }
1927 | }
1928 | 
1929 | @media (max-width: 1024px) {
1930 |     .hero-wrap {
1931 |         margin-top: 2vh;
1932 |     }
1933 | 
1934 |     .hero-title {
1935 |         max-width: 750px;
1936 |     }
1937 | 
1938 |     .hero-search {
1939 |         max-width: 360px;
1940 |         margin-top: 4vh;
1941 |     }
1942 | }
1943 | 
1944 | @media (max-width: 768px) {
1945 |     .hero-title {
1946 |         font-size: 3.4rem;
1947 |         max-width: 620px;
1948 |     }
1949 | }
1950 | 
1951 | @media (max-width: 480px) {
1952 |     .hero-wrap {
1953 |         margin-top: 1vh;
1954 |         margin-bottom: 5.5vh;
1955 |     }
1956 | 
1957 |     .hero-title {
1958 |         text-align: left;
1959 |     }
1960 | 
1961 |     .hero-search {
1962 |         max-width: 100%;
1963 |     }
1964 | }
1965 | 
1966 | /* --------------------------------------------------------------------------
1967 |    4.Widgets
1968 |    -------------------------------------------------------------------------- */
1969 | .widget-section {
1970 |     margin-bottom: 4.5vh;
1971 | }
1972 | 
1973 | .widget-wrap {
1974 |     display: grid;
1975 |     width: 100%;
1976 |     gap: calc(var(--grid-gap) / 3);
1977 |     grid-auto-columns: 1fr;
1978 |     grid-gap: calc(var(--grid-gap) / 3);
1979 | }
1980 | 
1981 | .widget-wrap.is-tags {
1982 |     grid-template-columns: repeat(7, 1fr);
1983 | }
1984 | 
1985 | .widget-wrap.is-authors {
1986 |     grid-template-columns: repeat(8, 1fr);
1987 | }
1988 | 
1989 | /* Item
1990 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
1991 | .widget-wrap .item {
1992 |     position: relative;
1993 |     display: flex;
1994 |     align-items: flex-end;
1995 |     margin: 0;
1996 |     transition: transform 0.3s ease;
1997 |     will-change: transform;
1998 | }
1999 | 
2000 | .widget-wrap .item:hover {
2001 |     transform: translateY(-3px);
2002 | }
2003 | 
2004 | /* Image
2005 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2006 | .widget-image {
2007 |     position: absolute;
2008 |     z-index: -1;
2009 |     top: -1%;
2010 |     right: -1%;
2011 |     bottom: -1%;
2012 |     left: -1%;
2013 | }
2014 | 
2015 | /* Title
2016 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2017 | .widget-wrap .item-title {
2018 |     font-family: var(--font-family-three);
2019 |     font-size: 1.3rem;
2020 |     font-weight: var(--font-weight-three-medium);
2021 |     line-height: 1.2;
2022 |     overflow: hidden;
2023 |     box-sizing: border-box;
2024 |     width: auto;
2025 |     max-height: 30px;
2026 |     margin: 9px;
2027 |     padding: 7px 13px;
2028 |     white-space: nowrap;
2029 |     text-overflow: ellipsis;
2030 |     border-radius: 100px;
2031 |     background-color: var(--color-body);
2032 | }
2033 | 
2034 | .widget-wrap.is-authors .item-title {
2035 |     width: 100%;
2036 |     text-align: center;
2037 | }
2038 | 
2039 | /* RWD — Widgets
2040 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2041 | @media (max-width: 1280px) {
2042 |     .widget-wrap.is-tags {
2043 |         grid-template-columns: repeat(6, 1fr);
2044 |     }
2045 | 
2046 |     .widget-wrap.is-authors {
2047 |         grid-template-columns: repeat(7, 1fr);
2048 |     }
2049 | 
2050 |     .widget-wrap.is-tags .item:nth-child(7),
2051 |     .widget-wrap.is-authors .item:nth-child(8) {
2052 |         display: none;
2053 |     }
2054 | }
2055 | 
2056 | @media (max-width: 1024px) {
2057 |     .widget-wrap {
2058 |         gap: calc(var(--grid-gap) / 2);
2059 |         grid-gap: calc(var(--grid-gap) / 2);
2060 |     }
2061 | 
2062 |     .widget-wrap.is-authors {
2063 |         grid-template-columns: repeat(6, 1fr);
2064 |     }
2065 | 
2066 |     .widget-wrap.is-authors .item:nth-child(7) {
2067 |         display: none;
2068 |     }
2069 | }
2070 | 
2071 | @media (max-width: 768px) {
2072 |     .widget-wrap.is-tags {
2073 |         grid-template-columns: repeat(4, 1fr);
2074 |     }
2075 | 
2076 |     .widget-wrap.is-tags .item:nth-child(5),
2077 |     .widget-wrap.is-tags .item:nth-child(6),
2078 |     .widget-wrap.is-authors .item:nth-child(6) {
2079 |         display: none;
2080 |     }
2081 | }
2082 | 
2083 | @media (max-width: 480px) {
2084 |     .widget-wrap {
2085 |         gap: calc(var(--grid-gap) / 1.2);
2086 |         grid-gap: calc(var(--grid-gap) / 1.2);
2087 |     }
2088 | 
2089 |     .widget-wrap.is-tags,
2090 |     .widget-wrap.is-authors {
2091 |         grid-template-columns: repeat(3, 1fr);
2092 |     }
2093 | 
2094 |     .widget-wrap.is-tags .item:nth-child(4),
2095 |     .widget-wrap.is-authors .item:nth-child(4),
2096 |     .widget-wrap.is-authors .item:nth-child(5) {
2097 |         display: none;
2098 |     }
2099 | 
2100 |     .widget-wrap .item:hover {
2101 |         transform: translateY(0);
2102 |     }
2103 | 
2104 |     .widget-wrap.is-tags .item {
2105 |         text-align: center;
2106 |     }
2107 | 
2108 |     .widget-wrap.is-tags .item-title {
2109 |         margin: 7px;
2110 |         padding: 5px 9px;
2111 |     }
2112 | }
2113 | 
2114 | /* --------------------------------------------------------------------------
2115 |    5.Featured
2116 |    -------------------------------------------------------------------------- */
2117 | .featured-section {
2118 |     position: relative;
2119 |     z-index: 0;
2120 |     box-sizing: border-box;
2121 |     width: 100%;
2122 |     margin-bottom: 7vh;
2123 |     padding: 6vh 7vw 8vh;
2124 |     background-color: var(--color-five);
2125 | }
2126 | 
2127 | .featured-section.is-accent,
2128 | .featured-section.is-accent-gray {
2129 |     background-color: var(--ghost-accent-color);
2130 | }
2131 | 
2132 | .featured-content {
2133 |     display: grid;
2134 |     gap: var(--grid-gap);
2135 |     grid-auto-columns: 1fr;
2136 |     grid-gap: var(--grid-gap);
2137 |     grid-template-columns: repeat(6, 1fr);
2138 | }
2139 | 
2140 | .featured-subtitle,
2141 | .featured-title {
2142 |     text-align: center;
2143 | }
2144 | 
2145 | .featured-section + .loop-subtitle {
2146 |     display: block;
2147 | }
2148 | 
2149 | /* Item
2150 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2151 | .featured-content .item {
2152 |     position: relative;
2153 |     z-index: 0;
2154 |     grid-column: span 2;
2155 | }
2156 | 
2157 | .featured-content.items-1 .item,
2158 | .featured-content.items-2 .item {
2159 |     grid-column: span 3;
2160 | }
2161 | 
2162 | /* Subtitle
2163 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2164 | .featured-subtitle {
2165 |     font-size: 1.7rem;
2166 |     font-weight: var(--font-weight-three-medium);
2167 |     display: block;
2168 |     margin-bottom: 0.8em;
2169 |     letter-spacing: 0.02em;
2170 | }
2171 | 
2172 | /* Section title
2173 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2174 | .featured-title {
2175 |     font-size: 5.2rem;
2176 |     font-weight: var(--font-weight-one-bold);
2177 |     line-height: 1.2;
2178 |     max-width: 540px;
2179 |     margin: 0 auto 7vh;
2180 |     letter-spacing: var(--letter-spacing, normal);
2181 | }
2182 | 
2183 | /* Image
2184 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2185 | .featured-content .item-image {
2186 |     margin-bottom: 1.4vh;
2187 | }
2188 | 
2189 | /* Meta
2190 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2191 | .featured-content .item-title + div > div {
2192 |     opacity: 1;
2193 | }
2194 | 
2195 | /* Button
2196 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2197 | .featured-button-wrap {
2198 |     text-align: right;
2199 | }
2200 | 
2201 | .featured-button {
2202 |     font-size: 1.6rem;
2203 |     display: inline-block;
2204 |     margin-top: 3vh;
2205 |     color: var(--color-font-one);
2206 | }
2207 | 
2208 | .featured-button:hover {
2209 |     text-decoration: underline;
2210 | }
2211 | 
2212 | /* RWD — Featured
2213 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2214 | @media (max-width: 1280px) {
2215 |     .featured-subtitle {
2216 |         font-size: 1.6rem;
2217 |         margin-bottom: 0.4em;
2218 |     }
2219 | 
2220 |     .featured-title {
2221 |         font-size: 4rem;
2222 |         max-width: 420px;
2223 |         margin-bottom: 5vh;
2224 |     }
2225 | }
2226 | 
2227 | @media (max-width: 1024px) {
2228 |     .featured-content .item-title {
2229 |         font-size: 2rem;
2230 |         margin-top: 0;
2231 |     }
2232 | 
2233 |     .featured-content .item-title + div {
2234 |         display: none;
2235 |     }
2236 | }
2237 | 
2238 | @media (max-width: 768px) {
2239 |     .featured-section {
2240 |         padding-top: 30px;
2241 |         padding-bottom: 30px;
2242 |     }
2243 | 
2244 |     .featured-title {
2245 |         font-size: 2.8rem;
2246 |     }
2247 | 
2248 |     .featured-content .item-image {
2249 |         margin-bottom: 1vh;
2250 |     }
2251 | 
2252 |     .featured-content .item-content {
2253 |         padding-right: 10px;
2254 |     }
2255 | 
2256 |     .featured-content .item-title {
2257 |         font-size: 1.8rem;
2258 |     }
2259 | 
2260 |     .featured-button {
2261 |         font-size: 1.4rem;
2262 |     }
2263 | }
2264 | 
2265 | @media (max-width: 480px) {
2266 |     .featured-section {
2267 |         padding-right: 26px;
2268 |         padding-left: 26px;
2269 |     }
2270 | 
2271 |     .featured-title {
2272 |         margin-bottom: 3vh;
2273 |     }
2274 | 
2275 |     .featured-content {
2276 |         padding: 16px;
2277 |         border-radius: calc(var(--border-radius) * 1.1);
2278 |         gap: 0;
2279 |         grid-gap: 0;
2280 |         grid-template-columns: repeat(1, 1fr);
2281 |     }
2282 | 
2283 |     .featured-section.is-gray-accent .featured-content {
2284 |         background-color: var(--ghost-accent-color);
2285 |     }
2286 | 
2287 |     .featured-section.is-gray .featured-content,
2288 |     .featured-section.is-accent-gray .featured-content {
2289 |         background-color: var(--color-body);
2290 |     }
2291 | 
2292 |     .featured-section.is-accent .featured-content {
2293 |         background-color: var(--opacity-three);
2294 |     }
2295 | 
2296 |     .featured-content .item {
2297 |         display: flex;
2298 |         align-items: flex-start;
2299 |         margin-bottom: 3vh;
2300 |     }
2301 | 
2302 |     .featured-content .item:last-of-type {
2303 |         margin-bottom: 0;
2304 |     }
2305 | 
2306 |     .featured-content .item-image {
2307 |         flex: 1 0 26%;
2308 |         width: 100%;
2309 |         max-width: 26%;
2310 |         margin-right: 3vw;
2311 |         margin-bottom: 0;
2312 |     }
2313 | 
2314 |     .featured-content .item-title {
2315 |         margin-top: 0;
2316 |     }
2317 | 
2318 |     .featured-button-wrap {
2319 |         text-align: center;
2320 |     }
2321 | 
2322 |     .featured-button {
2323 |         font-weight: var(--font-weight-three-medium);
2324 |     }
2325 | }
2326 | 
2327 | @media (min-width: 481px) {
2328 |     .featured-content .item {
2329 |         margin-bottom: 0;
2330 |         padding: 10px 10px 16px;
2331 |         transition: transform 0.3s ease;
2332 |         background-color: var(--color-body);
2333 |         will-change: transform;
2334 |     }
2335 | 
2336 |     .featured-content .item,
2337 |     .featured-content .item::before {
2338 |         border-radius: calc(var(--border-radius) / 1.2);
2339 |     }
2340 | 
2341 |     .featured-section.is-accent .item,
2342 |     .featured-section.is-gray-accent .item {
2343 |         background-color: var(--ghost-accent-color);
2344 |     }
2345 | 
2346 |     .featured-section.is-accent .item::before {
2347 |         position: absolute;
2348 |         z-index: -1;
2349 |         top: 0;
2350 |         right: 0;
2351 |         bottom: 0;
2352 |         left: 0;
2353 |         content: "";
2354 |         background-color: var(--opacity-three);
2355 |     }
2356 | 
2357 |     .featured-content .item:hover {
2358 |         transform: translateY(-3px);
2359 |     }
2360 | 
2361 |     .featured-content .item-content {
2362 |         padding-right: 0;
2363 |     }
2364 | 
2365 |     .featured-content .item-image:hover {
2366 |         transform: translateY(0);
2367 |     }
2368 | 
2369 |     .featured-content .item-image,
2370 |     .featured-content .item-image img {
2371 |         border-radius: calc(var(--border-radius) / 2.6);
2372 |     }
2373 | 
2374 |     .featured-content .item-title + div a {
2375 |         position: relative;
2376 |         z-index: 99;
2377 |     }
2378 | }
2379 | 
2380 | @media (min-width: 769px) {
2381 |     .featured-content .item {
2382 |         padding: 16px 16px 20px;
2383 |     }
2384 | 
2385 |     .featured-content .item,
2386 |     .featured-content .item::before {
2387 |         border-radius: var(--border-radius);
2388 |     }
2389 | 
2390 |     .featured-content.items-1 .item-title,
2391 |     .featured-content.items-2 .item-title {
2392 |         font-size: 2.4rem;
2393 |         max-width: 330px;
2394 |     }
2395 | }
2396 | 
2397 | @media (min-width: 1025px) {
2398 |     .featured-content .item {
2399 |         padding: 26px;
2400 |     }
2401 | 
2402 |     .featured-content.items-1 .item-title,
2403 |     .featured-content.items-2 .item-title {
2404 |         font-size: 3rem;
2405 |         max-width: 400px;
2406 |     }
2407 | 
2408 |     .featured-content.items-1 .item-image,
2409 |     .featured-content.items-2 .item-image {
2410 |         margin-bottom: 1.6vh;
2411 |     }
2412 | }
2413 | 
2414 | @media (min-width: 1481px) {
2415 |     .featured-content .item-title {
2416 |         font-size: 2.6rem;
2417 |     }
2418 | }
2419 | 
2420 | /* --------------------------------------------------------------------------
2421 |    6.Loop
2422 |    -------------------------------------------------------------------------- */
2423 | .loop-section {
2424 |     margin-bottom: 7vh;
2425 | }
2426 | 
2427 | .loop-wrap {
2428 |     display: grid;
2429 |     width: 100%;
2430 |     margin-bottom: var(--grid-gap);
2431 |     -webkit-animation: slideTop 0.8s ease;
2432 |     animation: slideTop 0.8s ease;
2433 |     gap: var(--grid-gap);
2434 |     grid-auto-columns: 1fr;
2435 |     grid-gap: var(--grid-gap);
2436 |     grid-template-columns: repeat(3, 1fr);
2437 |     will-change: transform;
2438 | }
2439 | 
2440 | .loop-subtitle {
2441 |     display: none;
2442 | }
2443 | 
2444 | /* Image
2445 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2446 | .item-image {
2447 |     margin-bottom: 1.8vh;
2448 |     transition: transform 0.3s ease;
2449 |     will-change: transform;
2450 | }
2451 | 
2452 | .item-image:hover {
2453 |     transform: translateY(-3px);
2454 | }
2455 | 
2456 | /* Content
2457 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2458 | .item-content {
2459 |     position: relative;
2460 |     display: flex;
2461 |     flex-direction: column;
2462 |     box-sizing: border-box;
2463 |     padding-right: 1.4vw;
2464 | }
2465 | 
2466 | /* Item
2467 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2468 | .item {
2469 |     margin-bottom: 1vh;
2470 | }
2471 | 
2472 | /* Title
2473 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2474 | .item-title {
2475 |     font-size: 3rem;
2476 |     font-weight: var(--font-weight-one-bold);
2477 |     line-height: 1.3;
2478 |     max-width: 490px;
2479 |     margin: 0;
2480 | }
2481 | 
2482 | .item-title a:hover {
2483 |     text-decoration: underline;
2484 |     text-decoration-thickness: 2px;
2485 |     text-underline-offset: 3px;
2486 | }
2487 | 
2488 | /* Excerpt
2489 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2490 | .item-excerpt {
2491 |     font-size: 1.6rem;
2492 |     display: -webkit-box;
2493 |     overflow-y: hidden;
2494 |     margin-top: 1.6vh;
2495 |     margin-bottom: 0.5vh;
2496 |     -webkit-box-orient: vertical;
2497 |     -webkit-line-clamp: 3;
2498 | }
2499 | 
2500 | .item-excerpt.no-image {
2501 |     -webkit-line-clamp: 10;
2502 | }
2503 | 
2504 | /* If 'top'
2505 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2506 | .loop-wrap.is-top {
2507 |     margin-bottom: 0;
2508 |     grid-template-columns: repeat(18, 1fr);
2509 |     grid-template-rows: -webkit-min-content;
2510 |     grid-template-rows: min-content;
2511 | }
2512 | 
2513 | .item.is-top {
2514 |     margin-bottom: 0;
2515 | }
2516 | 
2517 | .item.is-top,
2518 | .loop-wrap.is-top .subscribe-form {
2519 |     grid-column: span 6;
2520 | }
2521 | 
2522 | .item.is-top.is-first {
2523 |     margin-bottom: calc(var(--grid-gap) + 3vh);
2524 |     grid-column: span 12;
2525 |     grid-row: span 4;
2526 | }
2527 | 
2528 | .item.is-top.is-first .item-image {
2529 |     margin-bottom: 2.6vh;
2530 |     aspect-ratio: 4/3.05;
2531 | }
2532 | 
2533 | .item.is-top.is-first .item-content {
2534 |     padding-right: 1.8vw;
2535 | }
2536 | 
2537 | .item.is-top.is-first .item-title {
2538 |     font-size: 6.4rem;
2539 |     line-height: 1.2;
2540 |     max-width: 95%;
2541 |     letter-spacing: var(--letter-spacing, normal);
2542 | }
2543 | 
2544 | .item.is-top.is-first .item-excerpt {
2545 |     font-size: 2.5rem;
2546 |     max-width: 720px;
2547 |     margin-top: 2.6vh;
2548 |     margin-bottom: 1.3vh;
2549 |     -webkit-line-clamp: 10;
2550 | }
2551 | 
2552 | /* Animation
2553 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2554 | @-webkit-keyframes slideTop {
2555 |     0% {
2556 |         transform: translateY(40px);
2557 |     }
2558 | 
2559 |     100% {
2560 |         transform: translateY(0);
2561 |     }
2562 | }
2563 | 
2564 | @keyframes slideTop {
2565 |     0% {
2566 |         transform: translateY(40px);
2567 |     }
2568 | 
2569 |     100% {
2570 |         transform: translateY(0);
2571 |     }
2572 | }
2573 | 
2574 | /* RWD — Loop
2575 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2576 | @media (max-width: 1600px) {
2577 |     .item-title {
2578 |         font-size: 2.8rem;
2579 |     }
2580 | }
2581 | 
2582 | @media (max-width: 1480px) {
2583 |     .item-title {
2584 |         font-size: 2.6rem;
2585 |     }
2586 | 
2587 |     .item.is-top.is-first .item-title {
2588 |         font-size: 6rem;
2589 |     }
2590 | }
2591 | 
2592 | @media (max-width: 1280px) {
2593 |     .item-image {
2594 |         margin-bottom: 1.5vh;
2595 |     }
2596 | 
2597 |     .item.is-top.is-first .item-image {
2598 |         margin-bottom: 2vh;
2599 |     }
2600 | 
2601 |     .item-image:hover {
2602 |         transform: translateY(0);
2603 |     }
2604 | 
2605 |     .item-title {
2606 |         font-size: 2.4rem;
2607 |     }
2608 | 
2609 |     .item-excerpt,
2610 |     .item-excerpt.no-image {
2611 |         font-size: 1.5rem;
2612 |     }
2613 | 
2614 |     .item.is-top.is-first .item-content {
2615 |         padding-right: 1vw;
2616 |     }
2617 | 
2618 |     .item.is-top.is-first .item-title {
2619 |         font-size: 5.4rem;
2620 |     }
2621 | 
2622 |     .item.is-top.is-first .item-excerpt {
2623 |         font-size: 2.3rem;
2624 |     }
2625 | }
2626 | 
2627 | @media (max-width: 1024px) {
2628 |     .item-excerpt,
2629 |     .item-excerpt.no-image {
2630 |         -webkit-line-clamp: 5;
2631 |     }
2632 | 
2633 |     .item.is-top.is-first .item-title {
2634 |         font-size: 4rem;
2635 |     }
2636 | 
2637 |     .item.is-top.is-first .item-excerpt {
2638 |         max-width: 95%;
2639 |     }
2640 | 
2641 |     .item:not(.is-top):not(.custom-archive-item) .item-excerpt:not(.no-image) {
2642 |         display: none;
2643 |     }
2644 | }
2645 | 
2646 | @media (max-width: 1024px) and (min-width: 769px) {
2647 |     .loop-wrap.is-top,
2648 |     .loop-wrap .item {
2649 |         margin-bottom: 2vh;
2650 |     }
2651 | 
2652 |     .item-title {
2653 |         font-size: 2.2rem;
2654 |     }
2655 | 
2656 |     .item.is-top.is-first .item-excerpt {
2657 |         font-size: 2rem;
2658 |     }
2659 | }
2660 | 
2661 | @media (max-width: 768px) {
2662 |     .loop-wrap {
2663 |         grid-template-columns: repeat(1, 1fr);
2664 |     }
2665 | 
2666 |     .loop-wrap.is-top {
2667 |         margin-bottom: var(--grid-gap);
2668 |     }
2669 | 
2670 |     .loop-wrap .item,
2671 |     .item.is-top.is-first {
2672 |         margin-bottom: calc(var(--grid-gap) + 1.8vh);
2673 |     }
2674 | 
2675 |     .item.is-top.is-first {
2676 |         padding-bottom: 4vh;
2677 |         border-bottom: var(--border) var(--color-border-one);
2678 |     }
2679 | 
2680 |     .loop-wrap .item:not(.is-top.is-first):not(.custom-archive-item) {
2681 |         display: flex;
2682 |         align-items: flex-start;
2683 |     }
2684 | 
2685 |     .item:not(.is-first) .item-tags small:last-child,
2686 |     .item:not(.is-first) .item-tags a:last-child {
2687 |         margin-bottom: 0.5vh;
2688 |     }
2689 | 
2690 |     .item.is-top,
2691 |     .item.is-top.is-first {
2692 |         grid-column: span 18;
2693 |     }
2694 | 
2695 |     .item.is-top.is-first {
2696 |         grid-row: span 1;
2697 |     }
2698 | 
2699 |     .loop-wrap
2700 |         .item:not(.is-top.is-first):not(.custom-archive-item)
2701 |         .item-image {
2702 |         flex: 1 0 calc(33% - 1px - var(--grid-gap) / 2);
2703 |         width: 100%;
2704 |         max-width: calc(33% - 1px - var(--grid-gap) / 2);
2705 |         margin-right: 3.5vw;
2706 |         margin-bottom: 0;
2707 |     }
2708 | 
2709 |     .loop-wrap .item:not(.is-top.is-first) .item-content {
2710 |         width: 100%;
2711 |     }
2712 | 
2713 |     .loop-wrap .item:not(.is-top.is-first) .item-title {
2714 |         max-width: 380px;
2715 |     }
2716 | 
2717 |     .item-title {
2718 |         font-size: 2.8rem;
2719 |     }
2720 | 
2721 |     .item.is-top:not(.is-first) .item-excerpt:not(.no-image) {
2722 |         display: none;
2723 |     }
2724 | }
2725 | 
2726 | @media (max-width: 480px) {
2727 |     .loop-wrap.is-top + small {
2728 |         margin-top: 4vh;
2729 |     }
2730 | 
2731 |     .item.is-top.is-first .item-image {
2732 |         margin-bottom: 3vh;
2733 |     }
2734 | 
2735 |     .loop-wrap .item:not(.is-top.is-first) .item-content {
2736 |         max-width: 330px;
2737 |         padding-right: 5px;
2738 |     }
2739 | 
2740 |     .item.is-top.is-first .item-content {
2741 |         padding-right: 0;
2742 |     }
2743 | 
2744 |     .item.is-first .item-tags small:last-child,
2745 |     .item.is-first .item-tags a:last-child {
2746 |         margin-bottom: 2vh;
2747 |     }
2748 | 
2749 |     .item-title {
2750 |         font-size: 2rem;
2751 |     }
2752 | 
2753 |     .item.is-top.is-first .item-title {
2754 |         font-size: 3.2rem;
2755 |         max-width: 100%;
2756 |     }
2757 | 
2758 |     .item.is-top.is-first .item-excerpt,
2759 |     .item:not(.is-first) .item-tags {
2760 |         display: none;
2761 |     }
2762 | }
2763 | 
2764 | /* --------------------------------------------------------------------------
2765 |    7.Special
2766 |    -------------------------------------------------------------------------- */
2767 | .special-wrap {
2768 |     display: grid;
2769 |     width: 100%;
2770 |     margin-bottom: 6vh;
2771 |     gap: calc(var(--grid-gap) / 2);
2772 |     grid-auto-columns: 1fr;
2773 |     grid-gap: calc(var(--grid-gap) / 2);
2774 |     grid-template-columns: repeat(5, 1fr);
2775 | }
2776 | 
2777 | .item.is-special .item-image {
2778 |     margin-bottom: 1.2vh;
2779 | }
2780 | 
2781 | .special-wrap .item-content {
2782 |     padding-right: 5px;
2783 | }
2784 | 
2785 | .item.is-special .item-title {
2786 |     font-size: 2.2rem;
2787 | }
2788 | 
2789 | /* RWD — Special
2790 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2791 | @media (max-width: 1480px) {
2792 |     .item.is-special .item-title {
2793 |         font-size: 2rem;
2794 |     }
2795 | 
2796 |     .item.is-special .item-title + div {
2797 |         display: none;
2798 |     }
2799 | }
2800 | 
2801 | @media (max-width: 1024px) {
2802 |     .special-wrap {
2803 |         grid-template-columns: repeat(4, 1fr);
2804 |     }
2805 | 
2806 |     .item.is-special:nth-child(5) {
2807 |         display: none;
2808 |     }
2809 | 
2810 |     .item.is-special .item-title {
2811 |         font-size: 1.8rem;
2812 |     }
2813 | }
2814 | 
2815 | @media (max-width: 768px) {
2816 |     .special-wrap {
2817 |         gap: var(--grid-gap);
2818 |         grid-gap: var(--grid-gap);
2819 |         grid-template-columns: repeat(3, 1fr);
2820 |     }
2821 | }
2822 | 
2823 | @media (max-width: 768px) and (min-width: 481px) {
2824 |     .item.is-special:nth-child(4) {
2825 |         display: none;
2826 |     }
2827 | }
2828 | 
2829 | @media (max-width: 480px) {
2830 |     .special-wrap {
2831 |         grid-template-columns: repeat(2, 1fr);
2832 |     }
2833 | 
2834 |     .special-wrap,
2835 |     .special-wrap .item {
2836 |         margin-bottom: 3vh;
2837 |     }
2838 | }
2839 | 
2840 | /* --------------------------------------------------------------------------
2841 |    8.Subscribe form
2842 |    -------------------------------------------------------------------------- */
2843 | .subscribe-form {
2844 |     box-sizing: border-box;
2845 |     padding: 28px 34px 32px;
2846 |     background-color: var(--ghost-accent-color);
2847 | }
2848 | 
2849 | .subscribe-wrap {
2850 |     text-align: center;
2851 | }
2852 | 
2853 | /* Title
2854 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2855 | .subscribe-title {
2856 |     font-family: var(--font-family-two);
2857 |     font-size: 3.2rem;
2858 |     font-weight: var(--font-weight-two-bold);
2859 |     line-height: 1.2;
2860 |     margin: 0 0 2.4vh;
2861 | }
2862 | 
2863 | /* Button & input
2864 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2865 | .subscribe-wrap input {
2866 |     font-size: 1.6rem;
2867 |     display: block;
2868 |     box-sizing: border-box;
2869 |     margin-bottom: 1vh;
2870 |     word-break: normal;
2871 |     border: none;
2872 |     border-radius: 100px;
2873 | }
2874 | 
2875 | .subscribe-wrap input,
2876 | .subscribe-wrap button {
2877 |     line-height: 1;
2878 |     width: 100%;
2879 |     padding: 17px 1.5em;
2880 |     will-change: transform;
2881 | }
2882 | 
2883 | .subscribe-wrap input,
2884 | .subscribe-wrap button::before {
2885 |     background-color: var(--color-body);
2886 | }
2887 | 
2888 | .subscribe-wrap button {
2889 |     width: 94%;
2890 |     color: var(--color-font-one);
2891 | }
2892 | 
2893 | .subscribe-wrap button:hover::before {
2894 |     right: -3%;
2895 |     left: -3%;
2896 | }
2897 | 
2898 | /* Hero
2899 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2900 | .subscribe-wrap.is-hero {
2901 |     position: relative;
2902 |     width: 100%;
2903 |     max-width: 450px;
2904 |     margin: 5vh auto 0;
2905 |     border-radius: 100px;
2906 | }
2907 | 
2908 | .subscribe-wrap.is-hero form {
2909 |     display: flex;
2910 | }
2911 | 
2912 | .subscribe-wrap.is-hero input,
2913 | .subscribe-wrap.is-hero button {
2914 |     font-size: 2rem;
2915 | }
2916 | 
2917 | .subscribe-wrap.is-hero input {
2918 |     flex: 1 1 auto;
2919 |     margin-right: -60px;
2920 |     margin-bottom: 0;
2921 |     padding-right: calc(1.5em + 60px);
2922 |     transition: background-color 0.16s ease;
2923 |     background-color: var(--color-one);
2924 | }
2925 | 
2926 | .subscribe-wrap.is-hero input:hover,
2927 | .subscribe-wrap.is-hero input:focus {
2928 |     background-color: var(--color-two);
2929 | }
2930 | 
2931 | .subscribe-wrap.is-hero button {
2932 |     flex: 0 0 auto;
2933 |     width: auto;
2934 | }
2935 | 
2936 | .subscribe-wrap.is-hero button::before {
2937 |     background-color: var(--ghost-accent-color);
2938 | }
2939 | 
2940 | /* Alerts
2941 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2942 | .subscribe-wrap form.loading + .subscribe-alert .alert-loading,
2943 | .subscribe-wrap form.success + .subscribe-alert .alert-success,
2944 | .subscribe-wrap form.error + .subscribe-alert .alert-error {
2945 |     display: inline-block;
2946 |     margin-top: 1.4vh;
2947 | }
2948 | 
2949 | /* RWD — Subscribe form
2950 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
2951 | @media (max-width: 1480px) {
2952 |     .subscribe-form {
2953 |         padding: 30px;
2954 |     }
2955 | 
2956 |     .subscribe-wrap.is-hero {
2957 |         max-width: 400px;
2958 |     }
2959 | 
2960 |     .subscribe-title {
2961 |         font-size: 3rem;
2962 |         margin-bottom: 2vh;
2963 |     }
2964 | 
2965 |     .subscribe-wrap:not(.is-hero) input,
2966 |     .subscribe-wrap:not(.is-hero) button {
2967 |         padding-top: 14px;
2968 |         padding-bottom: 14px;
2969 |     }
2970 | 
2971 |     .subscribe-wrap.is-hero input,
2972 |     .subscribe-wrap.is-hero button {
2973 |         font-size: 1.8rem;
2974 |     }
2975 | }
2976 | 
2977 | @media (max-width: 1280px) {
2978 |     .subscribe-form {
2979 |         padding: 26px 2vw;
2980 |     }
2981 | 
2982 |     .subscribe-title {
2983 |         font-size: 2.5rem;
2984 |     }
2985 | 
2986 |     .subscribe-form button {
2987 |         font-size: 1.6rem;
2988 |     }
2989 | }
2990 | 
2991 | @media (max-width: 1024px) {
2992 |     .subscribe-form {
2993 |         padding: 20px;
2994 |     }
2995 | 
2996 |     .subscribe-wrap.is-hero {
2997 |         max-width: 340px;
2998 |         margin-top: 4vh;
2999 |     }
3000 | 
3001 |     .subscribe-title {
3002 |         font-size: 2.3rem;
3003 |         margin-bottom: 1.8vh;
3004 |     }
3005 | 
3006 |     .subscribe-form input {
3007 |         margin-bottom: 0.8vh;
3008 |         padding-top: 11px;
3009 |         padding-bottom: 11px;
3010 |     }
3011 | 
3012 |     .subscribe-form button {
3013 |         padding-top: 12px;
3014 |         padding-bottom: 12px;
3015 |     }
3016 | 
3017 |     .subscribe-wrap.is-hero input,
3018 |     .subscribe-wrap.is-hero button {
3019 |         font-size: 1.6rem;
3020 |     }
3021 | }
3022 | 
3023 | @media (max-width: 768px) {
3024 |     .subscribe-form {
3025 |         display: none;
3026 |     }
3027 | }
3028 | 
3029 | @media (max-width: 480px) {
3030 |     .subscribe-wrap.is-hero {
3031 |         max-width: 100%;
3032 |     }
3033 | }
3034 | 
3035 | @media (min-width: 1480px) {
3036 |     .subscribe-wrap.is-hero .subscribe-alert {
3037 |         position: absolute;
3038 |         top: 55px;
3039 |         right: 0;
3040 |         left: 0;
3041 |         text-align: center;
3042 |     }
3043 | }
3044 | 
3045 | /* --------------------------------------------------------------------------
3046 |    9.Pagination
3047 |    -------------------------------------------------------------------------- */
3048 | .pagination-section {
3049 |     text-align: center;
3050 | }
3051 | 
3052 | .pagination-section button {
3053 |     margin-bottom: 12vh;
3054 |     padding-top: 0.95em;
3055 |     padding-bottom: 0.95em;
3056 | }
3057 | 
3058 | /* --------------------------------------------------------------------------
3059 |    10.Search function
3060 |    -------------------------------------------------------------------------- */
3061 | .search-section {
3062 |     position: absolute;
3063 |     z-index: 997;
3064 |     display: none;
3065 | }
3066 | 
3067 | .search-wrap {
3068 |     max-width: 760px;
3069 |     margin: 7vh auto;
3070 | }
3071 | 
3072 | .search-overlay {
3073 |     position: fixed;
3074 |     z-index: 996;
3075 |     background-color: var(--opacity-search);
3076 |     -webkit-backdrop-filter: blur(2px);
3077 |     backdrop-filter: blur(2px);
3078 | }
3079 | 
3080 | .search-section,
3081 | .search-overlay,
3082 | .search-is-active .global-wrap {
3083 |     top: 0;
3084 |     right: 0;
3085 |     left: 0;
3086 |     min-height: 100%;
3087 | }
3088 | 
3089 | .search-wrap,
3090 | .search-content {
3091 |     position: relative;
3092 |     z-index: 998;
3093 | }
3094 | 
3095 | .search-wrap,
3096 | .search-meta {
3097 |     pointer-events: none;
3098 | }
3099 | 
3100 | .search-close,
3101 | .search-form input,
3102 | .search-results img,
3103 | .search-results span {
3104 |     pointer-events: auto;
3105 | }
3106 | 
3107 | /* If search is active
3108 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3109 | .search-is-active {
3110 |     overflow-y: scroll;
3111 |     -webkit-overflow-scrolling: auto;
3112 | }
3113 | 
3114 | .search-is-active .global-wrap {
3115 |     position: fixed;
3116 |     overflow: hidden;
3117 | }
3118 | 
3119 | /* Content
3120 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3121 | .search-content {
3122 |     max-width: 100%;
3123 |     margin: 0 2vw;
3124 |     background-color: var(--color-six);
3125 |     box-shadow:
3126 |         0 20px 25px -5px rgba(0, 0, 0, 0.1),
3127 |         0 8px 10px -6px rgba(0, 0, 0, 0.1);
3128 |     will-change: transform;
3129 | }
3130 | 
3131 | /* Close
3132 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3133 | .search-close {
3134 |     position: absolute;
3135 |     z-index: 999;
3136 |     top: 50%;
3137 |     right: 3vw;
3138 |     cursor: pointer;
3139 |     transform: translateY(-50%);
3140 | }
3141 | 
3142 | .search-close svg {
3143 |     width: 22px;
3144 |     height: 22px;
3145 |     fill: var(--color-font-one);
3146 | }
3147 | 
3148 | /* Form
3149 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3150 | .search-form {
3151 |     position: relative;
3152 |     box-sizing: border-box;
3153 |     width: 100%;
3154 |     padding: 3vh 2vw;
3155 | }
3156 | 
3157 | .search-form input {
3158 |     font-family: var(--font-family-one);
3159 |     font-size: 4.6rem;
3160 |     font-weight: var(--font-weight-one-bold);
3161 |     width: 100%;
3162 |     max-width: 500px;
3163 |     padding: 0;
3164 |     letter-spacing: var(--letter-spacing, normal);
3165 |     word-break: normal;
3166 | }
3167 | 
3168 | .search-form input::placeholder {
3169 |     opacity: 1;
3170 | }
3171 | 
3172 | .search-form input::-moz-placeholder {
3173 |     opacity: 1;
3174 | }
3175 | 
3176 | /* Meta
3177 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3178 | .search-meta {
3179 |     font-size: 1.4rem;
3180 |     margin-top: 0.8em;
3181 |     opacity: var(--opacity-one);
3182 | }
3183 | 
3184 | .search-meta .is-hide {
3185 |     display: none;
3186 | }
3187 | 
3188 | /* Results
3189 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3190 | .search-results {
3191 |     display: grid;
3192 |     box-sizing: border-box;
3193 |     width: 100%;
3194 |     height: 100%;
3195 |     padding: 0 2vw 7vh;
3196 |     grid-template-columns: repeat(1, 1fr);
3197 | }
3198 | 
3199 | .search-results:empty {
3200 |     padding-top: 0;
3201 |     padding-bottom: 0;
3202 | }
3203 | 
3204 | .search-results a {
3205 |     display: grid;
3206 |     align-items: start;
3207 |     padding: 1.2vh 0;
3208 |     grid-template-columns: repeat(7, 1fr);
3209 |     grid-template-rows: -webkit-min-content;
3210 |     grid-template-rows: min-content;
3211 | }
3212 | 
3213 | .search-results img {
3214 |     line-height: 0;
3215 |     width: 70px;
3216 |     height: 70px;
3217 |     margin-right: 10px;
3218 |     border-radius: calc(var(--border-radius) / 1.5);
3219 |     grid-column: span 1;
3220 |     grid-row: span 3;
3221 | }
3222 | 
3223 | .search-results h5 {
3224 |     font-size: 2.2rem;
3225 |     line-height: 1.3;
3226 |     display: inline-block;
3227 |     margin: 4px 0 0;
3228 | }
3229 | 
3230 | .search-results h5:hover {
3231 |     text-decoration: underline;
3232 | }
3233 | 
3234 | .search-results h5,
3235 | .search-results time {
3236 |     grid-column: span 6;
3237 | }
3238 | 
3239 | .search-results time {
3240 |     font-size: 1.2rem;
3241 |     display: block;
3242 |     margin-top: 0.6vh;
3243 |     opacity: var(--opacity-one);
3244 | }
3245 | 
3246 | /* Animation
3247 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3248 | .search-is-active .search-wrap {
3249 |     -webkit-animation: searchOne 0.2s ease;
3250 |     animation: searchOne 0.2s ease;
3251 | }
3252 | 
3253 | .search-is-active .search-overlay {
3254 |     -webkit-animation: searchTwo 0.2s ease;
3255 |     animation: searchTwo 0.2s ease;
3256 | }
3257 | 
3258 | body.search-no-active .search-section {
3259 |     visibility: hidden;
3260 |     -webkit-animation: searchThree 0s ease;
3261 |     animation: searchThree 0s ease;
3262 | }
3263 | 
3264 | @-webkit-keyframes searchOne {
3265 |     0% {
3266 |         transform: translateY(30px);
3267 |         opacity: 0;
3268 |     }
3269 | 
3270 |     100% {
3271 |         transform: translateY(0);
3272 |         opacity: 1;
3273 |     }
3274 | }
3275 | 
3276 | @keyframes searchOne {
3277 |     0% {
3278 |         transform: translateY(30px);
3279 |         opacity: 0;
3280 |     }
3281 | 
3282 |     100% {
3283 |         transform: translateY(0);
3284 |         opacity: 1;
3285 |     }
3286 | }
3287 | 
3288 | @-webkit-keyframes searchTwo {
3289 |     0% {
3290 |         opacity: 0;
3291 |     }
3292 | 
3293 |     100% {
3294 |         opacity: 1;
3295 |     }
3296 | }
3297 | 
3298 | @keyframes searchTwo {
3299 |     0% {
3300 |         opacity: 0;
3301 |     }
3302 | 
3303 |     100% {
3304 |         opacity: 1;
3305 |     }
3306 | }
3307 | 
3308 | @-webkit-keyframes searchThree {
3309 |     from,
3310 |     to {
3311 |         visibility: visible;
3312 |     }
3313 | }
3314 | 
3315 | @keyframes searchThree {
3316 |     from,
3317 |     to {
3318 |         visibility: visible;
3319 |     }
3320 | }
3321 | 
3322 | /* RWD — Search function
3323 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3324 | @media (max-width: 1280px) {
3325 |     .search-wrap {
3326 |         max-width: 600px;
3327 |     }
3328 | 
3329 |     .search-form,
3330 |     .search-results {
3331 |         padding-right: 3vw;
3332 |         padding-left: 3vw;
3333 |     }
3334 | 
3335 |     .search-form input {
3336 |         font-size: 3.6rem;
3337 |         max-width: 80%;
3338 |     }
3339 | 
3340 |     .search-meta {
3341 |         font-size: 1.3rem;
3342 |         margin-top: 5px;
3343 |     }
3344 | 
3345 |     .search-results img {
3346 |         width: 60px;
3347 |         height: 60px;
3348 |     }
3349 | 
3350 |     .search-results h5 {
3351 |         font-size: 1.8rem;
3352 |     }
3353 | }
3354 | 
3355 | @media (max-width: 480px) {
3356 |     .search-form,
3357 |     .search-results {
3358 |         padding-right: var(--margin-wrap-left-right);
3359 |         padding-left: var(--margin-wrap-left-right);
3360 |     }
3361 | 
3362 |     .search-close {
3363 |         right: var(--margin-wrap-left-right);
3364 |     }
3365 | 
3366 |     .search-form input {
3367 |         font-size: 3rem;
3368 |     }
3369 | }
3370 | 
3371 | /* --------------------------------------------------------------------------
3372 |    11.Post — Header
3373 |    -------------------------------------------------------------------------- */
3374 | .post-header {
3375 |     width: 100%;
3376 | }
3377 | 
3378 | .post-header-wrap {
3379 |     display: flex;
3380 |     flex-wrap: wrap;
3381 |     margin-top: 2vh;
3382 |     margin-bottom: 7vh;
3383 | }
3384 | 
3385 | .post-header-content,
3386 | .post-header-image {
3387 |     width: 100%;
3388 |     margin-right: auto;
3389 |     margin-left: auto;
3390 | }
3391 | 
3392 | /* Content
3393 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3394 | .post-header-content {
3395 |     max-width: var(--max-width-post-wrap-one);
3396 | }
3397 | 
3398 | /* Tags
3399 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3400 | .post-title + .post-tags,
3401 | .post-excerpt + .post-tags {
3402 |     max-width: 800px;
3403 |     margin-top: 3vh;
3404 | }
3405 | 
3406 | /* Title
3407 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3408 | .post-title {
3409 |     margin-top: 2vh;
3410 |     margin-bottom: 2.6vh;
3411 |     letter-spacing: var(--letter-spacing, normal);
3412 | }
3413 | 
3414 | /* Excerpt
3415 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3416 | .post-excerpt {
3417 |     margin-top: 2.6vh;
3418 |     margin-bottom: 0;
3419 | }
3420 | 
3421 | /* Image
3422 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3423 | .post-header-image {
3424 |     margin-top: 5vh;
3425 | }
3426 | 
3427 | .post-header-image figure {
3428 |     margin: 0;
3429 | }
3430 | 
3431 | /* Figcaption */
3432 | .post-header-image figcaption {
3433 |     font-size: 1rem;
3434 |     margin-top: 12px;
3435 |     text-align: left;
3436 |     opacity: var(--opacity-one);
3437 | }
3438 | 
3439 | .post-header-image figcaption a {
3440 |     transition: opacity 0.1s ease;
3441 |     text-decoration: underline;
3442 | }
3443 | 
3444 | .post-header-image figcaption a:hover {
3445 |     opacity: 0.6;
3446 | }
3447 | 
3448 | /* Meta
3449 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3450 | .post-meta-wrap {
3451 |     display: flex;
3452 |     margin-top: 2.4vh;
3453 |     padding-top: 2.4vh;
3454 |     border-top: var(--border) var(--color-border-one);
3455 | }
3456 | 
3457 | .post-excerpt + .post-meta-wrap {
3458 |     margin-top: 4vh;
3459 | }
3460 | 
3461 | /* Center
3462 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3463 | .post-header-wrap.is-center {
3464 |     text-align: center;
3465 | }
3466 | 
3467 | .post-header-wrap.is-center .post-excerpt {
3468 |     margin-right: auto;
3469 |     margin-left: auto;
3470 | }
3471 | 
3472 | /* RWD — Post — Header
3473 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3474 | @media (max-width: 1024px) {
3475 |     .post-header-wrap {
3476 |         margin-top: 0;
3477 |         margin-bottom: 5vh;
3478 |     }
3479 | 
3480 |     .post-header-content {
3481 |         max-width: var(--max-width-post-wrap-two);
3482 |     }
3483 | 
3484 |     .post-title {
3485 |         margin-top: 1.2vh;
3486 |         margin-bottom: 2.2vh;
3487 |     }
3488 | 
3489 |     .post-excerpt {
3490 |         margin-top: 2.2vh;
3491 |     }
3492 | }
3493 | 
3494 | @media (max-width: 768px) {
3495 |     .post-header-content {
3496 |         max-width: 100%;
3497 |     }
3498 | 
3499 |     .post-header-image {
3500 |         margin-top: 3.4vh;
3501 |     }
3502 | }
3503 | 
3504 | @media (min-width: 1025px) {
3505 |     .post-header .post-tags small {
3506 |         margin-bottom: 0.8vh;
3507 |     }
3508 | 
3509 |     .post-tags small,
3510 |     .post-tags a {
3511 |         padding: 8px 14px;
3512 |     }
3513 | 
3514 |     .post-header-image:not(.is-wide) {
3515 |         max-width: var(--max-width-post-wrap-one);
3516 |     }
3517 | 
3518 |     .post-section.is-sidebar .post-header-content,
3519 |     .post-section.is-sidebar .post-header-image:not(.is-wide) {
3520 |         max-width: var(--max-width-content-wrap);
3521 |     }
3522 | 
3523 |     .post-section.is-sidebar .post-title {
3524 |         font-size: 5.9rem;
3525 |         max-width: 800px;
3526 |     }
3527 | 
3528 |     .post-section.is-sidebar .post-excerpt {
3529 |         max-width: 700px;
3530 |     }
3531 | }
3532 | 
3533 | @media (min-width: 1280px) {
3534 |     .post-section.is-sidebar .post-title {
3535 |         font-size: 6.4rem;
3536 |         max-width: 840px;
3537 |     }
3538 | 
3539 |     .post-section.is-sidebar .post-excerpt {
3540 |         max-width: 780px;
3541 |     }
3542 | }
3543 | 
3544 | @media (min-width: 1480px) {
3545 |     .post-section.is-sidebar .post-title {
3546 |         font-size: 7rem;
3547 |         max-width: 860px;
3548 |     }
3549 | 
3550 |     .post-section.is-sidebar .post-excerpt {
3551 |         max-width: 800px;
3552 |     }
3553 | }
3554 | 
3555 | /* --------------------------------------------------------------------------
3556 |    12.Post — Content
3557 |    -------------------------------------------------------------------------- */
3558 | .post-wrap {
3559 |     position: relative;
3560 | }
3561 | 
3562 | .post-content {
3563 |     font-size: 2rem;
3564 |     max-width: var(--max-width-post-wrap-one);
3565 |     min-height: 1px;
3566 |     margin: 5vh auto 15vh;
3567 | }
3568 | 
3569 | /* Margin elements
3570 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3571 | .post-content h1:first-child,
3572 | .post-content h2:first-child,
3573 | .post-content h3:first-child,
3574 | .post-content h4:first-child,
3575 | .post-content h5:first-child,
3576 | .post-content h6:first-child,
3577 | .post-content p:first-child {
3578 |     margin-top: 0;
3579 | }
3580 | 
3581 | .post-content p,
3582 | .post-content iframe,
3583 | .post-content ol,
3584 | .post-content ul,
3585 | .post-content table {
3586 |     margin-top: 0;
3587 |     margin-bottom: 30px;
3588 | }
3589 | 
3590 | .post-content hr,
3591 | .post-content blockquote,
3592 | .post-content .kg-card.kg-header-card {
3593 |     margin-top: 55px;
3594 |     margin-bottom: 55px;
3595 | }
3596 | 
3597 | .post-content pre,
3598 | .post-content .kg-card {
3599 |     width: 100%;
3600 |     margin-top: 40px;
3601 |     margin-bottom: 40px;
3602 | }
3603 | 
3604 | .post-content blockquote,
3605 | .post-content .kg-card {
3606 |     margin-right: 0;
3607 |     margin-left: 0;
3608 | }
3609 | 
3610 | .post-content
3611 |     .kg-card:not(.kg-width-full):not(.kg-image-card):not(.kg-gallery-card):not(
3612 |         .kg-embed-card
3613 |     )
3614 |     + .kg-card {
3615 |     margin-top: -20px;
3616 | }
3617 | 
3618 | /* Social media
3619 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3620 | .post-content iframe,
3621 | .post-content .kg-embed-card > div,
3622 | .post-content .kg-embed-card > iframe,
3623 | .post-content .kg-embed-card > .fb-post,
3624 | .post-content .kg-embed-card > .twitter-tweet {
3625 |     margin-right: auto !important;
3626 |     margin-left: auto !important;
3627 | }
3628 | 
3629 | .post-content .kg-embed-card > .twitter-tweet > iframe {
3630 |     margin-bottom: 0;
3631 | }
3632 | 
3633 | /* Typography
3634 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3635 | .post-content h1,
3636 | .post-content h2,
3637 | .post-content h3 {
3638 |     line-height: 1.4;
3639 |     margin-top: 1em;
3640 |     margin-bottom: 18px;
3641 |     margin-left: -1px;
3642 | }
3643 | 
3644 | .post-content h4,
3645 | .post-content h5,
3646 | .post-content h6 {
3647 |     font-family: var(--font-family-three);
3648 |     font-weight: var(--font-weight-three-bold);
3649 |     line-height: 1.55;
3650 |     margin-top: 1.2em;
3651 |     margin-bottom: 10px;
3652 | }
3653 | 
3654 | .post-content h1 {
3655 |     font-size: 5.8rem;
3656 | }
3657 | 
3658 | .post-content h2 {
3659 |     font-size: 4.5rem;
3660 | }
3661 | 
3662 | .post-content h3 {
3663 |     font-size: 3.2rem;
3664 | }
3665 | 
3666 | .post-content h4 {
3667 |     font-size: 2.4rem;
3668 | }
3669 | 
3670 | .post-content h5 {
3671 |     font-size: 2rem;
3672 | }
3673 | 
3674 | .post-content h6 {
3675 |     font-size: 1.4rem;
3676 |     letter-spacing: 1px;
3677 |     text-transform: uppercase;
3678 | }
3679 | 
3680 | /* Paragraph
3681 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3682 | .post-content p {
3683 |     line-height: 1.6;
3684 |     position: relative;
3685 | }
3686 | 
3687 | /* Strong
3688 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3689 | .post-content strong {
3690 |     font-weight: var(--font-weight-three-bold);
3691 | }
3692 | 
3693 | /* Mark
3694 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3695 | .post-content mark a {
3696 |     color: var(--color-font-black);
3697 | }
3698 | 
3699 | /* hr
3700 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3701 | .post-content hr {
3702 |     border-top: var(--border) var(--color-border-one);
3703 |     border-right: 0;
3704 |     border-bottom: 0;
3705 |     border-left: 0;
3706 | }
3707 | 
3708 | /* kbd
3709 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3710 | .post-content kbd {
3711 |     font-size: 70%;
3712 |     display: inline-block;
3713 |     padding: 2px 8px 1px;
3714 |     border: 1px solid;
3715 |     border-radius: 4px;
3716 | }
3717 | 
3718 | /* iframe
3719 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3720 | .post-content iframe {
3721 |     display: block;
3722 | }
3723 | 
3724 | /* Links
3725 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3726 | .post-content a {
3727 |     transition: color 0.1s ease;
3728 |     text-decoration: underline;
3729 | }
3730 | 
3731 | .post-content a:hover {
3732 |     color: var(--ghost-accent-color);
3733 | }
3734 | 
3735 | /* Blockquote
3736 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3737 | .post-content blockquote,
3738 | .post-content blockquote p {
3739 |     line-height: 1.4;
3740 | }
3741 | 
3742 | .post-content blockquote p {
3743 |     margin: 0;
3744 | }
3745 | 
3746 | .post-content blockquote {
3747 |     font-family: var(--font-family-two);
3748 |     font-size: 2rem;
3749 |     font-weight: var(--font-weight-two-bold);
3750 |     box-sizing: border-box;
3751 |     width: 100%;
3752 |     padding-top: 5px;
3753 |     padding-bottom: 5px;
3754 |     padding-left: 1em;
3755 |     border-left: 4px solid var(--ghost-accent-color);
3756 | }
3757 | 
3758 | /* Alternative */
3759 | .post-content blockquote.kg-blockquote-alt {
3760 |     font-family: var(--font-family-one);
3761 |     font-size: 2rem;
3762 |     font-weight: var(--font-weight-one-bold);
3763 |     font-style: normal;
3764 |     line-height: 1.3;
3765 |     padding: 2vh 0;
3766 |     text-align: center;
3767 |     border: 0;
3768 | }
3769 | 
3770 | .post-content blockquote.kg-blockquote-alt::before {
3771 |     font-size: 120%;
3772 |     line-height: 0.4;
3773 |     display: block;
3774 |     content: "";
3775 |     color: var(--ghost-accent-color);
3776 | }
3777 | 
3778 | /* Lists
3779 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3780 | .post-content ul,
3781 | .post-content ol {
3782 |     margin-right: 0;
3783 |     margin-left: 15px;
3784 | }
3785 | 
3786 | .post-content ul {
3787 |     padding-left: 15px;
3788 |     list-style: disc outside;
3789 | }
3790 | 
3791 | .post-content ol {
3792 |     padding-left: 20px;
3793 | }
3794 | 
3795 | .post-content ul li ul {
3796 |     list-style: circle outside;
3797 | }
3798 | 
3799 | .post-content ol,
3800 | .post-content ol li ol {
3801 |     list-style: decimal outside;
3802 | }
3803 | 
3804 | .post-content ul ul,
3805 | .post-content ul ol,
3806 | .post-content ol ol,
3807 | .post-content ol ul {
3808 |     font-size: 90%;
3809 |     margin: 15px 0;
3810 | }
3811 | 
3812 | .post-content li {
3813 |     margin-bottom: 10px;
3814 | }
3815 | 
3816 | .post-content dl dt {
3817 |     float: left;
3818 |     clear: left;
3819 |     overflow: hidden;
3820 |     width: 180px;
3821 |     margin-bottom: 10px;
3822 |     text-align: right;
3823 |     white-space: nowrap;
3824 |     text-overflow: ellipsis;
3825 | }
3826 | 
3827 | .post-content dl dd {
3828 |     margin-bottom: 10px;
3829 |     margin-left: 200px;
3830 | }
3831 | 
3832 | /* Table
3833 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3834 | .post-content table {
3835 |     font-size: 1.4rem;
3836 |     display: table;
3837 |     width: 100%;
3838 |     max-width: 100%;
3839 |     border-spacing: 0;
3840 |     border-collapse: collapse;
3841 |     text-align: left;
3842 |     background-color: transparent;
3843 | }
3844 | 
3845 | .post-content th {
3846 |     font-size: 1.6rem;
3847 |     color: var(--color-font-two);
3848 |     background-color: var(--color-three);
3849 | }
3850 | 
3851 | .post-content th,
3852 | .post-content td {
3853 |     display: table-cell;
3854 |     padding: 10px 12px;
3855 | }
3856 | 
3857 | .post-content td {
3858 |     border-bottom: var(--border) var(--color-border-one);
3859 | }
3860 | 
3861 | .post-content th:first-child,
3862 | .post-content td:first-child {
3863 |     padding-left: 10px;
3864 | }
3865 | 
3866 | .post-content th:last-child,
3867 | .post-content td:last-child {
3868 |     padding-right: 10px;
3869 | }
3870 | 
3871 | /* Responsive */
3872 | .post-content .responsive-table {
3873 |     overflow-x: auto;
3874 |     word-break: normal;
3875 | }
3876 | 
3877 | /* Footnotes
3878 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3879 | .post-content .footnotes {
3880 |     padding: 10px 0 0;
3881 | }
3882 | 
3883 | .post-content .footnote-ref {
3884 |     font-size: 65%;
3885 | }
3886 | 
3887 | .post-content .footnotes-list {
3888 |     padding-left: 5px;
3889 |     list-style: decimal;
3890 | }
3891 | 
3892 | .post-content .footnotes-sep {
3893 |     display: none;
3894 | }
3895 | 
3896 | .post-content .footnotes p,
3897 | .post-content .footnote-item {
3898 |     font-size: 1.4rem;
3899 |     line-height: 1.3;
3900 |     margin-bottom: 10px;
3901 | }
3902 | 
3903 | /* Code
3904 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3905 | .post-content pre {
3906 |     min-width: 100%;
3907 | }
3908 | 
3909 | .post-content code {
3910 |     font-size: 85%;
3911 |     padding: 2px 5px;
3912 |     background-color: var(--color-five);
3913 | }
3914 | 
3915 | .post-content blockquote code {
3916 |     font-size: 75%;
3917 | }
3918 | 
3919 | .post-content blockquote code,
3920 | .post-content p code {
3921 |     border-radius: 5px;
3922 | }
3923 | 
3924 | .post-content pre > code {
3925 |     display: block;
3926 |     padding: 20px 25px;
3927 |     white-space: pre-wrap;
3928 | }
3929 | 
3930 | /* Image & Video
3931 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3932 | .post-content img {
3933 |     position: relative;
3934 |     max-width: 100%;
3935 |     height: auto;
3936 | }
3937 | 
3938 | .post-content .kg-image-card {
3939 |     line-height: 0;
3940 | }
3941 | 
3942 | .post-content .kg-image-card.kg-width-wide img {
3943 |     width: 100%;
3944 | }
3945 | 
3946 | .post-content .kg-image-card.kg-width-wide img,
3947 | .post-content .kg-image-card.kg-width-full img {
3948 |     max-width: initial;
3949 | }
3950 | 
3951 | .post-content .kg-video-card.kg-width-full,
3952 | .post-content .kg-image-card.kg-width-full img {
3953 |     position: relative;
3954 |     right: 50%;
3955 |     left: 50%;
3956 |     width: calc(100vw - var(--scrollbar-width, 0px));
3957 |     margin-left: calc(-50vw + var(--scrollbar-width, 0px) / 2);
3958 |     border-radius: 0;
3959 | }
3960 | 
3961 | /* Small image */
3962 | .post-content .kg-image-card:not(.kg-width-full):not(.kg-width-wide) {
3963 |     text-align: center;
3964 | }
3965 | 
3966 | /* Gallery
3967 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3968 | .post-content .kg-gallery-card .kg-gallery-image img {
3969 |     border-radius: 0;
3970 | }
3971 | 
3972 | .post-content .kg-gallery-card .kg-gallery-row:not(:first-of-type) {
3973 |     margin: 1.1vmin 0 0 0;
3974 | }
3975 | 
3976 | .post-content .kg-gallery-card .kg-gallery-image:not(:first-of-type) {
3977 |     margin: 0 0 0 1.1vmin;
3978 | }
3979 | 
3980 | /* Callouts
3981 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3982 | .post-content .kg-callout-card .kg-callout-emoji {
3983 |     flex-shrink: 0;
3984 | }
3985 | 
3986 | /* Audio & File
3987 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
3988 | .post-content .kg-file-card .kg-file-card-container {
3989 |     padding: 8px;
3990 | }
3991 | 
3992 | .post-content .kg-audio-card svg {
3993 |     fill: var(--color-three);
3994 | }
3995 | 
3996 | .post-content .kg-audio-card .kg-audio-playback-rate {
3997 |     color: var(--color-font-one);
3998 | }
3999 | 
4000 | .post-content .kg-audio-card .kg-audio-title,
4001 | .post-content .kg-file-card .kg-file-card-title {
4002 |     font-size: 1.8rem;
4003 | }
4004 | 
4005 | /* Buttons & Products
4006 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4007 | .post-content .kg-button-card .kg-btn:hover,
4008 | .post-content .kg-product-card .kg-product-card-button:hover {
4009 |     opacity: 0.8;
4010 | }
4011 | 
4012 | .kg-card.kg-product-card .kg-product-card-button {
4013 |     font-size: clamp(1.6rem, 0.3vw + 1.5rem, 2rem);
4014 | }
4015 | 
4016 | /* NFT
4017 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4018 | .post-content .kg-nft-card a {
4019 |     text-decoration: none;
4020 | }
4021 | 
4022 | /* Headers
4023 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4024 | .post-content .kg-header-card {
4025 |     position: relative;
4026 |     right: 50%;
4027 |     left: 50%;
4028 |     width: calc(100vw - var(--scrollbar-width, 0px));
4029 |     margin-left: calc(-50vw + var(--scrollbar-width, 0px) / 2);
4030 | }
4031 | 
4032 | .post-content .kg-header-card.kg-style-light {
4033 |     background-color: var(--color-five);
4034 | }
4035 | 
4036 | .post-content .kg-header-card.kg-style-dark {
4037 |     background-color: var(--color-three);
4038 | }
4039 | 
4040 | .post-content .kg-header-card.kg-style-dark .kg-header-card-header,
4041 | .post-content .kg-header-card.kg-style-dark .kg-header-card-subheader {
4042 |     color: var(--color-font-two);
4043 | }
4044 | 
4045 | .post-content .kg-header-card.kg-style-image .kg-header-card-button,
4046 | .post-content
4047 |     .kg-header-card.kg-style-accent:not(.kg-v2)
4048 |     .kg-header-card-button {
4049 |     color: var(--color-font-black);
4050 |     background-color: var(--color-white);
4051 | }
4052 | 
4053 | .post-content .kg-header-card.kg-style-dark .kg-header-card-button {
4054 |     color: var(--color-font-one);
4055 |     background-color: var(--color-four);
4056 | }
4057 | 
4058 | .post-content .kg-header-card .kg-header-card-header,
4059 | .post-content .kg-header-card .kg-header-card-header strong {
4060 |     font-weight: var(--font-weight-one-bold);
4061 | }
4062 | 
4063 | .post-content .kg-header-card h2 + .kg-header-card-subheader {
4064 |     margin-top: 2.5vh;
4065 | }
4066 | 
4067 | .post-content .kg-header-card .kg-header-card-subheader {
4068 |     margin-top: 1vh;
4069 |     margin-bottom: 1vh;
4070 |     opacity: 0.8;
4071 | }
4072 | 
4073 | /* Bookmarks
4074 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4075 | .post-content .kg-bookmark-card .kg-bookmark-title {
4076 |     font-size: 1.6rem;
4077 |     line-height: 1.3;
4078 | }
4079 | 
4080 | .post-content .kg-bookmark-card .kg-bookmark-metadata > :not(img) {
4081 |     opacity: 1;
4082 | }
4083 | 
4084 | .post-content .kg-bookmark-card .kg-bookmark-icon {
4085 |     border-radius: 0;
4086 | }
4087 | 
4088 | .post-content .kg-bookmark-card .kg-bookmark-thumbnail {
4089 |     min-width: 24%;
4090 |     margin: 10px;
4091 | }
4092 | 
4093 | .post-content .kg-bookmark-card .kg-bookmark-container,
4094 | .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4095 |     background: var(--color-body);
4096 |     color: var(--color-font-one);
4097 | }
4098 | 
4099 | /* Normalize 'Cards'
4100 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4101 | .post-content .kg-button-card .kg-btn,
4102 | .post-content .kg-audio-card .kg-audio-title,
4103 | .post-content .kg-file-card .kg-file-card-title,
4104 | .post-content .kg-toggle-card .kg-toggle-heading-text,
4105 | .post-content .kg-product-card .kg-product-card-title,
4106 | .post-content .kg-product-card .kg-product-card-button,
4107 | .post-content .kg-product-card .kg-product-card-description p,
4108 | .post-content .kg-product-card .kg-product-card-description ol,
4109 | .post-content .kg-product-card .kg-product-card-description ul,
4110 | .post-content .kg-header-card .kg-header-card-subheader,
4111 | .post-content .kg-header-card .kg-header-card-button,
4112 | .post-content .kg-bookmark-card .kg-bookmark-title,
4113 | .post-content .kg-bookmark-card .kg-bookmark-description,
4114 | .post-content .kg-bookmark-card .kg-bookmark-metadata > :not(img) {
4115 |     font-family: var(--font-family-three);
4116 | }
4117 | 
4118 | .post-content .kg-product-card .kg-product-card-description p,
4119 | .post-content .kg-product-card .kg-product-card-description ol,
4120 | .post-content .kg-product-card .kg-product-card-description ul,
4121 | .post-content .kg-header-card .kg-header-card-subheader,
4122 | .post-content .kg-bookmark-card .kg-bookmark-description {
4123 |     font-weight: var(--font-weight-three-regular);
4124 | }
4125 | 
4126 | .post-content .kg-button-card .kg-btn,
4127 | .post-content .kg-product-card .kg-product-card-button,
4128 | .post-content .kg-header-card .kg-header-card-button,
4129 | .post-content .kg-bookmark-card .kg-bookmark-metadata > :not(img) {
4130 |     font-weight: var(--font-weight-three-medium);
4131 | }
4132 | 
4133 | .post-content .kg-audio-card .kg-audio-title,
4134 | .post-content .kg-file-card .kg-file-card-title,
4135 | .post-content .kg-toggle-card .kg-toggle-heading-text,
4136 | .post-content .kg-product-card .kg-product-card-title,
4137 | .post-content .kg-bookmark-card .kg-bookmark-title {
4138 |     font-weight: var(--font-weight-three-bold);
4139 | }
4140 | 
4141 | .post-content .kg-button-card .kg-btn,
4142 | .post-content .kg-product-card .kg-product-card-button,
4143 | .post-content .kg-header-card .kg-header-card-button {
4144 |     transition: opacity 0.2s ease;
4145 |     border-radius: 100px;
4146 | }
4147 | 
4148 | .post-content .kg-button-card .kg-btn,
4149 | .post-content .kg-callout-card .kg-callout-card-accent,
4150 | .post-content .kg-product-card .kg-product-card-button,
4151 | .post-content
4152 |     .kg-header-card.kg-style-accent:not(.kg-v2)
4153 |     .kg-header-card-header,
4154 | .post-content
4155 |     .kg-header-card.kg-style-accent:not(.kg-v2)
4156 |     .kg-header-card-subheader,
4157 | .post-content .kg-header-card.kg-style-image .kg-header-card-header,
4158 | .post-content .kg-header-card.kg-style-image .kg-header-card-subheader,
4159 | .post-content .kg-header-card.kg-style-light .kg-header-card-button {
4160 |     color: var(--color-font-white);
4161 | }
4162 | 
4163 | .post-content .kg-file-card .kg-file-card-caption,
4164 | .post-content .kg-bookmark-card .kg-bookmark-description {
4165 |     font-size: 1rem;
4166 |     margin-top: 8px;
4167 | }
4168 | 
4169 | .post-content .kg-toggle-card,
4170 | .post-content .kg-product-card .kg-product-card-container,
4171 | .post-content .kg-bookmark-card .kg-bookmark-content {
4172 |     padding: 16px;
4173 | }
4174 | 
4175 | .post-content .kg-file-card .kg-file-card-container,
4176 | .post-content .kg-toggle-card,
4177 | .post-content .kg-bookmark-card .kg-bookmark-container,
4178 | .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4179 |     transition: border-color 0.15s ease;
4180 | }
4181 | 
4182 | .post-content .kg-audio-card,
4183 | .post-content .kg-file-card .kg-file-card-container,
4184 | .post-content .kg-toggle-card,
4185 | .post-content .kg-product-card .kg-product-card-container,
4186 | .post-content .kg-nft-card .kg-nft-card-container,
4187 | .post-content .kg-bookmark-card .kg-bookmark-container,
4188 | .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4189 |     border: var(--border) var(--color-border-one);
4190 |     box-shadow: none;
4191 | }
4192 | 
4193 | .post-content .kg-file-card .kg-file-card-container:hover,
4194 | .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4195 |     border-color: var(--color-border-two);
4196 | }
4197 | 
4198 | .post-content img,
4199 | .post-content code,
4200 | .post-content .kg-callout-card,
4201 | .post-content .kg-audio-card,
4202 | .post-content .kg-file-card .kg-file-card-container,
4203 | .post-content .kg-toggle-card,
4204 | .post-content .kg-product-card .kg-product-card-container,
4205 | .post-content .kg-nft-card .kg-nft-card-container,
4206 | .post-content .kg-bookmark-card .kg-bookmark-container,
4207 | .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4208 |     border-radius: calc(var(--border-radius) / 1.5);
4209 | }
4210 | 
4211 | .post-section.is-sidebar .kg-video-card.kg-width-full,
4212 | .post-section.is-sidebar .kg-image-card.kg-width-full img,
4213 | .post-section.is-sidebar .post-content .kg-header-card {
4214 |     border-radius: calc(var(--border-radius) / 1.5);
4215 | }
4216 | 
4217 | .post-content
4218 |     .kg-gallery-card
4219 |     .kg-gallery-row:first-of-type
4220 |     .kg-gallery-image:first-of-type
4221 |     img {
4222 |     border-top-left-radius: calc(var(--border-radius) / 1.5);
4223 | }
4224 | 
4225 | .post-content
4226 |     .kg-gallery-card
4227 |     .kg-gallery-row:first-of-type
4228 |     .kg-gallery-image:last-of-type
4229 |     img {
4230 |     border-top-right-radius: calc(var(--border-radius) / 1.5);
4231 | }
4232 | 
4233 | .post-content
4234 |     .kg-gallery-card
4235 |     .kg-gallery-row:last-of-type
4236 |     .kg-gallery-image:first-of-type
4237 |     img {
4238 |     border-bottom-left-radius: calc(var(--border-radius) / 1.5);
4239 | }
4240 | 
4241 | .post-content
4242 |     .kg-gallery-card
4243 |     .kg-gallery-row:last-of-type
4244 |     .kg-gallery-image:last-of-type
4245 |     img {
4246 |     border-bottom-right-radius: calc(var(--border-radius) / 1.5);
4247 | }
4248 | 
4249 | .post-content .kg-audio-card .kg-audio-thumbnail,
4250 | .post-content .kg-file-card .kg-file-card-icon::before,
4251 | .post-content .kg-product-card img,
4252 | .post-content .kg-nft-card .kg-nft-image,
4253 | .post-content .kg-bookmark-card .kg-bookmark-thumbnail img {
4254 |     border-radius: calc(var(--border-radius) / 3);
4255 | }
4256 | 
4257 | /* Figcaption
4258 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4259 | .post-content figcaption {
4260 |     font-size: 1.5rem;
4261 |     line-height: 1.2;
4262 |     display: block;
4263 |     width: 100%;
4264 |     margin-top: 10px;
4265 |     text-align: center;
4266 |     opacity: var(--opacity-one);
4267 | }
4268 | 
4269 | .post-content figcaption a {
4270 |     transition: opacity 0.1s ease;
4271 |     text-decoration: underline;
4272 | }
4273 | 
4274 | .post-content figcaption a:hover {
4275 |     opacity: 0.6;
4276 |     color: var(--color-font-one);
4277 | }
4278 | 
4279 | /* CTA
4280 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4281 | .post-content .members-cta {
4282 |     position: relative;
4283 |     z-index: 1;
4284 |     box-sizing: border-box;
4285 |     margin-bottom: 10vh;
4286 |     padding: 6vh 3vw;
4287 |     text-align: center;
4288 |     background-color: var(--color-five);
4289 | }
4290 | 
4291 | .post-content .members-cta h2 {
4292 |     font-size: 5.2rem;
4293 |     line-height: 1.2;
4294 |     margin: 0 auto 3vh;
4295 | }
4296 | 
4297 | .post-content .members-cta p {
4298 |     line-height: 1.5;
4299 |     max-width: 520px;
4300 |     margin: 3vh auto 4vh;
4301 | }
4302 | 
4303 | .post-content .members-cta small {
4304 |     margin-top: 4vh;
4305 | }
4306 | 
4307 | .post-content .members-cta-teaser {
4308 |     position: relative;
4309 | }
4310 | 
4311 | .post-content .members-cta-teaser::after {
4312 |     position: absolute;
4313 |     z-index: 0;
4314 |     right: 50%;
4315 |     bottom: 0;
4316 |     left: 50%;
4317 |     width: calc(100vw - 40px);
4318 |     height: 100%;
4319 |     max-height: 300px;
4320 |     margin-left: calc(-50vw + 20px);
4321 |     content: "";
4322 |     pointer-events: none;
4323 |     opacity: 1;
4324 |     background-color: var(--color-body);
4325 |     -webkit-mask-image: linear-gradient(
4326 |         to bottom,
4327 |         transparent,
4328 |         rgba(0, 0, 0, 0.013) 8.1%,
4329 |         rgba(0, 0, 0, 0.049) 15.5%,
4330 |         rgba(0, 0, 0, 0.104) 22.5%,
4331 |         rgba(0, 0, 0, 0.175) 29%,
4332 |         rgba(0, 0, 0, 0.259) 35.3%,
4333 |         rgba(0, 0, 0, 0.352) 41.2%,
4334 |         rgba(0, 0, 0, 0.45) 47.1%,
4335 |         rgba(0, 0, 0, 0.55) 52.9%,
4336 |         rgba(0, 0, 0, 0.648) 58.8%,
4337 |         rgba(0, 0, 0, 0.741) 64.7%,
4338 |         rgba(0, 0, 0, 0.825) 71%,
4339 |         rgba(0, 0, 0, 0.896) 77.5%,
4340 |         rgba(0, 0, 0, 0.951) 84.5%,
4341 |         rgba(0, 0, 0, 0.987) 91.9%,
4342 |         black
4343 |     );
4344 |     mask-image: linear-gradient(
4345 |         to bottom,
4346 |         transparent,
4347 |         rgba(0, 0, 0, 0.013) 8.1%,
4348 |         rgba(0, 0, 0, 0.049) 15.5%,
4349 |         rgba(0, 0, 0, 0.104) 22.5%,
4350 |         rgba(0, 0, 0, 0.175) 29%,
4351 |         rgba(0, 0, 0, 0.259) 35.3%,
4352 |         rgba(0, 0, 0, 0.352) 41.2%,
4353 |         rgba(0, 0, 0, 0.45) 47.1%,
4354 |         rgba(0, 0, 0, 0.55) 52.9%,
4355 |         rgba(0, 0, 0, 0.648) 58.8%,
4356 |         rgba(0, 0, 0, 0.741) 64.7%,
4357 |         rgba(0, 0, 0, 0.825) 71%,
4358 |         rgba(0, 0, 0, 0.896) 77.5%,
4359 |         rgba(0, 0, 0, 0.951) 84.5%,
4360 |         rgba(0, 0, 0, 0.987) 91.9%,
4361 |         black
4362 |     );
4363 | }
4364 | 
4365 | /* Beta editor
4366 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4367 | .post-wrap:first-child .post-content,
4368 | .post-wrap:first-child .post-content .kg-width-full:first-child,
4369 | .post-section:not(.is-sidebar) .kg-width-full + .kg-width-full {
4370 |     margin-top: 0;
4371 | }
4372 | 
4373 | .post-wrap:first-child .post-content,
4374 | .post-wrap:first-child .post-content .kg-width-full:first-child,
4375 | .post-section:not(.is-sidebar)
4376 |     .kg-width-full:not(.kg-width-full.kg-card-hascaption) {
4377 |     margin-bottom: 0;
4378 | }
4379 | 
4380 | .post-section:not(.is-sidebar)
4381 |     .kg-width-full:not(.kg-width-full.kg-card-hascaption)
4382 |     + :not(.kg-width-full) {
4383 |     margin-top: 5vh;
4384 | }
4385 | 
4386 | /* Signup card & Header card 'v2' */
4387 | .post-content .kg-signup-card.kg-width-full,
4388 | .post-content .kg-header-card.kg-v2.kg-width-full {
4389 |     position: relative;
4390 |     right: 50%;
4391 |     left: 50%;
4392 |     width: calc(100vw - var(--scrollbar-width, 0px));
4393 |     margin-left: calc(-50vw + var(--scrollbar-width, 0px) / 2);
4394 | }
4395 | 
4396 | .post-content .kg-signup-card.kg-width-regular,
4397 | .post-content .kg-signup-card.kg-width-wide,
4398 | .post-content .kg-header-card.kg-v2.kg-width-regular,
4399 | .post-content .kg-header-card.kg-v2.kg-width-wide {
4400 |     position: relative;
4401 |     right: 0;
4402 |     left: 0;
4403 |     overflow: hidden;
4404 |     width: 100%;
4405 |     margin-left: 0;
4406 |     border-radius: var(--border-radius);
4407 | }
4408 | 
4409 | .post-content .kg-signup-card.kg-width-full.kg-content-wide,
4410 | .post-content .kg-header-card.kg-v2.kg-width-full.kg-content-wide {
4411 |     padding-right: var(--margin-wrap-left-right);
4412 |     padding-left: var(--margin-wrap-left-right);
4413 | }
4414 | 
4415 | .post-content
4416 |     .kg-signup-card.kg-width-full.kg-content-wide
4417 |     .kg-signup-card-content,
4418 | .post-content
4419 |     .kg-header-card.kg-v2.kg-width-full.kg-content-wide
4420 |     .kg-header-card-content {
4421 |     width: var(--max-width-global-wrap);
4422 |     max-width: 100%;
4423 |     margin-right: auto;
4424 |     margin-left: auto;
4425 | }
4426 | 
4427 | .post-content .kg-signup-card.kg-width-full .kg-signup-card-image,
4428 | .post-content .kg-header-card.kg-v2.kg-width-full .kg-header-card-image {
4429 |     width: 100%;
4430 |     border-radius: 0;
4431 | }
4432 | 
4433 | .post-content .kg-header-card.kg-v2.kg-layout-split {
4434 |     display: -webkit-box;
4435 | }
4436 | 
4437 | .post-content .kg-signup-card h3.kg-signup-card-subheading,
4438 | .post-content .kg-header-card.kg-v2 h3.kg-header-card-subheading,
4439 | .post-content div.kg-signup-card .kg-signup-card-success {
4440 |     font-family: var(--font-family-two);
4441 |     font-weight: var(--font-weight-two-regular);
4442 |     line-height: 1.2;
4443 | }
4444 | 
4445 | .post-content div.kg-signup-card .kg-signup-card-success {
4446 |     font-size: clamp(1.05em, 2vw, 2.4rem);
4447 | }
4448 | 
4449 | .post-content .kg-signup-card h2 + h3.kg-signup-card-subheading,
4450 | .post-content .kg-header-card.kg-v2 h2 + h3.kg-header-card-subheading {
4451 |     margin: 1em 0 0;
4452 | }
4453 | 
4454 | .post-content .kg-signup-card .kg-signup-card-fields {
4455 |     padding: 0.3em;
4456 |     border: none;
4457 |     border-radius: 100px;
4458 | }
4459 | 
4460 | .post-content .kg-signup-card .kg-signup-card-fields,
4461 | .post-content .kg-signup-card-input {
4462 |     background-color: var(--color-body);
4463 | }
4464 | 
4465 | .post-content div.kg-signup-card .kg-signup-card-button,
4466 | .post-content .kg-header-card.kg-v2 .kg-header-card-button {
4467 |     font-family: var(--font-family-three);
4468 |     font-weight: var(--font-weight-three-medium);
4469 |     padding: 0.8em 1.8em;
4470 |     cursor: pointer;
4471 | }
4472 | 
4473 | .post-content div.kg-signup-card .kg-signup-card-button,
4474 | .post-content div.kg-signup-card .kg-signup-card-input,
4475 | .post-content div.kg-header-card.kg-v2 .kg-header-card-button {
4476 |     font-size: 1.8rem;
4477 |     border-radius: 100px;
4478 | }
4479 | 
4480 | .post-content .kg-signup-card-input {
4481 |     line-height: 1.2;
4482 |     overflow: hidden;
4483 |     white-space: nowrap;
4484 |     text-overflow: ellipsis;
4485 | }
4486 | 
4487 | .post-content .kg-signup-card-input::-moz-placeholder {
4488 |     opacity: var(--opacity-two);
4489 | }
4490 | 
4491 | .post-content .kg-signup-card-input::placeholder {
4492 |     opacity: var(--opacity-two);
4493 | }
4494 | 
4495 | .post-content div.kg-signup-card .kg-signup-card-disclaimer,
4496 | .post-content div.kg-signup-card .kg-signup-card-error {
4497 |     font-size: 1.3rem;
4498 |     margin: 1vh 0 0;
4499 |     opacity: var(--opacity-one);
4500 | }
4501 | 
4502 | /* If sidebar */
4503 | .post-section.is-sidebar .kg-signup-card:not(.kg-width-regular),
4504 | .post-section.is-sidebar .kg-header-card.kg-v2:not(.kg-width-regular) {
4505 |     right: 0;
4506 |     left: 0;
4507 |     overflow: hidden;
4508 |     width: 100%;
4509 |     max-width: 100%;
4510 |     margin-left: 0;
4511 |     padding: 0;
4512 |     border-radius: calc(var(--border-radius) / 1.5);
4513 | }
4514 | 
4515 | .post-section.is-sidebar
4516 |     .kg-signup-card.kg-layout-split
4517 |     .kg-signup-card-content,
4518 | .post-section.is-sidebar
4519 |     .kg-header-card.kg-v2.kg-layout-split
4520 |     .kg-header-card-content {
4521 |     display: flex;
4522 |     flex-direction: column;
4523 | }
4524 | 
4525 | .post-section.is-sidebar .kg-signup-card .kg-signup-card-text,
4526 | .post-section.is-sidebar .kg-header-card.kg-v2 .kg-header-card-text {
4527 |     padding: 4vmax 2vmax !important;
4528 | }
4529 | 
4530 | .post-section.is-sidebar .kg-header-card.kg-v2 {
4531 |     min-height: initial;
4532 |     padding: 0;
4533 | }
4534 | 
4535 | .post-section.is-sidebar .kg-signup-card .kg-signup-card-fields {
4536 |     max-width: 500px;
4537 | }
4538 | 
4539 | .post-section.is-sidebar .kg-signup-card.kg-layout-split.kg-swapped picture,
4540 | .post-section.is-sidebar
4541 |     .kg-header-card.kg-v2.kg-layout-split.kg-swapped
4542 |     picture {
4543 |     order: 2;
4544 | }
4545 | 
4546 | .post-section.is-sidebar .kg-signup-card.kg-layout-split img,
4547 | .post-section.is-sidebar .kg-header-card.kg-v2.kg-layout-split img {
4548 |     display: block;
4549 |     height: 100%;
4550 | }
4551 | 
4552 | .post-section.is-sidebar .kg-signup-card.kg-layout-split.kg-content-wide img,
4553 | .post-section.is-sidebar
4554 |     .kg-header-card.kg-layout-split.kg-v2.kg-content-wide
4555 |     img {
4556 |     padding: 2vmax 2vmax 0;
4557 | }
4558 | 
4559 | .post-section.is-sidebar
4560 |     .kg-signup-card.kg-layout-split.kg-content-wide.kg-swapped
4561 |     img,
4562 | .post-section.is-sidebar
4563 |     .kg-header-card.kg-layout-split.kg-v2.kg-content-wide.kg-swapped
4564 |     img {
4565 |     padding: 0 2vmax 2vmax;
4566 | }
4567 | 
4568 | .post-section.is-sidebar .kg-signup-card .kg-signup-card-heading,
4569 | .post-section.is-sidebar .kg-header-card.kg-v2 .kg-header-card-heading {
4570 |     font-size: clamp(2.8rem, 4vw, 4rem) !important;
4571 | }
4572 | 
4573 | .post-section.is-sidebar .kg-signup-card .kg-signup-card-subheading,
4574 | .post-section.is-sidebar .kg-header-card.kg-v2 .kg-header-card-subheading,
4575 | .post-section.is-sidebar div.kg-signup-card .kg-signup-card-success {
4576 |     font-size: clamp(1.05em, 2vw, 2rem) !important;
4577 | }
4578 | 
4579 | .post-section.is-sidebar
4580 |     .kg-signup-card:not(.kg-width-regular)
4581 |     .kg-signup-card-heading
4582 |     + .kg-signup-card-form,
4583 | .post-section.is-sidebar
4584 |     .kg-signup-card:not(.kg-width-regular)
4585 |     .kg-signup-card-subheading
4586 |     + .kg-signup-card-form {
4587 |     margin-top: 2.4vmax;
4588 | }
4589 | 
4590 | /* RWD — Beta editor */
4591 | @media (max-width: 1480px) and (min-width: 1025px) {
4592 |     .post-content .kg-signup-card.kg-width-wide,
4593 |     .post-content .kg-header-card.kg-v2.kg-width-wide {
4594 |         width: calc(100% + 50px + 50px);
4595 |         margin-left: -50px;
4596 |     }
4597 | }
4598 | 
4599 | @media (max-width: 1024px) {
4600 |     .post-content .kg-signup-card.kg-width-regular,
4601 |     .post-content .kg-signup-card.kg-width-wide,
4602 |     .post-content .kg-header-card.kg-v2.kg-width-regular,
4603 |     .post-content .kg-header-card.kg-v2.kg-width-wide {
4604 |         border-radius: calc(var(--border-radius) / 1.5);
4605 |     }
4606 | }
4607 | 
4608 | @media (max-width: 480px) {
4609 |     .post-content div.kg-signup-card .kg-signup-card-button,
4610 |     .post-content div.kg-signup-card .kg-signup-card-input,
4611 |     .post-content div.kg-header-card.kg-v2 .kg-header-card-button {
4612 |         font-size: 1.6rem;
4613 |     }
4614 | }
4615 | 
4616 | @media (min-width: 1481px) {
4617 |     .post-content .kg-signup-card.kg-width-wide,
4618 |     .post-content .kg-header-card.kg-v2.kg-width-wide {
4619 |         width: calc(100% + 70px + 70px);
4620 |         margin-left: -70px;
4621 |     }
4622 | }
4623 | 
4624 | /* RWD — Post content
4625 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4626 | @media (max-width: 1480px) and (min-width: 1025px) {
4627 |     .post-content .kg-video-card.kg-width-wide,
4628 |     .post-content .kg-image-card.kg-width-wide img,
4629 |     .post-content .kg-gallery-card .kg-gallery-container {
4630 |         width: calc(100% + 50px + 50px);
4631 |         margin-left: -50px;
4632 |     }
4633 | }
4634 | 
4635 | @media (max-width: 1024px) {
4636 |     .post-content {
4637 |         font-size: 1.8rem;
4638 |         max-width: var(--max-width-post-wrap-two);
4639 |     }
4640 | 
4641 |     .post-section.is-sidebar .kg-video-card.kg-width-full,
4642 |     .post-section.is-sidebar .kg-image-card.kg-width-full img,
4643 |     .post-section.is-sidebar .post-content .kg-header-card {
4644 |         border-radius: 0;
4645 |     }
4646 | 
4647 |     .post-content blockquote.kg-blockquote-alt {
4648 |         font-size: 3.8rem;
4649 |     }
4650 | 
4651 |     .post-content .members-cta h2 {
4652 |         font-size: 4.2rem;
4653 |     }
4654 | }
4655 | 
4656 | @media (max-width: 768px) {
4657 |     .post-content {
4658 |         max-width: 100%;
4659 |     }
4660 | 
4661 |     .post-content h1 {
4662 |         font-size: 4.8rem;
4663 |     }
4664 | 
4665 |     .post-content h2 {
4666 |         font-size: 3.8rem;
4667 |     }
4668 | 
4669 |     .post-content h3 {
4670 |         font-size: 3rem;
4671 |     }
4672 | 
4673 |     .post-content h4 {
4674 |         font-size: 2.2rem;
4675 |     }
4676 | 
4677 |     .post-content h5 {
4678 |         font-size: 1.9rem;
4679 |     }
4680 | 
4681 |     .post-content p,
4682 |     .post-content iframe,
4683 |     .post-content ol,
4684 |     .post-content ul,
4685 |     .post-content table {
4686 |         margin-bottom: 20px;
4687 |     }
4688 | 
4689 |     .post-content hr,
4690 |     .post-content blockquote,
4691 |     .post-content .kg-card.kg-header-card {
4692 |         margin-top: 35px;
4693 |         margin-bottom: 35px;
4694 |     }
4695 | 
4696 |     .post-content pre,
4697 |     .post-content .kg-card {
4698 |         margin-top: 30px;
4699 |         margin-bottom: 30px;
4700 |     }
4701 | 
4702 |     .post-content
4703 |         .kg-card:not(.kg-width-full):not(.kg-image-card):not(
4704 |             .kg-gallery-card
4705 |         ):not(.kg-embed-card)
4706 |         + .kg-card {
4707 |         margin-top: -15px;
4708 |     }
4709 | 
4710 |     .post-content .members-cta {
4711 |         padding-top: 4vh;
4712 |         padding-bottom: 4vh;
4713 |     }
4714 | 
4715 |     .post-content .members-cta h2 {
4716 |         font-size: 3.4rem;
4717 |     }
4718 | }
4719 | 
4720 | @media (max-width: 480px) {
4721 |     .post-content {
4722 |         margin-bottom: 10vh;
4723 |     }
4724 | 
4725 |     .post-content h1,
4726 |     .post-content h2,
4727 |     .post-content h3 {
4728 |         margin-bottom: 10px;
4729 |     }
4730 | 
4731 |     .post-content h1 {
4732 |         font-size: 3.4rem;
4733 |     }
4734 | 
4735 |     .post-content h2 {
4736 |         font-size: 2.9rem;
4737 |     }
4738 | 
4739 |     .post-content h3 {
4740 |         font-size: 2.4rem;
4741 |     }
4742 | 
4743 |     .post-content h4 {
4744 |         font-size: 2rem;
4745 |     }
4746 | 
4747 |     .post-content h5 {
4748 |         font-size: 1.8rem;
4749 |     }
4750 | 
4751 |     .post-content blockquote {
4752 |         font-size: 2rem;
4753 |         border-width: 3px;
4754 |     }
4755 | 
4756 |     .post-content blockquote.kg-blockquote-alt {
4757 |         font-size: 3rem;
4758 |     }
4759 | 
4760 |     .post-content img,
4761 |     .post-content code,
4762 |     .post-content .kg-callout-card,
4763 |     .post-content .kg-audio-card,
4764 |     .post-content .kg-file-card .kg-file-card-container,
4765 |     .post-content .kg-toggle-card,
4766 |     .post-content .kg-product-card .kg-product-card-container,
4767 |     .post-content .kg-nft-card .kg-nft-card-container,
4768 |     .post-content .kg-bookmark-card .kg-bookmark-container,
4769 |     .post-content .kg-bookmark-card .kg-bookmark-container:hover {
4770 |         border-radius: calc(var(--border-radius) / 2);
4771 |     }
4772 | 
4773 |     .post-content
4774 |         .kg-gallery-card
4775 |         .kg-gallery-row:first-of-type
4776 |         .kg-gallery-image:first-of-type
4777 |         img {
4778 |         border-top-left-radius: calc(var(--border-radius) / 2);
4779 |     }
4780 | 
4781 |     .post-content
4782 |         .kg-gallery-card
4783 |         .kg-gallery-row:first-of-type
4784 |         .kg-gallery-image:last-of-type
4785 |         img {
4786 |         border-top-right-radius: calc(var(--border-radius) / 2);
4787 |     }
4788 | 
4789 |     .post-content
4790 |         .kg-gallery-card
4791 |         .kg-gallery-row:last-of-type
4792 |         .kg-gallery-image:first-of-type
4793 |         img {
4794 |         border-bottom-left-radius: calc(var(--border-radius) / 2);
4795 |     }
4796 | 
4797 |     .post-content
4798 |         .kg-gallery-card
4799 |         .kg-gallery-row:last-of-type
4800 |         .kg-gallery-image:last-of-type
4801 |         img {
4802 |         border-bottom-right-radius: calc(var(--border-radius) / 2);
4803 |     }
4804 | 
4805 |     .post-content .kg-audio-card .kg-audio-thumbnail,
4806 |     .post-content .kg-file-card .kg-file-card-icon::before,
4807 |     .post-content .kg-product-card img,
4808 |     .post-content .kg-nft-card .kg-nft-image,
4809 |     .post-content .kg-bookmark-card .kg-bookmark-thumbnail img {
4810 |         border-radius: calc(var(--border-radius) / 4);
4811 |     }
4812 | 
4813 |     .post-content .kg-bookmark-card .kg-bookmark-icon {
4814 |         width: 16px;
4815 |         height: 16px;
4816 |         margin-right: 6px;
4817 |     }
4818 | 
4819 |     .post-content .kg-bookmark-card .kg-bookmark-description,
4820 |     .post-content .kg-bookmark-card .kg-bookmark-metadata {
4821 |         font-size: 1.2rem;
4822 |     }
4823 | 
4824 |     .post-content .kg-bookmark-card .kg-bookmark-thumbnail {
4825 |         height: 65px;
4826 |         margin: 16px 16px 0;
4827 |     }
4828 | 
4829 |     .post-content .members-cta-teaser::after {
4830 |         width: 100vw;
4831 |         margin-left: -50vw;
4832 |     }
4833 | }
4834 | 
4835 | @media (min-width: 1025px) {
4836 |     .post-section.is-sidebar .post-wrap {
4837 |         max-width: var(--max-width-content-wrap);
4838 |     }
4839 | 
4840 |     .post-section.is-sidebar .post-header-content {
4841 |         width: 100%;
4842 |     }
4843 | 
4844 |     .post-section.is-sidebar .post-content {
4845 |         width: 64%;
4846 |         max-width: calc(var(--max-width-post-wrap-one) - 70px);
4847 |         margin-right: 0;
4848 |         margin-left: 0;
4849 |     }
4850 | 
4851 |     .post-section.is-sidebar .kg-video-card.kg-width-wide,
4852 |     .post-section.is-sidebar .kg-image-card.kg-width-wide img,
4853 |     .post-section.is-sidebar .kg-video-card.kg-width-full,
4854 |     .post-section.is-sidebar .kg-image-card.kg-width-full img,
4855 |     .post-section.is-sidebar .kg-header-card,
4856 |     .post-section.is-sidebar .kg-gallery-card .kg-gallery-container {
4857 |         width: 100%;
4858 |         margin-left: 0;
4859 |     }
4860 | 
4861 |     .post-section.is-sidebar .kg-video-card.kg-width-full,
4862 |     .post-section.is-sidebar .kg-image-card.kg-width-full img,
4863 |     .post-section.is-sidebar .kg-header-card {
4864 |         right: 0;
4865 |         left: 0;
4866 |     }
4867 | 
4868 |     .post-section.is-sidebar blockquote.kg-blockquote-alt {
4869 |         font-size: 4rem;
4870 |         padding: 2vh 0;
4871 |     }
4872 | 
4873 |     .post-section.is-sidebar .kg-header-card {
4874 |         min-height: 30vh;
4875 |         padding-top: 10vmin;
4876 |         padding-bottom: 10vmin;
4877 |     }
4878 | 
4879 |     .post-section.is-sidebar .kg-header-card .kg-header-card-header {
4880 |         font-size: 4rem;
4881 |     }
4882 | 
4883 |     .post-section.is-sidebar .kg-header-card .kg-header-card-subheader {
4884 |         font-size: 2.2rem;
4885 |     }
4886 | }
4887 | 
4888 | @media (min-width: 1481px) {
4889 |     .post-content .kg-video-card.kg-width-wide,
4890 |     .post-content .kg-image-card.kg-width-wide img,
4891 |     .post-content .kg-gallery-card .kg-gallery-container {
4892 |         width: calc(100% + 70px + 70px);
4893 |         margin-left: -70px;
4894 |     }
4895 | }
4896 | 
4897 | @media (min-width: 1921px) {
4898 |     .post-content .kg-video-card.kg-width-full,
4899 |     .post-content .kg-image-card.kg-width-full img {
4900 |         width: var(--max-width-global-wrap);
4901 |         margin-left: calc(0px - var(--max-width-global-wrap) / 2);
4902 |         border-radius: calc(var(--border-radius) / 1.5);
4903 |     }
4904 | }
4905 | 
4906 | /* --------------------------------------------------------------------------
4907 |    13.Post — Sidebar
4908 |    -------------------------------------------------------------------------- */
4909 | .post-sidebar {
4910 |     position: absolute;
4911 |     z-index: 1;
4912 |     top: 0;
4913 |     right: var(--margin-wrap-left-right);
4914 |     width: 290px;
4915 |     height: 100%;
4916 | }
4917 | 
4918 | .post-sidebar div.is-authors,
4919 | .post-sidebar div.is-featured {
4920 |     margin-bottom: 5.5vh;
4921 | }
4922 | 
4923 | .post-sidebar div > a {
4924 |     display: flex;
4925 |     align-self: flex-start;
4926 |     margin-bottom: 1.5vh;
4927 |     padding-top: 1vh;
4928 |     pointer-events: none;
4929 | }
4930 | 
4931 | .post-sidebar div > a:first-of-type {
4932 |     padding-top: 1.7vh;
4933 |     border-top: var(--border) var(--color-border-one);
4934 | }
4935 | 
4936 | .post-sidebar a div {
4937 |     line-height: 0;
4938 |     display: inline-block;
4939 |     margin-top: 2px;
4940 | }
4941 | 
4942 | /* Title & Image
4943 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4944 | .post-sidebar-title {
4945 |     font-family: var(--font-family-two);
4946 |     font-size: 1.5rem;
4947 |     font-weight: var(--font-weight-two-bold);
4948 |     line-height: 1.35;
4949 |     display: inline;
4950 |     margin: 0;
4951 | }
4952 | 
4953 | .post-sidebar-title,
4954 | .post-sidebar img {
4955 |     pointer-events: auto;
4956 | }
4957 | 
4958 | .post-sidebar-title:hover,
4959 | .post-sidebar img {
4960 |     text-decoration: underline;
4961 | }
4962 | 
4963 | .post-sidebar picture {
4964 |     flex: 1 0 auto;
4965 |     width: 100%;
4966 |     max-width: 70px;
4967 |     margin-right: 4.4%;
4968 |     will-change: transform;
4969 |     transition: transform 0.2s ease;
4970 | }
4971 | 
4972 | .post-sidebar picture:hover {
4973 |     transform: translateY(-2px);
4974 | }
4975 | 
4976 | .post-sidebar img {
4977 |     width: 100%;
4978 |     -o-object-fit: cover;
4979 |     object-fit: cover;
4980 | }
4981 | 
4982 | /* Authors
4983 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
4984 | .post-sidebar .is-authors > a.no-bio {
4985 |     align-items: center;
4986 | }
4987 | 
4988 | .post-sidebar .is-authors img {
4989 |     height: 70px;
4990 |     border-radius: 100%;
4991 | }
4992 | 
4993 | .post-sidebar a.no-bio div {
4994 |     margin-top: 0;
4995 | }
4996 | 
4997 | .post-sidebar .is-authors p {
4998 |     font-size: 1.3rem;
4999 |     line-height: 1.35;
5000 |     display: -webkit-box;
5001 |     overflow-y: hidden;
5002 |     margin: 0.5vh 0 0;
5003 |     opacity: var(--opacity-one);
5004 |     -webkit-box-orient: vertical;
5005 |     -webkit-line-clamp: 3;
5006 | }
5007 | 
5008 | /* Featured
5009 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5010 | .post-sidebar .is-featured img {
5011 |     height: 50px;
5012 |     border-radius: calc(var(--border-radius) / 2);
5013 | }
5014 | 
5015 | /* Form
5016 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5017 | .post-sidebar .subscribe-form {
5018 |     top: 3vh;
5019 |     padding: 22px 25px 25px;
5020 | }
5021 | 
5022 | .post-sidebar .subscribe-form.is-sticky {
5023 |     position: sticky;
5024 | }
5025 | 
5026 | .post-sidebar .subscribe-title {
5027 |     font-size: 2.3rem;
5028 |     margin-bottom: 1.8vh;
5029 | }
5030 | 
5031 | .post-sidebar .subscribe-form small {
5032 |     font-size: 1.1rem;
5033 | }
5034 | 
5035 | .post-sidebar .subscribe-form input {
5036 |     margin-bottom: 0.8vh;
5037 |     padding-top: 11px;
5038 |     padding-bottom: 11px;
5039 | }
5040 | 
5041 | .post-sidebar .subscribe-form button {
5042 |     font-size: 1.6rem;
5043 |     padding-top: 12px;
5044 |     padding-bottom: 12px;
5045 | }
5046 | 
5047 | /* RWD — Post Sidebar
5048 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5049 | @media (max-width: 1024px) {
5050 |     .post-sidebar {
5051 |         display: none;
5052 |     }
5053 | }
5054 | 
5055 | /* --------------------------------------------------------------------------
5056 |    14.Post — Share
5057 |    -------------------------------------------------------------------------- */
5058 | .post-share {
5059 |     width: 100%;
5060 |     margin-top: 5vh;
5061 | }
5062 | 
5063 | .post-share > div {
5064 |     position: relative;
5065 |     display: inline-flex;
5066 |     width: 100%;
5067 | }
5068 | 
5069 | .post-share > div a {
5070 |     display: flex;
5071 |     align-items: center;
5072 |     flex: 1 0 60px;
5073 |     justify-content: center;
5074 |     height: 60px;
5075 |     transition: background-color 0.15s ease;
5076 |     background-color: var(--color-five);
5077 | }
5078 | 
5079 | .post-share > div a:hover {
5080 |     background-color: var(--color-two);
5081 | }
5082 | 
5083 | .post-share > div a:first-of-type {
5084 |     border-radius: calc(var(--border-radius) / 1.5) 0 0
5085 |         calc(var(--border-radius) / 1.5);
5086 | }
5087 | 
5088 | .post-share > div a:last-of-type {
5089 |     border-radius: 0 calc(var(--border-radius) / 1.5)
5090 |         calc(var(--border-radius) / 1.5) 0;
5091 | }
5092 | 
5093 | .post-share svg {
5094 |     width: 18px;
5095 |     height: 18px;
5096 |     transition: fill 0.15s ease;
5097 |     fill: var(--color-font-one);
5098 | }
5099 | 
5100 | /* Copy link
5101 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5102 | .post-share > div + input {
5103 |     display: block;
5104 |     cursor: default;
5105 |     opacity: 0;
5106 |     color: transparent;
5107 | }
5108 | 
5109 | .post-share-link {
5110 |     cursor: pointer;
5111 | }
5112 | 
5113 | .post-share-link svg {
5114 |     width: 21px;
5115 |     height: 21px;
5116 | }
5117 | 
5118 | .post-share-link + small {
5119 |     position: absolute;
5120 |     bottom: -27px;
5121 |     left: 0;
5122 |     display: inline-block;
5123 |     opacity: 0;
5124 | }
5125 | 
5126 | .post-share-link:not(:active) + small {
5127 |     transition: opacity 10s step-end;
5128 | }
5129 | 
5130 | .post-share-link:active + small {
5131 |     opacity: 1;
5132 | }
5133 | 
5134 | /* Header
5135 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5136 | .post-meta-wrap .post-share-wrap {
5137 |     margin-left: auto;
5138 | }
5139 | 
5140 | .post-meta-wrap .post-share-wrap,
5141 | .post-meta-wrap .post-share-wrap a {
5142 |     display: flex;
5143 | }
5144 | 
5145 | .post-meta-wrap .post-share-wrap svg {
5146 |     width: 18px;
5147 |     margin-left: 16px;
5148 |     transition: opacity 0.12s ease;
5149 |     opacity: var(--opacity-one);
5150 |     fill: var(--color-font-one);
5151 | }
5152 | 
5153 | .post-meta-wrap .post-share-wrap svg:hover {
5154 |     opacity: 1;
5155 | }
5156 | 
5157 | /* RWD — Post share
5158 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5159 | @media (max-width: 768px) {
5160 |     .post-meta-wrap .post-share-wrap {
5161 |         display: none;
5162 |     }
5163 | }
5164 | 
5165 | @media (max-width: 480px) {
5166 |     .post-share > div a {
5167 |         flex-grow: 0;
5168 |     }
5169 | 
5170 |     .post-share > div a:first-of-type {
5171 |         border-radius: calc(var(--border-radius) / 2) 0 0
5172 |             calc(var(--border-radius) / 2);
5173 |     }
5174 | 
5175 |     .post-share > div a:last-of-type {
5176 |         border-radius: 0 calc(var(--border-radius) / 2)
5177 |             calc(var(--border-radius) / 2) 0;
5178 |     }
5179 | 
5180 |     .post-share svg {
5181 |         width: 16px;
5182 |         height: 16px;
5183 |     }
5184 | 
5185 |     .post-share-link svg {
5186 |         width: 20px;
5187 |         height: 20px;
5188 |     }
5189 | }
5190 | 
5191 | /* --------------------------------------------------------------------------
5192 |    15.Post — Navigation
5193 |    -------------------------------------------------------------------------- */
5194 | .navigation-section {
5195 |     margin-bottom: 7vh;
5196 | }
5197 | 
5198 | .navigation-section + .special-section {
5199 |     margin-top: 10vh;
5200 | }
5201 | 
5202 | .navigation-wrap,
5203 | .navigation-wrap a > div {
5204 |     display: flex;
5205 | }
5206 | 
5207 | /* Elements
5208 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5209 | .navigation-wrap a {
5210 |     flex: 0 0 50%;
5211 |     box-sizing: border-box;
5212 |     pointer-events: none;
5213 | }
5214 | 
5215 | .navigation-wrap a:first-child:last-child {
5216 |     flex-grow: 1;
5217 | }
5218 | 
5219 | /* Label
5220 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5221 | .navigation-wrap small {
5222 |     margin-bottom: 2vh;
5223 |     padding-bottom: 0.7em;
5224 |     border-bottom: var(--border) var(--color-border-one);
5225 | }
5226 | 
5227 | /* Content
5228 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5229 | .navigation-wrap a > div {
5230 |     align-items: center;
5231 |     min-height: 100px;
5232 | }
5233 | 
5234 | .navigation-prev {
5235 |     margin-left: auto;
5236 |     text-align: right;
5237 | }
5238 | 
5239 | /* Title
5240 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5241 | .navigation-title {
5242 |     line-height: 0;
5243 |     display: inline-block;
5244 |     width: 100%;
5245 | }
5246 | 
5247 | .navigation-title > div {
5248 |     display: inline-block;
5249 |     box-sizing: border-box;
5250 |     max-width: 400px;
5251 | }
5252 | 
5253 | .navigation-next .navigation-title > div {
5254 |     padding-right: 2vw;
5255 | }
5256 | 
5257 | .navigation-prev .navigation-title > div {
5258 |     padding-left: 2vw;
5259 | }
5260 | 
5261 | .navigation-title h3 {
5262 |     font-size: 2.4rem;
5263 |     display: inline;
5264 |     margin: 0;
5265 |     pointer-events: auto;
5266 | }
5267 | 
5268 | .navigation-title h3:hover {
5269 |     text-decoration: underline;
5270 |     text-decoration-thickness: 2px;
5271 |     text-underline-offset: 3px;
5272 | }
5273 | 
5274 | /* Image
5275 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5276 | .navigation-image {
5277 |     line-height: 0;
5278 |     align-self: flex-start;
5279 |     flex: 0 0 auto;
5280 |     width: 100px;
5281 |     transition: transform 0.3s ease;
5282 |     pointer-events: auto;
5283 | }
5284 | 
5285 | .navigation-image:hover {
5286 |     transform: translateY(-3px);
5287 | }
5288 | 
5289 | .navigation-next .navigation-image {
5290 |     margin-right: 18px;
5291 | }
5292 | 
5293 | .navigation-prev .navigation-image {
5294 |     margin-left: 18px;
5295 | }
5296 | 
5297 | /* RWD — Post — Navigation
5298 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5299 | @media (max-width: 1280px) {
5300 |     .navigation-section + .special-section {
5301 |         margin-top: 7vh;
5302 |     }
5303 | }
5304 | 
5305 | @media (max-width: 1024px) {
5306 |     .navigation-wrap a > div {
5307 |         min-height: 80px;
5308 |     }
5309 | 
5310 |     .navigation-title h3 {
5311 |         font-size: 2rem;
5312 |     }
5313 | 
5314 |     .navigation-image {
5315 |         width: 80px;
5316 |     }
5317 | }
5318 | 
5319 | @media (max-width: 768px) {
5320 |     .navigation-wrap a > div {
5321 |         align-items: flex-start;
5322 |     }
5323 | 
5324 |     .navigation-title > div {
5325 |         max-width: 280px;
5326 |     }
5327 | 
5328 |     .navigation-title h3 {
5329 |         font-size: 1.8rem;
5330 |     }
5331 | 
5332 |     .navigation-next .navigation-image {
5333 |         margin-right: 12px;
5334 |     }
5335 | 
5336 |     .navigation-prev .navigation-image {
5337 |         margin-left: 12px;
5338 |     }
5339 | }
5340 | 
5341 | @media (max-width: 480px) {
5342 |     .navigation-section {
5343 |         margin-bottom: 6vh;
5344 |     }
5345 | 
5346 |     .navigation-wrap {
5347 |         flex-wrap: wrap;
5348 |     }
5349 | 
5350 |     .navigation-wrap a {
5351 |         flex-basis: 100%;
5352 |     }
5353 | 
5354 |     .navigation-wrap a + a {
5355 |         margin-top: 4vh;
5356 |     }
5357 | 
5358 |     .navigation-title h3 {
5359 |         font-size: 2rem;
5360 |     }
5361 | 
5362 |     .navigation-wrap .navigation-image {
5363 |         aspect-ratio: 4/3;
5364 |     }
5365 | }
5366 | 
5367 | /* --------------------------------------------------------------------------
5368 |    16.Post — Comments
5369 |    -------------------------------------------------------------------------- */
5370 | .comments-section {
5371 |     margin-bottom: 7vh;
5372 | }
5373 | 
5374 | .comments-section div > div[id] {
5375 |     padding-top: 3vh;
5376 |     border-top: 1px solid var(--color-border-one);
5377 | }
5378 | 
5379 | .comments-wrap {
5380 |     background-color: var(--color-five);
5381 | }
5382 | 
5383 | .comments-content {
5384 |     max-width: var(--max-width-post-wrap-one);
5385 |     margin-right: auto;
5386 |     margin-left: auto;
5387 |     padding-right: 4vw;
5388 |     padding-left: 4vw;
5389 | }
5390 | 
5391 | /* Content
5392 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5393 | .comments-content > div:first-of-type {
5394 |     padding-top: 8vh;
5395 | }
5396 | 
5397 | .comments-content > div:last-of-type {
5398 |     padding-bottom: 8vh;
5399 | }
5400 | 
5401 | /* Header
5402 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5403 | .comments-header {
5404 |     display: flex;
5405 |     align-items: flex-end;
5406 |     margin-bottom: 1vh;
5407 | }
5408 | 
5409 | .comments-header h3 {
5410 |     font-weight: var(--font-weight-three-bold);
5411 |     line-height: 1.1;
5412 |     flex: 1 0 60%;
5413 |     letter-spacing: -0.018em;
5414 | }
5415 | 
5416 | .comments-header h3,
5417 | .comments-header span {
5418 |     font-family: var(--font-family-three);
5419 |     display: block;
5420 |     margin: 0;
5421 | }
5422 | 
5423 | .comments-header span {
5424 |     font-size: 1.6rem;
5425 |     font-weight: var(--font-weight-three-regular);
5426 |     flex: 1 0 40%;
5427 |     text-align: right;
5428 |     opacity: var(--opacity-one);
5429 | }
5430 | 
5431 | /* RWD — Post — Comments
5432 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5433 | @media (max-width: 1024px) {
5434 |     .comments-content {
5435 |         max-width: var(--max-width-post-wrap-two);
5436 |     }
5437 | }
5438 | 
5439 | @media (max-width: 768px) {
5440 |     .comments-content {
5441 |         max-width: 100%;
5442 |     }
5443 | 
5444 |     .comments-content > div:first-of-type {
5445 |         padding-top: 4vh;
5446 |     }
5447 | 
5448 |     .comments-content > div:last-of-type {
5449 |         padding-bottom: 4vh;
5450 |     }
5451 | }
5452 | 
5453 | @media (max-width: 480px) {
5454 |     .comments-header h3 {
5455 |         font-size: 2rem;
5456 |     }
5457 | 
5458 |     .comments-header span {
5459 |         font-size: 1.5rem;
5460 |     }
5461 | }
5462 | 
5463 | /* --------------------------------------------------------------------------
5464 |    17.Author & Tag page
5465 |    -------------------------------------------------------------------------- */
5466 | .archive-image {
5467 |     box-sizing: border-box;
5468 |     width: 160px;
5469 |     height: 160px;
5470 |     margin: 0 auto;
5471 |     padding: 15px;
5472 |     background-color: var(--ghost-accent-color);
5473 | }
5474 | 
5475 | div.is-archive-image {
5476 |     margin-top: 0;
5477 | }
5478 | 
5479 | .archive-image,
5480 | .archive-image img {
5481 |     border-radius: 100%;
5482 | }
5483 | 
5484 | /* Author social
5485 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5486 | .archive-social {
5487 |     display: inline-flex;
5488 |     flex-wrap: wrap;
5489 |     justify-content: center;
5490 |     margin-top: 0.5vh;
5491 | }
5492 | 
5493 | .archive-social a,
5494 | .archive-social span {
5495 |     font-size: 1.6rem;
5496 |     display: flex;
5497 |     align-items: center;
5498 |     margin: 0 1em 4px;
5499 | }
5500 | 
5501 | .archive-social a:hover {
5502 |     text-decoration: underline;
5503 | }
5504 | 
5505 | .archive-social svg {
5506 |     width: 18px;
5507 |     height: 18px;
5508 |     margin-right: 6px;
5509 |     fill: var(--color-font-one);
5510 | }
5511 | 
5512 | /* RWD — Author & Tag page
5513 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5514 | @media (max-width: 480px) {
5515 |     .archive-image {
5516 |         width: 110px;
5517 |         height: 110px;
5518 |         padding: 11px;
5519 |     }
5520 | 
5521 |     .archive-social {
5522 |         margin-top: 1.5vh;
5523 |         margin-bottom: 1vh;
5524 |     }
5525 | 
5526 |     .archive-social a,
5527 |     .archive-social span {
5528 |         font-size: 1.4rem;
5529 |         margin-right: 0.5em;
5530 |         margin-left: 0.5em;
5531 |     }
5532 | }
5533 | 
5534 | /* --------------------------------------------------------------------------
5535 |    18.Footer
5536 |    -------------------------------------------------------------------------- */
5537 | .footer-wrap {
5538 |     margin-top: 8vh;
5539 |     margin-bottom: 3vh;
5540 | }
5541 | 
5542 | .footer-nav a:hover,
5543 | .footer-copyright a:hover {
5544 |     text-decoration: underline;
5545 | }
5546 | 
5547 | /* Content
5548 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5549 | .footer-content {
5550 |     display: flex;
5551 |     align-items: flex-start;
5552 |     max-width: 100%;
5553 | }
5554 | 
5555 | .footer-logo-wrap {
5556 |     align-self: center;
5557 |     flex: 1 0 45%;
5558 |     margin-right: 30px;
5559 |     margin-bottom: 3vh;
5560 | }
5561 | 
5562 | /* Description
5563 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5564 | .footer-description {
5565 |     font-size: 1.6rem;
5566 |     max-width: 330px;
5567 |     margin: 2vh 0 0;
5568 |     opacity: var(--opacity-one);
5569 | }
5570 | 
5571 | /* Subscribe
5572 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5573 | .footer-subscribe {
5574 |     align-items: center;
5575 |     flex: 0 0 400px;
5576 |     text-align: center;
5577 | }
5578 | 
5579 | .footer-subscribe a {
5580 |     padding-top: 0.95em;
5581 |     padding-bottom: 0.95em;
5582 | }
5583 | 
5584 | .footer-subscribe a,
5585 | .footer-subscribe small {
5586 |     width: 100%;
5587 | }
5588 | 
5589 | .footer-subscribe small {
5590 |     font-size: 1.3rem;
5591 |     line-height: 1.3;
5592 |     display: inline-block;
5593 |     margin: 1vh auto 0;
5594 |     opacity: var(--opacity-one);
5595 | }
5596 | 
5597 | /* Form */
5598 | .footer-section .subscribe-form-subtitle,
5599 | .footer-section .subscribe-form {
5600 |     display: none;
5601 | }
5602 | 
5603 | .footer-section .subscribe-form {
5604 |     width: 100%;
5605 |     margin-bottom: 8vh;
5606 |     padding: 20px 26px 28px;
5607 | }
5608 | 
5609 | .footer-section .subscribe-form > div:first-of-type {
5610 |     max-width: 400px;
5611 | }
5612 | 
5613 | .footer-section .subscribe-form .subscribe-title {
5614 |     font-size: 2.6rem;
5615 | }
5616 | 
5617 | /* Navigation
5618 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5619 | .footer-nav {
5620 |     display: flex;
5621 |     flex-wrap: wrap;
5622 |     margin-top: 3vh;
5623 |     padding-top: 5vh;
5624 |     border-top: var(--border) var(--color-border-one);
5625 | }
5626 | 
5627 | .footer-nav-column {
5628 |     flex-grow: 1;
5629 |     width: 170px;
5630 |     max-width: 230px;
5631 |     margin-bottom: 3vh;
5632 |     padding-right: 2vw;
5633 | }
5634 | 
5635 | .footer-nav-column ul {
5636 |     margin: 0;
5637 |     padding: 0;
5638 | }
5639 | 
5640 | .footer-nav-column small {
5641 |     font-weight: var(--font-weight-three-bold);
5642 |     line-height: 1.2;
5643 |     display: block;
5644 |     margin: 0 0 2vh;
5645 | }
5646 | 
5647 | .footer-nav-column small,
5648 | .footer-nav-column li {
5649 |     font-size: 1.5rem;
5650 | }
5651 | 
5652 | .footer-nav-column li {
5653 |     margin-bottom: 1vh;
5654 |     list-style: none;
5655 | }
5656 | 
5657 | .footer-nav-column li svg {
5658 |     width: 16px;
5659 |     height: 16px;
5660 |     margin-right: 8px;
5661 |     transform: translateY(3px);
5662 |     fill: var(--color-font-one);
5663 | }
5664 | 
5665 | /* Copyright
5666 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5667 | .footer-copyright {
5668 |     font-size: 1.4rem;
5669 |     width: 100%;
5670 |     margin-top: 4vh;
5671 |     opacity: var(--opacity-one);
5672 | }
5673 | 
5674 | /* RWD — Footer
5675 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5676 | @media (max-width: 1480px) {
5677 |     .footer-wrap {
5678 |         margin-top: 5vh;
5679 |     }
5680 | 
5681 |     .footer-nav-column {
5682 |         width: 100px;
5683 |     }
5684 | }
5685 | 
5686 | @media (max-width: 1024px) {
5687 |     .footer-subscribe {
5688 |         flex-basis: 300px;
5689 |     }
5690 | }
5691 | 
5692 | @media (max-width: 768px) {
5693 |     .footer-content {
5694 |         flex-wrap: wrap;
5695 |     }
5696 | 
5697 |     .footer-subscribe {
5698 |         display: none;
5699 |     }
5700 | 
5701 |     .footer-section .subscribe-form-subtitle,
5702 |     .footer-section .subscribe-form {
5703 |         display: block;
5704 |     }
5705 | 
5706 |     .footer-nav {
5707 |         margin-top: 0;
5708 |         padding-top: 2vh;
5709 |         border-top: none;
5710 |     }
5711 | 
5712 |     .footer-nav-column {
5713 |         flex-grow: 0;
5714 |         box-sizing: border-box;
5715 |         width: 33.333%;
5716 |     }
5717 | }
5718 | 
5719 | @media (max-width: 480px) {
5720 |     .footer-description {
5721 |         font-size: 1.8rem;
5722 |     }
5723 | 
5724 |     .footer-nav-column small {
5725 |         font-size: 1.7rem;
5726 |     }
5727 | 
5728 |     .footer-nav-column li {
5729 |         font-size: 1.6rem;
5730 |     }
5731 | 
5732 |     .footer-nav-column {
5733 |         box-sizing: border-box;
5734 |         width: 50%;
5735 |     }
5736 | }
5737 | 
5738 | @media (min-width: 769px) {
5739 |     .footer-nav-column:last-child {
5740 |         padding-right: 0;
5741 |     }
5742 | }
5743 | 
5744 | /* --------------------------------------------------------------------------
5745 |    19.Custom — Pages
5746 |    -------------------------------------------------------------------------- */
5747 | .custom-page {
5748 |     height: 100vh;
5749 | }
5750 | 
5751 | .custom-wrap {
5752 |     min-height: 100%;
5753 | }
5754 | 
5755 | .custom-wrap,
5756 | .custom-container,
5757 | .custom-content,
5758 | .custom-logo-wrap {
5759 |     display: flex;
5760 | }
5761 | 
5762 | .custom-content,
5763 | .custom-logo-wrap {
5764 |     align-items: center;
5765 | }
5766 | 
5767 | .custom-container {
5768 |     flex-direction: column;
5769 |     flex-grow: 1;
5770 |     text-align: center;
5771 | }
5772 | 
5773 | .custom-content {
5774 |     flex: 1 0 auto;
5775 |     width: 100%;
5776 |     max-width: 340px;
5777 |     margin: 0 auto 12vh;
5778 | }
5779 | 
5780 | /* Image
5781 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5782 | .custom-image {
5783 |     width: 35%;
5784 | }
5785 | 
5786 | /* Logo
5787 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5788 | .custom-logo-wrap {
5789 |     min-height: 90px;
5790 | }
5791 | 
5792 | .custom-logo {
5793 |     margin: 6vh auto 0;
5794 | }
5795 | 
5796 | /* Title
5797 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5798 | .custom-title {
5799 |     font-size: 3rem;
5800 |     line-height: 1.1;
5801 |     margin: 3vh 0;
5802 | }
5803 | 
5804 | /* Form
5805 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5806 | .custom-content form {
5807 |     width: 100%;
5808 | }
5809 | 
5810 | .custom-content input {
5811 |     word-break: break-all;
5812 |     border-radius: 100px;
5813 | }
5814 | 
5815 | .custom-content input,
5816 | .custom-content textarea {
5817 |     font-size: 1.6rem;
5818 |     display: block;
5819 |     box-sizing: border-box;
5820 |     width: 100%;
5821 |     margin-bottom: 1.5vh;
5822 |     padding: 1em 1.2em;
5823 |     transition: background-color 0.16s ease;
5824 |     background-color: var(--color-one);
5825 | }
5826 | 
5827 | .custom-content input:hover,
5828 | .custom-content input:focus,
5829 | .custom-content textarea:hover,
5830 | .custom-content textarea:focus {
5831 |     background-color: var(--color-two);
5832 | }
5833 | 
5834 | .custom-content input:last-of-type {
5835 |     margin-bottom: 1.5vh;
5836 | }
5837 | 
5838 | .custom-content textarea {
5839 |     min-height: 120px;
5840 |     resize: vertical;
5841 |     border-radius: calc(var(--border-radius) / 1.5);
5842 | }
5843 | 
5844 | .custom-content button {
5845 |     margin-top: 2vh;
5846 | }
5847 | 
5848 | /* Alerts
5849 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5850 | .custom-content .alert-loading,
5851 | .custom-content .alert-error {
5852 |     margin-top: 3vh;
5853 | }
5854 | 
5855 | .custom-content form.loading .alert-loading,
5856 | .custom-content form.success + .alert-success,
5857 | .custom-content form.error .alert-error {
5858 |     display: inline-block;
5859 | }
5860 | 
5861 | /* Success */
5862 | .custom-content form.success,
5863 | .custom-content form + .alert-success {
5864 |     display: none;
5865 | }
5866 | 
5867 | .custom-content form.success + .alert-success {
5868 |     width: 100%;
5869 | }
5870 | 
5871 | .custom-content .alert-success p {
5872 |     font-size: 1.8rem;
5873 |     margin-bottom: 4vh;
5874 |     opacity: var(--opacity-one);
5875 | }
5876 | 
5877 | /* RWD — Custom pages
5878 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5879 | @media (max-width: 1024px) {
5880 |     .custom-wrap {
5881 |         padding-right: var(--margin-wrap-left-right);
5882 |         padding-left: var(--margin-wrap-left-right);
5883 |     }
5884 | 
5885 |     .custom-image {
5886 |         display: none;
5887 |     }
5888 | }
5889 | 
5890 | @media (max-width: 480px) {
5891 |     .custom-content {
5892 |         margin-bottom: 20vh;
5893 |     }
5894 | }
5895 | 
5896 | /* --------------------------------------------------------------------------
5897 |    20.Custom — Error page
5898 |    -------------------------------------------------------------------------- */
5899 | .custom-error {
5900 |     text-align: center;
5901 | }
5902 | 
5903 | .custom-error + .loop-section .item:nth-child(4) {
5904 |     display: none;
5905 | }
5906 | 
5907 | .custom-error-content {
5908 |     flex-direction: column;
5909 |     margin-top: 3vh;
5910 |     margin-bottom: 10vh;
5911 | }
5912 | 
5913 | .custom-error h1 {
5914 |     font-family: var(--font-family-two);
5915 |     font-size: 16rem;
5916 |     font-weight: var(--font-weight-two-bold);
5917 |     line-height: 1;
5918 |     margin: 0;
5919 | }
5920 | 
5921 | .custom-error p {
5922 |     box-sizing: border-box;
5923 |     margin-top: 2vh;
5924 |     margin-bottom: 4vh;
5925 |     padding: 0 20px;
5926 | }
5927 | 
5928 | /* RWD — Error page
5929 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5930 | @media (max-width: 480px) {
5931 |     .custom-error h1 {
5932 |         font-size: 12rem;
5933 |     }
5934 | }
5935 | 
5936 | /* --------------------------------------------------------------------------
5937 |    21.Custom — Membership page
5938 |    -------------------------------------------------------------------------- */
5939 | .membership-section {
5940 |     margin-bottom: 7vh;
5941 |     padding-bottom: 7vh;
5942 | }
5943 | 
5944 | .membership-wrap {
5945 |     position: relative;
5946 |     z-index: 0;
5947 |     padding: 8vh 4vw;
5948 |     background-color: var(--color-five);
5949 | }
5950 | 
5951 | .membership-switch[data-active-public-paid-tiers="false"],
5952 | .membership-switch[data-active-price="yearly"]
5953 |     + .membership-cards
5954 |     [data-monthly],
5955 | .membership-switch[data-active-price="monthly"]
5956 |     + .membership-cards
5957 |     [data-yearly],
5958 | .membership-switch[data-active-price-plans] {
5959 |     display: none;
5960 | }
5961 | 
5962 | /* Switch
5963 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
5964 | .membership-switch,
5965 | .membership-switch::before,
5966 | .membership-switch-button {
5967 |     border-radius: 100px;
5968 | }
5969 | 
5970 | .membership-switch,
5971 | .membership-switch button {
5972 |     position: relative;
5973 | }
5974 | 
5975 | .membership-switch[data-active-price-plans*="monthly"][data-active-price-plans*="yearly"] {
5976 |     display: flex;
5977 | }
5978 | 
5979 | .membership-switch {
5980 |     display: flex;
5981 |     box-sizing: border-box;
5982 |     width: 100%;
5983 |     max-width: 240px;
5984 |     min-height: 50px;
5985 |     margin: 0 auto 4vh;
5986 |     padding: 5px;
5987 |     background-color: var(--color-body);
5988 | }
5989 | 
5990 | .membership-switch[data-active-price="monthly"]::before {
5991 |     transform: translateX(-100%);
5992 | }
5993 | 
5994 | .membership-switch::before {
5995 |     position: absolute;
5996 |     top: 5px;
5997 |     right: 5px;
5998 |     bottom: 5px;
5999 |     width: calc(50% - 5px);
6000 |     content: "";
6001 |     transition: transform 0.15s ease-in-out;
6002 |     background-color: var(--color-two);
6003 | }
6004 | 
6005 | .membership-switch button {
6006 |     font-size: 1.5rem;
6007 |     font-weight: var(--font-weight-three-medium);
6008 |     line-height: 1;
6009 |     width: 50%;
6010 |     padding: 0;
6011 |     cursor: pointer;
6012 |     -webkit-user-select: none;
6013 |     -moz-user-select: none;
6014 |     user-select: none;
6015 |     color: var(--color-font-one);
6016 |     border: 0;
6017 |     outline: none;
6018 |     background-color: transparent;
6019 |     box-shadow: none;
6020 | }
6021 | 
6022 | /* Cards
6023 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6024 | .membership-cards,
6025 | .membership-card {
6026 |     display: flex;
6027 |     flex-wrap: wrap;
6028 | }
6029 | 
6030 | .membership-cards {
6031 |     justify-content: center;
6032 |     -webkit-animation: slideTop 0.8s ease;
6033 |     animation: slideTop 0.8s ease;
6034 | }
6035 | 
6036 | .membership-cards,
6037 | .membership-card-content {
6038 |     width: 100%;
6039 | }
6040 | 
6041 | .membership-card {
6042 |     position: relative;
6043 |     flex: 1 0 calc(33.333% - var(--grid-gap));
6044 |     box-sizing: border-box;
6045 |     min-width: 280px;
6046 |     max-width: 450px;
6047 |     margin: calc(var(--grid-gap) / 2);
6048 |     padding: 3vh 2.6vh 2.6vh;
6049 |     color: var(--color-font-one);
6050 |     background-color: var(--color-body);
6051 | }
6052 | 
6053 | /* Label */
6054 | .membership-card small {
6055 |     font-size: 1.3rem;
6056 |     font-weight: var(--font-weight-three-medium);
6057 |     line-height: 1;
6058 |     position: absolute;
6059 |     top: 10px;
6060 |     right: 10px;
6061 |     display: inline-block;
6062 |     box-sizing: border-box;
6063 |     margin: 0;
6064 |     padding: 0.3em 0.8em;
6065 |     border: var(--border) var(--color-border-two);
6066 |     border-radius: 100px;
6067 | }
6068 | 
6069 | /* Price */
6070 | .membership-card-price {
6071 |     font-size: 6rem;
6072 |     line-height: 1;
6073 |     margin: 0;
6074 | }
6075 | 
6076 | .membership-card-price sup {
6077 |     font-size: 57%;
6078 |     font-weight: var(--font-weight-three-bold);
6079 | }
6080 | 
6081 | .membership-card-price sup,
6082 | .membership-card-price span {
6083 |     font-family: var(--font-family-three);
6084 | }
6085 | 
6086 | .membership-card-price span {
6087 |     font-size: 1.6rem;
6088 |     font-weight: var(--font-weight-three-medium);
6089 | }
6090 | 
6091 | /* Description */
6092 | .membership-card-excerpt {
6093 |     margin-top: 2vh;
6094 |     margin-bottom: 0;
6095 | }
6096 | 
6097 | /* List */
6098 | .membership-card-list ul {
6099 |     margin: 2.5vh 0 0;
6100 |     padding: 2.5vh 0 0;
6101 |     border-top: var(--border) var(--color-border-one);
6102 | }
6103 | 
6104 | .membership-card-list li {
6105 |     font-size: 1.6rem;
6106 |     margin: 0 0 0.5em;
6107 |     list-style: none;
6108 |     opacity: var(--opacity-one);
6109 | }
6110 | 
6111 | .membership-card-list li::before {
6112 |     font-family: var(--font-family-system);
6113 |     font-size: 1.6rem;
6114 |     font-weight: bold;
6115 |     margin-right: 7px;
6116 |     content: "✓";
6117 |     transform: translateY(-3px);
6118 | }
6119 | 
6120 | /* Button */
6121 | .membership-button {
6122 |     align-self: flex-end;
6123 |     width: 100%;
6124 |     margin: 4vh auto 0;
6125 | }
6126 | 
6127 | /* Question
6128 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6129 | .membership-wrap + small {
6130 |     margin-top: 2vh;
6131 |     text-align: center;
6132 | }
6133 | 
6134 | /* FAQs
6135 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6136 | .faq-section {
6137 |     margin-top: -3vh;
6138 |     margin-bottom: 15vh;
6139 | }
6140 | 
6141 | .faq-title {
6142 |     margin: 0 0 4vh;
6143 |     text-align: center;
6144 | }
6145 | 
6146 | .faq-content {
6147 |     max-width: 820px;
6148 |     margin: 0 auto;
6149 | }
6150 | 
6151 | .faq-content .kg-toggle-card {
6152 |     padding: 0;
6153 |     border-top: 0;
6154 |     border-bottom: var(--border) var(--color-border-one);
6155 |     border-radius: 0;
6156 |     box-shadow: none;
6157 | }
6158 | 
6159 | .faq-content .kg-toggle-card:first-of-type {
6160 |     border-top: var(--border) var(--color-border-one);
6161 | }
6162 | 
6163 | .faq-content .kg-toggle-card,
6164 | .faq-content .kg-toggle-card + .kg-toggle-card {
6165 |     margin-top: 0;
6166 | }
6167 | 
6168 | .faq-content .kg-toggle-card .kg-toggle-heading {
6169 |     position: relative;
6170 |     padding: 3.2vh 12vw 3.2vh 0;
6171 | }
6172 | 
6173 | .faq-content .kg-toggle-card .kg-toggle-heading-text {
6174 |     font-family: var(--font-family-one);
6175 |     font-size: 2.6rem;
6176 |     font-weight: var(--font-weight-one-bold);
6177 |     line-height: 1.3;
6178 | }
6179 | 
6180 | .faq-content .kg-toggle-card .kg-toggle-card-icon {
6181 |     position: absolute;
6182 |     top: calc(50% - 10px);
6183 |     right: 10px;
6184 |     margin: 0;
6185 |     padding: 0;
6186 |     cursor: pointer;
6187 | }
6188 | 
6189 | .faq-content .kg-toggle-card .kg-toggle-card-icon,
6190 | .faq-content .kg-toggle-card .kg-toggle-card-icon svg {
6191 |     width: 20px;
6192 |     height: 20px;
6193 |     color: var(--color-three);
6194 | }
6195 | 
6196 | .faq-content [data-kg-toggle-state="open"] .kg-toggle-card-icon {
6197 |     transform: rotate(0);
6198 | }
6199 | 
6200 | .faq-content .kg-toggle-card .kg-toggle-content p {
6201 |     font-size: 2rem;
6202 |     box-sizing: initial;
6203 |     max-width: 700px;
6204 |     margin-bottom: 5vh;
6205 |     padding: 0 4vw 0 0;
6206 |     opacity: var(--opacity-one);
6207 | }
6208 | 
6209 | /* RWD — Membership page
6210 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6211 | @media (max-width: 1480px) {
6212 |     .membership-wrap {
6213 |         padding: 3vh;
6214 |     }
6215 | 
6216 |     .membership-switch {
6217 |         margin-top: 4vh;
6218 |     }
6219 | }
6220 | 
6221 | @media (max-width: 1024px) {
6222 |     .membership-section {
6223 |         padding-bottom: 5vh;
6224 |     }
6225 | 
6226 |     .membership-card {
6227 |         max-width: calc(100% - var(--grid-gap));
6228 |     }
6229 | 
6230 |     .membership-card-list li {
6231 |         font-size: 1.4rem;
6232 |         margin-bottom: 2px;
6233 |     }
6234 | }
6235 | 
6236 | @media (max-width: 768px) {
6237 |     .faq-section {
6238 |         margin-bottom: 12vh;
6239 |     }
6240 | 
6241 |     .faq-content .kg-toggle-card .kg-toggle-heading-text {
6242 |         font-size: 2rem;
6243 |     }
6244 | 
6245 |     .faq-content .kg-toggle-card .kg-toggle-card-icon {
6246 |         right: 0;
6247 |     }
6248 | }
6249 | 
6250 | @media (max-width: 480px) {
6251 |     .membership-wrap {
6252 |         padding-right: 26px;
6253 |         padding-left: 26px;
6254 |     }
6255 | 
6256 |     .membership-switch {
6257 |         max-width: 70%;
6258 |         min-height: 42px;
6259 |     }
6260 | 
6261 |     .membership-switch button {
6262 |         font-size: 1.3rem;
6263 |     }
6264 | 
6265 |     .membership-card {
6266 |         min-width: 220px;
6267 |         max-width: 100%;
6268 |         margin: 0 0 2vh;
6269 |     }
6270 | 
6271 |     .membership-card-price {
6272 |         font-size: 5rem;
6273 |     }
6274 | 
6275 |     .faq-content .kg-toggle-card .kg-toggle-content p {
6276 |         font-size: 1.6rem;
6277 |     }
6278 | }
6279 | 
6280 | /* --------------------------------------------------------------------------
6281 |    22.Custom — Account page
6282 |    -------------------------------------------------------------------------- */
6283 | .account-section + .special-section {
6284 |     margin-top: 14vh;
6285 | }
6286 | 
6287 | .account-section + .membership-section {
6288 |     margin-bottom: 0;
6289 | }
6290 | 
6291 | /* Image
6292 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6293 | .archive-image.is-account {
6294 |     position: relative;
6295 | }
6296 | 
6297 | .archive-image.is-account::before {
6298 |     top: 1px;
6299 |     right: 1px;
6300 |     bottom: 1px;
6301 |     left: 1px;
6302 |     content: "";
6303 |     background-color: var(--ghost-accent-color);
6304 | }
6305 | 
6306 | .archive-image.is-account::before {
6307 |     border-radius: 100%;
6308 | }
6309 | 
6310 | .archive-image.is-account img {
6311 |     position: relative;
6312 |     z-index: 1;
6313 |     background-color: transparent;
6314 | }
6315 | 
6316 | .archive-image.is-account::before,
6317 | .archive-image.is-account svg {
6318 |     position: absolute;
6319 |     z-index: 0;
6320 | }
6321 | 
6322 | .archive-image.is-account svg {
6323 |     top: 50%;
6324 |     left: 50%;
6325 |     width: 30px;
6326 |     height: 30px;
6327 |     transform: translate(-15px, -15px);
6328 | }
6329 | 
6330 | /* Details
6331 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6332 | .account-details {
6333 |     max-width: 600px;
6334 |     margin: 0 auto 8vh;
6335 |     text-align: left;
6336 | }
6337 | 
6338 | .account-details + .account-details {
6339 |     margin-top: 20px;
6340 | }
6341 | 
6342 | .account-details-wrap,
6343 | .account-detail-column > div {
6344 |     box-sizing: border-box;
6345 | }
6346 | 
6347 | .account-details-wrap {
6348 |     margin-bottom: 10px;
6349 |     background-color: var(--color-five);
6350 | }
6351 | 
6352 | .account-details-content {
6353 |     display: flex;
6354 |     flex-wrap: wrap;
6355 |     padding: 30px 6% 20px;
6356 | }
6357 | 
6358 | .account-detail-column {
6359 |     flex-basis: auto;
6360 |     min-width: 210px;
6361 |     padding-right: 35px;
6362 | }
6363 | 
6364 | .account-detail-column > div {
6365 |     padding: 12px 0;
6366 | }
6367 | 
6368 | .account-detail-column + small {
6369 |     margin-top: 12px;
6370 | }
6371 | 
6372 | .account-detail-heading {
6373 |     font-size: 1.3rem;
6374 |     line-height: 1;
6375 |     display: block;
6376 |     opacity: var(--opacity-one);
6377 | }
6378 | 
6379 | .account-detail-content {
6380 |     font-size: 1.6rem;
6381 |     font-weight: var(--font-weight-three-bold);
6382 |     display: inline-block;
6383 |     margin-top: 10px;
6384 | }
6385 | 
6386 | /* Sign out button */
6387 | .account-signout-wrap {
6388 |     width: 100%;
6389 |     margin-top: 2vh;
6390 |     padding-top: 18px;
6391 |     text-align: right;
6392 |     border-top: var(--border) var(--color-border-one);
6393 | }
6394 | 
6395 | /* Expired */
6396 | .account-alert-expired {
6397 |     font-size: 1.2rem;
6398 |     opacity: var(--opacity-one);
6399 | }
6400 | 
6401 | /* Buttons
6402 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6403 | .account-buttons {
6404 |     font-size: 1.2rem;
6405 |     position: relative;
6406 |     display: flex;
6407 |     flex-wrap: wrap;
6408 |     width: 100%;
6409 |     opacity: var(--opacity-one);
6410 | }
6411 | 
6412 | .account-button {
6413 |     margin-right: 12px;
6414 | }
6415 | 
6416 | .account-button:hover {
6417 |     text-decoration: underline;
6418 | }
6419 | 
6420 | .account-button + .cancel-error {
6421 |     position: absolute;
6422 |     bottom: -6vh;
6423 |     left: 50%;
6424 |     transform: translateX(-50%);
6425 | }
6426 | 
6427 | .account-button.error + .cancel-error {
6428 |     display: inline-table;
6429 |     padding: 3px 10px;
6430 |     color: var(--color-font-black);
6431 |     border-radius: 100px;
6432 |     background-color: var(--color-alert-error);
6433 | }
6434 | 
6435 | /* RWD — Account page
6436 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6437 | @media (max-width: 480px) {
6438 |     .account-details-content {
6439 |         padding-right: 26px;
6440 |         padding-left: 26px;
6441 |     }
6442 | }
6443 | 
6444 | /* --------------------------------------------------------------------------
6445 |    23.Custom — Authors & Tags page
6446 |    -------------------------------------------------------------------------- */
6447 | .custom-archive {
6448 |     margin-bottom: 9vh;
6449 | }
6450 | 
6451 | .custom-archive > div {
6452 |     gap: calc(var(--grid-gap) / 2);
6453 |     grid-gap: calc(var(--grid-gap) / 2);
6454 | }
6455 | 
6456 | .custom-archive > div.is-tags {
6457 |     grid-template-columns: repeat(6, 1fr);
6458 | }
6459 | 
6460 | .custom-archive > div.is-authors {
6461 |     grid-template-columns: repeat(5, 1fr);
6462 | }
6463 | 
6464 | .custom-archive .item {
6465 |     margin-bottom: 2.4vh;
6466 | }
6467 | 
6468 | .custom-archive .item-content {
6469 |     padding-right: 5px;
6470 | }
6471 | 
6472 | .custom-archive .item small {
6473 |     font-size: 1.3rem;
6474 |     font-weight: var(--font-weight-three-medium);
6475 |     margin-top: 0.4vh;
6476 |     opacity: var(--opacity-one);
6477 | }
6478 | 
6479 | .custom-archive .item-image {
6480 |     margin-bottom: 1.3vh;
6481 | }
6482 | 
6483 | .custom-archive .item-title {
6484 |     font-size: 2.4rem;
6485 |     margin-top: 0;
6486 | }
6487 | 
6488 | .custom-archive .item-excerpt {
6489 |     margin-top: 1.3vh;
6490 | }
6491 | 
6492 | .custom-archive .item-excerpt.is-authors {
6493 |     -webkit-line-clamp: 6;
6494 | }
6495 | 
6496 | /* RWD — Authors & Tags page
6497 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6498 | @media (max-width: 1480px) {
6499 |     .custom-archive > div.is-tags {
6500 |         grid-template-columns: repeat(5, 1fr);
6501 |     }
6502 | }
6503 | 
6504 | @media (max-width: 1280px) {
6505 |     .custom-archive > div.is-tags {
6506 |         grid-template-columns: repeat(4, 1fr);
6507 |     }
6508 | 
6509 |     .custom-archive > div.is-authors {
6510 |         grid-template-columns: repeat(4, 1fr);
6511 |     }
6512 | }
6513 | 
6514 | @media (max-width: 1024px) {
6515 |     .custom-archive > div.is-authors {
6516 |         grid-template-columns: repeat(3, 1fr);
6517 |     }
6518 | }
6519 | 
6520 | @media (max-width: 768px) {
6521 |     .custom-archive > div {
6522 |         gap: var(--grid-gap);
6523 |         grid-gap: var(--grid-gap);
6524 |     }
6525 | 
6526 |     .custom-archive > div.is-tags {
6527 |         grid-template-columns: repeat(3, 1fr);
6528 |     }
6529 | 
6530 |     .custom-archive .item-title {
6531 |         font-size: 2rem;
6532 |     }
6533 | }
6534 | 
6535 | @media (max-width: 480px) {
6536 |     .custom-archive {
6537 |         margin-bottom: 6vh;
6538 |     }
6539 | 
6540 |     .custom-archive > div.is-tags,
6541 |     .custom-archive > div.is-authors {
6542 |         grid-template-columns: repeat(2, 1fr);
6543 |     }
6544 | }
6545 | 
6546 | 
6547 | .rough-notes-post-card {
6548 |     border: 1px solid #e0e0e0;
6549 |     border-radius: 8px;
6550 |     padding: 20px;
6551 |     margin-bottom: 30px;
6552 |     background-color: #f9f9f9;
6553 | }
6554 | 
6555 | .rough-notes-post-card .post-card-title a {
6556 |     color: #333;
6557 |     text-decoration: none;
6558 |     font-size: 1.5em;
6559 | }
6560 | 
6561 | .rough-notes-post-card .post-card-date {
6562 |     color: #666;
6563 |     font-size: 0.9em;
6564 | }
6565 | 
6566 | .rough-notes-post-card .post-card-image {
6567 |     width: 100%;
6568 |     height: auto;
6569 |     margin: 15px 0;
6570 | }
6571 | 
6572 | .rough-notes-post-card .post-card-excerpt {
6573 |     color: #444;
6574 |     font-size: 1em;
6575 |     line-height: 1.6;
6576 | }
6577 | 
6578 | .rough-notes-post-card .post-card-tag {
6579 |     background-color: #e0e0e0;
6580 |     color: #333;
6581 |     padding: 3px 8px;
6582 |     border-radius: 3px;
6583 |     font-size: 0.8em;
6584 |     margin-right: 5px;
6585 | }
6586 | 
6587 | .rough-notes-post-card .post-card-reading-time {
6588 |     color: #666;
6589 |     font-size: 0.9em;
6590 | }
6591 | 
6592 | 
6593 | .rough-notes-grid {
6594 |     display: grid;
6595 |     grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
6596 |     gap: 2rem;
6597 |   }
6598 |   
6599 |   .rough-notes-loader {
6600 |     text-align: center;
6601 |     padding: 2rem 0;
6602 |   }
6603 |   
6604 |   @media (max-width: 768px) {
6605 |     .rough-notes-grid {
6606 |       grid-template-columns: 1fr;
6607 |     }
6608 | }
6609 | 
6610 | .rough-notes-page {
6611 |     padding: 4rem 0;
6612 |   }
6613 |   
6614 |   .rough-notes-subtitle {
6615 |     font-size: 1.5rem;
6616 |     margin-bottom: 1.5rem;
6617 |     text-align: center;
6618 |   }
6619 |   
6620 |   .rough-notes-grid {
6621 |     display: grid;
6622 |     grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
6623 |     gap: 2rem;
6624 |   }
6625 |   
6626 |   .rough-notes-loader {
6627 |     text-align: center;
6628 |     padding: 2rem 0;
6629 |   }
6630 |   
6631 |   @media (max-width: 768px) {
6632 |     .rough-notes-grid {
6633 |       grid-template-columns: 1fr;
6634 |     }
6635 |   }
```

assets/js/global.js
```
1 | /* Minor scripts
2 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
3 |    Website : fueko.net
4 |    Author  : fueko
5 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
6 | !function(){function e(e){e.matches&&(t.checked=!1)}const t=document.getElementById("toggle"),g=document.querySelector(".post-content"),o=document.querySelector(".is-dropdown"),c=document.querySelectorAll(".header-checkbox:checked"),n=document.querySelector(".footer-nav-column.is-social li"),d=document.querySelector(".footer-nav-column.is-social");if(o&&(o.addEventListener("click",function(){o.classList.toggle("is-active")}),document.addEventListener("click",function(e){e.target.closest(".is-dropdown")||o.classList.remove("is-active")})),c){const i=window.matchMedia("(min-width: 1024px)");i.addListener(e),e(i)}n||d.remove();g&&g.style.setProperty("--scrollbar-width",window.innerWidth-document.documentElement.clientWidth+"px");}();
7 | 
8 | /* Fuse.js
9 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
10 |    Version : 6.6.2
11 |    Website : fusejs.io
12 |    Repo    : github.com/krisk/fuse
13 |    Author  : Kirollos Risk
14 |    License : Apache License 2.0
15 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
16 | var e,t;e=this,t=function(){"use strict";function e(e,t){var n=Object.keys(e);if(Object.getOwnPropertySymbols){var r=Object.getOwnPropertySymbols(e);t&&(r=r.filter((function(t){return Object.getOwnPropertyDescriptor(e,t).enumerable}))),n.push.apply(n,r)}return n}function t(t){for(var n=1;n<arguments.length;n++){var r=null!=arguments[n]?arguments[n]:{};n%2?e(Object(r),!0).forEach((function(e){a(t,e,r[e])})):Object.getOwnPropertyDescriptors?Object.defineProperties(t,Object.getOwnPropertyDescriptors(r)):e(Object(r)).forEach((function(e){Object.defineProperty(t,e,Object.getOwnPropertyDescriptor(r,e))}))}return t}function n(e){return n="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(e){return typeof e}:function(e){return e&&"function"==typeof Symbol&&e.constructor===Symbol&&e!==Symbol.prototype?"symbol":typeof e},n(e)}function r(e,t){if(!(e instanceof t))throw new TypeError("Cannot call a class as a function")}function i(e,t){for(var n=0;n<t.length;n++){var r=t[n];r.enumerable=r.enumerable||!1,r.configurable=!0,"value"in r&&(r.writable=!0),Object.defineProperty(e,r.key,r)}}function o(e,t,n){return t&&i(e.prototype,t),n&&i(e,n),Object.defineProperty(e,"prototype",{writable:!1}),e}function a(e,t,n){return t in e?Object.defineProperty(e,t,{value:n,enumerable:!0,configurable:!0,writable:!0}):e[t]=n,e}function c(e){return function(e){if(Array.isArray(e))return s(e)}(e)||function(e){if("undefined"!=typeof Symbol&&null!=e[Symbol.iterator]||null!=e["@@iterator"])return Array.from(e)}(e)||function(e,t){if(e){if("string"==typeof e)return s(e,t);var n=Object.prototype.toString.call(e).slice(8,-1);return"Object"===n&&e.constructor&&(n=e.constructor.name),"Map"===n||"Set"===n?Array.from(e):"Arguments"===n||/^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)?s(e,t):void 0}}(e)||function(){throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")}()}function s(e,t){(null==t||t>e.length)&&(t=e.length);for(var n=0,r=new Array(t);n<t;n++)r[n]=e[n];return r}function h(e){return Array.isArray?Array.isArray(e):"[object Array]"===g(e)}function u(e){return"string"==typeof e}function l(e){return"number"==typeof e}function d(e){return!0===e||!1===e||function(e){return function(e){return"object"===n(e)}(e)&&null!==e}(e)&&"[object Boolean]"==g(e)}function f(e){return null!=e}function v(e){return!e.trim().length}function g(e){return null==e?void 0===e?"[object Undefined]":"[object Null]":Object.prototype.toString.call(e)}var y="Extended search is not available",p=function(e){return"Pattern length exceeds max of ".concat(e,".")},m=Object.prototype.hasOwnProperty,b=function(){function e(t){var n=this;r(this,e),this._keys=[],this._keyMap={};var i=0;t.forEach((function(e){var t=k(e);i+=t.weight,n._keys.push(t),n._keyMap[t.id]=t,i+=t.weight})),this._keys.forEach((function(e){e.weight/=i}))}return o(e,[{key:"get",value:function(e){return this._keyMap[e]}},{key:"keys",value:function(){return this._keys}},{key:"toJSON",value:function(){return JSON.stringify(this._keys)}}]),e}();function k(e){var t=null,n=null,r=null,i=1,o=null;if(u(e)||h(e))r=e,t=M(e),n=w(e);else{if(!m.call(e,"name"))throw new Error(function(e){return"Missing ".concat(e," property in key")}("name"));var a=e.name;if(r=a,m.call(e,"weight")&&(i=e.weight)<=0)throw new Error(function(e){return"Property 'weight' in key '".concat(e,"' must be a positive integer")}(a));t=M(a),n=w(a),o=e.getFn}return{path:t,id:n,weight:i,src:r,getFn:o}}function M(e){return h(e)?e:e.split(".")}function w(e){return h(e)?e.join("."):e}var x={useExtendedSearch:!1,getFn:function(e,t){var n=[],r=!1;return function e(t,i,o){if(f(t))if(i[o]){var a=t[i[o]];if(!f(a))return;if(o===i.length-1&&(u(a)||l(a)||d(a)))n.push(function(e){return null==e?"":function(e){if("string"==typeof e)return e;var t=e+"";return"0"==t&&1/e==-1/0?"-0":t}(e)}(a));else if(h(a)){r=!0;for(var c=0,s=a.length;c<s;c+=1)e(a[c],i,o+1)}else i.length&&e(a,i,o+1)}else n.push(t)}(e,u(t)?t.split("."):t,0),r?n:n[0]},ignoreLocation:!1,ignoreFieldNorm:!1,fieldNormWeight:1},L=t(t(t(t({},{isCaseSensitive:!1,includeScore:!1,keys:[],shouldSort:!0,sortFn:function(e,t){return e.score===t.score?e.idx<t.idx?-1:1:e.score<t.score?-1:1}}),{includeMatches:!1,findAllMatches:!1,minMatchCharLength:1}),{location:0,threshold:.6,distance:100}),x),_=/[^ ]+/g;function S(){var e=arguments.length>0&&void 0!==arguments[0]?arguments[0]:1,t=arguments.length>1&&void 0!==arguments[1]?arguments[1]:3,n=new Map,r=Math.pow(10,t);return{get:function(t){var i=t.match(_).length;if(n.has(i))return n.get(i);var o=1/Math.pow(i,.5*e),a=parseFloat(Math.round(o*r)/r);return n.set(i,a),a},clear:function(){n.clear()}}}var O=function(){function e(){var t=arguments.length>0&&void 0!==arguments[0]?arguments[0]:{},n=t.getFn,i=void 0===n?L.getFn:n,o=t.fieldNormWeight,a=void 0===o?L.fieldNormWeight:o;r(this,e),this.norm=S(a,3),this.getFn=i,this.isCreated=!1,this.setIndexRecords()}return o(e,[{key:"setSources",value:function(){var e=arguments.length>0&&void 0!==arguments[0]?arguments[0]:[];this.docs=e}},{key:"setIndexRecords",value:function(){var e=arguments.length>0&&void 0!==arguments[0]?arguments[0]:[];this.records=e}},{key:"setKeys",value:function(){var e=this,t=arguments.length>0&&void 0!==arguments[0]?arguments[0]:[];this.keys=t,this._keysMap={},t.forEach((function(t,n){e._keysMap[t.id]=n}))}},{key:"create",value:function(){var e=this;!this.isCreated&&this.docs.length&&(this.isCreated=!0,u(this.docs[0])?this.docs.forEach((function(t,n){e._addString(t,n)})):this.docs.forEach((function(t,n){e._addObject(t,n)})),this.norm.clear())}},{key:"add",value:function(e){var t=this.size();u(e)?this._addString(e,t):this._addObject(e,t)}},{key:"removeAt",value:function(e){this.records.splice(e,1);for(var t=e,n=this.size();t<n;t+=1)this.records[t].i-=1}},{key:"getValueForItemAtKeyId",value:function(e,t){return e[this._keysMap[t]]}},{key:"size",value:function(){return this.records.length}},{key:"_addString",value:function(e,t){if(f(e)&&!v(e)){var n={v:e,i:t,n:this.norm.get(e)};this.records.push(n)}}},{key:"_addObject",value:function(e,t){var n=this,r={i:t,$:{}};this.keys.forEach((function(t,i){var o=t.getFn?t.getFn(e):n.getFn(e,t.path);if(f(o))if(h(o))!function(){for(var e=[],t=[{nestedArrIndex:-1,value:o}];t.length;){var a=t.pop(),c=a.nestedArrIndex,s=a.value;if(f(s))if(u(s)&&!v(s)){var l={v:s,i:c,n:n.norm.get(s)};e.push(l)}else h(s)&&s.forEach((function(e,n){t.push({nestedArrIndex:n,value:e})}))}r.$[i]=e}();else if(u(o)&&!v(o)){var a={v:o,n:n.norm.get(o)};r.$[i]=a}})),this.records.push(r)}},{key:"toJSON",value:function(){return{keys:this.keys,records:this.records}}}]),e}();function A(e,t){var n=arguments.length>2&&void 0!==arguments[2]?arguments[2]:{},r=n.getFn,i=void 0===r?L.getFn:r,o=n.fieldNormWeight,a=void 0===o?L.fieldNormWeight:o,c=new O({getFn:i,fieldNormWeight:a});return c.setKeys(e.map(k)),c.setSources(t),c.create(),c}function j(e){var t=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{},n=t.errors,r=void 0===n?0:n,i=t.currentLocation,o=void 0===i?0:i,a=t.expectedLocation,c=void 0===a?0:a,s=t.distance,h=void 0===s?L.distance:s,u=t.ignoreLocation,l=void 0===u?L.ignoreLocation:u,d=r/e.length;if(l)return d;var f=Math.abs(c-o);return h?d+f/h:f?1:d}function E(){for(var e=arguments.length>0&&void 0!==arguments[0]?arguments[0]:[],t=arguments.length>1&&void 0!==arguments[1]?arguments[1]:L.minMatchCharLength,n=[],r=-1,i=-1,o=0,a=e.length;o<a;o+=1){var c=e[o];c&&-1===r?r=o:c||-1===r||((i=o-1)-r+1>=t&&n.push([r,i]),r=-1)}return e[o-1]&&o-r>=t&&n.push([r,o-1]),n}var I=32;function F(e){for(var t={},n=0,r=e.length;n<r;n+=1){var i=e.charAt(n);t[i]=(t[i]||0)|1<<r-n-1}return t}var C=function(){function e(t){var n=this,i=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{},o=i.location,a=void 0===o?L.location:o,c=i.threshold,s=void 0===c?L.threshold:c,h=i.distance,u=void 0===h?L.distance:h,l=i.includeMatches,d=void 0===l?L.includeMatches:l,f=i.findAllMatches,v=void 0===f?L.findAllMatches:f,g=i.minMatchCharLength,y=void 0===g?L.minMatchCharLength:g,p=i.isCaseSensitive,m=void 0===p?L.isCaseSensitive:p,b=i.ignoreLocation,k=void 0===b?L.ignoreLocation:b;if(r(this,e),this.options={location:a,threshold:s,distance:u,includeMatches:d,findAllMatches:v,minMatchCharLength:y,isCaseSensitive:m,ignoreLocation:k},this.pattern=m?t:t.toLowerCase(),this.chunks=[],this.pattern.length){var M=function(e,t){n.chunks.push({pattern:e,alphabet:F(e),startIndex:t})},w=this.pattern.length;if(w>I){for(var x=0,_=w%I,S=w-_;x<S;)M(this.pattern.substr(x,I),x),x+=I;if(_){var O=w-I;M(this.pattern.substr(O),O)}}else M(this.pattern,0)}}return o(e,[{key:"searchIn",value:function(e){var t=this.options,n=t.isCaseSensitive,r=t.includeMatches;if(n||(e=e.toLowerCase()),this.pattern===e){var i={isMatch:!0,score:0};return r&&(i.indices=[[0,e.length-1]]),i}var o=this.options,a=o.location,s=o.distance,h=o.threshold,u=o.findAllMatches,l=o.minMatchCharLength,d=o.ignoreLocation,f=[],v=0,g=!1;this.chunks.forEach((function(t){var n=t.pattern,i=t.alphabet,o=t.startIndex,y=function(e,t,n){var r=arguments.length>3&&void 0!==arguments[3]?arguments[3]:{},i=r.location,o=void 0===i?L.location:i,a=r.distance,c=void 0===a?L.distance:a,s=r.threshold,h=void 0===s?L.threshold:s,u=r.findAllMatches,l=void 0===u?L.findAllMatches:u,d=r.minMatchCharLength,f=void 0===d?L.minMatchCharLength:d,v=r.includeMatches,g=void 0===v?L.includeMatches:v,y=r.ignoreLocation,m=void 0===y?L.ignoreLocation:y;if(t.length>I)throw new Error(p(I));for(var b,k=t.length,M=e.length,w=Math.max(0,Math.min(o,M)),x=h,_=w,S=f>1||g,O=S?Array(M):[];(b=e.indexOf(t,_))>-1;){var A=j(t,{currentLocation:b,expectedLocation:w,distance:c,ignoreLocation:m});if(x=Math.min(A,x),_=b+k,S)for(var F=0;F<k;)O[b+F]=1,F+=1}_=-1;for(var C=[],N=1,P=k+M,W=1<<k-1,$=0;$<k;$+=1){for(var D=0,K=P;D<K;)j(t,{errors:$,currentLocation:w+K,expectedLocation:w,distance:c,ignoreLocation:m})<=x?D=K:P=K,K=Math.floor((P-D)/2+D);P=K;var T=Math.max(1,w-K+1),z=l?M:Math.min(w+K,M)+k,J=Array(z+2);J[z+1]=(1<<$)-1;for(var R=z;R>=T;R-=1){var U=R-1,B=n[e.charAt(U)];if(S&&(O[U]=+!!B),J[R]=(J[R+1]<<1|1)&B,$&&(J[R]|=(C[R+1]|C[R])<<1|1|C[R+1]),J[R]&W&&(N=j(t,{errors:$,currentLocation:U,expectedLocation:w,distance:c,ignoreLocation:m}))<=x){if(x=N,(_=U)<=w)break;T=Math.max(1,2*w-_)}}if(j(t,{errors:$+1,currentLocation:w,expectedLocation:w,distance:c,ignoreLocation:m})>x)break;C=J}var V={isMatch:_>=0,score:Math.max(.001,N)};if(S){var q=E(O,f);q.length?g&&(V.indices=q):V.isMatch=!1}return V}(e,n,i,{location:a+o,distance:s,threshold:h,findAllMatches:u,minMatchCharLength:l,includeMatches:r,ignoreLocation:d}),m=y.isMatch,b=y.score,k=y.indices;m&&(g=!0),v+=b,m&&k&&(f=[].concat(c(f),c(k)))}));var y={isMatch:g,score:g?v/this.chunks.length:1};return g&&r&&(y.indices=f),y}}]),e}(),N=[];function P(e,t){for(var n=0,r=N.length;n<r;n+=1){var i=N[n];if(i.condition(e,t))return new i(e,t)}return new C(e,t)}function W(e,t){var n=t.ignoreFieldNorm,r=void 0===n?L.ignoreFieldNorm:n;e.forEach((function(e){var t=1;e.matches.forEach((function(e){var n=e.key,i=e.norm,o=e.score,a=n?n.weight:null;t*=Math.pow(0===o&&a?Number.EPSILON:o,(a||1)*(r?1:i))})),e.score=t}))}function $(e,t){var n=e.matches;t.matches=[],f(n)&&n.forEach((function(e){if(f(e.indices)&&e.indices.length){var n={indices:e.indices,value:e.value};e.key&&(n.key=e.key.src),e.idx>-1&&(n.refIndex=e.idx),t.matches.push(n)}}))}function D(e,t){t.score=e.score}function K(e,t){var n=arguments.length>2&&void 0!==arguments[2]?arguments[2]:{},r=n.includeMatches,i=void 0===r?L.includeMatches:r,o=n.includeScore,a=void 0===o?L.includeScore:o,c=[];return i&&c.push($),a&&c.push(D),e.map((function(e){var n=e.idx,r={item:t[n],refIndex:n};return c.length&&c.forEach((function(t){t(e,r)})),r}))}var T=function(){function e(n){var i=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{},o=arguments.length>2?arguments[2]:void 0;if(r(this,e),this.options=t(t({},L),i),this.options.useExtendedSearch)throw new Error(y);this._keyStore=new b(this.options.keys),this.setCollection(n,o)}return o(e,[{key:"setCollection",value:function(e,t){if(this._docs=e,t&&!(t instanceof O))throw new Error("Incorrect 'index' type");this._myIndex=t||A(this.options.keys,this._docs,{getFn:this.options.getFn,fieldNormWeight:this.options.fieldNormWeight})}},{key:"add",value:function(e){f(e)&&(this._docs.push(e),this._myIndex.add(e))}},{key:"remove",value:function(){for(var e=arguments.length>0&&void 0!==arguments[0]?arguments[0]:function(){return!1},t=[],n=0,r=this._docs.length;n<r;n+=1){var i=this._docs[n];e(i,n)&&(this.removeAt(n),n-=1,r-=1,t.push(i))}return t}},{key:"removeAt",value:function(e){this._docs.splice(e,1),this._myIndex.removeAt(e)}},{key:"getIndex",value:function(){return this._myIndex}},{key:"search",value:function(e){var t=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{},n=t.limit,r=void 0===n?-1:n,i=this.options,o=i.includeMatches,a=i.includeScore,c=i.shouldSort,s=i.sortFn,h=i.ignoreFieldNorm,d=u(e)?u(this._docs[0])?this._searchStringList(e):this._searchObjectList(e):this._searchLogical(e);return W(d,{ignoreFieldNorm:h}),c&&d.sort(s),l(r)&&r>-1&&(d=d.slice(0,r)),K(d,this._docs,{includeMatches:o,includeScore:a})}},{key:"_searchStringList",value:function(e){var t=P(e,this.options),n=this._myIndex.records,r=[];return n.forEach((function(e){var n=e.v,i=e.i,o=e.n;if(f(n)){var a=t.searchIn(n),c=a.isMatch,s=a.score,h=a.indices;c&&r.push({item:n,idx:i,matches:[{score:s,value:n,norm:o,indices:h}]})}})),r}},{key:"_searchLogical",value:function(e){throw new Error("Logical search is not available")}},{key:"_searchObjectList",value:function(e){var t=this,n=P(e,this.options),r=this._myIndex,i=r.keys,o=r.records,a=[];return o.forEach((function(e){var r=e.$,o=e.i;if(f(r)){var s=[];i.forEach((function(e,i){s.push.apply(s,c(t._findMatches({key:e,value:r[i],searcher:n})))})),s.length&&a.push({idx:o,item:r,matches:s})}})),a}},{key:"_findMatches",value:function(e){var t=e.key,n=e.value,r=e.searcher;if(!f(n))return[];var i=[];if(h(n))n.forEach((function(e){var n=e.v,o=e.i,a=e.n;if(f(n)){var c=r.searchIn(n),s=c.isMatch,h=c.score,u=c.indices;s&&i.push({score:h,key:t,value:n,idx:o,norm:a,indices:u})}}));else{var o=n.v,a=n.n,c=r.searchIn(o),s=c.isMatch,u=c.score,l=c.indices;s&&i.push({score:u,key:t,value:o,norm:a,indices:l})}return i}}]),e}();return T.version="6.6.2",T.createIndex=A,T.parseIndex=function(e){var t=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{},n=t.getFn,r=void 0===n?L.getFn:n,i=t.fieldNormWeight,o=void 0===i?L.fieldNormWeight:i,a=e.keys,c=e.records,s=new O({getFn:r,fieldNormWeight:o});return s.setKeys(a),s.setIndexRecords(c),s},T.config=L,T},"object"==typeof exports&&"undefined"!=typeof module?module.exports=t():"function"==typeof define&&define.amd?define(t):(e="undefined"!=typeof globalThis?globalThis:e||self).Fuse=t();
17 | 
18 | /* Search function */
19 | document.addEventListener("DOMContentLoaded",function(){!function(e){"use strict";const t=document.body,n=document.querySelector(".search-section"),s=document.querySelectorAll(".search-open"),i=document.querySelector(".search-close"),c=document.querySelector(".search-input"),a=document.querySelector(".search-info"),o=document.querySelector(".search-counter"),r=document.querySelector(".search-results"),d=document.querySelector(".search-counter span"),l=document.querySelector(".search-overlay");if(n){function u(){t.classList.remove("search-is-active"),t.classList.add("search-no-active"),c.value="",r.innerHTML="",o.classList.add("is-hide"),a.classList.remove("is-hide"),window.scrollTo(0,0)}t.addEventListener("keyup",function(e){27==e.keyCode&&u()}),i.addEventListener("click",u),l.addEventListener("click",u),s.forEach(function(s){s.addEventListener("click",function(){t.classList.add("search-is-active"),t.classList.remove("search-no-active"),n.style.display="block",c.focus()}),s.addEventListener("click",function(){if(!1===m){var t=options.api,n=new XMLHttpRequest;n.open("GET",t,!0),n.onload=function(){var e,t;n.status>=200&&n.status<400&&(n.response,e=JSON.parse(n.responseText),t=new Fuse(e.posts,options),c.onkeyup=function(e){if(d.innerHTML="",r.innerHTML="",this.value.length>2&&(a.classList.add("is-hide"),o.classList.remove("is-hide")),this.value.length<3&&(a.classList.remove("is-hide"),o.classList.add("is-hide")),!(this.value.length<=2)){const n=t.search(e.target.value,{limit:options.limit});d.innerHTML=n.length,n.map(function(e){var t=new Date(e.item.published_at).toLocaleDateString(document.documentElement.lang,{year:"numeric",month:"long",day:"numeric"}),n=document.createElement("time"),s=document.createElement("h5"),i=document.createElement("span"),c=document.createElement("a");if(!0===options.images){var a=document.createElement("img");null!==e.item.feature_image&&(a.setAttribute("src",e.item.feature_image),c.appendChild(a))}n.textContent=n.innerHTML+=t,i.textContent=e.item.title,c.setAttribute("href",e.item.url),s.appendChild(i),r.appendChild(c),c.appendChild(s),c.appendChild(n)})}})},n.send(),s.removeEventListener("click",e)}m=!0})});var m=!1}}(window)});
```

assets/js/index.js
```
1 | /* Infinite Scroll
2 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
3 |    Version : 3.0.6
4 |    Website : infinite-scroll.com
5 |    Repo    : github.com/metafizzy/infinite-scroll
6 |    Author  : David DeSandro
7 |    License : Commercial Developer
8 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
9 | !function(t,e){"function"==typeof define&&define.amd?define("jquery-bridget/jquery-bridget",["jquery"],function(i){return e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("jquery")):t.jQueryBridget=e(t,t.jQuery)}(window,function(t,e){"use strict";function i(i,r,l){function a(t,e,n){var o,r="$()."+i+'("'+e+'")';return t.each(function(t,a){var h=l.data(a,i);if(!h)return void s(i+" not initialized. Cannot call methods, i.e. "+r);var c=h[e];if(!c||"_"==e.charAt(0))return void s(r+" is not a valid method");var u=c.apply(h,n);o=void 0===o?u:o}),void 0!==o?o:t}function h(t,e){t.each(function(t,n){var o=l.data(n,i);o?(o.option(e),o._init()):(o=new r(n,e),l.data(n,i,o))})}l=l||e||t.jQuery,l&&(r.prototype.option||(r.prototype.option=function(t){l.isPlainObject(t)&&(this.options=l.extend(!0,this.options,t))}),l.fn[i]=function(t){if("string"==typeof t){var e=o.call(arguments,1);return a(this,t,e)}return h(this,t),this},n(l))}function n(t){!t||t&&t.bridget||(t.bridget=i)}var o=Array.prototype.slice,r=t.console,s="undefined"==typeof r?function(){}:function(t){r.error(t)};return n(e||t.jQuery),i}),function(t,e){"function"==typeof define&&define.amd?define("ev-emitter/ev-emitter",e):"object"==typeof module&&module.exports?module.exports=e():t.EvEmitter=e()}("undefined"!=typeof window?window:this,function(){function t(){}var e=t.prototype;return e.on=function(t,e){if(t&&e){var i=this._events=this._events||{},n=i[t]=i[t]||[];return n.indexOf(e)==-1&&n.push(e),this}},e.once=function(t,e){if(t&&e){this.on(t,e);var i=this._onceEvents=this._onceEvents||{},n=i[t]=i[t]||{};return n[e]=!0,this}},e.off=function(t,e){var i=this._events&&this._events[t];if(i&&i.length){var n=i.indexOf(e);return n!=-1&&i.splice(n,1),this}},e.emitEvent=function(t,e){var i=this._events&&this._events[t];if(i&&i.length){i=i.slice(0),e=e||[];for(var n=this._onceEvents&&this._onceEvents[t],o=0;o<i.length;o++){var r=i[o],s=n&&n[r];s&&(this.off(t,r),delete n[r]),r.apply(this,e)}return this}},e.allOff=function(){delete this._events,delete this._onceEvents},t}),function(t,e){"use strict";"function"==typeof define&&define.amd?define("desandro-matches-selector/matches-selector",e):"object"==typeof module&&module.exports?module.exports=e():t.matchesSelector=e()}(window,function(){"use strict";var t=function(){var t=window.Element.prototype;if(t.matches)return"matches";if(t.matchesSelector)return"matchesSelector";for(var e=["webkit","moz","ms","o"],i=0;i<e.length;i++){var n=e[i],o=n+"MatchesSelector";if(t[o])return o}}();return function(e,i){return e[t](i)}}),function(t,e){"function"==typeof define&&define.amd?define("fizzy-ui-utils/utils",["desandro-matches-selector/matches-selector"],function(i){return e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("desandro-matches-selector")):t.fizzyUIUtils=e(t,t.matchesSelector)}(window,function(t,e){var i={};i.extend=function(t,e){for(var i in e)t[i]=e[i];return t},i.modulo=function(t,e){return(t%e+e)%e};var n=Array.prototype.slice;i.makeArray=function(t){if(Array.isArray(t))return t;if(null===t||void 0===t)return[];var e="object"==typeof t&&"number"==typeof t.length;return e?n.call(t):[t]},i.removeFrom=function(t,e){var i=t.indexOf(e);i!=-1&&t.splice(i,1)},i.getParent=function(t,i){for(;t.parentNode&&t!=document.body;)if(t=t.parentNode,e(t,i))return t},i.getQueryElement=function(t){return"string"==typeof t?document.querySelector(t):t},i.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},i.filterFindElements=function(t,n){t=i.makeArray(t);var o=[];return t.forEach(function(t){if(t instanceof HTMLElement){if(!n)return void o.push(t);e(t,n)&&o.push(t);for(var i=t.querySelectorAll(n),r=0;r<i.length;r++)o.push(i[r])}}),o},i.debounceMethod=function(t,e,i){i=i||100;var n=t.prototype[e],o=e+"Timeout";t.prototype[e]=function(){var t=this[o];clearTimeout(t);var e=arguments,r=this;this[o]=setTimeout(function(){n.apply(r,e),delete r[o]},i)}},i.docReady=function(t){var e=document.readyState;"complete"==e||"interactive"==e?setTimeout(t):document.addEventListener("DOMContentLoaded",t)},i.toDashed=function(t){return t.replace(/(.)([A-Z])/g,function(t,e,i){return e+"-"+i}).toLowerCase()};var o=t.console;return i.htmlInit=function(e,n){i.docReady(function(){var r=i.toDashed(n),s="data-"+r,l=document.querySelectorAll("["+s+"]"),a=document.querySelectorAll(".js-"+r),h=i.makeArray(l).concat(i.makeArray(a)),c=s+"-options",u=t.jQuery;h.forEach(function(t){var i,r=t.getAttribute(s)||t.getAttribute(c);try{i=r&&JSON.parse(r)}catch(l){return void(o&&o.error("Error parsing "+s+" on "+t.className+": "+l))}var a=new e(t,i);u&&u.data(t,n,a)})})},i}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/core",["ev-emitter/ev-emitter","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof module&&module.exports?module.exports=e(t,require("ev-emitter"),require("fizzy-ui-utils")):t.InfiniteScroll=e(t,t.EvEmitter,t.fizzyUIUtils)}(window,function(t,e,i){function n(t,e){var s=i.getQueryElement(t);if(!s)return void console.error("Bad element for InfiniteScroll: "+(s||t));if(t=s,t.infiniteScrollGUID){var l=r[t.infiniteScrollGUID];return l.option(e),l}this.element=t,this.options=i.extend({},n.defaults),this.option(e),o&&(this.$element=o(this.element)),this.create()}var o=t.jQuery,r={};n.defaults={},n.create={},n.destroy={};var s=n.prototype;i.extend(s,e.prototype);var l=0;s.create=function(){var t=this.guid=++l;this.element.infiniteScrollGUID=t,r[t]=this,this.pageIndex=1,this.loadCount=0,this.updateGetPath();var e=this.getPath&&this.getPath();if(!e)return void console.error("Disabling InfiniteScroll");this.updateGetAbsolutePath(),this.log("initialized",[this.element.className]),this.callOnInit();for(var i in n.create)n.create[i].call(this)},s.option=function(t){i.extend(this.options,t)},s.callOnInit=function(){var t=this.options.onInit;t&&t.call(this,this)},s.dispatchEvent=function(t,e,i){this.log(t,i);var n=e?[e].concat(i):i;if(this.emitEvent(t,n),o&&this.$element){t+=".infiniteScroll";var r=t;if(e){var s=o.Event(e);s.type=t,r=s}this.$element.trigger(r,i)}};var a={initialized:function(t){return"on "+t},request:function(t){return"URL: "+t},load:function(t,e){return(t.title||"")+". URL: "+e},error:function(t,e){return t+". URL: "+e},append:function(t,e,i){return i.length+" items. URL: "+e},last:function(t,e){return"URL: "+e},history:function(t,e){return"URL: "+e},pageIndex:function(t,e){return"current page determined to be: "+t+" from "+e}};s.log=function(t,e){if(this.options.debug){var i="[InfiniteScroll] "+t,n=a[t];n&&(i+=". "+n.apply(this,e)),console.log(i)}},s.updateMeasurements=function(){this.windowHeight=t.innerHeight;var e=this.element.getBoundingClientRect();this.top=e.top+t.pageYOffset},s.updateScroller=function(){var e=this.options.elementScroll;if(!e)return void(this.scroller=t);if(this.scroller=e===!0?this.element:i.getQueryElement(e),!this.scroller)throw"Unable to find elementScroll: "+e},s.updateGetPath=function(){var t=this.options.path;if(!t)return void console.error("InfiniteScroll path option required. Set as: "+t);var e=typeof t;if("function"==e)return void(this.getPath=t);var i="string"==e&&t.match("{{#}}");return i?void this.updateGetPathTemplate(t):void this.updateGetPathSelector(t)},s.updateGetPathTemplate=function(t){this.getPath=function(){var e=this.pageIndex+1;return t.replace("{{#}}",e)}.bind(this);var e=t.replace(/(\\\?|\?)/,"\\?").replace("{{#}}","(\\d\\d?\\d?)"),i=new RegExp(e),n=location.href.match(i);n&&(this.pageIndex=parseInt(n[1],10),this.log("pageIndex",[this.pageIndex,"template string"]))};var h=[/^(.*?\/?page\/?)(\d\d?\d?)(.*?$)/,/^(.*?\/?\?page=)(\d\d?\d?)(.*?$)/,/(.*?)(\d\d?\d?)(?!.*\d)(.*?$)/];return s.updateGetPathSelector=function(t){var e=document.querySelector(t);if(!e)return void console.error("Bad InfiniteScroll path option. Next link not found: "+t);for(var i,n,o=e.getAttribute("href"),r=0;o&&r<h.length;r++){n=h[r];var s=o.match(n);if(s){i=s.slice(1);break}}return i?(this.isPathSelector=!0,this.getPath=function(){var t=this.pageIndex+1;return i[0]+t+i[2]}.bind(this),this.pageIndex=parseInt(i[1],10)-1,void this.log("pageIndex",[this.pageIndex,"next link"])):void console.error("InfiniteScroll unable to parse next link href: "+o)},s.updateGetAbsolutePath=function(){var t=this.getPath(),e=t.match(/^http/)||t.match(/^\//);if(e)return void(this.getAbsolutePath=this.getPath);var i=location.pathname,n=t.match(/^\?/);if(n)return void(this.getAbsolutePath=function(){return i+this.getPath()});var o=i.substring(0,i.lastIndexOf("/"));this.getAbsolutePath=function(){return o+"/"+this.getPath()}},n.create.hideNav=function(){var t=i.getQueryElement(this.options.hideNav);t&&(t.style.display="none",this.nav=t)},n.destroy.hideNav=function(){this.nav&&(this.nav.style.display="")},s.destroy=function(){this.allOff();for(var t in n.destroy)n.destroy[t].call(this);delete this.element.infiniteScrollGUID,delete r[this.guid],o&&this.$element&&o.removeData(this.element,"infiniteScroll")},n.throttle=function(t,e){e=e||200;var i,n;return function(){var o=+new Date,r=arguments,s=function(){i=o,t.apply(this,r)}.bind(this);i&&o<i+e?(clearTimeout(n),n=setTimeout(s,e)):s()}},n.data=function(t){t=i.getQueryElement(t);var e=t&&t.infiniteScrollGUID;return e&&r[e]},n.setJQuery=function(t){o=t},i.htmlInit(n,"infinite-scroll"),s._init=function(){},o&&o.bridget&&o.bridget("infiniteScroll",n),n}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/page-load",["./core"],function(i){return e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("./core")):e(t,t.InfiniteScroll)}(window,function(t,e){function i(t){for(var e=document.createDocumentFragment(),i=0;t&&i<t.length;i++)e.appendChild(t[i]);return e}function n(t){for(var e=t.querySelectorAll("script"),i=0;i<e.length;i++){var n=e[i],r=document.createElement("script");o(n,r),r.innerHTML=n.innerHTML,n.parentNode.replaceChild(r,n)}}function o(t,e){for(var i=t.attributes,n=0;n<i.length;n++){var o=i[n];e.setAttribute(o.name,o.value)}}function r(t,e,i,n,o){var r=new XMLHttpRequest;r.open("GET",t,!0),r.responseType=e||"",r.setRequestHeader("X-Requested-With","XMLHttpRequest"),r.onload=function(){if(200==r.status)i(r.response);else if(204==r.status)o(r.response);else{var t=new Error(r.statusText);n(t)}},r.onerror=function(){var e=new Error("Network error requesting "+t);n(e)},r.send()}var s=e.prototype;return e.defaults.loadOnScroll=!0,e.defaults.checkLastPage=!0,e.defaults.responseType="document",e.create.pageLoad=function(){this.canLoad=!0,this.on("scrollThreshold",this.onScrollThresholdLoad),this.on("load",this.checkLastPage),this.options.outlayer&&this.on("append",this.onAppendOutlayer)},s.onScrollThresholdLoad=function(){this.options.loadOnScroll&&this.loadNextPage()},s.loadNextPage=function(){if(!this.isLoading&&this.canLoad){var t=this.getAbsolutePath();this.isLoading=!0;var e=function(e){this.onPageLoad(e,t)}.bind(this),i=function(e){this.onPageError(e,t)}.bind(this),n=function(e){this.lastPageReached(e,t)}.bind(this);r(t,this.options.responseType,e,i,n),this.dispatchEvent("request",null,[t])}},s.onPageLoad=function(t,e){return this.options.append||(this.isLoading=!1),this.pageIndex++,this.loadCount++,this.dispatchEvent("load",null,[t,e]),this.appendNextPage(t,e),t},s.appendNextPage=function(t,e){var n=this.options.append,o="document"==this.options.responseType;if(o&&n){var r=t.querySelectorAll(n),s=i(r),l=function(){this.appendItems(r,s),this.isLoading=!1,this.dispatchEvent("append",null,[t,e,r])}.bind(this);this.options.outlayer?this.appendOutlayerItems(s,l):l()}},s.appendItems=function(t,e){t&&t.length&&(e=e||i(t),n(e),this.element.appendChild(e))},s.appendOutlayerItems=function(i,n){var o=e.imagesLoaded||t.imagesLoaded;return o?void o(i,n):(console.error("[InfiniteScroll] imagesLoaded required for outlayer option"),void(this.isLoading=!1))},s.onAppendOutlayer=function(t,e,i){this.options.outlayer.appended(i)},s.checkLastPage=function(t,e){var i=this.options.checkLastPage;if(i){var n=this.options.path;if("function"==typeof n){var o=this.getPath();if(!o)return void this.lastPageReached(t,e)}var r;if("string"==typeof i?r=i:this.isPathSelector&&(r=n),r&&t.querySelector){var s=t.querySelector(r);s||this.lastPageReached(t,e)}}},s.lastPageReached=function(t,e){this.canLoad=!1,this.dispatchEvent("last",null,[t,e])},s.onPageError=function(t,e){return this.isLoading=!1,this.canLoad=!1,this.dispatchEvent("error",null,[t,e]),t},e.create.prefill=function(){if(this.options.prefill){var t=this.options.append;if(!t)return void console.error("append option required for prefill. Set as :"+t);this.updateMeasurements(),this.updateScroller(),this.isPrefilling=!0,this.on("append",this.prefill),this.once("error",this.stopPrefill),this.once("last",this.stopPrefill),this.prefill()}},s.prefill=function(){var t=this.getPrefillDistance();this.isPrefilling=t>=0,this.isPrefilling?(this.log("prefill"),this.loadNextPage()):this.stopPrefill()},s.getPrefillDistance=function(){return this.options.elementScroll?this.scroller.clientHeight-this.scroller.scrollHeight:this.windowHeight-this.element.clientHeight},s.stopPrefill=function(){this.log("stopPrefill"),this.off("append",this.prefill)},e}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/scroll-watch",["./core","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof module&&module.exports?module.exports=e(t,require("./core"),require("fizzy-ui-utils")):e(t,t.InfiniteScroll,t.fizzyUIUtils)}(window,function(t,e,i){var n=e.prototype;return e.defaults.scrollThreshold=400,e.create.scrollWatch=function(){this.pageScrollHandler=this.onPageScroll.bind(this),this.resizeHandler=this.onResize.bind(this);var t=this.options.scrollThreshold,e=t||0===t;e&&this.enableScrollWatch()},e.destroy.scrollWatch=function(){this.disableScrollWatch()},n.enableScrollWatch=function(){this.isScrollWatching||(this.isScrollWatching=!0,this.updateMeasurements(),this.updateScroller(),this.on("last",this.disableScrollWatch),this.bindScrollWatchEvents(!0))},n.disableScrollWatch=function(){this.isScrollWatching&&(this.bindScrollWatchEvents(!1),delete this.isScrollWatching)},n.bindScrollWatchEvents=function(e){var i=e?"addEventListener":"removeEventListener";this.scroller[i]("scroll",this.pageScrollHandler),t[i]("resize",this.resizeHandler)},n.onPageScroll=e.throttle(function(){var t=this.getBottomDistance();t<=this.options.scrollThreshold&&this.dispatchEvent("scrollThreshold")}),n.getBottomDistance=function(){return this.options.elementScroll?this.getElementBottomDistance():this.getWindowBottomDistance()},n.getWindowBottomDistance=function(){var e=this.top+this.element.clientHeight,i=t.pageYOffset+this.windowHeight;return e-i},n.getElementBottomDistance=function(){var t=this.scroller.scrollHeight,e=this.scroller.scrollTop+this.scroller.clientHeight;return t-e},n.onResize=function(){this.updateMeasurements()},i.debounceMethod(e,"onResize",150),e}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/history",["./core","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof module&&module.exports?module.exports=e(t,require("./core"),require("fizzy-ui-utils")):e(t,t.InfiniteScroll,t.fizzyUIUtils)}(window,function(t,e,i){var n=e.prototype;e.defaults.history="replace";var o=document.createElement("a");return e.create.history=function(){if(this.options.history){o.href=this.getAbsolutePath();var t=o.origin||o.protocol+"//"+o.host,e=t==location.origin;return e?void(this.options.append?this.createHistoryAppend():this.createHistoryPageLoad()):void console.error("[InfiniteScroll] cannot set history with different origin: "+o.origin+" on "+location.origin+" . History behavior disabled.")}},n.createHistoryAppend=function(){this.updateMeasurements(),this.updateScroller(),this.scrollPages=[{top:0,path:location.href,title:document.title}],this.scrollPageIndex=0,this.scrollHistoryHandler=this.onScrollHistory.bind(this),this.unloadHandler=this.onUnload.bind(this),this.scroller.addEventListener("scroll",this.scrollHistoryHandler),this.on("append",this.onAppendHistory),this.bindHistoryAppendEvents(!0)},n.bindHistoryAppendEvents=function(e){var i=e?"addEventListener":"removeEventListener";this.scroller[i]("scroll",this.scrollHistoryHandler),t[i]("unload",this.unloadHandler)},n.createHistoryPageLoad=function(){this.on("load",this.onPageLoadHistory)},e.destroy.history=n.destroyHistory=function(){var t=this.options.history&&this.options.append;t&&this.bindHistoryAppendEvents(!1)},n.onAppendHistory=function(t,e,i){if(i&&i.length){var n=i[0],r=this.getElementScrollY(n);o.href=e,this.scrollPages.push({top:r,path:o.href,title:t.title})}},n.getElementScrollY=function(t){return this.options.elementScroll?this.getElementElementScrollY(t):this.getElementWindowScrollY(t)},n.getElementWindowScrollY=function(e){var i=e.getBoundingClientRect();return i.top+t.pageYOffset},n.getElementElementScrollY=function(t){return t.offsetTop-this.top},n.onScrollHistory=function(){for(var t,e,i=this.getScrollViewY(),n=0;n<this.scrollPages.length;n++){var o=this.scrollPages[n];if(o.top>=i)break;t=n,e=o}t!=this.scrollPageIndex&&(this.scrollPageIndex=t,this.setHistory(e.title,e.path))},i.debounceMethod(e,"onScrollHistory",150),n.getScrollViewY=function(){return this.options.elementScroll?this.scroller.scrollTop+this.scroller.clientHeight/2:t.pageYOffset+this.windowHeight/2},n.setHistory=function(t,e){var i=this.options.history,n=i&&history[i+"State"];n&&(history[i+"State"](null,t,e),this.options.historyTitle&&(document.title=t),this.dispatchEvent("history",null,[t,e]))},n.onUnload=function(){var e=this.scrollPageIndex;if(0!==e){var i=this.scrollPages[e],n=t.pageYOffset-i.top+this.top;this.destroyHistory(),scrollTo(0,n)}},n.onPageLoadHistory=function(t,e){this.setHistory(t.title,e)},e}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/button",["./core","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof module&&module.exports?module.exports=e(t,require("./core"),require("fizzy-ui-utils")):e(t,t.InfiniteScroll,t.fizzyUIUtils)}(window,function(t,e,i){function n(t,e){this.element=t,this.infScroll=e,this.clickHandler=this.onClick.bind(this),this.element.addEventListener("click",this.clickHandler),e.on("request",this.disable.bind(this)),e.on("load",this.enable.bind(this)),e.on("error",this.hide.bind(this)),e.on("last",this.hide.bind(this))}return e.create.button=function(){var t=i.getQueryElement(this.options.button);if(t)return void(this.button=new n(t,this))},e.destroy.button=function(){this.button&&this.button.destroy()},n.prototype.onClick=function(t){t.preventDefault(),this.infScroll.loadNextPage()},n.prototype.enable=function(){this.element.removeAttribute("disabled")},n.prototype.disable=function(){this.element.disabled="disabled"},n.prototype.hide=function(){this.element.style.display="none"},n.prototype.destroy=function(){this.element.removeEventListener("click",this.clickHandler)},e.Button=n,e}),function(t,e){"function"==typeof define&&define.amd?define("infinite-scroll/js/status",["./core","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof module&&module.exports?module.exports=e(t,require("./core"),require("fizzy-ui-utils")):e(t,t.InfiniteScroll,t.fizzyUIUtils)}(window,function(t,e,i){function n(t){r(t,"none")}function o(t){r(t,"block")}function r(t,e){t&&(t.style.display=e)}var s=e.prototype;return e.create.status=function(){var t=i.getQueryElement(this.options.status);t&&(this.statusElement=t,this.statusEventElements={request:t.querySelector(".infinite-scroll-request"),error:t.querySelector(".infinite-scroll-error"),last:t.querySelector(".infinite-scroll-last")},this.on("request",this.showRequestStatus),this.on("error",this.showErrorStatus),this.on("last",this.showLastStatus),this.bindHideStatus("on"))},s.bindHideStatus=function(t){var e=this.options.append?"append":"load";this[t](e,this.hideAllStatus)},s.showRequestStatus=function(){this.showStatus("request")},s.showErrorStatus=function(){this.showStatus("error")},s.showLastStatus=function(){this.showStatus("last"),this.bindHideStatus("off")},s.showStatus=function(t){o(this.statusElement),this.hideStatusEventElements();var e=this.statusEventElements[t];o(e)},s.hideAllStatus=function(){n(this.statusElement),this.hideStatusEventElements()},s.hideStatusEventElements=function(){for(var t in this.statusEventElements){var e=this.statusEventElements[t];n(e)}},e}),function(t,e){"function"==typeof define&&define.amd?define(["infinite-scroll/js/core","infinite-scroll/js/page-load","infinite-scroll/js/scroll-watch","infinite-scroll/js/history","infinite-scroll/js/button","infinite-scroll/js/status"],e):"object"==typeof module&&module.exports&&(module.exports=e(require("./core"),require("./page-load"),require("./scroll-watch"),require("./history"),require("./button"),require("./status")))}(window,function(t){return t}),function(t,e){"use strict";"function"==typeof define&&define.amd?define("imagesloaded/imagesloaded",["ev-emitter/ev-emitter"],function(i){return e(t,i)}):"object"==typeof module&&module.exports?module.exports=e(t,require("ev-emitter")):t.imagesLoaded=e(t,t.EvEmitter)}("undefined"!=typeof window?window:this,function(t,e){function i(t,e){for(var i in e)t[i]=e[i];return t}function n(t){if(Array.isArray(t))return t;var e="object"==typeof t&&"number"==typeof t.length;return e?h.call(t):[t]}function o(t,e,r){if(!(this instanceof o))return new o(t,e,r);var s=t;return"string"==typeof t&&(s=document.querySelectorAll(t)),s?(this.elements=n(s),this.options=i({},this.options),"function"==typeof e?r=e:i(this.options,e),r&&this.on("always",r),this.getImages(),l&&(this.jqDeferred=new l.Deferred),void setTimeout(this.check.bind(this))):void a.error("Bad element for imagesLoaded "+(s||t))}function r(t){this.img=t}function s(t,e){this.url=t,this.element=e,this.img=new Image}var l=t.jQuery,a=t.console,h=Array.prototype.slice;o.prototype=Object.create(e.prototype),o.prototype.options={},o.prototype.getImages=function(){this.images=[],this.elements.forEach(this.addElementImages,this)},o.prototype.addElementImages=function(t){"IMG"==t.nodeName&&this.addImage(t),this.options.background===!0&&this.addElementBackgroundImages(t);var e=t.nodeType;if(e&&c[e]){for(var i=t.querySelectorAll("img"),n=0;n<i.length;n++){var o=i[n];this.addImage(o)}if("string"==typeof this.options.background){var r=t.querySelectorAll(this.options.background);for(n=0;n<r.length;n++){var s=r[n];this.addElementBackgroundImages(s)}}}};var c={1:!0,9:!0,11:!0};return o.prototype.addElementBackgroundImages=function(t){var e=getComputedStyle(t);if(e)for(var i=/url\((['"])?(.*?)\1\)/gi,n=i.exec(e.backgroundImage);null!==n;){var o=n&&n[2];o&&this.addBackground(o,t),n=i.exec(e.backgroundImage)}},o.prototype.addImage=function(t){var e=new r(t);this.images.push(e)},o.prototype.addBackground=function(t,e){var i=new s(t,e);this.images.push(i)},o.prototype.check=function(){function t(t,i,n){setTimeout(function(){e.progress(t,i,n)})}var e=this;return this.progressedCount=0,this.hasAnyBroken=!1,this.images.length?void this.images.forEach(function(e){e.once("progress",t),e.check()}):void this.complete()},o.prototype.progress=function(t,e,i){this.progressedCount++,this.hasAnyBroken=this.hasAnyBroken||!t.isLoaded,this.emitEvent("progress",[this,t,e]),this.jqDeferred&&this.jqDeferred.notify&&this.jqDeferred.notify(this,t),this.progressedCount==this.images.length&&this.complete(),this.options.debug&&a&&a.log("progress: "+i,t,e)},o.prototype.complete=function(){var t=this.hasAnyBroken?"fail":"done";if(this.isComplete=!0,this.emitEvent(t,[this]),this.emitEvent("always",[this]),this.jqDeferred){var e=this.hasAnyBroken?"reject":"resolve";this.jqDeferred[e](this)}},r.prototype=Object.create(e.prototype),r.prototype.check=function(){var t=this.getIsImageComplete();return t?void this.confirm(0!==this.img.naturalWidth,"naturalWidth"):(this.proxyImage=new Image,this.proxyImage.addEventListener("load",this),this.proxyImage.addEventListener("error",this),this.img.addEventListener("load",this),this.img.addEventListener("error",this),void(this.proxyImage.src=this.img.src))},r.prototype.getIsImageComplete=function(){return this.img.complete&&this.img.naturalWidth},r.prototype.confirm=function(t,e){this.isLoaded=t,this.emitEvent("progress",[this,this.img,e])},r.prototype.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},r.prototype.onload=function(){this.confirm(!0,"onload"),this.unbindEvents()},r.prototype.onerror=function(){this.confirm(!1,"onerror"),this.unbindEvents()},r.prototype.unbindEvents=function(){this.proxyImage.removeEventListener("load",this),this.proxyImage.removeEventListener("error",this),this.img.removeEventListener("load",this),this.img.removeEventListener("error",this)},s.prototype=Object.create(r.prototype),s.prototype.check=function(){this.img.addEventListener("load",this),this.img.addEventListener("error",this),this.img.src=this.url;var t=this.getIsImageComplete();t&&(this.confirm(0!==this.img.naturalWidth,"naturalWidth"),this.unbindEvents())},s.prototype.unbindEvents=function(){this.img.removeEventListener("load",this),this.img.removeEventListener("error",this)},s.prototype.confirm=function(t,e){this.isLoaded=t,this.emitEvent("progress",[this,this.element,e])},o.makeJQueryPlugin=function(e){e=e||t.jQuery,e&&(l=e,l.fn.imagesLoaded=function(t,e){var i=new o(this,t,e);return i.jqDeferred.promise(l(this))})},o.makeJQueryPlugin(),o});
10 | 
11 | /* Custom settings for Infinite Scroll */
12 | document.addEventListener("DOMContentLoaded", function() {
13 |    const nextPage = document.querySelector('.pagination-section a');
14 |    if (nextPage) {
15 |       var infScroll = new InfiniteScroll('.loop-section', {
16 |          path: '.pagination-section a',
17 |          append: '.loop-wrap',
18 |          button: '.pagination-section button',
19 |          hideNav: '.pagination-section a',
20 |          history: false,
21 |          scrollThreshold: false
22 |       });
23 |       
24 |       infScroll.on('append', function(response, path, items) {
25 |          for (var i = 0; i < items.length; i++) {
26 |             reloadSrcsetImgs(items[i]);
27 |          }
28 |       });
29 | 
30 |       function reloadSrcsetImgs(item) {
31 |          var imgs = item.querySelectorAll('img[srcset]');
32 |          for (var i = 0; i < imgs.length; i++) {
33 |             var img = imgs[i];
34 |             img.outerHTML = img.outerHTML;
35 |          }
36 |       }
37 |    }
38 | });
```

assets/js/post.js
```
1 | /* Progress bar
2 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
3 |    Website : ghost.org
4 |    Repo    : github.com/tryghost
5 |    Author  : Ghost
6 |    License : MIT
7 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
8 | const readingProgress=(e,t)=>{const o=document.querySelector(e),n=document.querySelector(t),a=()=>{const e=o.getBoundingClientRect(),t=window.innerHeight/2;Math.round(n.max-n.value);e.top>t&&(n.value=0),e.top<t&&(n.value=n.max),e.top<=t&&e.bottom>=t&&(n.value=n.max*Math.abs(e.top-t)/e.height),window.addEventListener("scroll",a)};window.addEventListener("scroll",a)};
9 | 
10 | /* Custom settings for progress bar */
11 | !function(){const a=document.querySelector(".post-progress");a&&readingProgress(".post-content",".post-progress")}();
12 | 
13 | /* clipboard.js
14 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
15 |    Version : 2.0.8
16 |    Website : clipboardjs.com
17 |    Repo    : github.com/zenorocha/clipboard.js
18 |    Author  : Zeno Rocha
19 |    License : MIT
20 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
21 | !function(t,e){"object"==typeof exports&&"object"==typeof module?module.exports=e():"function"==typeof define&&define.amd?define([],e):"object"==typeof exports?exports.ClipboardJS=e():t.ClipboardJS=e()}(this,function(){return n={134:(t,e,n)=>{"use strict";n.d(e,{default:()=>r});var e=n(817),o=n.n(e);function i(t){return(i="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(t){return typeof t}:function(t){return t&&"function"==typeof Symbol&&t.constructor===Symbol&&t!==Symbol.prototype?"symbol":typeof t})(t)}function a(t,e){for(var n=0;n<e.length;n++){var r=e[n];r.enumerable=r.enumerable||!1,r.configurable=!0,"value"in r&&(r.writable=!0),Object.defineProperty(t,r.key,r)}}const c=function(){function e(t){!function(t){if(!(t instanceof e))throw new TypeError("Cannot call a class as a function")}(this),this.resolveOptions(t),this.initSelection()}var t,n,r;return t=e,(n=[{key:"resolveOptions",value:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:{};this.action=t.action,this.container=t.container,this.emitter=t.emitter,this.target=t.target,this.text=t.text,this.trigger=t.trigger,this.selectedText=""}},{key:"initSelection",value:function(){this.text?this.selectFake():this.target&&this.selectTarget()}},{key:"selectFake",value:function(){var t=this,e="rtl"==document.documentElement.getAttribute("dir");this.removeFake(),this.fakeHandlerCallback=function(){return t.removeFake()},this.fakeHandler=this.container.addEventListener("click",this.fakeHandlerCallback)||!0,this.fakeElem=document.createElement("textarea"),this.fakeElem.style.fontSize="12pt",this.fakeElem.style.border="0",this.fakeElem.style.padding="0",this.fakeElem.style.margin="0",this.fakeElem.style.position="absolute",this.fakeElem.style[e?"right":"left"]="-9999px";e=window.pageYOffset||document.documentElement.scrollTop;this.fakeElem.style.top="".concat(e,"px"),this.fakeElem.setAttribute("readonly",""),this.fakeElem.value=this.text,this.container.appendChild(this.fakeElem),this.selectedText=o()(this.fakeElem),this.copyText()}},{key:"removeFake",value:function(){this.fakeHandler&&(this.container.removeEventListener("click",this.fakeHandlerCallback),this.fakeHandler=null,this.fakeHandlerCallback=null),this.fakeElem&&(this.container.removeChild(this.fakeElem),this.fakeElem=null)}},{key:"selectTarget",value:function(){this.selectedText=o()(this.target),this.copyText()}},{key:"copyText",value:function(){var e;try{e=document.execCommand(this.action)}catch(t){e=!1}this.handleResult(e)}},{key:"handleResult",value:function(t){this.emitter.emit(t?"success":"error",{action:this.action,text:this.selectedText,trigger:this.trigger,clearSelection:this.clearSelection.bind(this)})}},{key:"clearSelection",value:function(){this.trigger&&this.trigger.focus(),document.activeElement.blur(),window.getSelection().removeAllRanges()}},{key:"destroy",value:function(){this.removeFake()}},{key:"action",set:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:"copy";if(this._action=t,"copy"!==this._action&&"cut"!==this._action)throw new Error('Invalid "action" value, use either "copy" or "cut"')},get:function(){return this._action}},{key:"target",set:function(t){if(void 0!==t){if(!t||"object"!==i(t)||1!==t.nodeType)throw new Error('Invalid "target" value, use a valid Element');if("copy"===this.action&&t.hasAttribute("disabled"))throw new Error('Invalid "target" attribute. Please use "readonly" instead of "disabled" attribute');if("cut"===this.action&&(t.hasAttribute("readonly")||t.hasAttribute("disabled")))throw new Error('Invalid "target" attribute. You can\'t cut text from elements with "readonly" or "disabled" attributes');this._target=t}},get:function(){return this._target}}])&&a(t.prototype,n),r&&a(t,r),e}();var e=n(279),l=n.n(e),e=n(370),u=n.n(e);function s(t){return(s="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(t){return typeof t}:function(t){return t&&"function"==typeof Symbol&&t.constructor===Symbol&&t!==Symbol.prototype?"symbol":typeof t})(t)}function f(t,e){for(var n=0;n<e.length;n++){var r=e[n];r.enumerable=r.enumerable||!1,r.configurable=!0,"value"in r&&(r.writable=!0),Object.defineProperty(t,r.key,r)}}function h(t,e){return(h=Object.setPrototypeOf||function(t,e){return t.__proto__=e,t})(t,e)}function d(n){var r=function(){if("undefined"==typeof Reflect||!Reflect.construct)return!1;if(Reflect.construct.sham)return!1;if("function"==typeof Proxy)return!0;try{return Date.prototype.toString.call(Reflect.construct(Date,[],function(){})),!0}catch(t){return!1}}();return function(){var t,e=p(n);return t=r?(t=p(this).constructor,Reflect.construct(e,arguments,t)):e.apply(this,arguments),e=this,!(t=t)||"object"!==s(t)&&"function"!=typeof t?function(t){if(void 0!==t)return t;throw new ReferenceError("this hasn't been initialised - super() hasn't been called")}(e):t}}function p(t){return(p=Object.setPrototypeOf?Object.getPrototypeOf:function(t){return t.__proto__||Object.getPrototypeOf(t)})(t)}function y(t,e){t="data-clipboard-".concat(t);if(e.hasAttribute(t))return e.getAttribute(t)}const r=function(){!function(t,e){if("function"!=typeof e&&null!==e)throw new TypeError("Super expression must either be null or a function");t.prototype=Object.create(e&&e.prototype,{constructor:{value:t,writable:!0,configurable:!0}}),e&&h(t,e)}(o,l());var t,e,n,r=d(o);function o(t,e){var n;return function(t){if(!(t instanceof o))throw new TypeError("Cannot call a class as a function")}(this),(n=r.call(this)).resolveOptions(e),n.listenClick(t),n}return t=o,n=[{key:"isSupported",value:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:["copy","cut"],t="string"==typeof t?[t]:t,e=!!document.queryCommandSupported;return t.forEach(function(t){e=e&&!!document.queryCommandSupported(t)}),e}}],(e=[{key:"resolveOptions",value:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:{};this.action="function"==typeof t.action?t.action:this.defaultAction,this.target="function"==typeof t.target?t.target:this.defaultTarget,this.text="function"==typeof t.text?t.text:this.defaultText,this.container="object"===s(t.container)?t.container:document.body}},{key:"listenClick",value:function(t){var e=this;this.listener=u()(t,"click",function(t){return e.onClick(t)})}},{key:"onClick",value:function(t){t=t.delegateTarget||t.currentTarget;this.clipboardAction&&(this.clipboardAction=null),this.clipboardAction=new c({action:this.action(t),target:this.target(t),text:this.text(t),container:this.container,trigger:t,emitter:this})}},{key:"defaultAction",value:function(t){return y("action",t)}},{key:"defaultTarget",value:function(t){t=y("target",t);if(t)return document.querySelector(t)}},{key:"defaultText",value:function(t){return y("text",t)}},{key:"destroy",value:function(){this.listener.destroy(),this.clipboardAction&&(this.clipboardAction.destroy(),this.clipboardAction=null)}}])&&f(t.prototype,e),n&&f(t,n),o}()},828:t=>{var e;"undefined"==typeof Element||Element.prototype.matches||((e=Element.prototype).matches=e.matchesSelector||e.mozMatchesSelector||e.msMatchesSelector||e.oMatchesSelector||e.webkitMatchesSelector),t.exports=function(t,e){for(;t&&9!==t.nodeType;){if("function"==typeof t.matches&&t.matches(e))return t;t=t.parentNode}}},438:(t,e,n)=>{var a=n(828);function i(t,e,n,r,o){var i=function(e,n,t,r){return function(t){t.delegateTarget=a(t.target,n),t.delegateTarget&&r.call(e,t)}}.apply(this,arguments);return t.addEventListener(n,i,o),{destroy:function(){t.removeEventListener(n,i,o)}}}t.exports=function(t,e,n,r,o){return"function"==typeof t.addEventListener?i.apply(null,arguments):"function"==typeof n?i.bind(null,document).apply(null,arguments):("string"==typeof t&&(t=document.querySelectorAll(t)),Array.prototype.map.call(t,function(t){return i(t,e,n,r,o)}))}},879:(t,n)=>{n.node=function(t){return void 0!==t&&t instanceof HTMLElement&&1===t.nodeType},n.nodeList=function(t){var e=Object.prototype.toString.call(t);return void 0!==t&&("[object NodeList]"===e||"[object HTMLCollection]"===e)&&"length"in t&&(0===t.length||n.node(t[0]))},n.string=function(t){return"string"==typeof t||t instanceof String},n.fn=function(t){return"[object Function]"===Object.prototype.toString.call(t)}},370:(t,e,n)=>{var u=n(879),s=n(438);t.exports=function(t,e,n){if(!t&&!e&&!n)throw new Error("Missing required arguments");if(!u.string(e))throw new TypeError("Second argument must be a String");if(!u.fn(n))throw new TypeError("Third argument must be a Function");if(u.node(t))return c=e,l=n,(a=t).addEventListener(c,l),{destroy:function(){a.removeEventListener(c,l)}};if(u.nodeList(t))return r=t,o=e,i=n,Array.prototype.forEach.call(r,function(t){t.addEventListener(o,i)}),{destroy:function(){Array.prototype.forEach.call(r,function(t){t.removeEventListener(o,i)})}};if(u.string(t))return t=t,e=e,n=n,s(document.body,t,e,n);throw new TypeError("First argument must be a String, HTMLElement, HTMLCollection, or NodeList");var r,o,i,a,c,l}},817:t=>{t.exports=function(t){var e,n="SELECT"===t.nodeName?(t.focus(),t.value):"INPUT"===t.nodeName||"TEXTAREA"===t.nodeName?((e=t.hasAttribute("readonly"))||t.setAttribute("readonly",""),t.select(),t.setSelectionRange(0,t.value.length),e||t.removeAttribute("readonly"),t.value):(t.hasAttribute("contenteditable")&&t.focus(),n=window.getSelection(),(e=document.createRange()).selectNodeContents(t),n.removeAllRanges(),n.addRange(e),n.toString());return n}},279:t=>{function e(){}e.prototype={on:function(t,e,n){var r=this.e||(this.e={});return(r[t]||(r[t]=[])).push({fn:e,ctx:n}),this},once:function(t,e,n){var r=this;function o(){r.off(t,o),e.apply(n,arguments)}return o._=e,this.on(t,o,n)},emit:function(t){for(var e=[].slice.call(arguments,1),n=((this.e||(this.e={}))[t]||[]).slice(),r=0,o=n.length;r<o;r++)n[r].fn.apply(n[r].ctx,e);return this},off:function(t,e){var n=this.e||(this.e={}),r=n[t],o=[];if(r&&e)for(var i=0,a=r.length;i<a;i++)r[i].fn!==e&&r[i].fn._!==e&&o.push(r[i]);return o.length?n[t]=o:delete n[t],this}},t.exports=e,t.exports.TinyEmitter=e}},o={},r.n=t=>{var e=t&&t.__esModule?()=>t.default:()=>t;return r.d(e,{a:e}),e},r.d=(t,e)=>{for(var n in e)r.o(e,n)&&!r.o(t,n)&&Object.defineProperty(t,n,{enumerable:!0,get:e[n]})},r.o=(t,e)=>Object.prototype.hasOwnProperty.call(t,e),r(134).default;function r(t){if(o[t])return o[t].exports;var e=o[t]={exports:{}};return n[t](e,e.exports,r),e.exports}var n,o});
22 | 
23 | /* Custom settings for clipboard */
24 | new ClipboardJS("#copy");
25 | 
26 | /* lightense-images
27 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
28 |    Version : 1.0.17
29 |    Website : sparanoid.com/work/lightense-images/
30 |    Repo    : github.com/sparanoid/lightense-images
31 |    Author  : Tunghsiao Liu
32 |    License : MIT
33 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
34 | !function(e,t){"object"==typeof exports&&"object"==typeof module?module.exports=t():"function"==typeof define&&define.amd?define([],t):"object"==typeof exports?exports.Lightense=t():e.Lightense=t()}(this,(function(){return e={352:e=>{function t(e,t){var n=Object.keys(e);if(Object.getOwnPropertySymbols){var r=Object.getOwnPropertySymbols(e);t&&(r=r.filter((function(t){return Object.getOwnPropertyDescriptor(e,t).enumerable}))),n.push.apply(n,r)}return n}function n(e){for(var n=1;n<arguments.length;n++){var i=null!=arguments[n]?arguments[n]:{};n%2?t(Object(i),!0).forEach((function(t){r(e,t,i[t])})):Object.getOwnPropertyDescriptors?Object.defineProperties(e,Object.getOwnPropertyDescriptors(i)):t(Object(i)).forEach((function(t){Object.defineProperty(e,t,Object.getOwnPropertyDescriptor(i,t))}))}return e}function r(e,t,n){return t in e?Object.defineProperty(e,t,{value:n,enumerable:!0,configurable:!0,writable:!0}):e[t]=n,e}function i(e){return(i="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(e){return typeof e}:function(e){return e&&"function"==typeof Symbol&&e.constructor===Symbol&&e!==Symbol.prototype?"symbol":typeof e})(e)}var o=function(){"use strict";var e,t={time:300,padding:40,offset:40,keyboard:!0,cubicBezier:"cubic-bezier(.2, 0, .1, 1)",background:"var(--bg-color-80, rgba(255, 255, 255, .98))",zIndex:1e6,beforeShow:void 0,afterShow:void 0,beforeHide:void 0,afterHide:void 0},r={};function o(e){var t=r[e];if(t){if("function"!=typeof t)throw"config.".concat(e," must be a function!");Reflect.apply(t,r,[r])}}function a(e){switch(i(e)){case"undefined":throw"You need to pass an element!";case"string":return document.querySelectorAll(e);case"object":return e}}function c(e){var t=e.length;if(t)for(var n=0;n<t;n++)s(e[n]);else s(e)}function s(e){e.src&&!e.classList.contains("lightense-target")&&(e.classList.add("lightense-target"),e.addEventListener("click",(function(i){if(r.keyboard&&(i.metaKey||i.ctrlKey))return window.open(e.src,"_blank");!function(e){if(r.target=e,r.target.classList.contains("lightense-open"))return g();o("beforeShow"),r.scrollY=window.scrollY,function(e,t,n){e.addEventListener(t,(function r(i){Reflect.apply(n,this,i),e.removeEventListener(t,r)}))}(r.target,"transitionend",(function(){o("afterShow")}));var i=new Image;i.onload=function(){!function(e){var n=e.width,i=e.height,o=window.pageYOffset||document.documentElement.scrollTop||0,a=window.pageXOffset||document.documentElement.scrollLeft||0,c=r.target.getBoundingClientRect(),s=n/c.width,d=window.innerWidth||document.documentElement.clientWidth||0,l=window.innerHeight||document.documentElement.clientHeight||0,u=r.target.getAttribute("data-lightense-padding")||r.target.getAttribute("data-padding")||r.padding,g=d>u?d-u:d-t.padding,p=l>u?l-u:l-t.padding,f=n/i,b=g/p;r.scaleFactor=n<g&&i<p?s:f<b?p/i*s:g/n*s;var h=d/2,m=o+l/2,v=c.left+a+c.width/2,y=c.top+o+c.height/2;r.translateX=Math.round(h-v),r.translateY=Math.round(m-y)}(this),function(){r.target.classList.add("lightense-open"),r.wrap=document.createElement("div"),r.wrap.className="lightense-wrap",setTimeout((function(){r.target.style.transform="scale("+r.scaleFactor+")"}),20),r.target.parentNode.insertBefore(r.wrap,r.target),r.wrap.appendChild(r.target),setTimeout((function(){r.wrap.style.transform="translate3d("+r.translateX+"px, "+r.translateY+"px, 0)"}),20);var e={cubicBezier:r.target.getAttribute("data-lightense-cubic-bezier")||r.cubicBezier,background:r.target.getAttribute("data-lightense-background")||r.target.getAttribute("data-background")||r.background,zIndex:r.target.getAttribute("data-lightense-z-index")||r.zIndex},t=n(n({},r),e);d("lightense-images-css-computed","\n    :root {\n      --lightense-z-index: ".concat(t.zIndex-1,";\n      --lightense-backdrop: ").concat(t.background,";\n      --lightense-duration: ").concat(t.time,"ms;\n      --lightense-timing-func: ").concat(t.cubicBezier,";\n    }")),r.container.style.visibility="visible",setTimeout((function(){r.container.style.opacity="1"}),20)}(),window.addEventListener("keyup",f,!1),window.addEventListener("scroll",p,!1),r.container.addEventListener("click",g,!1)},i.src=r.target.src}(this)}),!1))}function d(e,t){var n=document.head||document.getElementsByTagName("head")[0];document.getElementById(e)&&document.getElementById(e).remove();var r=document.createElement("style");r.id=e,r.styleSheet?r.styleSheet.cssText=t:r.appendChild(document.createTextNode(t)),n.appendChild(r)}function l(){d("lightense-images-css","\n:root {\n  --lightense-z-index: ".concat(r.zIndex-1,";\n  --lightense-backdrop: ").concat(r.background,";\n  --lightense-duration: ").concat(r.time,"ms;\n  --lightense-timing-func: ").concat(r.cubicBezier,";\n}\n\n.lightense-backdrop {\n  box-sizing: border-box;\n  width: 100%;\n  height: 100%;\n  position: fixed;\n  top: 0;\n  left: 0;\n  overflow: hidden;\n  z-index: calc(var(--lightense-z-index) - 1);\n  padding: 0;\n  margin: 0;\n  transition: opacity var(--lightense-duration) ease;\n  cursor: zoom-out;\n  opacity: 0;\n  background-color: var(--lightense-backdrop);\n  visibility: hidden;\n}\n\n@supports (-webkit-backdrop-filter: blur(30px)) {\n  .lightense-backdrop {\n    background-color: var(--lightense-backdrop);\n    -webkit-backdrop-filter: blur(30px);\n  }\n}\n\n@supports (backdrop-filter: blur(30px)) {\n  .lightense-backdrop {\n    background-color: var(--lightense-backdrop);\n    backdrop-filter: blur(30px);\n  }\n}\n\n.lightense-wrap {\n  position: relative;\n  transition: transform var(--lightense-duration) var(--lightense-timing-func);\n  z-index: var(--lightense-z-index);\n  pointer-events: none;\n}\n\n.lightense-target {\n  cursor: zoom-in;\n  transition: transform var(--lightense-duration) var(--lightense-timing-func);\n  pointer-events: auto;\n}\n\n.lightense-open {\n  cursor: zoom-out;\n}\n\n.lightense-transitioning {\n  pointer-events: none;\n}"))}function u(){null===document.querySelector(".lightense-backdrop")?(r.container=document.createElement("div"),r.container.className="lightense-backdrop",document.body.appendChild(r.container)):r.container=document.querySelector(".lightense-backdrop")}function g(){o("beforeHide"),window.removeEventListener("keyup",f,!1),window.removeEventListener("scroll",p,!1),r.container.removeEventListener("click",g,!1),r.target.classList.remove("lightense-open"),r.wrap.style.transform="",r.target.style.transform="",r.target.classList.add("lightense-transitioning"),r.container.style.opacity="",setTimeout((function(){o("afterHide"),r.container.style.visibility="",r.container.style.backgroundColor="",r.wrap.parentNode.replaceChild(r.target,r.wrap),r.target.classList.remove("lightense-transitioning")}),r.time)}function p(){Math.abs(r.scrollY-window.scrollY)>=r.offset&&g()}function f(e){e.preventDefault(),27===e.keyCode&&g()}return function(i){var o=arguments.length>1&&void 0!==arguments[1]?arguments[1]:{};e=a(i),r=n(n({},t),o),l(),u(),c(e)}}();e.exports=o}},t={},function n(r){var i=t[r];if(void 0!==i)return i.exports;var o=t[r]={exports:{}};return e[r](o,o.exports,n),o.exports}(352);var e,t}));
35 | 
36 | /* Custom settings for lightense-images */
37 | window.addEventListener("load",function(){const e=document.querySelector(".post-content .kg-card img"),t=document.querySelectorAll(".post-content .kg-image-card a img");if(t)for(var n=0;n<t.length;n++)t[n].classList.add("no-lightense");e&&Lightense(".post-content .kg-image-card img:not(.no-lightense),.post-content .kg-gallery-card img:not(.no-lightense)",{padding:60,offset:0})},!1);
38 | 
39 | /* reframe.js
40 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– 
41 |    Version : 2.2.6
42 |    Website : dollarshaveclub.github.io/reframe.js
43 |    Repo    : github.com/yowainwright/reframe.js
44 |    Author  : Jeff Wainwright
45 |    License : MIT
46 |    –––––––––––––––––––––––––––––––––––––––––––––––––––– */
47 | !function(e,t){"object"==typeof exports&&"undefined"!=typeof module?module.exports=t():"function"==typeof define&&define.amd?define(t):(e=e||self).reframe=t()}(this,function(){"use strict";return function(e,t){var i="string"==typeof e?document.querySelectorAll(e):e,n=t||"js-reframe";"length"in i||(i=[i]);for(var o=0;o<i.length;o+=1){var r=i[o];if(!(-1!==r.className.split(" ").indexOf(n))){var f=r.getAttribute("height"),d=r.getAttribute("width");if(!(-1<d.indexOf("%")||-1<r.style.width.indexOf("%"))){var s=(f||r.offsetHeight)/(d||r.offsetWidth)*100,a=document.createElement("div");a.className=n;var l=a.style;l.position="relative",l.width="100%",l.paddingTop=s+"%";var p=r.style;p.position="absolute",p.width="100%",p.height="100%",p.left="0",p.top="0",r.parentNode.insertBefore(a,r),r.parentNode.removeChild(r),a.appendChild(r)}}}}});
48 | 
49 | /* Custom settings for reframe.js */
50 | reframe('.post-content iframe:not(.reframe-off)');
```

author.hbs
```
1 | {{!< default}}
2 | {{#author}}
3 | {{#contentFor "cover_image"}}
4 | {{#if cover_image}}
5 | <div class="global-cover" style="background-image:url({{{img_url cover_image size="xl" format="webp"}}})"></div>
6 | {{else if @site.cover_image}}
7 | <div class="global-cover" style="background-image:url({{{img_url @site.cover_image size="xl" format="webp"}}})"></div>
8 | {{/if}}
9 | {{/contentFor}}
10 | {{>posts/header archive_page=true is_custom=true title=name custom_excerpt=bio custom_image=profile_image}}
11 | {{/author}}
12 | {{>loop is_archive=true}}
13 | {{pagination}}
```

custom-account.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{#if @member.paid}}
4 | <div class="account-section global-padding">
5 | 	<div class="post-header">
6 | 		<div class="post-header-wrap global-padding is-center is-archive-image">
7 | 			<div class="post-header-content">
8 | 				<div class="archive-image global-image global-dynamic-color is-account">
9 | 					{{>icons/site/user}}
10 | 					{{#if @member.avatar_image}}
11 | 					<img src="{{@member.avatar_image}}">
12 | 					{{/if}}
13 | 				</div>
14 | 				<h1 class="post-title global-title">{{#if @member.name}}{{@member.name}}{{else}}{{t "Your account"}}{{/if}}</h1>
15 | 				<p class="post-excerpt global-excerpt">
16 | 					{{#if custom_excerpt}}
17 | 					{{custom_excerpt}}
18 | 					{{else}}
19 | 					{{t "Nice, you’re a paying subscriber! You’ve an active account with access to all posts."}}
20 | 					{{/if}}
21 | 				</p>
22 | 			</div>
23 | 		</div>
24 | 	</div>
25 | 	{{#foreach @member.subscriptions}}
26 | 	<div class="account-details">
27 | 		<small class="global-subtitle">{{t "Account details"}}</small>
28 | 		<div class="account-details-wrap global-radius">
29 | 			<div class="account-details-content">
30 | 				<div class="account-detail-column">
31 | 					<div>
32 | 						<label class="account-detail-heading">{{t "Email address"}}</label>
33 | 						<span class="account-detail-content">{{@member.email}}</span>
34 | 					</div>
35 | 					<div>
36 | 						<label class="account-detail-heading">{{t "Your plan"}}</label>
37 | 						<span class="account-detail-content">{{tier.name}} — {{price plan}}/{{plan.interval}}</span>
38 | 					</div>
39 | 				</div>
40 | 				<div class="account-detail-column">
41 | 					<div>
42 | 						<label class="account-detail-heading">{{t "Card"}}</label>
43 | 						<span class="account-detail-content">**** **** **** {{default_payment_card_last4}}</span>
44 | 					</div>
45 | 					<div>
46 | 						<label class="account-detail-heading">
47 | 							{{#if cancel_at_period_end}}
48 | 							{{t "Expires"}}
49 | 							{{else}}
50 | 							{{t "Next bill date"}}
51 | 							{{/if}}
52 | 						</label>
53 | 						<span class="account-detail-content">{{date current_period_end format="DD MMM YYYY"}}</span>
54 | 					</div>
55 | 				</div>
56 | 				{{#if cancel_at_period_end}}
57 | 				<small class="account-alert-expired">
58 | 				{{t "Your subscription will expire on"}} — {{date current_period_end format="DD MMMM YYYY"}}. {{t "If you change your mind in the meantime you can turn auto-renew back on to continue your subscription."}}
59 | 				</small>
60 | 				{{/if}}
61 | 				<div class="account-signout-wrap">
62 | 					<span class="global-button" data-members-signout>{{t "Sign out"}}</span>
63 | 				</div>
64 | 			</div>
65 | 		</div>
66 | 		<div class="account-buttons">
67 | 			<a href="javascript:" class="account-button" data-portal="account">{{t "Account settings"}}</a>
68 | 			{{cancel_link class="account-button" errorClass="cancel-error global-alert" cancelLabel=(t "Cancel subscription") continueLabel=(t "Continue subscription")}}
69 | 		</div>
70 | 	</div>
71 | 	{{/foreach}}
72 | </div>
73 | {{#get "posts" limit="5" filter="visibility:[members,paid,tiers]" include="authors" as |special_posts|}}
74 | 	{{#if special_posts}}
75 | 		{{>related label=(t "The latest posts only for subscribers")}}
76 | 	{{/if}}
77 | {{/get}}
78 | {{else if @member}}
79 | <div class="account-section global-padding">
80 | 	<div class="post-header">
81 | 		<div class="post-header-wrap global-padding is-center is-archive-image">
82 | 			<div class="post-header-content">
83 | 				<div class="archive-image global-image global-dynamic-color is-account">
84 | 					{{>icons/site/user}}
85 | 					{{#if @member.avatar_image}}
86 | 					<img src="{{@member.avatar_image}}">
87 | 					{{/if}}
88 | 				</div>
89 | 				<h1 class="post-title global-title">{{#if @member.name}}{{@member.name}}{{else}}{{t "Your account"}}{{/if}}</h1>
90 | 				<p class="post-excerpt global-excerpt">
91 | 					{{#if custom_excerpt}}
92 | 					{{custom_excerpt}}
93 | 					{{else}}
94 | 					{{#if @site.paid_members_enabled}}
95 | 					{{t "Currently, you’re not a paying subscriber. You’ve an active account with access to posts for subscribers only."}}
96 | 					{{else}}
97 | 					{{t "You’ve an active account with access to posts for subscribers."}}
98 | 					{{/if}}
99 | 					{{/if}}
100 | 				</p>
101 | 			</div>
102 | 		</div>
103 | 	</div>
104 | 	<div class="account-details">
105 | 		<small class="global-subtitle">{{t "Account details"}}</small>
106 | 		<div class="account-details-wrap global-radius">
107 | 			<div class="account-details-content">
108 | 				<div class="account-detail-column">
109 | 					<div>
110 | 						<label class="account-detail-heading">{{t "Email address"}}</label>
111 | 						<span class="account-detail-content">{{@member.email}}</span>
112 | 					</div>
113 | 				</div>
114 | 				{{#if @site.paid_members_enabled}}
115 | 				<div class="account-detail-column">
116 | 					<div>
117 | 						<label class="account-detail-heading">{{t "Your plan"}}</label>
118 | 						<span class="account-detail-content">{{t "Free"}}</span>
119 | 					</div>
120 | 				</div>
121 | 				{{/if}}
122 | 				<div class="account-signout-wrap">
123 | 					<span class="global-button" data-members-signout>{{t "Sign out"}}</span>
124 | 				</div>
125 | 			</div>
126 | 		</div>
127 | 		<div class="account-buttons">
128 | 			<a href="javascript:" class="account-button" data-portal="account">{{t "Account settings"}}</a>
129 | 		</div>
130 | 	</div>
131 | </div>
132 | {{#if @site.paid_members_enabled}}
133 | 	{{>members/tiers}}
134 | {{/if}}
135 | {{#get "posts" limit="5" filter="visibility:[members,paid,tiers]" include="authors" as |special_posts|}}
136 | 	{{#if special_posts}}
137 | 		{{>related label=(t "The latest posts only for subscribers")}}
138 | 	{{/if}}
139 | {{/get}}
140 | {{else}}
141 | {{#contentFor "script_js"}}
142 | <script>window.addEventListener("load",function(){window.location='{{@site.url}}'})</script>
143 | {{/contentFor}}
144 | {{/if}}
145 | {{/post}}
```

custom-authors.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{#match @page.show_title_and_feature_image}}
4 | {{>posts/header is_custom=true}}
5 | {{/match}}
6 | <div class="custom-archive global-padding">
7 | 	<small class="global-subtitle">{{t "Meet our authors"}}</small>
8 | 	{{#get "authors" limit="all" include="count.posts" order="count.posts desc" as |authors|}}
9 | 	{{#if authors}}
10 | 	<div class="loop-wrap is-authors">
11 | 		{{#foreach authors}}
12 | 		{{#if count.posts}}
13 | 		<div class="custom-archive-item item">
14 | 			{{#if profile_image}}
15 | 			<a href="{{url}}" class="item-image global-image global-image-orientation global-radius is-portrait">
16 | 				{{>images/archive_image archive_image=profile_image}}
17 | 			</a>
18 | 			{{/if}}
19 | 			<div class="item-content">
20 | 				<h2 class="item-title"><a href="{{url}}">{{name}}</a></h2>
21 | 				<small>{{#if location}}{{t "from"}} {{location}} ∙ {{/if}}{{plural count.posts empty=(t "No posts") singular=(t "1 post") plural=(t "% posts")}}</small>
22 | 				{{#if bio}}<p class="item-excerpt global-excerpt is-authors">{{bio}}</p>
23 | 				{{/if}}
24 | 			</div>
25 | 		</div>
26 | 		{{/if}}
27 | 		{{/foreach}}
28 | 	</div>
29 | 	{{/if}}
30 | 	{{/get}}
31 | </div>
32 | {{/post}}
```

custom-contact.hbs
```
1 | {{!< default-custom}}
2 | {{#post}}
3 | <div class="custom-wrap">
4 | 	<div class="custom-container">
5 | 		<div class="custom-logo-wrap">
6 | 			<div class="custom-logo global-logo is-header">{{>logo}}</div>
7 | 		</div>
8 | 		<div class="custom-content">
9 | 			<form method="POST" action="{{@custom.contact_form_endpoint}}">
10 | 				<h1 class="custom-title">{{title}}</h1>
11 | 				<input type="text" name="name" placeholder="{{t "Your name"}}" aria-label="{{t "Your name"}}" required>
12 | 				<input type="email" name="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
13 | 				<textarea name="message" placeholder="{{t "Your message"}}" aria-label="{{t "Your message"}}" required></textarea>
14 | 				<button class="global-button" type="submit">{{t "Send message"}}</button>
15 | 			</form>
16 | 		</div>
17 | 	</div>
18 | 	{{#if feature_image}}
19 | 	<div class="custom-image global-bg-image" style="background-image: url({{feature_image}})"></div>
20 | 	{{/if}}
21 | </div>
22 | {{/post}}
```

custom-featured.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{#match @page.show_title_and_feature_image}}
4 | {{>posts/header featured_page=true is_custom=true}}
5 | {{/match}}
6 | {{#get "posts" limit="all" filter="featured:true" include="authors,tags,tiers" as |featured|}}
7 | 	{{#if featured}}
8 | 		{{>loop is_archive=true is_featured=true label=false}}
9 | 	{{/if}}
10 | {{/get}}
11 | {{/post}}
```

custom-membership.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{#match @page.show_title_and_feature_image}}
4 | {{>posts/header membership_page=true is_custom=true}}
5 | {{/match}}
6 | {{>members/tiers membership_page=true}}
7 | {{#if html}}
8 | <div class="faq-section global-padding">
9 | 	<div class="faq-wrap">
10 | 		<h2 class="faq-title global-title">{{t "FAQs"}}</h2>
11 | 		<div class="faq-content">
12 | 			{{content}}
13 | 		</div>
14 | 	</div>
15 | </div>
16 | {{/if}}
17 | {{#get "posts" limit="5" filter="visibility:[members,paid,tiers]" include="authors" as |special_posts|}}
18 | 	{{#if special_posts}}
19 | 		{{>related label=(t "The latest posts only for subscribers")}}
20 | 	{{/if}}
21 | {{/get}}
22 | {{/post}}
```

custom-sign-in.hbs
```
1 | {{!< default-custom}}
2 | {{#post}}
3 | <div class="custom-wrap">
4 | 	<div class="custom-container">
5 | 		<div class="custom-logo-wrap">
6 | 			<div class="custom-logo global-logo is-header">{{>logo}}</div>
7 | 		</div>
8 | 		<div class="custom-content">
9 | 			<form data-members-form="signin" data-members-autoredirect="false">
10 | 				<h1 class="custom-title">{{title}}</h1>
11 | 				<input data-members-email type="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
12 | 				<button class="global-button" type="submit">{{t "Send login link"}}</button>
13 | 				<div>
14 | 					<small class="alert-loading global-alert">{{t "Processing your application"}}</small>
15 | 					<small class="alert-error global-alert">{{t "There was an error sending the email"}}</small>
16 | 				</div>
17 | 				<small class="global-question"><span>{{t "Don’t have an account yet?"}}</span> <a href="{{@site.url}}/signup/">{{t "Sign up"}}</a></small>
18 | 			</form>
19 | 			<div class="alert-success">
20 | 				<h2 class="global-title">{{t "Great!"}}</h2>
21 | 				<p>{{t "Please check your inbox and click the link to complete signin."}}</p>
22 | 				<a href="{{@site.url}}" class="global-button">{{t "Back to homepage"}}</a>
23 | 			</div>
24 | 		</div>
25 | 	</div>
26 | 	{{#if feature_image}}
27 | 	<div class="custom-image global-bg-image" style="background-image: url({{feature_image}})"></div>
28 | 	{{/if}}
29 | </div>
30 | {{/post}}
```

custom-sign-up.hbs
```
1 | {{!< default-custom}}
2 | {{#post}}
3 | <div class="custom-wrap">
4 | 	<div class="custom-container">
5 | 		<div class="custom-logo-wrap">
6 | 			<div class="custom-logo global-logo is-header">{{>logo}}</div>
7 | 		</div>
8 | 		<div class="custom-content">
9 | 			<form data-members-form="signup" data-members-autoredirect="false">
10 | 				<h1 class="custom-title">{{title}}</h1>
11 | 				{{#if @site.portal_name}}
12 | 				<input data-members-name type="text" placeholder="{{t "Your name"}}" aria-label="{{t "Your name"}}" required>
13 | 				{{/if}}
14 | 				<input data-members-email type="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
15 | 				<button class="global-button" type="submit">{{t "Continue"}}</button>
16 | 				<div>
17 | 					<small class="alert-loading global-alert">{{t "Processing your application"}}</small>
18 | 					<small class="alert-error global-alert">{{t "There was an error sending the email"}}</small>
19 | 				</div>
20 | 				<small class="global-question"><span>{{t "Already have an account?"}}</span> <a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></small>
21 | 			</form>
22 | 			<div class="alert-success">
23 | 				<h2 class="global-title">{{t "Great!"}}</h2>
24 | 				<p>{{t "Please check your inbox and click the link to confirm your signup."}}</p>
25 | 				<a href="{{@site.url}}" class="global-button">{{t "Back to homepage"}}</a>
26 | 			</div>
27 | 		</div>
28 | 	</div>
29 | 	{{#if feature_image}}
30 | 	<div class="custom-image global-bg-image" style="background-image: url({{feature_image}})"></div>
31 | 	{{/if}}
32 | </div>
33 | {{/post}}
```

custom-subscribe.hbs
```
1 | {{!< default-custom}}
2 | {{#post}}
3 | <div class="custom-wrap">
4 | 	<div class="custom-container">
5 | 		<div class="custom-logo-wrap">
6 | 			<div class="custom-logo global-logo is-header">{{>logo}}</div>
7 | 		</div>
8 | 		<div class="custom-content">
9 | 			<form data-members-form="subscribe" data-members-autoredirect="false">
10 | 				<h1 class="custom-title">{{title}}</h1>
11 | 				{{#if @site.portal_name}}
12 | 				<input data-members-name type="text" placeholder="{{t "Your name"}}" aria-label="{{t "Your name"}}" required>
13 | 				{{/if}}
14 | 				<input data-members-email type="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
15 | 				<button class="global-button" type="submit">{{t "Subscribe"}}</button>
16 | 				<div>
17 | 					<small class="alert-loading global-alert">{{t "Processing your application"}}</small>
18 | 					<small class="alert-error global-alert">{{t "There was an error sending the email"}}</small>
19 | 				</div>
20 | 			</form>
21 | 			<div class="alert-success">
22 | 				<h2 class="global-title">{{t "Great!"}}</h2>
23 | 				<p>{{t "Please check your inbox and click the link to confirm your subscription."}}</p>
24 | 				<a href="{{@site.url}}" class="global-button">{{t "Back to homepage"}}</a>
25 | 			</div>
26 | 		</div>
27 | 	</div>
28 | 	{{#if feature_image}}
29 | 	<div class="custom-image global-bg-image" style="background-image: url({{feature_image}})"></div>
30 | 	{{/if}}
31 | </div>
32 | {{/post}}
```

custom-tags.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{#match @page.show_title_and_feature_image}}
4 | {{>posts/header is_custom=true}}
5 | {{/match}}
6 | <div class="custom-archive global-padding">
7 | 	<small class="global-subtitle">{{t "Explore tags"}}</small>
8 | 	{{#get "tags" limit="all" filter="visibility:public+slug:-rough-notes" include="count.posts" order="count.posts desc" as |tags|}}
9 | 	{{#if tags}}
10 | 	<div class="loop-wrap is-tags">
11 | 		{{#foreach tags}}
12 | 		{{#if count.posts}}
13 | 		<div class="custom-archive-item item">
14 | 			{{#if feature_image}}
15 | 			<a href="{{url}}" class="item-image global-image global-image-orientation global-radius">
16 | 				{{>images/archive_image archive_image=feature_image}}
17 | 			</a>
18 | 			{{/if}}
19 | 			<div class="item-content">
20 | 				<h2 class="item-title"><a href="{{url}}">{{name}}</a></h2>
21 | 				<small>{{plural count.posts empty=(t "No posts") singular=(t "1 post") plural=(t "% posts")}}</small>
22 | 				{{^if feature_image}}
23 | 				{{#if description}}<p class="item-excerpt global-excerpt">{{description}}</p>{{/if}}
24 | 				{{/if}}
25 | 			</div>
26 | 		</div>
27 | 		{{/if}}
28 | 		{{/foreach}}
29 | 	</div>
30 | 	{{/if}}
31 | 	{{/get}}
32 | </div>
33 | {{/post}}
```

default-custom.hbs
```
1 | <!DOCTYPE html>
2 | <html lang="{{@site.locale}}"{{#match @custom.color_scheme "Dark"}} class="dark-mode"{{/match}}{{#match @custom.color_scheme "Sepia"}} class="sepia-mode"{{/match}}{{#match @custom.color_scheme "Auto: Light/Dark"}} class="auto-dark-mode"{{/match}}{{#match @custom.color_scheme "Auto: Sepia/Dark"}} class="sepia-mode auto-dark-mode"{{/match}}>
3 | 	<head>
4 | 		<meta charset="utf-8">
5 | 		<meta http-equiv="X-UA-Compatible" content="IE=edge">
6 | 		<title>{{@site.title}} — {{meta_title}}</title>
7 | 		<meta name="HandheldFriendly" content="True">
8 | 		<meta name="viewport" content="width=device-width, initial-scale=1">
9 | 		{{>services/google_fonts}}
10 | 		<link rel="stylesheet" type="text/css" href="{{asset "css/screen.css"}}">
11 | 		{{{block "fonts_css"}}}
12 | 		<script>
13 | 		/* getContrast.js
14 | 		––––––––––––––––––––––––––––––––––––––––––––––––––––
15 | 		Website : vanillajstoolkit.com/helpers/getcontrast/
16 | 		Authors : Chris Ferdinandi & Brian Suda
17 | 		License : MIT
18 | 		–––––––––––––––––––––––––––––––––––––––––––––––––––– */
19 | 		function getContrast(t){"use strict";return"#"===t.slice(0,1)&&(t=t.slice(1)),3===t.length&&(t=t.split("").map(function(t){return t+t}).join("")),(299*parseInt(t.substr(0,2),16)+587*parseInt(t.substr(2,2),16)+114*parseInt(t.substr(4,2),16))/1000>=128?"no-white-text":"is-white-text"}{{#contentFor "get_contrast_js"}}<script>!function(){"use strict";const t=document.body,o=getComputedStyle(t).getPropertyValue("--ghost-accent-color").trim();o&&t.classList.add(getContrast(o))}();</script>{{/contentFor}}
20 | 		</script>
21 | 		{{ghost_head}}
22 | 	</head>
23 | 	<body class="{{body_class}} custom-page">
24 | 		{{{block "get_contrast_js"}}}
25 | 		{{{body}}}
26 | 		{{ghost_foot}}
27 | 	</body>
28 | </html>
```

default.hbs
```
1 | <!DOCTYPE html>
2 | <html lang="{{@site.locale}}"{{#match @custom.color_scheme "Dark"}} class="dark-mode"{{/match}}{{#match @custom.color_scheme "Sepia"}} class="sepia-mode"{{/match}}{{#match @custom.color_scheme "Auto: Light/Dark"}} class="auto-dark-mode"{{/match}}{{#match @custom.color_scheme "Auto: Sepia/Dark"}} class="sepia-mode auto-dark-mode"{{/match}}>
3 | 	<head>
4 | 		<meta charset="utf-8">
5 | 		<meta http-equiv="X-UA-Compatible" content="IE=edge">
6 | 		<title>{{meta_title page=(t "meta-page")}}</title>
7 | 		<meta name="HandheldFriendly" content="True">
8 | 		<meta name="viewport" content="width=device-width, initial-scale=1">
9 | 		{{>services/google_fonts}}
10 | 		<link href="https://fonts.cdnfonts.com/css/canela-text-trial" rel="stylesheet">
11 | 		<link rel="stylesheet" type="text/css" href="{{asset "css/screen.css"}}">
12 | 		{{{block "fonts_css"}}}
13 | 		<script>
14 | 		/* getContrast.js
15 | 		––––––––––––––––––––––––––––––––––––––––––––––––––––
16 | 		Website : vanillajstoolkit.com/helpers/getcontrast/
17 | 		Authors : Chris Ferdinandi & Brian Suda
18 | 		License : MIT
19 | 		–––––––––––––––––––––––––––––––––––––––––––––––––––– */
20 | 		function getContrast(t){"use strict";return"#"===t.slice(0,1)&&(t=t.slice(1)),3===t.length&&(t=t.split("").map(function(t){return t+t}).join("")),(299*parseInt(t.substr(0,2),16)+587*parseInt(t.substr(2,2),16)+114*parseInt(t.substr(4,2),16))/1000>=128?"no-white-text":"is-white-text"}{{#contentFor "get_contrast_js"}}<script>!function(){"use strict";const t=document.body,o=getComputedStyle(t).getPropertyValue("--ghost-accent-color").trim();o&&t.classList.add(getContrast(o))}();</script>{{/contentFor}}
21 | 		</script>
22 | 		{{ghost_head}}
23 | 	</head>
24 | 	<body class="{{body_class}}">
25 | 		{{{block "get_contrast_js"}}}
26 | 		<div class="global-wrap">
27 | 			{{>images/background_cover custom_cover=@site.cover_image}}
28 | 			<div class="global-content">
29 | 				{{>header}}
30 | 				<main class="global-main">
31 | 					{{{body}}}
32 | 				</main>
33 | 				{{>footer}}
34 | 			</div>
35 | 		</div>
36 | 		{{>members/notifications}}
37 | 		{{>search is_search_core=true}}
38 | 		<script src="{{asset "js/global.js"}}"></script>
39 | 		{{#if pagination.pages}}
40 | 		<script src="{{asset "js/index.js"}}"></script>
41 | 		{{/if}}
42 | 		{{#is "post,page"}}
43 | 		<script src="{{asset "js/post.js"}}"></script>
44 | 		{{/is}}
45 | 		{{{block "script_js"}}}
46 | 		{{ghost_foot}}
47 | 	</body>
48 | </html>
```

error.hbs
```
1 | {{!< default}}
2 | <div class="custom-error custom-wrap">
3 | 	<div class="custom-container">
4 | 		<div class="custom-error-content custom-content">
5 | 			<h1>{{statusCode}}</h1>
6 | 			<p class="global-excerpt">{{message}}</p>
7 | 			<a href="{{@site.url}}" class="global-button">{{t "Back to homepage"}}</a>
8 | 		</div>
9 | 	</div>
10 | </div>
11 | {{#get "posts" limit="3" filter="feature_image:-null" include="authors,tags,tiers" as |special_posts|}}
12 | 	{{#if special_posts}}
13 | 		{{>loop is_archive=true label=(t "Check out the latest posts")}}
14 | 	{{/if}}
15 | {{/get}}
```

index.hbs
```
1 | {{!< default}}
2 | {{>hero}}
3 | {{>widgets}}
4 | {{>loop}}
5 | {{pagination}}
6 | {{>sections}}
```

locales/en.json
```
1 | {
2 |   "Column 1": "Links",
3 |   "Column 2": "Links",
4 |   "Column 3": "Links",
5 |   "Column 4": "Links",
6 |   "Column 5": "Links",
7 |   "{start-bold}Hey, we’re {site-title}.{end-bold}{new-line}See our thoughts, stories and ideas.": "{start-bold}Hey, we’re {site-title}.{end-bold}{new-line}See our thoughts, stories and ideas.",
8 |   "Popular tags": "Popular tags",
9 |   "Best authors": "Best authors",
10 |   "What’s new?": "What’s new?",
11 |   "Newsletter": "Newsletter",
12 |   "Thoughts on product, modern software and leadership, 3-4x /month.": "Thoughts on product, modern software and leadership, 3-4x /month.",
13 |   "Previous posts": "Previous posts",
14 |   "You might also like": "You might also like",
15 |   "Explore our tags": "Explore tags",
16 |   "Meet our authors": "Meet our authors",
17 |   "from": "from",
18 |   "No posts": "No posts",
19 |   "1 post": "1 post",
20 |   "% posts": "% posts",
21 |   "1 featured post": "1 featured post",
22 |   "% featured posts": "% featured posts",
23 |   "Social": "Social",
24 |   "Website": "Website",
25 |   "by": "by",
26 |   "Written by": "Written by",
27 |   "&": " & ",
28 |   "and": " and ",
29 |   "and others": "and others",
30 |   "1 minute read": "1 min read",
31 |   "% minutes read": "% min read",
32 |   "The link has been copied!": "The link has been copied!",
33 |   "Newer post": "Newer post",
34 |   "Older post": "Older post",
35 |   "Member discussion": "Member discussion",
36 |   "0 comments": "0 comments",
37 |   "comment": "comment",
38 |   "comments": "comments",
39 |   "Load more": "Load more",
40 |   "Featured posts": "Featured posts",
41 |   "Top picks": "Top picks",
42 |   "Opinionated, longform narrative writing with an agenda.": "Opinionated, longform narrative writing with an agenda.",
43 |   "A curated list of the most interesting thoughts, stories and ideas": "A curated list of the most interesting thoughts, stories and ideas",
44 |   "See all featured posts →": "See all featured posts →",
45 |   "Search": "Search",
46 |   "Please enter at least 3 characters": "Please enter at least 3 characters",
47 |   "{counter} results for your search": "{counter} results for your search",
48 |   "Click here to search for posts": "Click here to search for posts",
49 |   "Search posts, tags and authors": "Search posts, tags and authors",
50 |   "Members": "Members",
51 |   "Paid-members": "Paid-members",
52 |   "This post is for subscribers only": "This post is for subscribers only",
53 |   "This post is for paying subscribers only": "This post is for paying subscribers only",
54 |   "No tiers": "No tiers",
55 |   "This post is for subscribers with the tier:": "This post is for subscribers with the tier:",
56 |   "This post is for subscribers with any of the tiers:": "This post is for subscribers with any of the tiers:",
57 |   "or": " or ",
58 |   "Upgrade your account to get access to the post.": "Upgrade your account to get access to the post.",
59 |   "Sign up now and upgrade your account to get access to the post.": "Sign up now and upgrade your account to get access to the post.",
60 |   "Sign up now to read the post and get access to the full library of posts for subscribers only.": "Sign up now to read the post and get access to the full library of posts for subscribers only.",
61 |   "Upgrade your account to read the post and get access to the full library of posts for paying subscribers only.": "Upgrade your account to read the post and get access to the full library of posts for paying subscribers only.",
62 |   "Sign up now and upgrade your account to read the post and get access to the full library of posts for paying subscribers only.": "Sign up now and upgrade your account to read the post and get access to the full library of posts for paying subscribers only.",
63 |   "Sign in": "Sign in",
64 |   "Sign up": "Sign up",
65 |   "Sign up now": "Sign up now",
66 |   "Sign up for free": "Sign up for free",
67 |   "Start {trial}-day free trial": "Start {trial}-day free trial",
68 |   "Sign out": "Sign out",
69 |   "Account": "Account",
70 |   "See plans": "See plans",
71 |   "Become a subscriber": "Become a subscriber",
72 |   "Become a subscriber →": "Become a subscriber →",
73 |   "Continue": "Continue",
74 |   "Send login link": "Send login link",
75 |   "You’ve successfully subscribed to {site-title}": "You’ve successfully subscribed to {site-title}",
76 |   "Welcome back! You’ve successfully signed in.": "Welcome back! You’ve successfully signed in.",
77 |   "Success! Your email is updated.": "Success! Your email is updated.",
78 |   "Great!": "Great!",
79 |   "Great! You’ve successfully signed up.": "Great! You’ve successfully signed up.",
80 |   "Already have an account?": "Already have an account?",
81 |   "Don’t have an account yet?": "Don’t have an account yet?",
82 |   "Account details": "Account details",
83 |   "Account settings": "Account settings",
84 |   "Monthly": "Monthly",
85 |   "Yearly": "Yearly",
86 |   "month": "month",
87 |   "year": "year",
88 |   "$": "$",
89 |   "Email address": "Email address",
90 |   "Your account": "Your account",
91 |   "Your plan": "Your plan",
92 |   "Your name": "Your name",
93 |   "Your email": "Your email",
94 |   "Your message": "Your message",
95 |   "Send message": "Send message",
96 |   "Card": "Card",
97 |   "Free": "Free",
98 |   "Expires": "Expires",
99 |   "Next bill date": "Next bill date",
100 |   "Subscribe": "Subscribe",
101 |   "See pricing plans": "See pricing plans",
102 |   "FAQs": "FAQs",
103 |   "Check out the latest posts": "Check out the latest posts",
104 |   "The latest posts only for subscribers": "The latest posts only for subscribers",
105 |   "Cancel subscription": "Cancel subscription",
106 |   "Continue subscription": "Continue subscription",
107 |   "Your link has expired": "Your link has expired",
108 |   "Processing your application": "Processing your application",
109 |   "Please check your inbox and click the link to confirm your subscription.": "Please check your inbox and click the link to confirm your subscription.",
110 |   "Please check your inbox and click the link to complete signin.": "Please check your inbox and click the link to complete signin.",
111 |   "Please check your inbox and click the link to confirm your signup.": "Please check your inbox and click the link to confirm your signup.",
112 |   "There was an error sending the email": "There was an error sending the email",
113 |   "Success! Check your email for magic link to sign-in.": "Success! Check your email for magic link to sign-in.",
114 |   "Success! You now have access to additional content.": "Success! You now have access to additional content.",
115 |   "Unlock full access to {site-title} and see the entire library of subscribers-only content & updates": "Unlock full access to {site-title} and see the entire library of subscribers-only content & updates",
116 |   "You’ve an active account with access to posts for subscribers.": "You’ve an active account with access to posts for subscribers.",
117 |   "Nice, you’re a paying subscriber! You’ve an active account with access to all posts.": "Nice, you’re a paying subscriber! You’ve an active account with access to all posts.",
118 |   "Currently, you’re not a paying subscriber. You’ve an active account with access to posts for subscribers only.": "Currently, you’re not a paying subscriber. You’ve an active account with access to posts for subscribers only.",
119 |   "Your subscription will expire on": "Your subscription will expire on",
120 |   "If you change your mind in the meantime you can turn auto-renew back on to continue your subscription.": "If you change your mind in the meantime you can turn auto-renew back on to continue your subscription.",
121 |   "Back to homepage": "Back to homepage",
122 |   "meta-page": " (Page %)",
123 |   "Published with {ghost-link} and {theme-name}.": "Published with {ghost-link} and {theme-name}."
124 | }
```

package.json
```
1 | {
2 |   "name": "reiro",
3 |   "demo": "https://reiro.fueko.net",
4 |   "version": "1.4.0",
5 |   "docs": "https://fueko.net/docs/reiro/",
6 |   "author": {
7 |     "name": "fueko",
8 |     "email": "hello@fueko.net",
9 |     "url": "https://fueko.net"
10 |   },
11 |   "keywords": [
12 |     "ghost-theme",
13 |     "shreyas",
14 |     "indiehacking",
15 |     "indiemaking",
16 |     "modern-software",
17 |     "product"
18 |   ],
19 |   "config": {
20 |     "posts_per_page": 27,
21 |     "card_assets": true,
22 |     "image_sizes": {
23 |       "s": {
24 |         "width": 300
25 |       },
26 |       "m": {
27 |         "width": 600
28 |       },
29 |       "l": {
30 |         "width": 1200
31 |       },
32 |       "xl": {
33 |         "width": 1600
34 |       },
35 |       "xxl": {
36 |         "width": 2000
37 |       }
38 |     },
39 |     "custom": {
40 |       "color_scheme": {
41 |         "type": "select",
42 |         "options": [
43 |           "Light",
44 |           "Dark",
45 |           "Sepia",
46 |           "Auto: Light/Dark",
47 |           "Auto: Sepia/Dark"
48 |         ],
49 |         "default": "Light"
50 |       },
51 |       "logo_for_dark_version": {
52 |         "type": "image",
53 |         "visibility": "color_scheme:[Dark,'Auto: Light/Dark','Auto: Sepia/Dark']"
54 |       },
55 |       "fonts": {
56 |         "type": "select",
57 |         "options": [
58 |           "System fonts",
59 |           "Archivo + System fonts",
60 |           "Figtree + Inter",
61 |           "Fraunces + System fonts",
62 |           "IBM Plex Sans",
63 |           "Inter",
64 |           "Libre Franklin + System fonts",
65 |           "Livvic + System fonts",
66 |           "Lora + System fonts",
67 |           "Manrope + System fonts",
68 |           "Nunito",
69 |           "Nunito Sans",
70 |           "Oswald + Roboto",
71 |           "Playfair + System fonts",
72 |           "Poppins + Inter",
73 |           "Radio Canada + System fonts",
74 |           "Readex Pro + System fonts",
75 |           "Roboto",
76 |           "Space Grotesk + Inter",
77 |           "Source Serif Pro + Inter"
78 |         ],
79 |         "default": "Fraunces + System fonts"
80 |       },
81 |       "show_author": {
82 |         "type": "boolean",
83 |         "default": true,
84 |         "description": "Use if you don’t want to display the author in the feed and on the post page"
85 |       },
86 |       "slug_for_become_a_subscriber_button": {
87 |         "type": "text",
88 |         "default": "/signup/"
89 |       },
90 |       "content_api_key_for_search": {
91 |         "type": "text"
92 |       },
93 |       "contact_form_endpoint": {
94 |         "type": "text"
95 |       },
96 |       "footer_copyright": {
97 |         "type": "text"
98 |       },
99 |       "hero_title_text": {
100 |         "type": "text",
101 |         "group": "homepage"
102 |       },
103 |       "hero_options": {
104 |         "type": "select",
105 |         "options": [
106 |           "Subscribe form",
107 |           "Search box (Flat style)",
108 |           "Search box (Linear style)",
109 |           "Search box (Shadow style)",
110 |           "Disable"
111 |         ],
112 |         "default": "Disable",
113 |         "group": "homepage"
114 |       },
115 |       "style_for_featured_section": {
116 |         "type": "select",
117 |         "options": [
118 |           "Gray",
119 |           "Gray/Accent color",
120 |           "Accent color",
121 |           "Accent color/Gray",
122 |           "Disable"
123 |         ],
124 |         "default": "Gray/Accent color",
125 |         "group": "homepage"
126 |       },
127 |       "slug_for_see_all_featured_button": {
128 |         "type": "text",
129 |         "group": "homepage"
130 |       },
131 |       "widgets": {
132 |         "type": "select",
133 |         "options": [
134 |           "Popular tags",
135 |           "Best authors",
136 |           "Disable"
137 |         ],
138 |         "default": "Popular tags",
139 |         "group": "homepage"
140 |       },
141 |       "slugs_for_selected_tags_or_authors": {
142 |         "type": "text",
143 |         "group": "homepage"
144 |       },
145 |       "tags_for_special_section": {
146 |         "type": "text",
147 |         "group": "homepage",
148 |         "description": "Provide the tag (or tags) slug you want to display in the section below the 'Load more' button"
149 |       },
150 |       "feature_image_orientation": {
151 |         "type": "select",
152 |         "options": [
153 |           "Natural",
154 |           "Landscape",
155 |           "Panoramic",
156 |           "Natural wide",
157 |           "Landscape wide",
158 |           "Panoramic wide",
159 |           "Disable"
160 |         ],
161 |         "default": "Panoramic wide",
162 |         "group": "post"
163 |       },
164 |       "sidebar": {
165 |         "type": "select",
166 |         "options": [
167 |           "Without Subscription form",
168 |           "With Subscription form",
169 |           "With sticky Subscription form",
170 |           "Disable"
171 |         ],
172 |         "default": "With sticky Subscription form",
173 |         "group": "post"
174 |       }
175 |     }
176 |   }
177 | }
```

partials/featured.hbs
```
1 | {{^match @custom.style_for_featured_section "Disable"}}
2 | {{#if @custom.slug_for_see_all_featured_button}}
3 | {{#get "posts" limit="3" filter="featured:true" include="authors" as |featured|}}
4 | {{#if featured}}
5 | <small class="global-subtitle">{{t "Featured posts"}}</small>
6 | <div class="featured-section global-radius{{#match @custom.style_for_featured_section "Gray"}} is-gray{{else match @custom.style_for_featured_section "Accent color"}} global-dynamic-color is-accent{{else match @custom.style_for_featured_section "Accent color/Gray"}} is-accent-gray{{else match @custom.style_for_featured_section "Gray/Accent color"}} is-gray-accent{{/match}}">
7 | 	{{#foreach featured to="1"}}{{>images/background_cover custom_cover=feature_image is_featured=true}}{{/foreach}}
8 | 	<small class="featured-subtitle{{#match @custom.style_for_featured_section "Accent color/Gray"}} global-dynamic-color{{/match}}">{{t "Essays"}}</small>
9 | 	<h2 class="featured-title{{#match @custom.style_for_featured_section "Accent color/Gray"}} global-dynamic-color{{/match}}">{{t "Opinionated, longform narrative with an agenda"}}</h2>
10 | 	<div class="featured-content{{#foreach posts}}{{#if @last}} items-{{@number}}{{/if}}{{/foreach}}{{#match @custom.style_for_featured_section "Gray/Accent color"}} global-dynamic-color{{/match}}">
11 | 		{{#foreach featured}}
12 | 		{{>item show_excerpt=false is_featured=true}}
13 | 		{{/foreach}}
14 | 	</div>
15 | 	<div class="featured-button-wrap">
16 | 		<a href="{{@site.url}}{{@custom.slug_for_see_all_featured_button}}" class="featured-button{{#match @custom.style_for_featured_section "Accent color/Gray"}} global-dynamic-color{{/match}}">{{t "See all featured essays →"}}</a>
17 | 	</div>
18 | </div>
19 | {{/if}}
20 | {{/get}}
21 | {{else}}
22 | {{#get "posts" limit="6" filter="featured:true" include="authors" as |featured|}}
23 | {{#if featured}}
24 | <small class="global-subtitle">{{t "Featured posts"}}</small>
25 | <div class="featured-section global-radius{{#match @custom.style_for_featured_section "Gray"}} is-gray{{else match @custom.style_for_featured_section "Accent color"}} global-dynamic-color is-accent{{else match @custom.style_for_featured_section "Accent color/Gray"}} is-accent-gray{{else match @custom.style_for_featured_section "Gray/Accent color"}} is-gray-accent{{/match}}">
26 | 	{{#foreach featured to="1"}}{{>images/background_cover custom_cover=feature_image is_featured=true}}{{/foreach}}
27 | 	<small class="featured-subtitle{{#match @custom.style_for_featured_section "Accent color/Gray"}} global-dynamic-color{{/match}}">{{t "Top picks"}}</small>
28 | 	<h2 class="featured-title{{#match @custom.style_for_featured_section "Accent color/Gray"}} global-dynamic-color{{/match}}">{{t "Opinionated, longform narrative with an agenda"}}</h2>
29 | 	<div class="featured-content{{#foreach posts}}{{#if @last}} items-{{@number}}{{/if}}{{/foreach}}{{#match @custom.style_for_featured_section "Gray/Accent color"}} global-dynamic-color{{/match}}">
30 | 		{{#foreach featured}}
31 | 		{{>item show_excerpt=false is_featured=true}}
32 | 		{{/foreach}}
33 | 	</div>
34 | </div>
35 | {{/if}}
36 | {{/get}}
37 | {{/if}}
38 | {{/match}}
```

partials/footer.hbs
```
1 | <footer class="footer-section global-footer">
2 | 	{{>members/subscribe_form is_box=true is_footer=true}}
3 | 	<div class="footer-wrap global-padding">
4 | 		<div class="footer-content">
5 | 			<div class="footer-logo-wrap">
6 | 				<div class="global-logo is-footer">{{>logo}}</div>
7 | 				{{#if @site.description}}
8 | 				<p class="footer-description">{{@site.description}}</p>
9 | 				{{/if}}
10 | 			</div>
11 | 			{{>members/subscribe_form is_button=true}}
12 | 		</div>
13 | 		<div class="footer-nav">
14 | 			<div class="footer-nav-column is-social">
15 | 				<small>{{t "Social"}}</small>
16 | 				<ul>
17 | 					{{#if @site.facebook}}
18 | 					<li><a href="{{facebook_url}}" target="_blank" rel="noopener">{{>icons/social/facebook}}Facebook</a></li>
19 | 					{{/if}}
20 | 					{{#if @site.twitter}}
21 | 					<li><a href="{{twitter_url}}" target="_blank" rel="noopener">{{>icons/social/x}}X/Twitter</a></li>
22 | 					{{/if}}
23 | 					{{>footer_icons}}
24 | 				</ul>
25 | 			</div>
26 | 			{{#if @site.secondary_navigation}}
27 | 			{{navigation type="secondary"}}
28 | 			{{/if}}
29 | 		</div>
30 | 		<div class="footer-copyright">
31 | 			&copy; {{date format="YYYY"}} <a href="{{@site.url}}">{{@site.title}}</a>.
32 | 			{{#if @custom.footer_copyright}}
33 | 			{{{@custom.footer_copyright}}}
34 | 			{{else}}
35 | 			{{{t "Published with {ghost-link} and {theme-name}." ghost-link="<a href=\"https://ghost.org\" target=\"_blank\" rel=\"noopener noreferrer\">Ghost</a>" theme-name="<a href=\"https://fueko.net\" target=\"_blank\" rel=\"noopener\">Reiro</a>"}}}
36 | 			{{/if}}
37 | 		</div>
38 | 	</div>
39 | </footer>
```

partials/footer_icons.hbs
```
1 | {{! Detailed instructions can be found in the Documentation >> Activation >> Social accounts }}
2 | 
3 | {{! RSS }}
4 | {{!-- <li><a href="/rss">{{>icons/site/rss}}RSS</a></li> --}}
5 | 
6 | {{! Adobe Creative Cloud }}
7 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/adobecreativecloud}}Adobe Creative Cloud</a></li> --}}
8 | {{! Airbnb }}
9 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/airbnb}}Airbnb</a></li> --}}
10 | {{! Amazon }}
11 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/amazon}}Amazon</a></li> --}}
12 | {{! Android }}
13 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/android}}Android</a></li> --}}
14 | {{! AngelList }}
15 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/angellist}}AngelList</a></li> --}}
16 | {{! Angular }}
17 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/angular}}Angular</a></li> --}}
18 | {{! Apple }}
19 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/apple}}Apple</a></li> --}}
20 | {{! Apple Music }}
21 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/applemusic}}Apple Music</a></li> --}}
22 | {{! Apple Pay }}
23 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/applepay}}Apple Pay</a></li> --}}
24 | {{! Asana }}
25 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/asana}}Asana</a></li> --}}
26 | {{! Atlassian }}
27 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/atlassian}}Atlassian</a></li> --}}
28 | {{! Baidu }}
29 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/baidu}}Baidu</a></li> --}}
30 | {{! BandCamp }}
31 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bandcamp}}BandCamp</a></li> --}}
32 | {{! Basecamp }}
33 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/basecamp}}Basecamp</a></li> --}}
34 | {{! Behance }}
35 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/behance}}Behance</a></li> --}}
36 | {{! Big Cartel }}
37 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bigcartel}}Big Cartel</a></li> --}}
38 | {{! Bitcoin }}
39 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bitcoin}}Bitcoin</a></li> --}}
40 | {{! Bitbucket }}
41 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bitbucket}}Bitbucket</a></li> --}}
42 | {{! Bitly }}
43 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bitly}}Bitly</a></li> --}}
44 | {{! Blogger }}
45 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/blogger}}Blogger</a></li> --}}
46 | {{! Bluesky }}
47 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bluesky}}Bluesky</a></li> --}}
48 | {{! Bower }}
49 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/bower}}Bower</a></li> --}}
50 | {{! Buffer }}
51 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/buffer}}Buffer</a></li> --}}
52 | {{! Buy me a coffee }}
53 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/buymeacoffee}}Buy me a coffee</a></li> --}}
54 | {{! BuzzFeed }}
55 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/buzzfeed}}BuzzFeed</a></li> --}}
56 | {{! CashApp }}
57 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/cashapp}}CashApp</a></li> --}}
58 | {{! Castro }}
59 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/castro}}Castro</a></li> --}}
60 | {{! Codecov }}
61 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/codecov}}Codecov</a></li> --}}
62 | {{! CodeIgniter }}
63 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/codeigniter}}CodeIgniter</a></li> --}}
64 | {{! CodePen }}
65 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/codepen}}CodePen</a></li> --}}
66 | {{! Codewars }}
67 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/codewars}}Codewars</a></li> --}}
68 | {{! Dailymotion }}
69 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/dailymotion}}Dailymotion</a></li> --}}
70 | {{! Debian }}
71 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/debian}}Debian</a></li> --}}
72 | {{! Deezer }}
73 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/deezer}}Deezer</a></li> --}}
74 | {{! Delicious }}
75 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/delicious}}Delicious</a></li> --}}
76 | {{! DeviantArt }}
77 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/deviantart}}DeviantArt</a></li> --}}
78 | {{! Diaspora }}
79 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/diaspora}}Diaspora</a></li> --}}
80 | {{! Digg }}
81 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/digg}}Digg</a></li> --}}
82 | {{! Discord }}
83 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/discord}}Discord</a></li> --}}
84 | {{! Discourse }}
85 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/discourse}}Discourse</a></li> --}}
86 | {{! Disqus }}
87 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/disqus}}Disqus</a></li> --}}
88 | {{! Django }}
89 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/django}}Django</a></li> --}}
90 | {{! Dribbble }}
91 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/dribbble}}Dribbble</a></li> --}}
92 | {{! Dropbox }}
93 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/dropbox}}Dropbox</a></li> --}}
94 | {{! DTube }}
95 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/dtube}}DTube</a></li> --}}
96 | {{! Envato }}
97 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/envato}}Envato</a></li> --}}
98 | {{! Etsy }}
99 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/etsy}}Etsy</a></li> --}}
100 | {{! Evernote }}
101 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/evernote}}Evernote</a></li> --}}
102 | {{! Everplaces }}
103 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/everplaces}}Everplaces</a></li> --}}
104 | {{! Feedly }}
105 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/feedly}}Feedly</a></li> --}}
106 | {{! Figma }}
107 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/figma}}Figma</a></li> --}}
108 | {{! Flickr }}
109 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/flickr}}Flickr</a></li> --}}
110 | {{! Flipboard }}
111 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/flipboard}}Flipboard</a></li> --}}
112 | {{! Framer }}
113 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/framer}}Framer</a></li> --}}
114 | {{! Foursquare }}
115 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/foursquare}}Foursquare</a></li> --}}
116 | {{! Gatsby }}
117 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gatsby}}Gatsby</a></li> --}}
118 | {{! Ghost }}
119 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/ghost}}Ghost</a></li> --}}
120 | {{! Git }}
121 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/git}}Git</a></li> --}}
122 | {{! GitHub }}
123 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/github}}GitHub</a></li> --}}
124 | {{! GitLab }}
125 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gitlab}}GitLab</a></li> --}}
126 | {{! Gmail }}
127 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gmail}}Gmail</a></li> --}}
128 | {{! GNU Social }}
129 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gnusocial}}GNU Social</a></li> --}}
130 | {{! GoldenLine }}
131 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/goldenline}}GoldenLine</a></li> --}}
132 | {{! Google Allo }}
133 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googleallo}}Google Allo</a></li> --}}
134 | {{! Google Analytics }}
135 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googleanalytics}}Google Analytics</a></li> --}}
136 | {{! Google Drive }}
137 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googledrive}}Google Drive</a></li> --}}
138 | {{! Google Pay }}
139 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googlepay}}Google Pay</a></li> --}}
140 | {{! Google Play }}
141 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googleplay}}Google Play</a></li> --}}
142 | {{! Google Plus }}
143 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googleplus}}Google Plus</a></li> --}}
144 | {{! Google Podcasts }}
145 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/googlepodcasts}}Google Podcasts</a></li> --}}
146 | {{! Gravatar }}
147 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gravatar}}Gravatar</a></li> --}}
148 | {{! Groupon }}
149 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/groupon}}Groupon</a></li> --}}
150 | {{! Gulp }}
151 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gulp}}Gulp</a></li> --}}
152 | {{! Gumroad }}
153 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gumroad}}Gumroad</a></li> --}}
154 | {{! Gumtree }}
155 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/gumtree}}Gumtree</a></li> --}}
156 | {{! HackerRank }}
157 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/hackerrank}}HackerRank</a></li> --}}
158 | {{! Heroku }}
159 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/heroku}}Heroku</a></li> --}}
160 | {{! Hipchat }}
161 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/hipchat}}Hipchat</a></li> --}}
162 | {{! Hootsuite }}
163 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/hootsuite}}Hootsuite</a></li> --}}
164 | {{! Houzz }}
165 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/houzz}}Houzz</a></li> --}}
166 | {{! Hulu }}
167 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/hulu}}Hulu</a></li> --}}
168 | {{! Humble Bundle }}
169 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/humblebundle}}Humble Bundle</a></li> --}}
170 | {{! ICQ }}
171 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/icq}}ICQ</a></li> --}}
172 | {{! iFixit }}
173 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/ifixit}}iFixit</a></li> --}}
174 | {{! IMDb }}
175 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/imdb}}IMDb</a></li> --}}
176 | {{! Instagram }}
177 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/instagram}}Instagram</a></li> --}}
178 | {{! Instapaper }}
179 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/instapaper}}Instapaper</a></li> --}}
180 | {{! Intercom }}
181 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/intercom}}Intercom</a></li> --}}
182 | {{! InVision }}
183 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/invision}}InVision</a></li> --}}
184 | {{! JavaScript }}
185 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/javascript}}JavaScript</a></li> --}}
186 | {{! Jira }}
187 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/jira}}Jira</a></li> --}}
188 | {{! Joomla }}
189 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/joomla}}Joomla</a></li> --}}
190 | {{! jQuery }}
191 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/jquery}}jQuery</a></li> --}}
192 | {{! JSFiddle }}
193 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/jsfiddle}}JSFiddle</a></li> --}}
194 | {{! JustGiving }}
195 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/justgiving}}JustGiving</a></li> --}}
196 | {{! Khan Academy }}
197 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/khanacademy}}Khan Academy</a></li> --}}
198 | {{! Kickstarter }}
199 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/kickstarter}}Kickstarter</a></li> --}}
200 | {{! Kik }}
201 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/kik}}Kik</a></li> --}}
202 | {{! Ko-fi }}
203 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/kofi}}Ko-fi</a></li> --}}
204 | {{! Last.fm }}
205 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/lastfm}}Last.fm</a></li> --}}
206 | {{! Line }}
207 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/line}}Line</a></li> --}}
208 | {{! Linkedin }}
209 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/linkedin}}Linkedin</a></li> --}}
210 | {{! Livestream }}
211 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/livestream}}Livestream</a></li> --}}
212 | {{! Mailchimp }}
213 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/mailchimp}}Mailchimp</a></li> --}}
214 | {{! MakerBot }}
215 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/makerbot}}MakerBot</a></li> --}}
216 | {{! MasterCard }}
217 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/mastercard}}MasterCard</a></li> --}}
218 | {{! Mastodon }}
219 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/mastodon}}Mastodon</a></li> --}}
220 | {{! Medium }}
221 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/medium}}Medium</a></li> --}}
222 | {{! Meetup }}
223 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/meetup}}Meetup</a></li> --}}
224 | {{! Messenger }}
225 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/messenger}}Messenger</a></li> --}}
226 | {{! Micro.blog }}
227 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/microblog}}Micro.blog</a></li> --}}
228 | {{! .NET }}
229 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/net}}.NET</a></li> --}}
230 | {{! Netlify }}
231 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/netlify}}Netlify</a></li> --}}
232 | {{! Netflix }}
233 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/netflix}}Netflix</a></li> --}}
234 | {{! Nintendo Switch }}
235 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/nintendoswitch}}Nintendo Switch</a></li> --}}
236 | {{! Notion }}
237 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/notion}}Notion</a></li> --}}
238 | {{! npm }}
239 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/npm}}npm</a></li> --}}
240 | {{! NVIDIA }}
241 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/nvidia}}NVIDIA</a></li> --}}
242 | {{! Oculus }}
243 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/oculus}}Oculus</a></li> --}}
244 | {{! Odnoklassniki }}
245 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/odnoklassniki}}Odnoklassniki</a></li> --}}
246 | {{! Origin }}
247 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/origin}}Origin</a></li> --}}
248 | {{! Overcast }}
249 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/overcast}}Overcast</a></li> --}}
250 | {{! PayPal }}
251 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/paypal}}PayPal</a></li> --}}
252 | {{! Patreon }}
253 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/patreon}}Patreon</a></li> --}}
254 | {{! Periscope }}
255 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/periscope}}Periscope</a></li> --}}
256 | {{! Pinboard }}
257 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/pinboard}}Pinboard</a></li> --}}
258 | {{! Pingdom }}
259 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/pingdom}}Pingdom</a></li> --}}
260 | {{! Pinterest }}
261 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/pinterest}}Pinterest</a></li> --}}
262 | {{! Player.me }}
263 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/playerme}}Player.me</a></li> --}}
264 | {{! Plex }}
265 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/plex}}Plex</a></li> --}}
266 | {{! Pocket }}
267 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/pocket}}Pocket</a></li> --}}
268 | {{! Podcasts }}
269 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/podcasts}}Podcasts</a></li> --}}
270 | {{! ProcessWire }}
271 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/processwire}}ProcessWire</a></li> --}}
272 | {{! Product Hunt }}
273 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/producthunt}}Product Hunt</a></li> --}}
274 | {{! Proto.io }}
275 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/protoio}}Proto.io</a></li> --}}
276 | {{! Python }}
277 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/python}}Python</a></li> --}}
278 | {{! Quantopian }}
279 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/quantopian}}Quantopian</a></li> --}}
280 | {{! Quip }}
281 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/quip}}Quip</a></li> --}}
282 | {{! Quora }}
283 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/quora}}Quora</a></li> --}}
284 | {{! Raspberry Pi }}
285 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/raspberrypi}}Raspberry Pi</a></li> --}}
286 | {{! Riot }}
287 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/riot}}Riot</a></li> --}}
288 | {{! Runkeeper }}
289 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/runkeeper}}Runkeeper</a></li> --}}
290 | {{! Redbubble }}
291 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/redbubble}}Redbubble</a></li> --}}
292 | {{! Reddit }}
293 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/reddit}}Reddit</a></li> --}}
294 | {{! Sauce Labs }}
295 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/saucelabs}}Sauce Labs</a></li> --}}
296 | {{! Sellfy }}
297 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/sellfy}}Sellfy</a></li> --}}
298 | {{! Shopify }}
299 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/shopify}}Shopify</a></li> --}}
300 | {{! Skype }}
301 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/skype}}Skype</a></li> --}}
302 | {{! Slack }}
303 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/slack}}Slack</a></li> --}}
304 | {{! SlickPic }}
305 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/slickpic}}SlickPic</a></li> --}}
306 | {{! Smashing Magazine }}
307 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/smashingmagazine}}Smashing Magazine</a></li> --}}
308 | {{! Snapchat }}
309 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/snapchat}}Snapchat</a></li> --}}
310 | {{! Songkick }}
311 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/songkick}}Songkick</a></li> --}}
312 | {{! SoundCloud }}
313 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/soundcloud}}SoundCloud</a></li> --}}
314 | {{! SparkPost }}
315 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/sparkpost}}SparkPost</a></li> --}}
316 | {{! Spotify }}
317 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/spotify}}Spotify</a></li> --}}
318 | {{! Squarespace }}
319 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/squarespace}}Squarespace</a></li> --}}
320 | {{! Strava }}
321 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/strava}}Strava</a></li> --}}
322 | {{! Stack Overflow }}
323 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/stackoverflow}}Stack Overflow</a></li> --}}
324 | {{! Steam }}
325 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/steam}}Steam</a></li> --}}
326 | {{! Stripe }}
327 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/stripe}}Stripe</a></li> --}}
328 | {{! TED }}
329 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/ted}}TED</a></li> --}}
330 | {{! Tencent QQ }}
331 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/tencentqq}}Tencent QQ</a></li> --}}
332 | {{! Telegram }}
333 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/telegram}}Telegram</a></li> --}}
334 | {{! The Mighty }}
335 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/themighty}}The Mighty</a></li> --}}
336 | {{! Threads }}
337 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/threads}}Threads</a></li> --}}
338 | {{! TikTok }}
339 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/tiktok}}TikTok</a></li> --}}
340 | {{! Tinder }}
341 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/tinder}}Tinder</a></li> --}}
342 | {{! Trakt }}
343 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/trakt}}Trakt</a></li> --}}
344 | {{! Trello }}
345 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/trello}}Trello</a></li> --}}
346 | {{! Tumblr }}
347 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/tumblr}}Tumblr</a></li> --}}
348 | {{! Twilio }}
349 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/twilio}}Twilio</a></li> --}}
350 | {{! Twitch }}
351 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/twitch}}Twitch</a></li> --}}
352 | {{! Twoo }}
353 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/twoo}}Twoo</a></li> --}}
354 | {{! Udacity }}
355 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/udacity}}Udacity</a></li> --}}
356 | {{! Udemy }}
357 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/udemy}}Udemy</a></li> --}}
358 | {{! Unsplash }}
359 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/unsplash}}Unsplash</a></li> --}}
360 | {{! Upwork }}
361 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/upwork}}Upwork</a></li> --}}
362 | {{! Vimeo }}
363 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/vimeo}}Vimeo</a></li> --}}
364 | {{! Vine }}
365 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/vine}}Vine</a></li> --}}
366 | {{! Visa }}
367 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/visa}}Visa</a></li> --}}
368 | {{! vk }}
369 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/vk}}vk</a></li> --}}
370 | {{! VSCO }}
371 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/vsco}}VSCO</a></li> --}}
372 | {{! WhatsApp }}
373 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/whatsapp}}WhatsApp</a></li> --}}
374 | {{! WeChat }}
375 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/wechat}}WeChat</a></li> --}}
376 | {{! Weibo }}
377 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/weibo}}Weibo</a></li> --}}
378 | {{! Wikipedia }}
379 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/wikipedia}}Wikipedia</a></li> --}}
380 | {{! Wire }}
381 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/wire}}Wire</a></li> --}}
382 | {{! WordPress }}
383 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/wordpress}}WordPress</a></li> --}}
384 | {{! Xbox }}
385 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/xbox}}Xbox</a></li> --}}
386 | {{! YouTube }}
387 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/youtube}}YouTube</a></li> --}}
388 | {{! YouTube Music}}
389 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/youtubemusic}}YouTube Music</a></li> --}}
390 | {{! Zendesk }}
391 | {{!-- <li><a href="#" target="_blank" rel="noopener">{{>icons/social/zendesk}}Zendesk</a></li> --}}
```

partials/header.hbs
```
1 | <header class="header-section">
2 | 	<div class="header-wrap">
3 | 		<div class="header-logo global-logo is-header">{{>logo}}</div>
4 | 		<div class="header-nav">
5 | 			{{>search is_mobile=true}}
6 | 			<input id="toggle" class="header-checkbox" type="checkbox">
7 | 			<label class="header-toggle" for="toggle">
8 | 				<span>
9 | 					<span class="bar"></span>
10 | 					<span class="bar"></span>
11 | 					<span class="bar"></span>
12 | 				</span>
13 | 			</label>
14 | 			<nav{{^if @site.members_enabled}} class="is-right"{{/if}}>{{navigation}}</nav>
15 | 		</div>
16 | 	</div>
17 | </header>
```

partials/hero.hbs
```
1 | <div class="hero-section">
2 | 	<div class="hero-wrap global-padding">
3 | 		<h1 class="hero-title global-title">{{#if @custom.hero_title_text}}{{{@custom.hero_title_text}}}{{else}}{{{t "{start-bold}Hey, we’re {site-title}.{end-bold}{new-line}See our thoughts, stories and ideas." new-line="<br>" start-bold="<span>" end-bold="</span>" site-title=@site.title}}}{{/if}}</h1>
4 | 		{{>search is_hero=true}}
5 | 		{{>members/subscribe_form is_hero=true}}
6 | 	</div>
7 | </div>
```

partials/icons/site/close.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.997 10.846L1.369.219 1.363.214A.814.814 0 00.818.005.821.821 0 000 .822c0 .201.074.395.208.545l.006.006L10.842 12 .214 22.626l-.006.006a.822.822 0 00-.208.546c0 .447.37.817.818.817a.814.814 0 00.551-.215l10.628-10.627 10.628 10.628.005.005a.816.816 0 001.368-.603.816.816 0 00-.213-.552l-.006-.005L13.151 12l10.63-10.627c.003 0 .004-.003.006-.005A.82.82 0 0024 .817a.817.817 0 00-1.37-.602l-.004.004-10.63 10.627z"/></svg>
```

partials/icons/site/copy.hbs
```
1 | <svg role="img" viewBox="0 0 33 24" xmlns="http://www.w3.org/2000/svg"><path d="M27.3999996,13.4004128 L21.7999996,13.4004128 L21.7999996,19 L18.9999996,19 L18.9999996,13.4004128 L13.3999996,13.4004128 L13.3999996,10.6006192 L18.9999996,10.6006192 L18.9999996,5 L21.7999996,5 L21.7999996,10.6006192 L27.3999996,10.6006192 L27.3999996,13.4004128 Z M12,20.87 C7.101,20.87 3.13,16.898 3.13,12 C3.13,7.102 7.101,3.13 12,3.13 C12.091,3.13 12.181,3.139 12.272,3.142 C9.866,5.336 8.347,8.487 8.347,12 C8.347,15.512 9.866,18.662 12.271,20.857 C12.18,20.859 12.091,20.87 12,20.87 Z M20.347,0 C18.882,0 17.484,0.276 16.186,0.756 C14.882,0.271 13.473,0 12,0 C5.372,0 0,5.373 0,12 C0,18.628 5.372,24 12,24 C13.471,24 14.878,23.726 16.181,23.242 C17.481,23.724 18.88,24 20.347,24 C26.975,24 32.347,18.628 32.347,12 C32.347,5.373 26.975,0 20.347,0 Z"/></svg>
```

partials/icons/site/dots.hbs
```
1 | <svg role="img" viewBox="0 0 20 4" xmlns="http://www.w3.org/2000/svg"><path d="M2 4A2 2 0 102.001.001 2 2 0 002 4zm8 0a2 2 0 10.001-3.999A2 2 0 0010 4zm8 0a2 2 0 10.001-3.999A2 2 0 0018 4z"/></svg>
```

partials/icons/site/link.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 12C0 5.374 5.374 0 12 0c6.628 0 12 5.374 12 12 0 6.628-5.372 12-12 12-6.626 0-12-5.372-12-12zm5.593-.866a5.34 5.34 0 0 0-1.558 3.74c0 2.868 2.369 5.237 5.174 5.174a5.235 5.235 0 0 0 3.74-1.558l1.559-1.558-1.746-1.745-1.558 1.558a2.737 2.737 0 0 1-1.933.81c-1.496 0-2.743-1.246-2.743-2.743 0-.748.313-1.434.81-1.932l1.559-1.558-1.745-1.746-1.559 1.559v-.001zm7.62-1.962l-4.85 4.85 1.698 1.696 4.848-4.85-1.696-1.696zm4.843 4.212a5.34 5.34 0 0 0 1.558-3.741c0-2.868-2.368-5.236-5.173-5.174A5.232 5.232 0 0 0 10.7 6.03L9.142 7.585l1.746 1.746 1.558-1.56a2.738 2.738 0 0 1 1.932-.809c1.496 0 2.743 1.246 2.743 2.742a2.74 2.74 0 0 1-.81 1.933l-1.56 1.559 1.746 1.745 1.56-1.558z"/></svg>
```

partials/icons/site/pin.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C6.908 0 2.766 4.143 2.766 9.234c0 1.529.456 3.028 1.108 4.388C5.872 17.785 11.79 24 12 24c.21 0 6.524-6.908 8.128-10.382.632-1.368 1.106-2.855 1.106-4.384C21.234 4.143 17.092 0 12 0zm0 4.425a4.663 4.663 0 014.661 4.661A4.663 4.663 0 0112 13.747a4.663 4.663 0 01-4.661-4.661A4.663 4.663 0 0112 4.425z"/></svg>
```

partials/icons/site/rss.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.199 24C19.199 13.467 10.533 4.8 0 4.8V0c13.165 0 24 10.835 24 24h-4.801zM3.291 17.415c1.814 0 3.293 1.479 3.293 3.295 0 1.813-1.485 3.29-3.301 3.29C1.47 24 0 22.526 0 20.71s1.475-3.294 3.291-3.295zM15.909 24h-4.665c0-6.169-5.075-11.245-11.244-11.245V8.09c8.727 0 15.909 7.184 15.909 15.91z"/></svg>
```

partials/icons/site/search.hbs
```
1 | {{#if is_mobile}}
2 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.877 18.456l5.01 5.011c.208.197.484.308.771.308a1.118 1.118 0 00.809-1.888l-5.011-5.01c3.233-4.022 2.983-9.923-.746-13.654l-.291-.29a.403.403 0 00-.095-.075C13.307-.77 7.095-.649 3.223 3.223c-3.997 3.998-3.997 10.489 0 14.485 3.731 3.731 9.633 3.981 13.654.748zm-.784-13.617a7.96 7.96 0 010 11.254 7.961 7.961 0 01-11.253 0 7.96 7.96 0 010-11.254 7.961 7.961 0 0111.253 0z"/></svg>
3 | {{else}}
4 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="m16.822 18.813 4.798 4.799c.262.248.61.388.972.388.772-.001 1.407-.637 1.407-1.409 0-.361-.139-.709-.387-.971l-4.799-4.797c3.132-4.108 2.822-10.005-.928-13.756l-.007-.007-.278-.278a.6985.6985 0 0 0-.13-.107C13.36-1.017 7.021-.888 3.066 3.067c-4.088 4.089-4.088 10.729 0 14.816 3.752 3.752 9.65 4.063 13.756.93Zm-.965-13.719c2.95 2.953 2.95 7.81 0 10.763-2.953 2.949-7.809 2.949-10.762 0-2.951-2.953-2.951-7.81 0-10.763 2.953-2.95 7.809-2.95 10.762 0Z"/></svg>
5 | {{/if}}
```

partials/icons/site/user.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd"><path d="M1.631 23.361l-.001-.078c0-5.723 4.647-10.37 10.37-10.37 5.723 0 10.37 4.647 10.37 10.37l-.001.078h-1.5l.001-.078c0-4.895-3.975-8.87-8.87-8.87s-8.87 3.975-8.87 8.87l.001.078h-1.5zM12 .639a5.657 5.657 0 015.654 5.655A5.657 5.657 0 0112 11.948a5.657 5.657 0 01-5.654-5.654A5.657 5.657 0 0112 .639zm0 1.5a4.156 4.156 0 010 8.309 4.156 4.156 0 010-8.309z"/></svg>
```

partials/icons/social/adobecreativecloud.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 11.599v.803c-.008.044-.017.087-.022.13-.04.35-.067.701-.124 1.048a8.663 8.663 0 0 1-1.176 3.144 8.848 8.848 0 0 1-3.645 3.36 8.422 8.422 0 0 1-2.812.843c-.217.026-.435.049-.652.073H7.138c-.043-.008-.085-.02-.128-.024a7.092 7.092 0 0 1-2.448-.598c-1.697-.755-2.963-1.98-3.791-3.664a7.298 7.298 0 0 1-.7-2.37L0 13.742v-.78c.008-.043.02-.086.023-.13a7.286 7.286 0 0 1 .461-2.175C1.2 8.777 2.45 7.381 4.222 6.478a7.227 7.227 0 0 1 2.928-.77 7.998 7.998 0 0 1 1.503.071.188.188 0 0 0 .142-.047 8.898 8.898 0 0 1 2.458-1.81 8.493 8.493 0 0 1 2.825-.848c.234-.027.467-.05.7-.074h.72c.046.007.094.016.14.021.357.043.715.07 1.068.13a8.37 8.37 0 0 1 3.073 1.186 8.89 8.89 0 0 1 3.319 3.713 8.76 8.76 0 0 1 .83 2.862c.026.229.048.458.072.687m-13.42-5.2c.015.02.019.029.025.032.493.247.965.538 1.41.867.028.02.098.012.132-.01 1.222-.787 2.547-1.059 3.97-.802 1.395.251 2.53.96 3.397 2.092.982 1.28 1.357 2.73 1.086 4.34-.182 1.08-.608 2.05-1.33 2.861-1.32 1.48-2.973 2.092-4.918 1.833-1.197-.16-2.23-.685-3.086-1.564-1.098-1.128-2.204-2.248-3.305-3.373-.147-.15-.31-.27-.521-.297a.826.826 0 0 0-.864.48c-.142.3-.124.64.185.948 1.227 1.226 2.444 2.462 3.67 3.69.21.21.435.405.674.582.896.661 1.906 1.027 3 1.174.858.116 1.71.09 2.555-.102 1.612-.369 2.948-1.205 4-2.497a7.213 7.213 0 0 0 1.576-3.67 7.313 7.313 0 0 0-.065-2.36c-.244-1.27-.773-2.408-1.62-3.377-1.618-1.846-3.653-2.67-6.074-2.487a6.664 6.664 0 0 0-2.641.79 6.962 6.962 0 0 0-1.255.85M9.988 19.29a15.79 15.79 0 0 1-.1-.094c-.501-.482-1.006-.96-1.502-1.449a.403.403 0 0 0-.32-.137c-.502.012-1.005.014-1.5-.1-2.461-.565-3.89-3.286-2.983-5.68.715-1.889 2.696-3.038 4.649-2.684.875.159 1.644.536 2.274 1.197.77.808 1.562 1.592 2.34 2.391.176.182.38.265.625.23.316-.046.569-.2.683-.516.112-.31.058-.605-.173-.844-.816-.84-1.613-1.702-2.462-2.507-1.647-1.561-3.588-2.026-5.736-1.362-2.888.893-4.579 3.926-3.919 6.919.602 2.727 2.947 4.64 5.691 4.643h2.299c.038 0 .076-.004.134-.007" /></svg>
```

partials/icons/social/airbnb.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.998 18.267c-1.352-1.696-2.147-3.182-2.412-4.455-.263-1.026-.159-1.847.291-2.464.477-.71 1.187-1.055 2.12-1.055s1.642.345 2.119 1.062c.446.61.558 1.432.286 2.464-.291 1.298-1.085 2.784-2.411 4.456zm9.597 1.14c-.185 1.245-1.034 2.278-2.2 2.782-2.251.98-4.48-.583-6.388-2.703 3.155-3.95 3.738-7.025 2.384-9.014-.795-1.14-1.933-1.695-3.393-1.695-2.943 0-4.561 2.49-3.925 5.38.37 1.564 1.351 3.342 2.915 5.33-.98 1.084-1.909 1.855-2.73 2.332-.636.344-1.245.557-1.828.608-2.677.399-4.776-2.198-3.823-4.877.132-.345.395-.98.845-1.961l.025-.053C4.94 12.36 6.717 8.75 8.759 4.746l.053-.132.58-1.115c.45-.822.635-1.19 1.351-1.643.345-.209.769-.314 1.245-.314.954 0 1.697.557 2.015 1.006.158.239.345.557.582.953l.558 1.088.08.159c2.04 4.002 3.819 7.605 5.276 10.789l.026.025.533 1.22.318.764c.243.612.294 1.221.213 1.857zm1.219-2.389c-.186-.583-.504-1.271-.9-2.093v-.03c-1.887-4.005-3.64-7.605-5.304-10.84l-.111-.162C15.313 1.461 14.464 0 11.998 0 9.56 0 8.524 1.694 7.465 3.897l-.081.16c-1.668 3.234-3.42 6.839-5.301 10.842v.053l-.558 1.219c-.21.504-.317.768-.345.847-1.35 3.712 1.432 6.972 4.8 6.972.027 0 .132 0 .264-.027h.372c1.75-.213 3.553-1.325 5.382-3.316 1.828 1.988 3.633 3.103 5.38 3.316h.372c.132.027.238.027.264.027 3.368.003 6.15-3.26 4.8-6.972z"/></svg>
```

partials/icons/social/amazon.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M.045 18.02c.072-.116.187-.124.348-.022 3.636 2.11 7.594 3.166 11.87 3.166 2.852 0 5.668-.533 8.447-1.595l.315-.14c.138-.06.234-.1.293-.13.226-.088.39-.046.525.13.12.174.09.336-.12.48-.256.19-.6.41-1.006.654-1.244.743-2.64 1.316-4.185 1.726-1.53.406-3.045.61-4.516.61-2.265 0-4.41-.396-6.435-1.187-2.02-.794-3.82-1.91-5.43-3.35-.1-.074-.15-.15-.15-.22 0-.047.02-.09.05-.13zm6.565-6.218c0-1.005.247-1.863.743-2.577.495-.71 1.17-1.25 2.04-1.615.796-.335 1.756-.575 2.912-.72.39-.046 1.033-.103 1.92-.174v-.37c0-.93-.105-1.558-.3-1.875-.302-.43-.78-.65-1.44-.65h-.182c-.48.046-.896.196-1.246.46-.35.27-.575.63-.675 1.096-.06.3-.206.465-.435.51l-2.52-.315c-.248-.06-.372-.18-.372-.39 0-.046.007-.09.022-.15.247-1.29.855-2.25 1.82-2.88.976-.616 2.1-.975 3.39-1.05h.54c1.65 0 2.957.434 3.888 1.29.135.15.27.3.405.48.12.165.224.314.283.45.075.134.15.33.195.57.06.254.105.42.135.51.03.104.062.3.076.615.01.313.02.493.02.553v5.28c0 .376.06.72.165 1.036.105.313.21.54.315.674l.51.674c.09.136.136.256.136.36 0 .12-.06.226-.18.314-1.2 1.05-1.86 1.62-1.963 1.71-.165.135-.375.15-.63.045-.195-.166-.375-.332-.526-.496l-.31-.347c-.06-.074-.166-.21-.317-.42l-.3-.435c-.81.886-1.603 1.44-2.4 1.665-.494.15-1.093.227-1.83.227-1.11 0-2.04-.343-2.76-1.034-.72-.69-1.08-1.665-1.08-2.94l-.05-.076zm3.753-.438c0 .566.14 1.02.425 1.364.285.34.675.512 1.155.512.045 0 .106-.007.195-.02.09-.016.134-.023.166-.023.614-.16 1.08-.553 1.424-1.178.165-.28.285-.58.36-.91.09-.32.12-.59.135-.8.015-.195.015-.54.015-1.005v-.54c-.84 0-1.484.06-1.92.18-1.275.36-1.92 1.17-1.92 2.43l-.035-.02zm9.162 7.027c.03-.06.075-.11.132-.17.362-.243.714-.41 1.05-.5.55-.133 1.09-.222 1.612-.24.14-.012.28 0 .41.03.65.06 1.05.168 1.172.33.063.09.09.228.09.39v.15c0 .51-.14 1.11-.415 1.8-.278.69-.664 1.248-1.156 1.68-.073.06-.14.09-.197.09-.03 0-.06 0-.09-.012-.09-.044-.107-.12-.064-.24.54-1.26.806-2.143.806-2.64 0-.15-.03-.27-.087-.344-.145-.166-.55-.257-1.224-.257-.243 0-.533.016-.87.046-.363.045-.7.09-1 .135-.09 0-.148-.014-.18-.044-.03-.03-.036-.047-.02-.077 0-.017.006-.03.02-.063v-.06z"/></svg>
```

partials/icons/social/android.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.146 9.227c0-.815-.658-1.478-1.476-1.478s-1.48.66-1.48 1.48v6.19c0 .81.663 1.48 1.483 1.48.814 0 1.476-.67 1.476-1.48v-6.2h-.01zM5.393 8.032l.004 9.6c0 .885.704 1.59 1.573 1.59h1.063v3.28c0 .82.66 1.482 1.47 1.482s1.467-.66 1.48-1.468v-3.28h1.993v3.28c0 .823.66 1.483 1.47 1.483.823 0 1.482-.66 1.482-1.49v-3.28h1.078c.87 0 1.573-.71 1.573-1.578v-9.63L5.35 8.03l.04.002zm9.648-2.93c-.31 0-.56-.25-.56-.56 0-.305.25-.558.56-.56.31 0 .56.255.56.56 0 .31-.25.56-.56.56m-6.06 0c-.31 0-.56-.25-.56-.56 0-.307.25-.558.56-.558.31 0 .56.255.56.57s-.252.567-.57.567m6.29-2.9L16.29.33c.06-.105.014-.226-.076-.285C16.11 0 15.99.03 15.93.135l-1.05 1.9c-.868-.405-1.856-.63-2.89-.63s-2.018.215-2.892.603L8.064.105c-.053-.098-.18-.135-.278-.08-.1.045-.136.18-.08.27l1.03 1.875c-2.03 1.047-3.4 3.04-3.4 5.33h13.328c0-2.29-1.368-4.283-3.396-5.33M3.33 7.742c-.817 0-1.48.665-1.48 1.483v6.192c0 .82.664 1.48 1.484 1.48.814 0 1.477-.66 1.477-1.48v-6.19c0-.815-.66-1.478-1.47-1.478"/></svg>
```

partials/icons/social/angellist.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.465 9.954c.735-2 1.31-3.65 1.723-4.954.41-1.3.618-2.1.618-2.4 0-.315-.07-.564-.21-.738-.135-.174-.324-.264-.567-.264-.31 0-.63.255-.94.765-.32.51-.67 1.334-1.06 2.467l-1.65 4.76 2.08.362h-.01v.002zm-2.193 4.435c-.474-.03-.923-.08-1.344-.15-.42-.08-.83-.19-1.216-.33.177.35.335.7.472 1.05.138.35.25.69.34 1.04.26-.33.54-.63.83-.9.292-.27.6-.51.915-.72zm-1.862-5l-1.78-5.14c-.464-1.31-.82-2.16-1.075-2.57-.25-.4-.525-.6-.822-.6-.23 0-.417.08-.56.26-.144.18-.214.41-.214.7 0 .5.19 1.38.57 2.64.38 1.25.96 2.89 1.73 4.93.06-.12.16-.21.28-.26.12-.05.28-.08.49-.08.06 0 .19.01.39.01.19.02.52.04.97.09zm-1.618 7.96c.188 0 .36-.09.51-.26.15-.18.234-.36.234-.55 0-.21-.15-.7-.452-1.46-.3-.76-.68-1.51-1.13-2.25-.33-.55-.655-.97-.97-1.25-.324-.28-.625-.42-.91-.42-.23 0-.484.14-.767.44-.28.29-.42.56-.42.81 0 .26.14.66.413 1.18.275.53.645 1.09 1.104 1.68.485.65.94 1.15 1.37 1.51.428.36.77.54 1.02.54h-.002zm-4.945-.4c.156.19.37.46.646.82.723 1 1.395 1.5 2.01 1.5.21 0 .397-.07.563-.2.164-.14.247-.27.247-.42 0-.17-.11-.44-.33-.83-.222-.39-.524-.82-.907-1.3-.44-.56-.805-.97-1.098-1.23-.288-.26-.525-.39-.697-.39-.38 0-.74.21-1.06.62-.32.4-.48.9-.48 1.46 0 .45.12.95.35 1.51.23.55.55 1.11.98 1.67.65.87 1.46 1.53 2.42 2 .96.46 2.03.69 3.19.69 2.14 0 3.94-.8 5.38-2.4 1.45-1.6 2.17-3.6 2.17-6.01 0-.74-.05-1.33-.16-1.76-.11-.43-.29-.75-.54-.95-.45-.38-1.33-.71-2.63-1.01-1.3-.3-2.66-.45-4.08-.45-.39 0-.68.07-.84.2-.16.13-.24.36-.24.673 0 .75.42 1.29 1.26 1.626.84.34 2.19.51 4.06.51h.676c.15 0 .28.06.37.174.09.11.15.28.18.52-.19.17-.57.37-1.154.6-.59.22-1.03.45-1.34.665-.66.484-1.19 1.06-1.59 1.724-.4.66-.6 1.29-.6 1.883 0 .36.086.8.258 1.31.17.51.26.823.26.95v.11l-.03.15c-.48-.03-.86-.313-1.14-.85-.287-.53-.42-1.24-.42-2.13v-.15c-.09.075-.176.135-.26.165-.086.034-.178.05-.27.05-.1 0-.198-.006-.29-.02-.09-.016-.18-.04-.29-.075.03.12.057.24.076.353.01.12.02.21.02.27 0 .406-.16.76-.48 1.05-.32.287-.7.43-1.14.43-.69 0-1.397-.34-2.11-1.01-.715-.674-1.07-1.34-1.07-1.985 0-.12.015-.23.04-.323s.075-.17.14-.24zm11.807-6.73c.985.18 1.685.6 2.09 1.25.41.64.61 1.66.61 3.06 0 2.77-.828 5.03-2.492 6.79-1.667 1.76-3.797 2.65-6.387 2.65-1.023 0-2.016-.19-2.976-.56-.97-.37-1.79-.89-2.49-1.54-.79-.73-1.39-1.49-1.78-2.3-.4-.81-.6-1.64-.6-2.48 0-.95.2-1.68.6-2.19.4-.52 1.05-.87 1.93-1.06-.17-.39-.29-.71-.36-.98-.08-.27-.12-.47-.12-.61 0-.5.26-1.01.78-1.52.52-.52 1.01-.78 1.47-.78.19 0 .4.03.62.11.22.07.47.19.75.35-.81-2.35-1.43-4.2-1.81-5.5-.39-1.31-.58-2.2-.58-2.7 0-.68.17-1.23.52-1.63.36-.4.84-.6 1.44-.6 1.03 0 2.34 2.31 3.93 6.923.28.79.48 1.4.63 1.83l.51-1.453c1.59-4.55 2.95-6.83 4.1-6.83.56 0 1.01.19 1.34.57.33.383.5.887.5 1.523 0 .48-.19 1.36-.56 2.65-.367 1.28-.92 2.96-1.67 5.04"/></svg>
```

partials/icons/social/angular.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M9.93 12.645h4.134L11.996 7.74M11.996.009L.686 3.988l1.725 14.76 9.585 5.243 9.588-5.238L23.308 3.99 11.996.01zm7.058 18.297h-2.636l-1.42-3.501H8.995l-1.42 3.501H4.937l7.06-15.648 7.057 15.648z"/></svg>
```

partials/icons/social/apple.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.078 23.55c-.473-.316-.893-.703-1.244-1.15-.383-.463-.738-.95-1.064-1.454-.766-1.12-1.365-2.345-1.78-3.636-.5-1.502-.743-2.94-.743-4.347 0-1.57.34-2.94 1.002-4.09.49-.9 1.22-1.653 2.1-2.182.85-.53 1.84-.82 2.84-.84.35 0 .73.05 1.13.15.29.08.64.21 1.07.37.55.21.85.34.95.37.32.12.59.17.8.17.16 0 .39-.05.645-.13.145-.05.42-.14.81-.31.386-.14.692-.26.935-.35.37-.11.728-.21 1.05-.26.39-.06.777-.08 1.148-.05.71.05 1.36.2 1.94.42 1.02.41 1.843 1.05 2.457 1.96-.26.16-.5.346-.725.55-.487.43-.9.94-1.23 1.505-.43.77-.65 1.64-.644 2.52.015 1.083.29 2.035.84 2.86.387.6.904 1.114 1.534 1.536.31.21.582.355.84.45-.12.375-.252.74-.405 1.1-.347.807-.76 1.58-1.25 2.31-.432.63-.772 1.1-1.03 1.41-.402.48-.79.84-1.18 1.097-.43.285-.935.436-1.452.436-.35.015-.7-.03-1.034-.127-.29-.095-.576-.202-.856-.323-.293-.134-.596-.248-.905-.34-.38-.1-.77-.148-1.164-.147-.4 0-.79.05-1.16.145-.31.088-.61.196-.907.325-.42.175-.695.29-.855.34-.324.096-.656.154-.99.175-.52 0-1.004-.15-1.486-.45zm6.854-18.46c-.68.34-1.326.484-1.973.436-.1-.646 0-1.31.27-2.037.24-.62.56-1.18 1-1.68.46-.52 1.01-.95 1.63-1.26.66-.34 1.29-.52 1.89-.55.08.68 0 1.35-.25 2.07-.228.64-.568 1.23-1 1.76-.435.52-.975.95-1.586 1.26z"/></svg>
```

partials/icons/social/applemusic.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.997 6.124c0-.738-.065-1.47-.24-2.19-.317-1.31-1.062-2.31-2.18-3.043C21.003.517 20.373.285 19.7.164c-.517-.093-1.038-.135-1.564-.15-.04-.003-.083-.01-.124-.013H5.988c-.152.01-.303.017-.455.026C4.786.07 4.043.15 3.34.428 2.004.958 1.04 1.88.475 3.208c-.192.448-.292.925-.363 1.408-.056.392-.088.785-.1 1.18 0 .032-.007.062-.01.093v12.223c.01.14.017.283.027.424.05.815.154 1.624.497 2.373.65 1.42 1.738 2.353 3.234 2.802.42.127.856.187 1.293.228.555.053 1.11.06 1.667.06h11.03c.525 0 1.048-.034 1.57-.1.823-.106 1.597-.35 2.296-.81.84-.553 1.472-1.287 1.88-2.208.186-.42.293-.87.37-1.324.113-.675.138-1.358.137-2.04-.002-3.8 0-7.595-.003-11.393zm-6.423 3.99v5.712c0 .417-.058.827-.244 1.206-.29.59-.76.962-1.388 1.14-.35.1-.706.157-1.07.173-.95.045-1.773-.6-1.943-1.536-.142-.773.227-1.624 1.038-2.022.323-.16.67-.25 1.018-.324.378-.082.758-.153 1.134-.24.274-.063.457-.23.51-.516.014-.063.02-.13.02-.193 0-1.815 0-3.63-.002-5.443 0-.062-.01-.125-.026-.185-.04-.15-.15-.243-.304-.234-.16.01-.318.035-.475.066-.76.15-1.52.303-2.28.456l-2.326.47-1.374.278c-.016.003-.032.01-.048.013-.277.077-.377.203-.39.49-.002.042 0 .086 0 .13-.002 2.602 0 5.204-.003 7.805 0 .42-.047.836-.215 1.227-.278.64-.77 1.04-1.434 1.233-.35.1-.71.16-1.075.172-.96.036-1.755-.6-1.92-1.544-.14-.812.23-1.685 1.154-2.075.357-.15.73-.232 1.108-.31.287-.06.575-.116.86-.177.383-.083.583-.323.6-.714v-.15c0-2.96 0-5.922.002-8.882 0-.123.013-.25.042-.37.07-.285.273-.448.546-.518.255-.066.515-.112.774-.165.733-.15 1.466-.296 2.2-.444l2.27-.46c.67-.134 1.34-.27 2.01-.403.22-.043.443-.088.664-.106.31-.025.523.17.554.482.008.073.012.148.012.223.002 1.91.002 3.822 0 5.732z"/></svg>
```

partials/icons/social/applepay.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.388 8.284c-.282.337-.732.602-1.182.564-.056-.455.164-.938.422-1.237C3.91 7.265 4.402 7.02 4.8 7c.047.474-.136.938-.412 1.284zm.407.654c-.651-.038-1.21.375-1.518.375-.315 0-.788-.356-1.304-.346-.67.01-1.293.393-1.635 1.005C-.366 11.194.155 13.005.834 14c.333.493.732 1.033 1.257 1.014.496-.019.693-.327 1.293-.327.605 0 .778.327 1.304.318.543-.01.885-.493 1.218-.986.38-.56.535-1.104.544-1.133-.01-.01-1.05-.412-1.06-1.625-.009-1.015.82-1.498.858-1.526-.468-.702-1.2-.778-1.453-.797zM8.56 7.564v7.389h1.135v-2.526h1.57c1.434 0 2.442-.996 2.442-2.436 0-1.441-.989-2.427-2.404-2.427H8.559zm1.135.967h1.308c.984 0 1.546.53 1.546 1.464 0 .934-.562 1.47-1.551 1.47H9.694V8.53zm6.084 6.478c.713 0 1.374-.364 1.674-.943h.023v.887h1.05v-3.678c0-1.066-.844-1.754-2.142-1.754-1.205 0-2.095.697-2.128 1.654h1.022c.084-.455.501-.753 1.073-.753.694 0 1.083.327 1.083.929v.407l-1.416.086c-1.317.08-2.03.625-2.03 1.573 0 .957.736 1.592 1.791 1.592zm.305-.876c-.605 0-.99-.294-.99-.744 0-.465.371-.735 1.079-.778l1.26-.08v.417c0 .692-.58 1.185-1.35 1.185zm3.844 2.83c1.106 0 1.626-.427 2.08-1.721L24 9.592h-1.153l-1.336 4.365h-.023l-1.336-4.365h-1.186l1.921 5.38-.103.327c-.173.554-.454.767-.956.767-.089 0-.262-.01-.333-.019v.887c.066.019.347.028.432.028z"/></svg>
```

partials/icons/social/asana.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.78 12.653c-2.882 0-5.22 2.336-5.22 5.22s2.338 5.22 5.22 5.22 5.22-2.34 5.22-5.22-2.336-5.22-5.22-5.22zm-13.56 0c-2.88 0-5.22 2.337-5.22 5.22s2.338 5.22 5.22 5.22 5.22-2.338 5.22-5.22-2.336-5.22-5.22-5.22zm12-6.525c0 2.883-2.337 5.22-5.22 5.22-2.882 0-5.22-2.337-5.22-5.22 0-2.88 2.338-5.22 5.22-5.22 2.883 0 5.22 2.34 5.22 5.22z"/></svg>
```

partials/icons/social/atlassian.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.31 23.957H15.71a1.26 1.26 0 0 1-1.312-.792c-1.332-2.665-2.78-5.288-3.987-8.046a15.25 15.25 0 0 1 .885-14.47c.166-.281.52-.625.791-.625s.593.375.74.666q5.444 10.89 10.898 21.788c.542 1.041.292 1.468-.905 1.479zm-14.573 0H1.04c-1.041 0-1.27-.417-.812-1.333q2.8-5.538 5.549-11.055c.5-1.041.895-1.041 1.592-.177a12.221 12.221 0 0 1 2.51 11.17c-.344 1.322-.532 1.405-1.864 1.405z"/></svg>
```

partials/icons/social/baidu.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.312 12.65c2.61-.562 2.25-3.684 2.176-4.366-.128-1.05-1.366-2.888-3.044-2.74-2.11.186-2.418 3.24-2.418 3.24-.287 1.41.682 4.426 3.286 3.865m4.845-5.24c1.44 0 2.604-1.66 2.604-3.71 0-2.04-1.16-3.7-2.6-3.7S6.55 1.65 6.55 3.7c0 2.05 1.17 3.71 2.61 3.71m6.207.245c1.93.26 3.162-1.8 3.412-3.36.25-1.55-1-3.36-2.36-3.67-1.37-.316-3.06 1.874-3.23 3.3-.18 1.75.25 3.49 2.17 3.737M23 10.284c0-.746-.613-2.993-2.91-2.993-2.295 0-2.61 2.12-2.61 3.62 0 1.43.118 3.42 2.985 3.36 2.855-.07 2.543-3.24 2.543-3.99M20.1 16.82s-2.985-2.31-4.726-4.8c-2.36-3.677-5.715-2.18-6.834-.316-1.12 1.883-2.86 3.062-3.105 3.377-.25.31-3.6 2.12-2.854 5.42.75 3.3 3.36 3.24 3.36 3.24s1.92.19 4.16-.31 4.16.12 4.16.12 5.207 1.75 6.648-1.61c1.424-3.37-.81-5.11-.81-5.11"/></svg>
```

partials/icons/social/bandcamp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 18.75l7.437-13.5H24l-7.438 13.5H0z"/></svg>
```

partials/icons/social/basecamp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 2C5.54 2 .48 10.22 0 17.16 2.028 20.68 6.915 22 12 22s9.975-1.32 12-4.84C23.52 10.218 18.46 2 12 2zm.15 18.4c-9.54 0-10.456-4.034-10.456-4.034l.18-.976S4.5 9.72 6.15 9.72s2.34 2.34 3.69 2.34 4.274-5.19 5.324-5.19c1.047 0 2.82 1.95 4.27 3.75 1.45 1.802 2.878 4.887 2.878 4.887l-.008.034.15.886S21.688 20.4 12.148 20.4z"/></svg>
```

partials/icons/social/behance.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M6.938 4.503c.702 0 1.34.06 1.92.188.577.13 1.07.33 1.485.61.41.28.733.65.96 1.12.225.47.34 1.05.34 1.73 0 .74-.17 1.36-.507 1.86-.338.5-.837.9-1.502 1.22.906.26 1.576.72 2.022 1.37.448.66.665 1.45.665 2.36 0 .75-.13 1.39-.41 1.93-.28.55-.67 1-1.16 1.35-.48.348-1.05.6-1.67.767-.61.165-1.252.254-1.91.254H0V4.51h6.938v-.007zM16.94 16.665c.44.428 1.073.643 1.894.643.59 0 1.1-.148 1.53-.447.424-.29.68-.61.78-.94h2.588c-.403 1.28-1.048 2.2-1.9 2.75-.85.56-1.884.83-3.08.83-.837 0-1.584-.13-2.272-.4-.673-.27-1.24-.65-1.72-1.14-.464-.49-.823-1.08-1.077-1.77-.253-.69-.373-1.45-.373-2.27 0-.803.135-1.54.403-2.23.27-.7.644-1.28 1.12-1.79.495-.51 1.063-.895 1.736-1.194s1.4-.433 2.22-.433c.91 0 1.69.164 2.38.523.67.34 1.22.82 1.66 1.4.44.586.75 1.26.94 2.02.19.75.25 1.54.21 2.38h-7.69c0 .84.28 1.632.71 2.065l-.08.03zm-10.24.05c.317 0 .62-.03.906-.093.29-.06.548-.165.763-.3.21-.135.39-.328.52-.583.13-.24.19-.57.19-.96 0-.75-.22-1.29-.64-1.62-.43-.32-.99-.48-1.69-.48H3.24v4.05H6.7v-.03zm13.607-5.65c-.352-.385-.94-.592-1.657-.592-.468 0-.855.074-1.166.238-.302.15-.55.35-.74.59-.19.24-.317.48-.392.75-.075.26-.12.5-.135.71h4.762c-.07-.75-.33-1.3-.68-1.69v.01zM6.52 10.45c.574 0 1.05-.134 1.425-.412.374-.27.554-.72.554-1.338 0-.344-.07-.625-.18-.846-.13-.22-.3-.39-.5-.512-.21-.124-.45-.21-.72-.257-.27-.053-.56-.074-.84-.074H3.23v3.44h3.29zm9.098-4.958h5.968v1.454h-5.968V5.48v.01z"/></svg>
```

partials/icons/social/bigcartel.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 13.068v-1.006c0-.63.252-1.256.88-1.508l7.79-4.9c.503-.252.755-.88.755-1.51V0L12 6.03 2.575 0v12.69c0 3.394 1.51 6.284 4.02 7.917L11.875 24l5.28-3.393c2.513-1.51 4.02-4.398 4.02-7.916V7.036L12 13.068z"/></svg>
```

partials/icons/social/bitbucket.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M.778 1.211c-.424-.006-.772.334-.778.758 0 .045.002.09.01.134l3.263 19.811c.084.499.515.867 1.022.872H19.95c.382.004.708-.271.77-.646l3.27-20.03c.068-.418-.216-.813-.635-.881-.045-.008-.089-.011-.133-.01L.778 1.211zM14.52 15.528H9.522L8.17 8.464h7.561l-1.211 7.064z"/></svg>
```

partials/icons/social/bitcoin.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.638 14.904c-1.602 6.43-8.113 10.34-14.542 8.736C2.67 22.05-1.244 15.525.362 9.105 1.962 2.67 8.475-1.243 14.9.358c6.43 1.605 10.342 8.115 8.738 14.548v-.002zm-6.35-4.613c.24-1.59-.974-2.45-2.64-3.03l.54-2.153-1.315-.33-.525 2.107c-.345-.087-.705-.167-1.064-.25l.526-2.127-1.32-.33-.54 2.165c-.285-.067-.565-.132-.84-.2l-1.815-.45-.35 1.407s.975.225.955.236c.535.136.63.486.615.766l-1.477 5.92c-.075.166-.24.406-.614.314.015.02-.96-.24-.96-.24l-.66 1.51 1.71.426.93.242-.54 2.19 1.32.327.54-2.17c.36.1.705.19 1.05.273l-.51 2.154 1.32.33.545-2.19c2.24.427 3.93.257 4.64-1.774.57-1.637-.03-2.58-1.217-3.196.854-.193 1.5-.76 1.68-1.93h.01zm-3.01 4.22c-.404 1.64-3.157.75-4.05.53l.72-2.9c.896.23 3.757.67 3.33 2.37zm.41-4.24c-.37 1.49-2.662.735-3.405.55l.654-2.64c.744.18 3.137.524 2.75 2.084v.006z"/></svg>
```

partials/icons/social/bitly.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.055 21.26c-1.345.022-2.325-.41-2.386-1.585-.025-.44-.018-.91.002-1.192.137-1.716 1.333-2.95 2.53-3.19 1.482-.294 2.455.38 2.455 2.31 0 1.303-.36 3.618-2.59 3.657h-.016zM11.923 0C5.32 0 0 5.297 0 12.224c0 3.594 1.92 7.062 4.623 9.147.52.4 1.138.367 1.497.02.297-.285.272-.984-.285-1.475-2.16-1.886-3.652-4.76-3.652-7.635 0-5.15 4.58-9.49 9.74-9.49 6.28 0 9.636 5.102 9.636 9.43 0 2.65-1.29 5.84-3.626 7.874.015 0 .493-.942.493-2.784 0-3.13-1.976-4.836-4.28-4.836-1.663 0-2.667.598-3.34 1.152 0-1.272.045-3.652.045-3.652 0-1.572-.54-2.83-2.47-2.86-1.11-.015-1.932.493-2.44 1.647-.18.436-.12.916.254 1.125.3.18.81.046 1.046-.284.165-.21.254-.254.404-.24.24.03.257.405.257.66.014.193.193 2.903.088 9.865C7.98 21.798 9.493 24 13.1 24c1.56 0 2.756-.435 4.493-1.422C20.243 21.08 24 17.758 24 12.128 23.953 5.045 18.265 0 11.933 0"/></svg>
```

partials/icons/social/blogger.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.976 24H2.026C.9 24 0 23.1 0 21.976V2.026C0 .9.9 0 2.025 0H22.05C23.1 0 24 .9 24 2.025v19.95C24 23.1 23.1 24 21.976 24zM12 3.975H9c-2.775 0-5.025 2.25-5.025 5.025v6c0 2.774 2.25 5.024 5.025 5.024h6c2.774 0 5.024-2.25 5.024-5.024v-3.975c0-.6-.45-1.05-1.05-1.05H18c-.524 0-.976-.45-.976-.976 0-2.776-2.25-5.026-5.024-5.026zm3.074 12H9c-.525 0-.975-.45-.975-.975s.45-.976.975-.976h6.074c.526 0 .977.45.977.976s-.45.976-.975.976zm-2.55-7.95c.527 0 .976.45.976.975s-.45.975-.975.975h-3.6c-.525 0-.976-.45-.976-.975s.45-.975.975-.975h3.6z"/></svg>
```

partials/icons/social/bluesky.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="m12 10.8c-1.087-2.114-4.046-6.053-6.798-7.995-2.636-1.861-3.641-1.539-4.3-1.24-.763.343-.902 1.515-.902 2.203 0 .69.378 5.65.624 6.479.815 2.736 3.713 3.66 6.383 3.364.136-.02.275-.039.415-.056-.138.022-.276.04-.415.056-3.912.58-7.387 2.005-2.83 7.078 5.013 5.19 6.87-1.113 7.823-4.308.953 3.195 2.05 9.271 7.733 4.308 4.267-4.308 1.172-6.498-2.74-7.078a8.741 8.741 0 0 1 -.415-.056c.14.017.279.036.415.056 2.67.297 5.568-.628 6.383-3.364.246-.828.624-5.79.624-6.478 0-.69-.139-1.861-.902-2.206-.659-.298-1.664-.62-4.3 1.24-2.752 1.945-5.711 5.884-6.798 7.997z"/></svg>
```

partials/icons/social/bower.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.54157 11.3053c-1.2341-1.18676-7.40717-1.92715-9.35444-2.14222.0943-.22248.1748-.45344.24155-.69076.26593-.11654.55198-.2246.84863-.31466.03603.107.2066.5149.303.70878 3.9168.10806 4.1181-2.91032 4.27702-3.73775.15574-.80837.14832-1.59025 1.4917-3.0184-2.0013-.58375-4.87983.90372-5.84393 3.11798-.36234-.1356-.72574-.23626-1.0849-.2977C14.16277 3.8923 12.82257 1 9.30624 1c-2.27782 0-4.5747.9408-6.30162 2.58083-.9302.88358-1.6612 1.93244-2.17293 3.11903C.2797 7.98073 0 9.39086 0 10.8921c0 5.22735 3.56824 9.80736 5.58437 9.80736.8804 0 1.63792-.65898 1.8159-1.25015.1494.40578.606 1.66547.75645 1.98542.2225.47464 1.2491.88465 1.6983.392.5774.32102 1.63792.51384 2.21532-.3422 1.11243.2352 2.09666-.42802 2.11785-1.2205.5456-.0286.81365-.79564.695-1.40588-.08794-.4492-1.02662-2.06276-1.3932-2.61897.72468.5901 2.56177.75645 2.78425 0 1.16858.91748 2.99084.4365 3.13492-.31042 1.42073.3687 3.0491-.4418 2.78213-1.42285 2.28206-.15785 1.99026-2.58515 1.35027-3.2006zM17.5991 7.2815c-.6007-.23626-1.363-.38565-1.89696-.38565-.7575 0-1.21943.42908-1.93244.42908-.14938 0-.50642.00106-.79353-.1017.1886.1981.42273.30512.87723.30512.27122 0 .80942-.1388 1.24486-.2691.00635.09217.0159.18222.0286.27334-.81578.19493-1.6718.71406-1.91973.8486-.5509-1.2173-.07734-2.36787.36022-2.89865 1.9621.00423 3.54757 1.35186 4.03174 1.79895zm.84915-.09112l-.29983-.28075c-.3083-.28923-.6293-.54986-.95986-.78188.4916-.9747 1.10925-2.03945 1.889-2.69842-.85815.34644-1.70678 1.38046-2.2079 2.48547-.25532-.1621-.5149-.30724-.77658-.43332.69924-1.49276 2.32338-2.73868 4.11386-2.83615-1.1993 1.08806-.74903 3.25782-1.75975 4.544l.00105.00105zM15.9845 8.20693c-.13244-.2871-.2654-.76228-.2495-1.04197.22247-.0053.6505.0784.7183.0943-.0265.13136-.04026.41953-.04026.4566.04238-.0731.15997-.32418.20765-.42377.428.08157.99058.21824 1.32007.37186-.38776.2511-1.04515.5239-1.95628.54297zm-7.07214-1.9516c-.48483-.1739-.48483-.61095 0-.78484.48484-.1739 1.09417.04464 1.09417.3924 0 .34777-.60933.5663-1.09417.39242zm1.61647.1622c0-.96003-1.04643-1.5633-1.87905-1.0833-.83262.48002-.83262 1.68657 0 2.16658.83262.48003 1.87905-.12325 1.87905-1.08328zm2.7832-1.5749c-1.56482 1.586-.94716 3.5926-.37718 4.49844-.81048 1.3487-2.4039 2.2704-4.25476 2.68995 2.07758 0 3.3002-.53502 4.01108-1.0584.45345-.33478.69924-.66427.8253-.84755 3.0809.19917 7.95862 1.19188 8.43432 1.5129.1907.12925.38776.41424.41742.68758-2.3149-.3242-6.4881-.66534-7.58038-.72255.77552.1102 6.433 1.1813 7.41405 1.43238-.29878.4863-.97895.8306-2.00344.59118.5541.75433-.52125 1.6591-2.01932 1.16116.3295.74056-1.0033 1.40695-2.51938.63567.01907.74055-1.88052.82636-2.63062.0074.01484.09748.10383.28394.14197.36658-.24155 2.1634-2.014 3.50573-3.82885 3.50573-4.44335 0-8.3146-3.60955-8.3146-8.411 0-5.07582 3.75154-8.86443 8.27858-8.86443 2.59354 0 3.7653 2.04157 4.0058 2.81497z"/></svg>
```

partials/icons/social/buffer.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.784 18.24c.287.142.287.267 0 .374l-11.357 5.223c-.287.145-.57.145-.854 0L.213 18.614c-.284-.107-.284-.232 0-.375l2.722-1.23c.284-.14.57-.14.852 0l7.787 3.573c.285.14.57.14.854 0l7.787-3.574c.283-.14.568-.14.852 0l2.717 1.23zm0-6.454c.287.143.287.285 0 .426L12.427 17.44c-.287.104-.57.104-.854 0L.213 12.21c-.284-.143-.284-.284 0-.426l2.722-1.227c.284-.144.57-.144.852 0l7.787 3.57c.285.144.57.144.854 0l7.787-3.57c.283-.144.568-.144.852 0l2.717 1.226zM.214 5.76c-.285-.143-.285-.267 0-.375L11.574.16c.283-.14.57-.14.852 0l11.358 5.23c.287.107.287.232 0 .375l-11.357 5.223c-.287.143-.57.143-.854 0L.213 5.76z"/></svg>
```

partials/icons/social/buymeacoffee.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M6.898 0L5.682 2.799H3.877v2.523h.695L5.277 9.8H4.172l1.46 8.23.938-.01L7.512 24h8.918l.062-.4.88-5.58.888.01 1.46-8.231h-1.056l.705-4.477h.756V2.8h-1.918L16.99 0H6.898zm.528.805h9.043l.771 1.78H6.652l.774-1.78zm-2.75 2.797H19.32v.92H4.676v-.92zm.453 6.998h13.635l-1.176 6.62-5.649-.06-5.636.06-1.174-6.62z"/></svg>
```

partials/icons/social/buzzfeed.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 12c0 6.627-5.373 12-12 12S0 18.627 0 12 5.373 0 12 0s12 5.373 12 12zm-4.148-.273l-.977-6.94-6.5 2.624 2.575 1.487-2.435 4.215L8.3 10.68l-4.153 7.19 2.327 1.346 2.812-4.868L13.5 16.78l3.777-6.54 2.575 1.487z"/></svg>
```

partials/icons/social/cashapp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.59 3.47A5.1 5.1 0 0 0 20.54.42C19.23 0 18.04 0 15.62 0H8.36c-2.4 0-3.61 0-4.9.4A5.1 5.1 0 0 0 .41 3.46C0 4.76 0 5.96 0 8.36v7.27c0 2.41 0 3.6.4 4.9a5.1 5.1 0 0 0 3.05 3.05c1.3.41 2.5.41 4.9.41h7.28c2.41 0 3.61 0 4.9-.4a5.1 5.1 0 0 0 3.06-3.06c.41-1.3.41-2.5.41-4.9V8.38c0-2.41 0-3.61-.41-4.91zM17.42 8.1l-.93.93a.5.5 0 0 1-.67.01 5 5 0 0 0-3.22-1.18c-.97 0-1.94.32-1.94 1.21 0 .9 1.04 1.2 2.24 1.65 2.1.7 3.84 1.58 3.84 3.64 0 2.24-1.74 3.78-4.58 3.95l-.26 1.2a.49.49 0 0 1-.48.39H9.63l-.09-.01a.5.5 0 0 1-.38-.59l.28-1.27a6.54 6.54 0 0 1-2.88-1.57v-.01a.48.48 0 0 1 0-.68l1-.97a.49.49 0 0 1 .67 0c.91.86 2.13 1.34 3.39 1.32 1.3 0 2.17-.55 2.17-1.42 0-.87-.88-1.1-2.54-1.72-1.76-.63-3.43-1.52-3.43-3.6 0-2.42 2.01-3.6 4.39-3.71l.25-1.23a.48.48 0 0 1 .48-.38h1.78l.1.01c.26.06.43.31.37.57l-.27 1.37c.9.3 1.75.77 2.48 1.39l.02.02c.19.2.19.5 0 .68z"/></svg>
```

partials/icons/social/castro.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.372 0 0 5.373 0 12s5.372 12 12 12c6.627 0 12-5.373 12-12S18.627 0 12 0zm-.002 13.991a2.052 2.052 0 1 1 0-4.105 2.052 2.052 0 0 1 0 4.105zm4.995 4.853l-2.012-2.791a5.084 5.084 0 1 0-5.982.012l-2.014 2.793A8.526 8.526 0 0 1 11.979 3.42a8.526 8.526 0 0 1 8.526 8.526 8.511 8.511 0 0 1-3.512 6.898z"/></svg>
```

partials/icons/social/codecov.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.007.48C5.391.485.005 5.831 0 12.399v.03l2.042 1.191.028-.019a5.821 5.821 0 0 1 3.308-1.02c.371 0 .734.034 1.086.1l-.036-.006a5.69 5.69 0 0 1 2.874 1.431l-.004-.003.35.326.198-.434c.192-.42.414-.814.66-1.173.099-.144.208-.29.332-.446l.205-.257-.252-.211a8.33 8.33 0 0 0-3.836-1.807l-.052-.008a8.566 8.566 0 0 0-4.081.251l.061-.016c.971-4.257 4.714-7.224 9.133-7.227a9.31 9.31 0 0 1 6.601 2.713 9.197 9.197 0 0 1 2.508 4.499 8.386 8.386 0 0 0-2.498-.379h-.154c-.356.006-.7.033-1.037.078l.045-.005-.042.006a8.104 8.104 0 0 0-.39.06c-.057.01-.114.022-.17.033a8.103 8.103 0 0 0-.392.089l-.138.035a9.21 9.21 0 0 0-.483.144l-.029.01c-.355.12-.709.268-1.051.439l-.027.014c-.152.076-.305.16-.469.256l-.036.022a8.217 8.217 0 0 0-2.108 1.801l-.011.013-.075.092a8.346 8.346 0 0 0-.378.503c-.088.13-.177.269-.288.452l-.06.104a8.986 8.986 0 0 0-.234.432l-.016.029c-.17.341-.317.698-.44 1.063l-.017.053a8.053 8.053 0 0 0-.411 2.717v-.007l.001.112c.006.158.013.295.023.431l-.002-.037a11.677 11.677 0 0 0 .042.412l.005.042.013.103c.018.127.038.252.062.378.241 1.266.845 2.532 1.745 3.66l.041.051.042-.05c.359-.424 1.249-1.77 1.325-2.577l.001-.015-.007-.013a5.56 5.56 0 0 1-.64-2.595v-.001c0-3.016 2.371-5.521 5.397-5.702l.199-.007a5.93 5.93 0 0 1 3.47 1.025l.028.019 2.041-1.187v-.03a11.771 11.771 0 0 0-3.511-8.424A11.963 11.963 0 0 0 12.008.48z"/></svg>
```

partials/icons/social/codeigniter.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M8.49 24c-1.54-.68-2.586-2.146-2.723-3.824.09-1.727 1.002-3.305 2.45-4.246-.238.58-.18 1.24.15 1.77.376.525 1.022.777 1.655.646.902-.254 1.43-1.19 1.176-2.092-.09-.316-.27-.602-.516-.818-1.02-.83-1.532-2.133-1.35-3.436.175-.69.557-1.314 1.096-1.785-.405 1.08.737 2.146 1.504 2.67 1.36.816 2.67 1.713 3.924 2.686 1.37 1.08 2.117 2.77 2 4.5-.308 1.84-1.61 3.36-3.385 3.93 3.55-.79 7.21-3.61 7.28-7.61-.07-3.2-1.98-6.072-4.9-7.38h-.13c.065.157.096.326.09.496.01-.11.01-.22 0-.33.016.13.016.26 0 .39-.222.91-1.14 1.47-2.052 1.248-.364-.09-.69-.295-.924-.59-1.17-1.5 0-3.207.196-4.857.12-2.11-.844-4.127-2.554-5.36.856 1.427-.284 3.3-1.113 4.366-.83 1.066-2.03 1.86-3.008 2.79-1.054.98-2.02 2.058-2.887 3.21-1.874 2.29-2.61 5.31-2 8.205.836 2.79 3.155 4.886 6.015 5.43H8.5z"/></svg>
```

partials/icons/social/codepen.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 8.182l-.018-.087-.017-.05c-.01-.024-.018-.05-.03-.075-.003-.018-.015-.034-.02-.05l-.035-.067-.03-.05-.044-.06-.046-.045-.06-.045-.046-.03-.06-.044-.044-.04-.015-.02L12.58.19c-.347-.232-.796-.232-1.142 0L.453 7.502l-.015.015-.044.035-.06.05-.038.04-.05.056-.037.045-.05.06c-.02.017-.03.03-.03.046l-.05.06-.02.06c-.02.01-.02.04-.03.07l-.01.05C0 8.12 0 8.15 0 8.18v7.497c0 .044.003.09.01.135l.01.046c.005.03.01.06.02.086l.015.05c.01.027.016.053.027.075l.022.05c0 .01.015.04.03.06l.03.04c.015.01.03.04.045.06l.03.04.04.04c.01.013.01.03.03.03l.06.042.04.03.01.014 10.97 7.33c.164.12.375.163.57.163s.39-.06.57-.18l10.99-7.28.014-.01.046-.037.06-.043.048-.036.052-.058.033-.045.04-.06.03-.05.03-.07.016-.052.03-.077.015-.045.03-.08v-7.5c0-.05 0-.095-.016-.14l-.014-.045.044.003zm-11.99 6.28l-3.65-2.44 3.65-2.442 3.65 2.44-3.65 2.44zm-1.034-6.674l-4.473 2.99L2.89 8.362l8.086-5.39V7.79zm-6.33 4.233l-2.582 1.73V10.3l2.582 1.726zm1.857 1.25l4.473 2.99v4.82L2.89 15.69l3.618-2.417v-.004zm6.537 2.99l4.474-2.98 3.613 2.42-8.087 5.39v-4.82zm6.33-4.23l2.583-1.72v3.456l-2.583-1.73zm-1.855-1.24L13.042 7.8V2.97l8.085 5.39-3.612 2.415v.003z"/></svg>
```

partials/icons/social/codewars.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M.76 12.2l-.08-.04c-.18-.1-.32-.25-.42-.44-.14-.26-.2-.5-.2-.75l.02-.13c0-.2.05-.38.14-.55l.08-.15c.04-.08.1-.15.15-.22.06-.07.07-.16.05-.24l-.05-.16c-.06-.2-.1-.4-.1-.6L.32 8.8c0-.22.06-.44.2-.6l.1-.13c.07-.1.18-.16.3-.2.1-.03.17-.13.18-.25l.02-.34c0-.27.13-.52.33-.7l.24-.18c.05-.05.1-.1.14-.18.05-.06.06-.14.05-.2-.02-.1 0-.13.05-.14.16.06.26.04.33-.04l.13-.17.36-.4c.1-.1.14-.28.08-.42l-.12-.26c-.02-.06 0-.13.05-.15.13 0 .22.05.26.13l.04.07c.06.12.2.18.3.13.22-.08.4-.1.57-.1h.32c.22 0 .4-.15.44-.38.04-.28.14-.5.28-.65.15-.17.32-.3.52-.4.26-.14.42-.34.47-.6.07-.32.24-.55.47-.7l.76-.43.22-.13c.13-.08.25-.18.35-.3l.2-.24c.1-.1.2-.17.32-.2.1-.03.24-.05.36-.04l.4.03c.2 0 .36.05.52.12l.1.05c.1.04.2.02.25-.05L10 .7l.43-.45c.1-.1.22-.14.35-.12.13.02.26.07.38.13.18.1.33.14.5.14h.1c.22 0 .44.03.66.08l.15.04c.15.04.3-.02.4-.14.03-.05.1-.06.14-.02.03.02.04.04.05.07.02.2.14.35.3.4l.16.05c.17.05.32.16.42.3.1.15.22.3.36.4l.1.1c.1.1.24.14.38.13h.59c.24 0 .47.04.7.14.22.1.45.12.66.04.22-.07.45-.1.68-.07l.43.07c.2.02.4.12.52.27l.05.05c.1.1.2.23.3.37.06.13.2.2.34.2h.62c.15 0 .3.03.42.1.13.1.24.2.34.3l.1.13c.12.14.18.33.17.53 0 .16.12.3.28.3l.2.02c.14 0 .26.1.33.23l.1.2.26.58c.04.1.05.2.04.28 0 .1.03.18.1.22l.1.07c.13.1.2.25.18.42l-.07.47-.02.2c-.02.1.03.23.12.3.15.1.22.23.23.38v.2c0 .1-.02.22-.1.3-.06.08-.1.18-.1.3l.03.23c0 .16.1.3.2.4.14.1.22.26.24.42.04.25.05.45.05.65v.23c0 .08 0 .16.03.24.02.07.07.14.13.18l.2.15c.2.13.34.3.42.53.1.22.13.45.13.68v.08c0 .18-.02.37-.08.54-.05.18-.04.35.03.5.08.14.13.3.15.47.04.2.02.4-.05.56l-.02.07c-.05.12-.13.23-.23.32-.1.1-.2.16-.26.23-.06.06-.1.16-.07.25l.03.14c.05.2.05.4 0 .58v.08c-.04.15-.1.28-.16.4-.07.13-.17.23-.3.3l-.15.1c-.07.04-.12.13-.12.22 0 .1-.04.2-.1.26l-.15.2c-.1.13-.23.24-.37.3-.14.1-.26.2-.35.3-.1.12-.18.26-.22.4-.04.18-.18.28-.33.28h-.54c-.14 0-.27.1-.33.22-.07.16-.14.27-.23.37-.1.1-.16.22-.2.36-.02.12-.12.2-.22.16-.13-.06-.26 0-.32.1-.12.2-.24.35-.37.48l-.07.06c-.13.1-.3.18-.45.18-.18 0-.27.08-.3.2-.03.1-.05.23-.06.34-.02.12-.06.23-.1.33l-.05.06c-.1.15-.18.3-.28.43l-.04.06c-.13.17-.3.3-.5.35-.24.08-.45.1-.66.1h-.14c-.1 0-.2.06-.27.16l-.06.1-.06.12-.13.22c-.1.18-.25.3-.45.36-.2.05-.43.07-.64.06l-.16-.02c-.14 0-.27-.04-.4-.1-.1-.04-.24 0-.3.1-.1.14-.22.22-.35.26l-.3.1c-.2.05-.42.05-.63 0l-.16-.05c-.1 0-.2-.05-.28-.1-.1-.05-.2-.07-.3-.06l-.13.02c-.2.02-.38 0-.56-.05l-.27-.06c-.12-.04-.23-.12-.3-.23-.05-.1-.16-.18-.3-.2H9.9c-.2-.03-.38-.1-.5-.25L9 22.5l-.14-.12-.22-.16-.13-.1c-.15-.1-.33-.18-.52-.2l-.6-.1c-.06 0-.1-.02-.16-.03L7 21.74c-.1-.02-.2-.1-.27-.2-.06-.1-.17-.14-.27-.1-.2.08-.36.1-.52.13H5.8c-.26.02-.5-.02-.74-.13-.24-.1-.4-.25-.55-.44-.12-.17-.3-.3-.52-.34l-.28-.06c-.2-.04-.4-.12-.58-.24-.2-.14-.3-.27-.38-.43-.08-.15-.13-.32-.14-.5v-.08c-.02-.2-.16-.38-.35-.43-.23-.07-.4-.17-.55-.3-.14-.13-.22-.32-.22-.52l.02-.44c0-.17-.05-.32-.17-.43-.12-.12-.2-.27-.2-.43l-.03-.36c-.02-.26-.07-.52-.13-.78-.06-.23.03-.46.22-.57l.07-.05c.1-.07.14-.2.08-.32l-.08-.1c-.1-.1-.2-.17-.3-.2-.08-.02-.1-.1-.1-.15l.1-.12c.06-.07.05-.18 0-.24-.08-.08-.12-.18-.13-.28l-.02-.7c0-.14.02-.28.06-.42.04-.12 0-.26-.12-.32zm9.9-1.32c.07-.07.06-.2 0-.25-.1-.08-.17-.17-.23-.27l-.1-.16c-.07-.13-.16-.24-.26-.34l-.02-.02c-.1-.08-.17-.18-.23-.3-.05-.1-.05-.2 0-.3l.06-.1c.06-.1.1-.24.1-.36v-.04c0-.1-.04-.2-.1-.3-.04-.08-.08-.18-.1-.28V8.1c-.03-.12 0-.25.08-.35.08-.13.14-.25.17-.4v-.02c.04-.1.02-.23-.04-.33s-.08-.2-.04-.32l.07-.2c.06-.18.15-.34.27-.48l.14-.15.1-.12.06-.06c.06-.06.07-.16.02-.24-.05-.1-.08-.2-.06-.3l.02-.14c.03-.2.1-.4.23-.56l.04-.04c.15-.2.34-.33.56-.4l.27-.1c.12-.04.2-.17.2-.3 0-.16.05-.3.14-.43l.05-.05c.1-.17.22-.34.3-.52l.07-.13c.02-.03.03-.07.03-.1 0-.17-.1-.32-.26-.33L11.76 2c-.25-.02-.5 0-.74 0l-.85.1c-.13 0-.23.1-.24.24 0 .14-.1.26-.22.3l-.36.1-.1.03-.3.1c-.22.07-.4.23-.5.45l-.08.13c-.1.22-.27.4-.48.53-.2.13-.3.34-.32.58v.1c-.02.2-.08.4-.2.54l-.05.08c-.08.1-.1.23-.05.34.05.12.08.25.07.38v.53c0 .14-.1.26-.2.3-.14.05-.23.16-.27.3l-.05.2c-.04.2.03.4.2.52.16.12.26.3.3.52v.18c.03.2.14.4.32.5.18.12.32.3.4.5l.05.16c.08.22.26.35.46.37h.06c.18 0 .34.1.44.26.1.16.26.27.44.3l.28.08c.17.05.33.14.46.27l.02.02c.1.08.26.07.35-.04l.07-.08zm1.14-.92c.1.06.2.03.24-.06l.03-.05c.07-.14.16-.28.26-.4l.2-.3c.03 0 .04-.02.05-.04l.24-.32c.1-.1.22-.17.36-.17.13 0 .24-.07.3-.2.04-.14.1-.27.22-.38l.05-.06c.1-.1.2-.15.3-.2.13-.02.25-.04.37-.04h.3c.12 0 .22-.05.28-.15.06-.1.15-.17.25-.22l.1-.04c.16-.07.34-.12.52-.14l.2-.02c.12 0 .25 0 .37.07.1.07.23.06.33-.02l.07-.04c.15-.1.32-.18.5-.2h.02c.2-.04.38-.04.58-.03h.1c.2.03.37.1.5.25l.03.04c.1.1.26.18.4.18h.17c.05 0 .1-.02.13-.07.03-.03.08-.06.13-.06h.1c.14 0 .27.04.4.08l.17.07c.16.05.33.1.5.12h.12c.08 0 .13-.05.13-.12 0-.1-.02-.2-.07-.28L20.68 7c-.08-.13-.14-.27-.2-.4l-.02-.05c-.05-.1-.05-.2 0-.3V6.2c.02-.08-.02-.17-.1-.2L20.28 6c-.16-.05-.3-.14-.4-.27l-.1-.1c-.1-.1-.16-.25-.2-.4-.05-.13-.16-.23-.3-.23h-.42c-.15-.02-.28-.1-.37-.22l-.04-.05c-.07-.1-.13-.22-.17-.34-.05-.1-.16-.16-.26-.13l-.12.04c-.2.07-.4.1-.6.08l-.16-.02c-.17 0-.33-.07-.46-.17l-.1-.07c-.08-.06-.16-.1-.25-.14-.1-.04-.18-.02-.24.05l-.05.06c-.1.1-.24.18-.38.2l-.54.03c-.1 0-.2.05-.27.12-.08.07-.17.12-.27.14h-.02c-.1 0-.2.07-.3.14v.02c-.1.1-.23.15-.36.15l-.04.02c-.12 0-.24 0-.36.03h-.12c-.17.03-.3.17-.34.35l-.04.23c-.03.16-.1.3-.2.43-.1.12-.22.2-.37.2h-.15-.02c-.1.02-.2.13-.18.25.02.17 0 .32-.03.47l-.04.17c-.04.15-.14.27-.27.32l-.06.03h-.02c-.06.04-.1.13-.05.2.06.1.08.2.07.3l-.03.32c0 .12-.05.23-.1.33-.06.1-.06.2-.02.3l.1.22c.05.1.06.2.03.32-.03.1-.05.2-.04.3 0 .1.06.2.14.24l.02.02zm7.9 7.23c.1.1.25.14.37.06l.2-.13c.1-.07.18-.17.22-.3v-.02l.1-.3.06-.1.04-.1.04-.07c.04-.08.1-.14.2-.17l.04-.02c.08-.02.13-.1.13-.18 0-.1.05-.18.1-.25l.08-.07.2-.26v-.02c.06-.08.1-.17.12-.27.02-.1 0-.2-.04-.3l-.02-.04c-.04-.1-.06-.17-.07-.26l-.03-.28-.03-.3c0-.1.04-.2.1-.3.07-.08.12-.18.16-.28v-.04l.02-.02c.02-.1-.03-.2-.12-.2-.1-.05-.2-.13-.23-.25l-.03-.06c-.05-.18-.08-.36-.08-.54l.02-.5v-.03c0-.17-.14-.3-.3-.3h-.02c-.2 0-.36-.06-.5-.2l-.08-.1-.2-.23-.26-.3c-.1-.14-.2-.26-.33-.38-.1-.1-.25-.2-.4-.22l-.2-.03c-.1-.02-.23-.07-.34-.14-.08-.06-.2-.04-.28.04l-.13.14-.06.04c-.07.02-.14-.02-.17-.1-.04-.12-.04-.26.02-.38v-.06c0-.07-.06-.12-.12-.1h-.16c-.18 0-.36-.02-.53-.1l-.1-.04c-.1-.05-.22-.08-.33-.08-.1 0-.2.02-.3.08l-.04.03c-.12.08-.26.12-.4.13h-.33c-.15 0-.3.05-.4.13-.13.08-.27.13-.42.16l-.27.04c-.12.03-.25.08-.36.17-.1.1-.24.16-.37.2l-.05.02c-.16.05-.3.15-.4.3l-.12.12c-.07.1-.07.22 0 .32.06.1.18.13.3.1l.15-.06c.08-.03.17 0 .24.04.06.05.15.08.24.07l.25-.03c.14 0 .28 0 .42.04.15.05.28.1.4.2s.25.14.4.16c.15.02.3.05.44.1l.1.02c.1.03.18.1.24.2.05.08.1.2.1.3v.03c0 .12.1.2.2.2h.06c.16 0 .33.02.5.07l.07.03c.1.04.2.1.27.2.08.1.13.2.16.3l.03.14c.03.15.04.3.04.46v.05c0 .1.07.2.18.24.1.02.22.06.33.12l.05.02c.13.08.26.18.36.3l.05.07c.13.15.2.34.2.53v.07c0 .15-.03.3-.08.44-.04.12 0 .26.13.3l.07.05c.15.06.28.17.38.3.1.15.14.32.14.5v.3c-.02.1-.05.18-.1.25s-.05.17 0 .24l.06.1zm-6.4-5.12h-.02c-.04 0-.06.05-.05.1l.04.2c.04.16.06.32.08.48.02.16.1.3.22.4h.04c.15.12.24.3.25.48v.5c-.02.1 0 .2.06.28l.05.05c.1.12.14.26.15.4l.03.55c0 .13-.08.24-.2.26l-.1.02c-.07 0-.1.08-.1.15 0 .08.03.17.06.25v.02c.03.1.04.2.03.3l-.04.27c-.04.2-.1.38-.2.56l-.07.12c-.05.1-.12.16-.2.2-.1.04-.17.12-.2.22l-.08.36c-.05.2-.14.4-.26.6h-.02c-.12.16-.27.3-.45.4l-.12.08-.3.15c-.1.04-.16.13-.18.24l-.05.33c-.03.2-.1.37-.24.5l-.13.15-.15.15L11 21c-.12.14-.3.2-.5.17l-.36-.07-.33-.04h-.09c-.04.04-.05.1-.02.16.07.12.18.2.3.2l.22.04c.1 0 .22.05.32.1.1.07.2.12.32.15h.02c.13.05.27.06.4.05l.15-.02c.17-.02.33 0 .47.06l.12.04c.05.02.13 0 .18-.05.06-.06.12-.1.2-.13l.08-.02c.13-.04.26-.06.4-.06h.08c.12 0 .23.02.33.08l.04.02c.07.03.15 0 .2-.06.03-.07.1-.14.17-.2l.25-.17.16-.1.08-.05c.1-.07.24-.1.36-.1l.36-.03c.14-.02.26-.12.3-.26.04-.15.1-.3.2-.43s.2-.24.3-.34c.13-.1.26-.15.4-.16h.08c.16-.03.28-.18.27-.34v-.02V18.77c.02-.1.06-.23.12-.33l.2-.3.08-.1c.06-.05.1-.12.17-.2l.1-.13c.06-.1.06-.23-.02-.32-.1-.1-.15-.24-.17-.38v-.04c-.02-.16-.02-.33.03-.5v-.05c.05-.13.12-.26.2-.38.08-.1.07-.24-.03-.32l-.17-.15c-.14-.12-.22-.3-.24-.48l-.02-.2c0-.06 0-.13-.02-.2l-.02-.15c-.02-.17-.12-.3-.26-.4l-.07-.02c-.1-.06-.2-.15-.28-.27-.08-.1-.12-.24-.15-.38l-.03-.17c0-.06-.04-.1-.1-.13l-.16-.05-.32-.1c-.1-.02-.2-.1-.27-.17h-.02c-.06-.08-.16-.08-.22-.02l-.1.1c-.02.03-.04.04-.07.03-.06 0-.1-.05-.08-.1.02-.16-.04-.32-.17-.42l-.13-.1-.3-.2c-.08-.03-.2 0-.24.1l-.04.06c0 .02-.03.03-.04.04-.04 0-.1 0-.1-.05l-.03-.05c-.03-.06-.1-.1-.16-.12zm-1.2 1l-.05-.05c-.05-.04-.1-.03-.15.02-.07.12-.13.25-.16.38v.02c-.03.13-.15.22-.27.2h-.1-.02c-.14 0-.25.12-.25.26 0 .18-.06.36-.17.5l-.06.06c-.1.13-.25.22-.4.27l-.08.02c-.1.03-.18.1-.2.22 0 .1-.06.2-.14.28l-.1.08c-.12.13-.3.2-.48.22l-.5.05c-.16 0-.3.1-.4.25-.1.15-.25.25-.4.27l-.22.02c-.16.02-.33.02-.5-.02l-.1-.02-.27-.07c-.1-.03-.18 0-.24.07l-.1.13c-.13.15-.32.22-.5.2l-.65-.08c-.1 0-.18-.05-.27-.1-.1-.06-.17-.13-.24-.2l-.25-.3c-.03-.02-.08-.03-.13-.02l-.14.06-.56.14c-.1.03-.23 0-.33-.06-.1-.08-.22-.1-.34-.1H3.2c-.12.03-.2.16-.16.28l.04.2c.03.1.02.22-.03.32s-.04.2.03.3l.06.08c.08.12.2.22.3.32.1.1.2.2.28.33l.15.27c.08.14.2.22.36.22.15 0 .3.05.42.15l.3.28c.08.07.2.08.28.02l.05-.02c.06 0 .1.04.1.1v.05c0 .13.1.25.23.3l.45.1c.16.05.32.1.47.2h.08c.08 0 .15-.07.14-.16v-.35c0-.1.04-.2.12-.24l.05-.02c.05.02.1.06.08.1v.17c0 .13.04.25.13.34.1.1.23.12.34.08.12-.05.24-.06.37-.05l.37.02c.18.02.35 0 .5-.07.18-.06.33-.14.47-.25l.06-.04.3-.27c.1-.1.23-.15.35-.15h.4c.2-.02.38-.2.4-.4l.04-.2c0-.13.06-.25.15-.35.1-.1.2-.16.3-.2l.12-.05c.17-.07.3-.22.36-.4l.06-.24c.05-.2.15-.4.3-.53l.02-.02c.12-.1.14-.3.06-.44l-.03-.07c-.07-.1-.08-.25-.03-.38.05-.14.1-.26.18-.38l.1-.14c.04-.08.04-.2-.02-.27-.06-.08-.1-.18-.1-.28l-.02-.14v-.34c.02-.1 0-.23-.03-.33l-.04-.12zm-1.43-.76v-.03c0-.1-.06-.16-.14-.16h-.26c-.1.02-.2.02-.28 0h-.45c-.23 0-.45-.04-.67-.1l-.24-.06-.2-.06-.45-.15c-.24-.07-.42-.23-.53-.45l-.05-.1c-.07-.15-.22-.23-.37-.2-.17 0-.34 0-.5-.08l-.12-.05c-.23-.1-.4-.3-.4-.57l-.04-.27c-.03-.14-.12-.27-.24-.32-.14-.06-.27-.14-.4-.23l-.05-.03c-.15-.12-.28-.28-.35-.47l-.02-.06c-.05-.16-.06-.33-.02-.5l.02-.06c.04-.13.05-.26.05-.4 0-.12-.05-.24-.14-.33l-.14-.13c-.16-.13-.26-.32-.27-.53-.02-.22-.02-.43.02-.64V6.3v-.03c0-.12-.1-.2-.2-.2H4.2c-.13 0-.24.08-.3.2-.05.14-.13.25-.22.36l-.04.05-.2.2-.1.1c-.1.1-.16.25-.18.4-.02.15-.06.3-.12.44l-.02.05c-.05.12-.13.23-.23.3-.1.08-.17.2-.17.32l-.02.46c0 .2-.03.4-.1.6l-.02.08c-.05.13 0 .27.12.33l.42.18.04.02c.03 0 .04.02.05.05.03.04 0 .1-.03.1l-.1.05c-.06.02-.1.08-.12.15l-.02.1v.02l-.1.56c-.02.08-.02.17-.02.26 0 .08.05.15.12.18l.22.1c.1.06.22.13.3.2l.1.08c.03.04.08.08.12.1l.04.04c.07.06.12.14.14.23l.1.45c0 .12.1.22.2.25l.16.05s.03 0 .05.02l.2.06c.16.05.3.14.42.26.12.1.24.23.34.37l.04.04c.08.1.2.15.32.12s.25-.04.38-.04h.15c.1 0 .23.03.34.1.1.06.23.1.35.15h.03c.12.05.25.03.35-.04.1-.08.23-.12.36-.12l.47.03c.1 0 .2-.02.25-.1h.02l.17-.16.05-.05c.08-.1.2-.14.32-.15h.45c.12 0 .23-.1.28-.2.05-.1.15-.18.27-.2l.2-.04c.08 0 .15-.07.18-.16.03-.1.08-.18.15-.24l.16-.16c.1-.1.15-.2.17-.32z"/></svg>
```

partials/icons/social/dailymotion.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.068 11.313c-1.754 0-3.104 1.427-3.104 3.11 0 1.753 1.35 3.085 3.255 3.085l-.016.002c1.59 0 2.925-1.31 2.925-3.04 0-1.8-1.336-3.157-3.062-3.157zM0 0v24h24V0H0zm20.693 20.807h-3.576v-1.41c-1.1 1.08-2.223 1.47-3.715 1.47-1.522 0-2.832-.495-3.93-1.485-1.448-1.275-2.198-2.97-2.198-4.936 0-1.8.7-3.414 2.01-4.674 1.17-1.146 2.595-1.73 4.185-1.73 1.52 0 2.69.513 3.53 1.59V4.157l3.693-.765V3.39l.002.003h-.002v17.414z"/></svg>
```

partials/icons/social/debian.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.88 12.68c-.4 0 .08.2.6.28.14-.1.27-.22.39-.33a3 3 0 0 1-.99.05M16.02 12.15c.23-.33.4-.69.47-1.06-.06.27-.2.5-.33.73-.75.47-.07-.27 0-.56-.8 1.01-.11.6-.14.89M16.8 10.1c.05-.72-.14-.5-.2-.22.07.04.13.5.2.22M12.38.31c.2.04.45.07.42.12.23-.05.28-.1-.43-.12M12.8.43l-.15.03.14-.01V.43M19.42 10.37c.02.64-.2.95-.38 1.5l-.35.18c-.28.54.03.35-.17.78-.44.39-1.34 1.22-1.62 1.3-.2 0 .14-.25.19-.34-.59.4-.48.6-1.37.85l-.03-.06c-2.22 1.04-5.3-1.02-5.25-3.84-.03.17-.07.13-.12.2a3.55 3.55 0 0 1 2-3.5 3.36 3.36 0 0 1 3.73.48 3.34 3.34 0 0 0-2.72-1.3c-1.18.01-2.28.76-2.65 1.57-.6.38-.67 1.47-.93 1.66-.36 2.6.66 3.72 2.38 5.04.27.19.08.21.12.35a4.7 4.7 0 0 1-1.53-1.16c.23.33.47.66.8.91-.55-.18-1.27-1.3-1.48-1.35.93 1.66 3.78 2.92 5.26 2.3a6.2 6.2 0 0 1-2.33-.28c-.33-.16-.77-.51-.7-.57a5.8 5.8 0 0 0 5.9-.84c.44-.35.93-.94 1.07-.95-.2.32.04.16-.12.44.44-.72-.2-.3.46-1.24l.24.33c-.09-.6.74-1.32.66-2.26.19-.3.2.3 0 .97.29-.74.08-.85.15-1.46.08.2.18.42.23.63-.18-.7.2-1.2.28-1.6-.09-.05-.28.3-.32-.53 0-.37.1-.2.14-.28-.08-.05-.26-.32-.38-.86.08-.13.22.33.34.34-.08-.42-.2-.75-.2-1.08-.34-.68-.12.1-.4-.3-.34-1.09.3-.25.34-.74.54.77.84 1.96.98 2.46-.1-.6-.28-1.2-.49-1.76.16.07-.26-1.24.21-.37A7.82 7.82 0 0 0 17.7 1.6c.18.17.42.39.33.42-.75-.45-.62-.48-.73-.67-.61-.25-.65.02-1.06 0C15.08.73 14.86.8 13.8.4l.05.23c-.77-.25-.9.1-1.73 0-.05-.04.27-.14.53-.18-.74.1-.7-.14-1.43.03.17-.13.36-.21.55-.32-.6.04-1.44.35-1.18.07C9.6.68 7.85 1.3 6.87 2.22L6.84 2c-.45.54-1.96 1.61-2.08 2.31l-.13.03c-.23.4-.38.85-.57 1.26-.3.52-.45.2-.4.28-.6 1.22-.9 2.25-1.16 3.1.18.27 0 1.65.07 2.76-.3 5.46 3.84 10.77 8.36 12 .67.23 1.65.23 2.49.25-.99-.28-1.12-.15-2.08-.49-.7-.32-.85-.7-1.34-1.13l.2.35c-.97-.34-.57-.42-1.36-.67l.21-.27c-.31-.03-.83-.53-.97-.81l-.34.01c-.41-.5-.63-.87-.61-1.16l-.11.2c-.13-.21-1.52-1.9-.8-1.51-.13-.12-.31-.2-.5-.55l.14-.17c-.35-.44-.64-1.02-.62-1.2.2.24.32.3.45.33-.88-2.17-.93-.12-1.6-2.2l.15-.02c-.1-.16-.18-.34-.26-.51l.06-.6c-.63-.74-.18-3.1-.09-4.4.07-.54.53-1.1.88-1.98l-.21-.04c.4-.71 2.34-2.87 3.24-2.76.43-.55-.09 0-.18-.14.96-.99 1.26-.7 1.9-.88.7-.4-.6.16-.27-.15 1.2-.3.85-.7 2.42-.85.16.1-.39.14-.52.26 1-.49 3.15-.37 4.56.27 1.63.77 3.46 3.01 3.53 5.13l.08.02c-.04.85.13 1.82-.17 2.71l.2-.42M9.54 13.23l-.05.28c.26.35.47.73.8 1.01-.24-.47-.42-.66-.75-1.3M10.16 13.2c-.14-.15-.22-.34-.31-.52.08.32.26.6.43.88l-.12-.36M21.1 10.82l-.07.15c-.1.76-.34 1.51-.69 2.21.4-.73.65-1.54.75-2.36M12.45.12c.27-.1.66-.05.95-.12-.37.03-.74.05-1.1.1l.15.02M3.01 5.14c.07.57-.43.8.11.42.3-.66-.11-.18-.1-.42M2.38 7.8c.12-.39.15-.62.2-.84-.35.44-.17.53-.2.83"/></svg>
```

partials/icons/social/deezer.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.717 18.695h4.375V17.37h-4.377v1.325h.002zm-9.81 0H9.28V17.37H4.906v1.325h.004zm-4.907 0h4.375V17.37H0v1.325zm9.81 0h4.38V17.37H9.81v1.325zm9.815 0H24V17.37h-4.375v1.325zm0-1.724H24v-1.32h-4.375v1.34-.01zm-9.814 0h4.39v-1.32H9.81v1.34-.01zm-9.81 0h4.38v-1.32H0v1.34-.01zm4.91 0h4.38v-1.32H4.91v1.34l.002-.01zm9.83 0h4.38v-1.32h-4.4v1.34l.017-.01zm0-1.72h4.38v-1.32h-4.4v1.33h.017zm-9.805 0h4.36v-1.32H4.91v1.33h.016zm-4.906 0h4.36v-1.32H0v1.33h.016zm9.81 0h4.38v-1.32h-4.4v1.33h.016zm9.825 0H24v-1.32h-4.375v1.33h.027zm0-1.72H24V12.2h-4.375v1.326h.027zm-9.81 0h4.363V12.2h-4.4v1.326h.033zm-9.81 0H4.4V12.2H0v1.326h.03zm14.73 0h4.38V12.2h-4.43v1.326h.044zm0-1.72h4.38v-1.33h-4.43v1.32h.044zm-14.73 0H4.4v-1.32H0v1.32h.03zm9.81 0h4.38v-1.32H9.81v1.32h.032zm9.81 0H24v-1.33h-4.375v1.328l.027-.002zM9.81 10.08h4.38V8.754H9.81v1.326zm9.815-.002H24V8.753h-4.375v1.325zM9.81 8.355h4.38V7.028H9.81v1.327zm9.815 0H24V7.028h-4.375v1.327zm0-1.725H24V5.304h-4.375V6.63z"/></svg>
```

partials/icons/social/delicious.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 12H0v12h12V12zM24 0H12v12h12V0z"/></svg>
```

partials/icons/social/deviantart.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.207 4.794l.23-.43V0H15.07l-.436.44-2.058 3.925-.646.436H4.58v5.993h4.04l.36.436-4.175 7.98-.24.43V24H8.93l.436-.44 2.07-3.925.644-.436h7.35v-5.993h-4.05l-.36-.438 4.186-7.977z"/></svg>
```

partials/icons/social/diaspora.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.26 21.896l-2.332-3.256c-.622-.87-1.127-1.547-1.154-1.547s-1.006 1.314-2.316 3.113C8.21 21.92 7.178 23.32 7.163 23.32c-.033 0-4.498-3.144-4.51-3.177-.006-.016 1.005-1.498 2.242-3.293 1.24-1.795 2.254-3.29 2.254-3.326 0-.055-.408-.193-3.557-1.245L0 11.08c-.03-.018.156-.64.793-2.65.46-1.446.844-2.64.855-2.655.014-.016 1.71.524 3.772 1.205 2.063.68 3.765 1.234 3.788 1.234.022 0 .046-.03.053-.07.01-.03.03-1.786.04-3.9.02-2.1.04-3.84.05-3.87.02-.03.6-.03 2.73-.03 1.484 0 2.713.015 2.733.03.025.016.065 1.186.136 3.78.11 4.275.11 4.335.18 4.335.025 0 1.66-.54 3.63-1.22 1.973-.66 3.592-1.2 3.605-1.186.03.044 1.65 5.31 1.635 5.325-.017.016-1.667.585-3.66 1.26-2.76.93-3.647 1.245-3.647 1.29-.014.03.93 1.455 2.146 3.21 1.184 1.74 2.143 3.165 2.143 3.18-.015.046-4.44 3.302-4.483 3.302-.015 0-.585-.766-1.245-1.695l.005-.067z"/></svg>
```

partials/icons/social/digg.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.76 8.16v8.16h3.84v.96h-3.84v1.92H24V8.16h-6.24zm-7.2 0v8.16h3.84v.96h-3.84v1.92h6.24V8.16h-6.24zM3.84 4.8v3.36H0v8.16h6.24V4.8h-2.4zM9.6 8.16H7.2v8.16h2.4V8.16zm12 6.24h-1.44v-4.32h1.44v4.32zm-17.76 0H2.4v-4.32h1.44v4.32zm10.56 0h-1.44v-4.32h1.44v4.32zM9.6 4.8H7.2v2.4h2.4V4.8z"/></svg>
```

partials/icons/social/discord.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.222 0c1.406 0 2.54 1.137 2.607 2.475V24l-2.677-2.273-1.47-1.338-1.604-1.398.67 2.205H3.71c-1.402 0-2.54-1.065-2.54-2.476V2.48C1.17 1.142 2.31.003 3.715.003h16.5L20.222 0zm-6.118 5.683h-.03l-.202.2c2.073.6 3.076 1.537 3.076 1.537-1.336-.668-2.54-1.002-3.744-1.137-.87-.135-1.74-.064-2.475 0h-.2c-.47 0-1.47.2-2.81.735-.467.203-.735.336-.735.336s1.002-1.002 3.21-1.537l-.135-.135s-1.672-.064-3.477 1.27c0 0-1.805 3.144-1.805 7.02 0 0 1 1.74 3.743 1.806 0 0 .4-.533.805-1.002-1.54-.468-2.14-1.404-2.14-1.404s.134.066.335.2h.06c.03 0 .044.015.06.03v.006c.016.016.03.03.06.03.33.136.66.27.93.4.466.202 1.065.403 1.8.536.93.135 1.996.2 3.21 0 .6-.135 1.2-.267 1.8-.535.39-.2.87-.4 1.397-.737 0 0-.6.936-2.205 1.404.33.466.795 1 .795 1 2.744-.06 3.81-1.8 3.87-1.726 0-3.87-1.815-7.02-1.815-7.02-1.635-1.214-3.165-1.26-3.435-1.26l.056-.02zm.168 4.413c.703 0 1.27.6 1.27 1.335 0 .74-.57 1.34-1.27 1.34-.7 0-1.27-.6-1.27-1.334.002-.74.573-1.338 1.27-1.338zm-4.543 0c.7 0 1.266.6 1.266 1.335 0 .74-.57 1.34-1.27 1.34-.7 0-1.27-.6-1.27-1.334 0-.74.57-1.338 1.27-1.338z"/></svg>
```

partials/icons/social/discourse.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.103 0C18.666 0 24 5.485 24 11.997c0 6.51-5.33 11.99-11.9 11.99L0 24V11.79C0 5.28 5.532 0 12.103 0zm.116 4.563c-2.593-.003-4.996 1.352-6.337 3.57-1.33 2.208-1.387 4.957-.148 7.22L4.4 19.61l4.794-1.074c2.745 1.225 5.965.676 8.136-1.39 2.17-2.054 2.86-5.228 1.737-7.997-1.135-2.778-3.84-4.59-6.84-4.585h-.008z"/></svg>
```

partials/icons/social/disqus.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.438 23.654c-2.853 0-5.46-1.04-7.476-2.766L0 21.568l1.917-4.733C1.25 15.36.875 13.725.875 12 .875 5.564 6.05.346 12.44.346 18.82.346 24 5.564 24 12c0 6.438-5.176 11.654-11.562 11.654zm6.315-11.687v-.033c0-3.363-2.373-5.76-6.462-5.76H7.877V17.83h4.35c4.12 0 6.525-2.5 6.525-5.863h.004zm-6.415 2.998h-1.29V9.04h1.29c1.897 0 3.157 1.08 3.157 2.945v.03c0 1.884-1.26 2.95-3.157 2.95z"/></svg>
```

partials/icons/social/django.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.146 0h3.924v18.165c-2.013.382-3.491.535-5.096.535-4.791 0-7.288-2.166-7.288-6.32 0-4.001 2.65-6.6 6.753-6.6.637 0 1.121.051 1.707.204V0zm0 9.143a3.894 3.894 0 0 0-1.325-.204c-1.988 0-3.134 1.223-3.134 3.364 0 2.09 1.096 3.236 3.109 3.236.433 0 .79-.025 1.35-.102V9.142zM21.314 6.06v9.097c0 3.134-.229 4.638-.917 5.937-.637 1.249-1.478 2.039-3.211 2.905l-3.644-1.733c1.733-.815 2.574-1.529 3.109-2.625.561-1.121.739-2.421.739-5.835V6.059h3.924zM17.39.021h3.924v4.026H17.39V.021z"/></svg>
```

partials/icons/social/dribbble.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 24C5.385 24 0 18.615 0 12S5.385 0 12 0s12 5.385 12 12-5.385 12-12 12zm10.12-10.358c-.35-.11-3.17-.953-6.384-.438 1.34 3.684 1.887 6.684 1.992 7.308 2.3-1.555 3.936-4.02 4.395-6.87zm-6.115 7.808c-.153-.9-.75-4.032-2.19-7.77l-.066.02c-5.79 2.015-7.86 6.025-8.04 6.4 1.73 1.358 3.92 2.166 6.29 2.166 1.42 0 2.77-.29 4-.814zm-11.62-2.58c.232-.4 3.045-5.055 8.332-6.765.135-.045.27-.084.405-.12-.26-.585-.54-1.167-.832-1.74C7.17 11.775 2.206 11.71 1.756 11.7l-.004.312c0 2.633.998 5.037 2.634 6.855zm-2.42-8.955c.46.008 4.683.026 9.477-1.248-1.698-3.018-3.53-5.558-3.8-5.928-2.868 1.35-5.01 3.99-5.676 7.17zM9.6 2.052c.282.38 2.145 2.914 3.822 6 3.645-1.365 5.19-3.44 5.373-3.702-1.81-1.61-4.19-2.586-6.795-2.586-.825 0-1.63.1-2.4.285zm10.335 3.483c-.218.29-1.935 2.493-5.724 4.04.24.49.47.985.68 1.486.08.18.15.36.22.53 3.41-.43 6.8.26 7.14.33-.02-2.42-.88-4.64-2.31-6.38z"/></svg>
```

partials/icons/social/dropbox.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="m6 1.807-6 3.822 6 3.822 6.001-3.822zm12 0-6 3.822 6 3.822 6-3.822zm-18 11.467 6 3.822 6.001-3.822-6.001-3.822zm18-3.822-6 3.822 6 3.822 6-3.822zm-12 8.919 6.001 3.822 6-3.822-6-3.822z"/></svg>
```

partials/icons/social/dtube.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.6 5.5a9.91 9.91 0 0 0-3.88-4.04A11.18 11.18 0 0 0 13.08.04H.18l6.91 4h5.99c1.94 0 3.41.62 4.42 1.88C18.5 7.17 19 9 19 11.43v1.27c-.01 2.34-.53 4.14-1.55 5.4-1.02 1.26-2.5 1.89-4.42 1.89H6.86L0 23.95h13.13c2.09 0 3.97-.49 5.63-1.44 1.66-.95 2.95-2.3 3.87-4.02S24 14.79 24 12.56v-1.1c0-2.22-.47-4.2-1.4-5.96z"/><path d="M.13 3.96v16.1L14.07 12z"/></svg>
```

partials/icons/social/envato.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.4.197c-.74-.371-2.721-.247-5.195.62-4.207 2.968-7.674 7.175-8.044 14.109 0 .241-.493 0-.617-.126-1.114-2.104-1.61-4.455-.62-7.921.247-.247-.37-.617-.37-.494-.249.123-1.114 1.113-1.734 2.103-2.847 4.947-.99 11.511 3.961 14.231 4.947 2.721 11.382.988 14.231-4.086 3.342-5.814.369-17.322-1.612-18.436"/></svg>
```

partials/icons/social/etsy.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M8.564 2.445c0-.325.033-.52.59-.52h7.465c1.3 0 2.02 1.11 2.54 3.193l.42 1.666h1.27c.23-4.728.43-6.784.43-6.784s-3.196.36-5.09.36H6.64L1.526.196v1.37l1.725.326c1.21.24 1.5.496 1.6 1.606 0 0 .11 3.27.11 8.64 0 5.385-.09 8.61-.09 8.61 0 .973-.39 1.333-1.59 1.573l-1.722.33V24l5.13-.165h8.55c1.935 0 6.39.165 6.39.165.105-1.17.75-6.48.855-7.064h-1.2L20 19.846c-1.005 2.28-2.476 2.445-4.11 2.445h-4.906c-1.63 0-2.415-.64-2.415-2.05V12.8s3.62 0 4.79.096c.912.064 1.463.325 1.76 1.598l.39 1.695h1.41l-.09-4.278.192-4.305H15.63l-.45 1.89c-.283 1.244-.48 1.47-1.754 1.6-1.666.17-4.815.14-4.815.14V2.45h-.05z"/></svg>
```

partials/icons/social/evernote.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.692 5.445c0 .239-.02.637-.256.895-.257.24-.652.259-.888.259H4.022c-.73 0-1.165 0-1.46.04-.159.02-.356.1-.455.14-.04.019-.04 0-.02-.02L7.85.848c.02-.02.04-.02.02.02-.04.099-.118.298-.138.457-.04.298-.04.736-.04 1.472v2.647zm5.348 17.869c-.67-.438-1.026-1.015-1.164-1.373a2.924 2.924 0 0 1-.217-1.095 3.007 3.007 0 0 1 3-3.004c.493 0 .888.398.888.895a.88.88 0 0 1-.454.776c-.099.06-.237.1-.336.12-.098.02-.473.06-.65.218-.198.16-.356.418-.356.697 0 .298.118.577.316.776.355.358.829.557 1.342.557a2.436 2.436 0 0 0 2.427-2.447c0-1.214-.809-2.289-1.875-2.766-.158-.08-.414-.14-.651-.2a8.04 8.04 0 0 0-.592-.099c-.829-.1-2.901-.756-3.04-2.606 0 0-.611 2.785-1.835 3.541-.118.06-.276.12-.454.16-.177.04-.374.06-.434.06-1.993.119-4.105-.518-5.565-2.03 0 0-.987-.816-1.5-3.104-.118-.558-.355-1.553-.493-2.488-.06-.338-.08-.597-.099-.836 0-.975.592-1.631 1.342-1.73h4.026c.69 0 1.086-.18 1.342-.419.336-.318.415-.776.415-1.313v-4.08-.118C8.52.669 9.173.052 10.139.052h.474c.197 0 .434.02.651.04.158.02.296.06.533.12 1.204.298 1.46 1.532 1.46 1.532s2.27.398 3.415.597c1.085.199 3.77.378 4.282 3.104 1.204 6.487.474 12.775.415 12.775-.849 6.129-5.901 5.83-5.901 5.83a4.1 4.1 0 0 1-2.428-.736zm4.54-13.034c-.652-.06-1.204.2-1.402.697-.04.1-.079.219-.059.278.02.06.06.08.099.1.237.12.631.179 1.204.239.572.06.967.1 1.223.06.04 0 .08-.02.119-.08.04-.06.02-.18.02-.279-.06-.537-.553-.935-1.204-1.015z"/></svg>
```

partials/icons/social/everplaces.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M10.839 23.972C4.76 23.388 0 18.257 0 12.028c0-6.623 5.377-12 12-12s12 5.377 12 12c0 6.23-4.76 11.359-10.839 11.943v-7.046c2.22-.525 3.87-2.521 3.87-4.897 0-2.778-2.253-5.033-5.031-5.033S6.968 9.25 6.968 12.028c0 2.377 1.653 4.372 3.87 4.897l.001 7.047zm-.388-14.655c.642 0 1.162.521 1.162 1.162 0 .641-.521 1.162-1.162 1.162-.641 0-1.16-.521-1.16-1.162 0-.641.52-1.161 1.16-1.162z"/></svg>
```

partials/icons/social/facebook.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.9981 11.9991C23.9981 5.37216 18.626 0 11.9991 0C5.37216 0 0 5.37216 0 11.9991C0 17.9882 4.38789 22.9522 10.1242 23.8524V15.4676H7.07758V11.9991H10.1242V9.35553C10.1242 6.34826 11.9156 4.68714 14.6564 4.68714C15.9692 4.68714 17.3424 4.92149 17.3424 4.92149V7.87439H15.8294C14.3388 7.87439 13.8739 8.79933 13.8739 9.74824V11.9991H17.2018L16.6698 15.4676H13.8739V23.8524C19.6103 22.9522 23.9981 17.9882 23.9981 11.9991Z"/></svg>
```

partials/icons/social/feedly.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.396 21.932L.62 15.108c-.825-.824-.825-2.609 0-3.39l9.709-9.752c.781-.78 2.521-.78 3.297 0l9.756 9.753c.826.825.826 2.611 0 3.391l-6.779 6.824c-.411.41-1.053.686-1.695.686H9c-.596-.001-1.19-.276-1.604-.688zm6.184-2.656c.137-.138.137-.413 0-.55l-1.328-1.328c-.138-.15-.412-.15-.549 0l-1.329 1.319c-.138.134-.138.405 0 .54l1.054 1.005h1.099l1.065-1.02-.012.034zm0-5.633c.092-.09.092-.32 0-.412l-1.42-1.409c-.09-.091-.32-.091-.412 0l-4.121 4.124c-.139.15-.139.465 0 .601l.959.96h1.102l3.893-3.855v-.009zm0-5.587c.092-.091.137-.366 0-.458l-1.375-1.374c-.09-.104-.365-.104-.502 0l-6.914 6.915c-.094.09-.14.359-.049.449l1.1 1.05h1.053l6.687-6.582z"/></svg>
```

partials/icons/social/figma.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 12a4 4 0 1 1 8 0 4 4 0 0 1-8 0zM4 20a4 4 0 0 1 4-4h4v4a4 4 0 1 1-8 0z"/><path d="M12 0v8h4a4 4 0 1 0 0-8h-4zM4 4a4 4 0 0 0 4 4h4V0H8a4 4 0 0 0-4 4zM4 12a4 4 0 0 0 4 4h4V8H8a4 4 0 0 0-4 4z"/></svg>
```

partials/icons/social/flickr.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 12c0 3.074 2.494 5.564 5.565 5.564 3.075 0 5.569-2.49 5.569-5.564S8.641 6.436 5.565 6.436C2.495 6.436 0 8.926 0 12zm12.866 0c0 3.074 2.493 5.564 5.567 5.564C21.496 17.564 24 15.074 24 12s-2.492-5.564-5.564-5.564c-3.075 0-5.57 2.49-5.57 5.564z"/></svg>
```

partials/icons/social/flipboard.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 0v24h24V0H0zm19.2 9.6h-4.8v4.8H9.6v4.8H4.8V4.8h14.4v4.8z"/></svg>
```

partials/icons/social/foursquare.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.727 3.465l-.535 2.799c-.064.303-.445.623-.801.623H11.41c-.562 0-.963.391-.963.945v.614c0 .569.405.96.966.96h4.23c.395 0 .785.436.697.855l-.535 2.76c-.051.24-.314.63-.785.63h-3.457c-.63 0-.818.091-1.239.601-.42.524-4.206 5.069-4.206 5.069-.037.045-.074.029-.074-.015V3.42c0-.359.311-.78.776-.78h10.274c.375 0 .73.356.633.821v.004zm.451 10.98c.145-.578 1.746-8.784 2.281-11.385M18.486 0H5.683C3.918 0 3.4 1.328 3.4 2.164v20.34c0 .94.504 1.291.789 1.405.284.117 1.069.214 1.541-.328 0 0 6.044-7.014 6.146-7.117.165-.157.165-.157.315-.157h3.914c1.65 0 1.906-1.17 2.086-1.86.15-.569 1.754-8.774 2.279-11.385C20.875 1.08 20.365 0 18.49 0h-.004z"/></svg>
```

partials/icons/social/framer.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4 0h16v8h-8zM4 8h8l8 8H4zM4 16h8v8z"/></svg>
```

partials/icons/social/gatsby.hbs
```
1 | <svg role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12.001.007C5.326.007.007 5.326.007 12S5.326 23.995 12 23.995s11.994-5.319 11.994-11.994S18.676.007 12.001.007zM2.614 12.105l9.283 9.283c-5.111 0-9.283-4.172-9.283-9.283zm11.473 9.074L2.823 9.915C3.76 5.743 7.516 2.614 12 2.614a9.476 9.476 0 0 1 7.614 3.86L18.259 7.62a7.657 7.657 0 0 0-6.362-3.337A7.555 7.555 0 0 0 4.7 9.393l9.804 9.805c2.4-.835 4.276-2.92 4.798-5.424h-4.068v-1.773h6.154c0 4.485-3.129 8.24-7.301 9.178z"/></svg>
```

partials/icons/social/ghost.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M9.604 19.199H.008V24h9.597v-4.801zm14.39 0h-9.591V24h9.591v-4.801zm.003-9.599H0v4.8h23.997V9.6zM24 0h-4.801v4.801H24V0zm-9.596 0H.008v4.801h14.396V0z"/></svg>
```

partials/icons/social/git.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.546 10.93L13.067.452c-.604-.603-1.582-.603-2.188 0L8.708 2.627l2.76 2.76c.645-.215 1.379-.07 1.889.441.516.515.658 1.258.438 1.9l2.658 2.66c.645-.223 1.387-.078 1.9.435.721.72.721 1.884 0 2.604-.719.719-1.881.719-2.6 0-.539-.541-.674-1.337-.404-1.996L12.86 8.955v6.525c.176.086.342.203.488.348.713.721.713 1.883 0 2.6-.719.721-1.889.721-2.609 0-.719-.719-.719-1.879 0-2.598.182-.18.387-.316.605-.406V8.835c-.217-.091-.424-.222-.6-.401-.545-.545-.676-1.342-.396-2.009L7.636 3.7.45 10.881c-.6.605-.6 1.584 0 2.189l10.48 10.477c.604.604 1.582.604 2.186 0l10.43-10.43c.605-.603.605-1.582 0-2.187"/></svg>
```

partials/icons/social/github.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
```

partials/icons/social/gitlab.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.844.904a1.007 1.007 0 00-.955.692l-2.53 7.783c0 .007-.005.012-.007.02L.07 13.335a1.437 1.437 0 00.522 1.607l11.072 8.045a.566.566 0 00.67-.004l11.074-8.04a1.436 1.436 0 00.522-1.61l-1.26-3.867a.547.547 0 00-.031-.104l-2.526-7.775a1.004 1.004 0 00-.957-.684.987.987 0 00-.949.69l-2.406 7.408H8.203l-2.41-7.408a.987.987 0 00-.943-.69h-.006zm-.006 1.42l2.174 6.678H2.674l2.164-6.678zm14.328 0l2.168 6.678h-4.342l2.174-6.678zm-10.594 7.81h6.862l-2.15 6.618L12 20.693 8.572 10.135zm-5.515.005h4.322l3.086 9.5-7.408-9.5zm13.568 0h4.326l-6.703 8.588-.709.914 2.959-9.108.127-.394zM2.1 10.762l6.978 8.947-7.818-5.682a.305.305 0 01-.112-.341l.952-2.924zm19.8 0l.952 2.922a.305.305 0 01-.11.341v.002l-7.82 5.68.025-.035 6.953-8.91Z"/></svg>
```

partials/icons/social/gmail.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 4.5v15c0 .85-.65 1.5-1.5 1.5H21V7.387l-9 6.463-9-6.463V21H1.5C.649 21 0 20.35 0 19.5v-15c0-.425.162-.8.431-1.068C.7 3.16 1.076 3 1.5 3H2l10 7.25L22 3h.5c.425 0 .8.162 1.069.432.27.268.431.643.431 1.068z"/></svg>
```

partials/icons/social/gnusocial.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.217 0C2.474 0 1.06 1.413 1.06 3.156V15.77c0 1.744 1.414 3.158 3.157 3.158h9.367C13.567 22.498 8.756 24 8.756 24s8.138-.038 9.305-5.072h1.72c1.744 0 3.157-1.414 3.157-3.157V3.157C22.938 1.413 21.524 0 19.782 0H4.218zm4.527 2.53c.073-.013.132-.003.174.034.335.3-.556.593-.484 2.063.032.646-.16 1.146 1.076 1.146.826 0 .483-.734 1.523-.734.656 0 .86.435.934.767.072-.33.274-.768.93-.768 1.04 0 .7.733 1.525.733 1.237 0 1.044-.5 1.076-1.146.072-1.47-.82-1.764-.484-2.063.042-.037.1-.042.172-.02.5.143 1.607 1.558 1.638 2.155.038.71.04 1.825-1.015 2.407 1.19 1.167 1.352 2.72 1.352 2.72l-2.045-.034s-.464-2.118-2.94-2.01c-2.474.108-2.796.538-2.796 3.156 0 2.617 1.147 3.517 2.905 3.585 2.76.108 2.51-1.433 2.51-1.433l-1.29.072-.718-1.937h4.41c0 2.116-.897 5.414-5.092 5.2-4.196-.216-5.128-3.515-5.164-5.74-.018-1.225.188-2.602 1.2-3.574-1.052-.58-1.033-1.7-1.033-2.414 0-.88 1.13-2.084 1.637-2.17z"/></svg>
```

partials/icons/social/goldenline.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.377 21.658c0 1.225-.989 2.215-2.212 2.215-1.224 0-2.217-.99-2.217-2.215 0-1.223.993-2.215 2.217-2.215 1.223 0 2.213.993 2.212 2.215zm-4.715-.172L6.47 22.7s-.287.08-.392-.215c-.06-.181.091-.398.091-.398l5.213-8.514s.267-.402.77-.549c.418-.121.872.16.872.16l8.351 5.253s.362.147.348.438c-.015.293-.333.343-.333.343l-5.04 1.178c-.426-.744-1.23-1.244-2.156-1.244-1.32 0-2.413 1.032-2.504 2.335h-.028zM3.898 7.297l1.513-5.263s.072-.303.381-.242c.186.031.303.273.303.273l4.889 8.698s.223.425.106.941c-.099.425-.567.683-.567.683L1.864 17.11s-.307.243-.547.084c-.242-.163-.136-.463-.136-.463l1.472-5.116c1.177-.206 2.071-1.233 2.071-2.47 0-.738-.319-1.396-.826-1.859v.011zm.532 1.858c0 1.225-.989 2.218-2.214 2.218C.995 11.373 0 10.38 0 9.155c0-1.221.995-2.213 2.216-2.213 1.225 0 2.217.992 2.217 2.213H4.43zm15.666-1.734l3.81 4.18s.211.212.003.445c-.124.141-.394.111-.394.111l-9.974-.395s-.478-.035-.853-.402c-.31-.303-.282-.838-.282-.838l.51-9.852s-.05-.389.212-.511c.27-.122.467.129.467.129l3.318 3.628c-.188.35-.293.744-.293 1.17 0 1.381 1.123 2.504 2.509 2.504.341 0 .667-.075.964-.197l.003.028zm1.25-2.317c0 1.229-.986 2.217-2.212 2.217-1.224 0-2.217-.987-2.217-2.217 0-1.215.993-2.201 2.217-2.201 1.223 0 2.213 1.002 2.213 2.217l-.001-.016z"/></svg>
```

partials/icons/social/googleallo.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.665.005c-.702.018-1.417.098-2.14.243C4.788 1.193 1.08 4.974.21 9.728c-1.36 7.406 4.096 14.256 11.16 14.256L22.227 24c.98 0 1.774-.793 1.774-1.774V12C24 5.26 18.445-.18 11.665.005zM12 6.135c3.238 0 5.862 2.626 5.862 5.865v5.61c0 .245-.293.367-.467.194l-1.46-1.46c-1.04.944-2.42 1.52-3.936 1.52-3.24 0-5.865-2.626-5.865-5.864 0-3.24 2.627-5.865 5.865-5.865z"/></svg>
```

partials/icons/social/googleanalytics.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.074 24H1.895C.852 24 0 23.147 0 22.104v-4.419c0-1.043.852-1.896 1.895-1.896H7.58V9.474c0-1.042.852-1.894 1.894-1.894h6.331V1.925C15.805.87 16.674 0 17.729 0h4.346C23.13 0 24 .87 24 1.926v20.148C24 23.13 23.13 24 22.074 24z"/></svg>
```

partials/icons/social/googledrive.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.433 22.396l4-6.929H24l-4 6.929H4.433zm3.566-6.929l-3.998 6.929L0 15.467 7.785 1.98l3.999 6.931-3.785 6.556zm15.784-.375h-7.999L7.999 1.605h8.002l7.785 13.486h-.003z"/></svg>
```

partials/icons/social/googlepay.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 10l-3.134 7h-.968l1.163-2.45L19 10h1.02l1.49 3.49h.02L22.978 10zM10.983 12.166V15H10V8h2.607a2.48 2.48 0 0 1 1.687.606c.458.377.715.915.706 1.478a1.867 1.867 0 0 1-.706 1.485c-.455.398-1.018.596-1.687.596h-1.624zm-.002-3.304v2.444h1.648c.365.01.718-.122.973-.362.252-.225.395-.533.395-.856 0-.322-.143-.63-.395-.855a1.343 1.343 0 0 0-.973-.371h-1.648zM16.972 10c.627 0 1.122.174 1.485.522.362.348.543.826.543 1.432v2.893h-.811v-.652h-.037c-.351.537-.818.805-1.4.805-.498 0-.914-.153-1.25-.46A1.493 1.493 0 0 1 15 13.39c0-.485.177-.871.53-1.158.353-.287.825-.43 1.415-.431.503 0 .918.096 1.243.287v-.201a1.02 1.02 0 0 0-.35-.78 1.175 1.175 0 0 0-.818-.322c-.474 0-.849.208-1.124.623l-.747-.488c.41-.613 1.018-.92 1.823-.92zm-1.097 3.41a.713.713 0 0 0 .282.575c.187.153.42.234.659.23.357-.001.7-.15.953-.412a1.31 1.31 0 0 0 .422-.967c-.265-.22-.633-.329-1.106-.329-.345 0-.632.087-.862.26-.232.174-.348.387-.348.643zM4.081 8a3.966 3.966 0 0 1 2.73 1.042l-1.164 1.142a2.24 2.24 0 0 0-1.566-.6 2.436 2.436 0 0 0-2.291 1.65 2.351 2.351 0 0 0 0 1.532 2.436 2.436 0 0 0 2.291 1.65c.551 0 1.023-.138 1.39-.381.429-.28.723-.72.814-1.217H4.081v-1.54H7.93c.047.269.07.54.07.813 0 1.217-.444 2.247-1.214 2.943-.676.612-1.604.966-2.705.966a4.09 4.09 0 0 1-3.646-2.204 3.929 3.929 0 0 1 0-3.592A4.09 4.09 0 0 1 4.08 8z"/></svg>
```

partials/icons/social/googleplay.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M1.22 0c-.03.093-.06.185-.06.308v23.229c0 .217.061.34.184.463l11.415-12.093L1.22 0zm12.309 12.708l2.951 3.045-4.213 2.4s-5.355 3.044-8.308 4.739l9.57-10.184zm.801-.831l3.166 3.292c.496-.276 4.371-2.492 4.924-2.8.584-.338.525-.8.029-1.046-.459-.255-4.334-2.475-4.92-2.835l-3.203 3.392.004-.003zm-.803-.8l2.984-3.169-4.259-2.431S5.309 1.505 2.999.179l10.53 10.898h-.002z"/></svg>
```

partials/icons/social/googleplus.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.635 10.909v2.619h4.335c-.173 1.125-1.31 3.295-4.331 3.295-2.604 0-4.731-2.16-4.731-4.823 0-2.662 2.122-4.822 4.728-4.822 1.485 0 2.479.633 3.045 1.178l2.073-1.994c-1.33-1.245-3.056-1.995-5.115-1.995C3.412 4.365 0 7.785 0 12s3.414 7.635 7.635 7.635c4.41 0 7.332-3.098 7.332-7.461 0-.501-.054-.885-.12-1.265H7.635zm16.365 0h-2.183V8.726h-2.183v2.183h-2.182v2.181h2.184v2.184h2.189V13.09H24"/></svg>
```

partials/icons/social/googlepodcasts.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="m1.5 9.68c-.83 0-1.5.67-1.5 1.5v1.63a1.5 1.5 0 1 0 3 0v-1.63c0-.83-.67-1.5-1.5-1.5zm21 0c-.83 0-1.5.67-1.5 1.5v1.63a1.5 1.5 0 1 0 3 0v-1.63c0-.83-.67-1.5-1.5-1.5zm-15.82 4.91c-.83 0-1.5.67-1.5 1.5v1.63a1.5 1.5 0 1 0 3 0v-1.62c0-.83-.67-1.5-1.5-1.5zm0-9.82c-.83 0-1.5.67-1.5 1.5v5.36a1.5 1.5 0 0 0 3 0v-5.37c0-.83-.67-1.5-1.5-1.5zm10.64 0c-.83 0-1.5.67-1.5 1.5v1.64a1.5 1.5 0 0 0 3 0v-1.64c0-.83-.67-1.5-1.5-1.5zm-5.32-4.77c-.83 0-1.5.67-1.5 1.5v1.63a1.5 1.5 0 1 0 3 0v-1.63c0-.83-.67-1.5-1.5-1.5zm0 19.36c-.83 0-1.5.67-1.5 1.5v1.64a1.5 1.5 0 1 0 3 .01v-1.64c0-.82-.67-1.5-1.5-1.5zm5.32-8.46c-.83 0-1.5.68-1.5 1.5v5.33a1.5 1.5 0 0 0 3 0v-5.33c0-.83-.67-1.5-1.5-1.5zm-5.32-4.77c-.83 0-1.5.68-1.5 1.5v8.73a1.5 1.5 0 0 0 3 0v-8.72c0-.83-.67-1.5-1.5-1.5z"/></svg>
```

partials/icons/social/gravatar.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0c-1.326 0-2.4 1.074-2.4 2.4v8.4c0 1.324 1.074 2.398 2.4 2.398s2.4-1.074 2.4-2.398V5.21c2.795.99 4.799 3.654 4.799 6.789 0 3.975-3.225 7.199-7.199 7.199S4.801 15.975 4.801 12c0-1.989.805-3.789 2.108-5.091.938-.938.938-2.458 0-3.396s-2.458-.938-3.396 0C1.344 5.686 0 8.686 0 12c0 6.627 5.373 12 12 12s12-5.373 12-12S18.627 0 12 0"/></svg>
```

partials/icons/social/groupon.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M3.316 20.334C5.618 22.736 8.554 24 12.012 24c3.988 0 7.739-1.95 9.978-5.163 1.353-1.95 2.01-4.158 2.01-6.755 0-.484-.032-1.006-.063-1.529H10.595v4.61h6.687c-1.155 2.012-3.094 3.12-5.27 3.12-3.229 0-6.125-2.824-6.125-6.497 0-3.315 2.699-6.069 6.125-6.069 1.844 0 3.355.749 4.811 2.239h6.52C21.468 3.019 17.084 0 12.083 0c-3.323 0-6.22 1.17-8.53 3.409C1.25 5.647 0 8.572 0 11.754c-.008 3.417 1.108 6.271 3.316 8.58z"/></svg>
```

partials/icons/social/gulp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.156 19.432l.636-1.084s-1.444.591-3.86.591c-2.418 0-3.84-.568-3.84-.568l.711 1.183.252 3.729c0 .403 1.314.718 2.936.718 1.623 0 2.938-.314 2.938-.718l.229-3.835v-.016zm.615-7.046c-.769.046-1.153.903-1.539 1.805-.143.33-.63 1.737-.948 1.563-.318-.173.413-1.329.619-2.017-.237.174-1.105.849-1.329.215-.358.314-1.129.48-1.042-.329-.191.345-.621.823-1.139.614-.673-.255.395-2.411.66-2.307.266.121-.053.6-.136.794-.186.419-.398.958-.255 1.063.24.194.904-.703.919-.719.124-.165.479-1.229.763-1.107.285.134-.711 1.541-.34 1.826.076.06.383-.03.569-.239.12-.12.078-.42.479-1.378.404-.959.764-2.156 1.039-2.066s.049.703-.051.943c-.464 1.078-1.268 2.844-.89 2.71.374-.135.569-.135.943-.569.374-.434.345-1.152.599-1.137.24.014.21.254.15.418.24-.27 1.152-.868 1.363-.284.254.688-1.304 1.692-.914 1.632.375-.045.988-.434 1.258-.793l.719-6.5s-.734.6-5.361.6-5.284-.584-5.284-.584l.613 5.93c.33-.928 1.108-2.814 2.322-2.74.554.03 1.303 1.109.658 1.139-.27.015-.3-.539-.614-.614-.239-.046-.554.135-.763.345-.404.404-1.304 2.006-1.184 2.801.15 1.018 1.407-.346 1.617-.75.149-.283.254-1.138.568-1.048.33.09-.029.974-.27 1.737-.27.869-.404 1.781-.732 1.676-.33-.104.209-1.227.178-1.422-.313.299-.883 1.02-1.631.659l.374 3.699s1.019.793 4.073.793 4.118-.793 4.118-.793l.479-4.283c-.389.39-1.617 1.063-1.692.3-.059-.614 1.333-1.498.974-1.514l.06-.069zM17.346.669l-2.659 2.8-.486 1.901c1.881.12 3.189.386 3.189.694 0 .419-2.414.757-5.391.757s-5.39-.343-5.39-.763c0-.419 2.414-.764 5.391-.764.423 0 .844 0 1.264.016l.561-2.276L16.65.039c.068-.09.28-.015.474.15.194.149.299.344.239.434v.03l-.017.016zm-3.834 5.795s-.523 0-.61-.08c-.022-.025-.036-.058-.036-.09 0-.058.039-.091.09-.11l.044.075c-.021.006-.029.015-.033.023 0 .041.314.069.555.066.239-.003.531-.023.533-.064 0-.012-.023-.023-.061-.033l.045-.072c.063.02.117.058.117.121 0 .11-.141.128-.23.141-.107.015-.412.023-.412.023h-.002z"/></svg>
```

partials/icons/social/gumroad.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.826 15.069a1.018 1.018 0 1 1-.001 2.036 1.018 1.018 0 0 1 0-2.036zM21.327 1.11a1.018 1.018 0 1 1 .001 2.036 1.018 1.018 0 0 1 0-2.036zM3.322 3.107h16.116a2.13 2.13 0 0 0 1.89 1.151c1.174 0 2.129-.955 2.129-2.13A2.131 2.131 0 0 0 21.327 0c-.89 0-1.654.55-1.97 1.329H3.321C1.764 1.329.543 2.51.543 4.019v17.156C.543 22.706 1.816 24 3.322 24h17.155c1.51 0 2.738-1.267 2.738-2.825V10.998c0-1.532-1.228-2.78-2.738-2.78H10.3c-1.553 0-2.866 1.274-2.866 2.78v3.198c0 1.484 1.286 2.691 2.866 2.691h3.554a2.132 2.132 0 0 0 1.972 1.329c1.174 0 2.129-.956 2.129-2.13s-.955-2.129-2.13-2.129a2.13 2.13 0 0 0-1.889 1.152H10.3c-.523 0-1.088-.349-1.088-.913v-3.198c0-.524.519-1 1.088-1h10.177c.538 0 .96.439.96 1v10.177c0 .567-.44 1.047-.96 1.047H3.322c-.533 0-1-.49-1-1.047V4.02c0-.52.43-.912 1-.912"/></svg>
```

partials/icons/social/gumtree.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.829 6.52c-.189-.127-.315-.315-.315-.57C18.198 2.596 15.412 0 11.994 0s-6.203 2.594-6.52 5.949c0 .255-.126.442-.314.57-1.711 1.202-2.785 3.165-2.785 5.378 0 3.038 2.087 5.573 4.872 6.331.507.127.95.189 1.14.061.379-.188.76-1.832.57-2.213-.128-.189-.57-.379-1.014-.506-1.646-.443-2.848-1.961-2.848-3.732 0-1.015.379-1.9 1.014-2.6.252-.315.63-.567.948-.757.696-.38 1.14-1.142 1.14-1.964 0-.45.063-.826.189-1.201.506-1.532 1.961-2.659 3.67-2.659 1.711 0 3.166 1.127 3.672 2.659.126.375.189.751.189 1.201 0 .812.381 1.578 1.142 1.953.379.18.694.436.946.752.634.69 1.014 1.576 1.014 2.598 0 2.148-1.709 3.861-3.86 3.861-2.468 0-4.431 2.013-4.431 4.416v2.523c0 .496.064 1.006.19 1.142.315.316 1.962.316 2.278 0 .136-.136.195-.631.195-1.142v-2.583c0-.946.766-1.713 1.713-1.713 3.605 0 6.52-2.915 6.52-6.52 0-2.163-1.066-4.116-2.78-5.317l-.015.033z"/></svg>
```

partials/icons/social/hackerrank.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0c1.285 0 9.75 4.886 10.392 6 .645 1.115.645 10.885 0 12S13.287 24 12 24s-9.75-4.885-10.395-6c-.641-1.115-.641-10.885 0-12C2.25 4.886 10.715 0 12 0zm2.295 6.799c-.141 0-.258.115-.258.258v3.875H9.963V6.908h.701c.141 0 .254-.115.254-.258 0-.094-.049-.176-.123-.221L9.223 4.92c-.049-.063-.141-.109-.226-.109-.084 0-.16.045-.207.107L7.11 6.43c-.072.045-.12.126-.12.218 0 .143.113.258.255.258h.704l.008 10.035c0 .145.111.258.254.258h1.492c.142 0 .259-.115.259-.256v-4.004h4.073v4.152h-.699c-.143 0-.256.115-.256.258 0 .092.048.174.119.219l1.579 1.51c.044.061.141.109.225.109.085 0 .159-.045.208-.109l1.679-1.51c.072-.045.12-.127.12-.219 0-.143-.115-.258-.255-.258h-.704l-.007-10.034c0-.145-.114-.26-.255-.26h-1.494v.002z"/></svg>
```

partials/icons/social/heroku.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.61 0H3.39C2.189 0 1.23.96 1.23 2.16v19.681c0 1.198.959 2.159 2.16 2.159h17.22c1.2 0 2.159-.961 2.159-2.159V2.16C22.77.96 21.811 0 20.61 0zm.96 21.841c0 .539-.421.96-.96.96H3.39c-.54 0-.96-.421-.96-.96V2.16c0-.54.42-.961.96-.961h17.22c.539 0 .96.421.96.961v19.681zM6.63 20.399L9.33 18l-2.7-2.4v4.799zm9.72-9.719c-.479-.48-1.379-1.08-2.879-1.08-1.621 0-3.301.421-4.5.84V3.6h-2.4v10.38l1.68-.78s2.76-1.26 5.16-1.26c1.2 0 1.5.66 1.5 1.26v7.2h2.4v-7.2c.059-.179.059-1.501-.961-2.52zM13.17 7.5h2.4c1.08-1.26 1.62-2.521 1.8-3.9h-2.399c-.241 1.379-.841 2.64-1.801 3.9z"/></svg>
```

partials/icons/social/hipchat.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.736 19.056s.103-.073.267-.198C22.46 16.958 24 14.203 24 11.139 24 5.424 18.627.787 12.003.787 5.377.787 0 5.424 0 11.139c0 5.717 5.371 10.356 11.998 10.356.847 0 1.694-.073 2.524-.228l.262-.045c1.683 1.092 4.139 1.99 6.288 1.99.665 0 .978-.546.552-1.104-.648-.795-1.541-2.068-1.888-3.052zm-1.462-4.526c-.716 1.069-2.934 2.889-6.254 2.889h-.046c-3.328 0-5.543-1.831-6.254-2.889a1.137 1.137 0 0 1-.273-.574.49.49 0 0 1 .447-.526c.008-.003.014-.003.021-.003.117.006.23.043.328.111a9.137 9.137 0 0 0 5.754 2.056 8.805 8.805 0 0 0 5.76-2.059.461.461 0 0 1 .313-.122c.267 0 .478.213.483.475a1.321 1.321 0 0 1-.268.643h-.011z"/></svg>
```

partials/icons/social/hootsuite.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.002 0h.023c1.311.004 2.603.322 3.766.928C16.948.332 18.23.022 19.532.022h.676V24l-.656-.002C15.369 24 11.356 22.336 8.4 19.373 5.43 16.43 3.77 12.414 3.791 8.23V.021h.677c1.301 0 2.586.311 3.741.906C9.381.318 10.682 0 12.002 0zm0 .654c-1.381 0-2.676.373-3.791 1.021-1.138-.655-2.428-1.001-3.742-1h-.022V8.23c-.025 8.35 6.764 15.09 15.107 15.113V.675h-.022c-1.313-.001-2.604.343-3.743.999-1.144-.666-2.443-1.018-3.766-1.02h-.021zm3.252 2.754c1.79.002 3.238 1.453 3.237 3.242-.003 1.791-1.454 3.238-3.244 3.236-.616 0-1.22-.176-1.739-.508l-1.516 1.508-1.507-1.516c-1.514.952-3.515.495-4.465-1.02-.952-1.516-.495-3.516 1.021-4.467s3.516-.494 4.467 1.022c.273.437.44.933.483 1.446l.016-.02.015.018c.154-1.667 1.556-2.945 3.232-2.941zM8.76 8.789c1.192.006 2.163-.959 2.168-2.15.001-.219-.031-.436-.096-.644-.243.544-.882.788-1.426.546-.545-.244-.79-.883-.546-1.428.109-.243.304-.437.548-.547-1.137-.355-2.347.276-2.705 1.414-.066.207-.099.424-.1.642-.003 1.192.96 2.163 2.153 2.167h.004zm6.478.019c1.193.003 2.163-.962 2.166-2.155s-.963-2.162-2.155-2.164c-.216-.002-.431.03-.638.094.545.244.789.883.547 1.428-.244.543-.883.787-1.428.545-.245-.109-.439-.307-.549-.553-.355 1.139.279 2.352 1.417 2.707.209.063.423.097.64.098z"/></svg>
```

partials/icons/social/houzz.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.93 12v8L12 24v-8.002L5.07 20V3.998L12 0v8l-6.928 4L12 15.998V8l6.93-4.002V12z"/></svg>
```

partials/icons/social/hulu.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.4 7.355h-3.607a5.91 5.91 0 0 0-2.063.405V-.03H2.94v24.06h5.8v-9.51a1.61 1.61 0 0 1 1.56-1.7h3.39a1.59 1.59 0 0 1 1.59 1.56v9.59h5.78V13.54c0-4.41-2.25-6.162-5.9-6.162"/></svg>
```

partials/icons/social/humblebundle.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.145 23.996c.12-.463.23-.9.343-1.338.692-2.713 1.322-5.44 1.82-8.197.245-1.35.446-2.71.633-4.074.142-1.028.217-2.064.198-3.105-.01-.557-.034-1.116-.193-1.655-.07-.24-.174-.473-.3-.686-.165-.273-.43-.378-.75-.368-.883.026-1.633.363-2.272.96-.727.68-1.202 1.527-1.553 2.445-.166.435-.284.887-.422 1.33-.02.066-.026.123-.115.122C1.04 9.424.545 9.425.05 9.424c-.013 0-.024-.008-.036-.01 0-.193-.02-.385.003-.572.346-2.853 1.57-5.267 3.668-7.226C4.47.882 5.4.373 6.462.142 8.017-.196 9.258.4 9.996 1.822c.375.72.578 1.496.71 2.293.21 1.287.218 2.586.175 3.885-.014.42-.04.84-.062 1.26-.002.054 0 .108 0 .176.057.003.105.008.154.008.905 0 1.81-.002 2.717.005.124 0 .16-.047.18-.16.575-3.113 1.367-6.17 2.39-9.166.024-.074.05-.124.147-.124 1.12.004 2.24.004 3.362.004.017 0 .035.004.07.008l-.193.753C18.89 3.7 18.21 6.65 17.66 9.628c-.288 1.546-.533 3.1-.69 4.664-.086.875-.14 1.752-.113 2.63.016.53.054 1.062.22 1.57.064.202.16.4.273.58.167.26.426.366.74.356 1.16-.033 2.042-.59 2.746-1.47.707-.88 1.133-1.9 1.434-2.98.028-.1.06-.202.076-.306.014-.082.054-.104.13-.104.467.002.933.004 1.4 0 .102-.002.12.043.117.13-.014.804-.157 1.583-.39 2.347-.59 1.928-1.557 3.635-2.992 5.06-.813.81-1.762 1.407-2.88 1.706-.677.183-1.355.212-2.025-.028-.76-.27-1.276-.816-1.66-1.504-.402-.725-.613-1.512-.75-2.322-.24-1.406-.24-2.824-.172-4.242.042-.89.127-1.777.193-2.666.014-.19.016-.19-.174-.19-.855 0-1.71.002-2.566-.002-.104 0-.153.024-.17.137-.27 1.813-.637 3.608-1.074 5.387-.453 1.842-.974 3.664-1.587 5.46-.044.127-.104.16-.233.16-1.065-.006-2.13-.004-3.197-.004h-.17z"/></svg>
```

partials/icons/social/icq.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.406.133C14.65.07 13.93.223 13.226.6c-.94.503-1.61 1.275-1.912 2.28v.067l-.035.235-.134-.235-.335-.603c-.536-.837-1.206-1.34-2.044-1.574C8.03.604 7.426.673 6.79 1.01c-.705.436-1.106 1.106-1.274 2.045-.168.972 0 1.91.502 2.847l.236.336-.807-.267c-1.005-.236-1.944-.104-2.883.4C1.592 6.87.99 7.576.588 8.55c-.37.938-.336 1.843.133 2.68.202.37.504.67.772.872.402.402.905.636 1.508.736l.234.066-.502.438c-.47.402-.738.903-.906 1.406-.168.603-.1 1.207.236 1.777.17.268.334.503.602.67.268.235.604.403 1.006.436.738.17 1.508.168 2.346-.1l-.604 1.005-.168.436c-.335 1.074-.233 2.01.27 2.983.235.37.5.705.77 1.006.4.368.906.602 1.51.77 1.004.268 2.01.236 2.98-.267.94-.503 1.543-1.31 1.845-2.315l.032-.2c.637.703 1.24 1.173 1.912 1.34.67.202 1.34.17 1.944-.233.57-.335.973-.906 1.174-1.61.168-.738.168-1.474 0-2.312.335.235.67.4 1.072.502 1.073.335 2.01.3 2.95-.2.904-.504 1.508-1.308 1.81-2.347.268-1.005.202-1.977-.3-2.916l-.17-.27c-.267-.402-.537-.804-.94-1.072-.334-.235-.735-.402-1.104-.57 1.04-.503 1.776-1.207 2.11-2.112.236-.738.17-1.342-.167-1.945v-.066c-.402-.67-.937-1.105-1.775-1.34-.503-.1-1.072-.102-1.574-.068l-1.108.235.37-.838c.334-1.073.235-2.112-.335-3.084l-.1-.17c-.503-.838-1.24-1.34-2.246-1.607-.26-.067-.516-.113-.768-.133zm-.57 1.414c.323-.03.65.012.967.13.704.166 1.207.534 1.51 1.104v.003c.168.335.267.736.267 1.172l-.1.738c-.134.37-.302.703-.503 1.004l-3.016 3.69c-.3-.235-.637-.403-.972-.57l-.336-3.79-.033-1.34.032-.335c.168-.67.638-1.173 1.24-1.508.302-.168.62-.268.944-.297zm-6.883.537c.134-.004.276.03.41.096.603.168 1.106.603 1.508 1.44.17.336.336.67.403 1.073l.67 3.957-.504.168-2.983-3.252-.168-.334c-.27-.604-.435-1.173-.368-1.777v-.002c.034-.603.268-1.003.67-1.238.1-.084.227-.127.36-.13zm12.13 5.033c.15 0 .297.007.448.024.57.068.972.337 1.173.74l.135.433-.067.335c-.234.603-.738 1.074-1.575 1.442-.335.168-.703.235-1.105.3l-4.123.503-.067-.235-.068-.1.135-.167 3.387-2.816.4-.166.002-.002c.45-.2.885-.286 1.328-.29zM4.622 7.3c.16.008.324.033.49.075v.002l.908.367 2.95 2.147c-.27.336-.435.67-.536 1.005l-4.828.603-.334-.066c-.603-.1-1.007-.37-1.276-.87-.27-.503-.267-1.006-.066-1.51.235-.636.67-1.14 1.306-1.407.453-.252.906-.373 1.387-.346zm7.16 2.69c.604 0 1.175.236 1.544.604.47.47.67.973.67 1.576 0 .603-.2 1.172-.67 1.574-.436.436-.94.67-1.543.67-.636 0-1.17-.235-1.573-.67-.436-.402-.67-.97-.67-1.574 0-.603.234-1.107.67-1.576.402-.37.937-.604 1.574-.604zm8.415 2.58l.336.035c.504.168.973.468 1.24.97.336.37.503.873.503 1.443l-.1.67c-.167.67-.57 1.173-1.14 1.44-.603.336-1.207.403-1.877.17-.402-.1-.67-.268-.904-.536l-3.52-2.918.235-.502.1-.403 3.788-.335 1.34-.035zm-6.636 2.448l1.407 1.44.87 1.073.17.337c.3.57.468 1.105.4 1.742-.066.602-.267 1.038-.67 1.206-.234.168-.502.17-.77.135-.637-.166-1.14-.668-1.508-1.473l-.403-1.108-.502-2.917.568-.2.436-.235zm-3.62.068c.334.167.67.334 1.04.367.066 1.14.165 2.347.332 3.654v1.342l-.033.333c-.236.603-.638 1.107-1.24 1.375-.604.335-1.24.402-1.845.235-.67-.167-1.173-.57-1.44-1.106-.17-.335-.304-.74-.304-1.14l.17-.77c.066-.335.235-.67.503-.94l2.816-3.35z"/></svg>
```

partials/icons/social/ifixit.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.345 12.506l2.37 3.131c.198.261.211.69.025.961l-.119.177c-.181.27-.55.645-.814.831l-.285.201c-.266.195-.697.195-.956-.016l-3.135-2.369c-.255-.195-.681-.195-.94 0l-3.136 2.369c-.258.211-.689.211-.956.03l-.207-.135c-.27-.181-.641-.556-.825-.81l-.181-.256c-.186-.27-.18-.689.018-.96l2.377-3.149c.195-.256.195-.675 0-.945L6.197 8.43c-.194-.263-.203-.69-.013-.957l.2-.285c.187-.264.56-.629.828-.814l.175-.119c.27-.196.703-.182.961.014l3.135 2.37c.26.195.684.195.942 0l3.135-2.385c.258-.195.698-.226.979-.061l.33.195c.28.165.639.524.795.81l.12.21c.154.285.123.721-.075.99l-2.37 3.135c-.194.255-.194.676 0 .945l.006.028zM12 0C5.37 0 0 5.373 0 12s5.37 12 12 12c6.627 0 12-5.373 12-12S18.627 0 12 0z"/></svg>
```

partials/icons/social/imdb.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.31 9.588v.005c-.077-.048-.227-.07-.42-.07v4.815c.27 0 .44-.06.5-.165.062-.104.095-.405.095-.885v-2.866c0-.33-.004-.54-.033-.63-.022-.096-.067-.163-.14-.204z"/><path d="M22.416 0H1.62C.742.06.06.744 0 1.596V22.38c.06.874.712 1.542 1.555 1.617.015.003.03.003.045.003h20.845c.88-.088 1.55-.826 1.555-1.71V1.71C24 .82 23.305.07 22.416 0zM4.792 15.626H2.887V8.26h1.905v7.366zm6.54-.002H9.67v-4.97L9 15.623H7.812l-.698-4.86-.007 4.86H5.44V8.26h2.468c.083.523.16 1.048.23 1.574l.27 1.87.442-3.444h2.483v7.364zm4.977-2.18c0 .655-.044 1.094-.104 1.32-.062.22-.17.4-.326.52-.15.13-.34.218-.57.266-.223.045-.57.075-1.02.075l-.004-.002H11.98V8.26h1.426c.914 0 1.45.047 1.77.128.325.09.575.225.745.42.165.18.273.404.313.645.05.235.076.705.076 1.402v2.588zm4.944.475c0 .45-.045.764-.09.99-.06.224-.195.404-.405.568-.226.166-.48.24-.78.24-.22 0-.5-.06-.68-.136-.19-.094-.358-.237-.515-.427l-.116.47h-1.717V8.26l-.02-.003h1.8v2.4c.15-.175.315-.31.51-.4.196-.083.466-.127.69-.127.226-.003.45.036.66.115.17.07.32.185.436.33.09.125.15.27.18.42.03.138.044.43.044.87v2.054z"/><path d="M19.08 11.205c-.12 0-.194.04-.225.12-.03.08-.06.29-.06.624v1.946c0 .324.03.533.06.623.04.086.13.14.226.134.12 0 .272-.047.3-.14.03-.097.046-.32.046-.674l.03-.002v-1.89c0-.303-.015-.508-.06-.603-.044-.1-.195-.14-.315-.14z"/></svg>
```

partials/icons/social/instagram.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C8.74 0 8.333.015 7.053.072 5.775.132 4.905.333 4.14.63c-.789.306-1.459.717-2.126 1.384S.935 3.35.63 4.14C.333 4.905.131 5.775.072 7.053.012 8.333 0 8.74 0 12s.015 3.667.072 4.947c.06 1.277.261 2.148.558 2.913.306.788.717 1.459 1.384 2.126.667.666 1.336 1.079 2.126 1.384.766.296 1.636.499 2.913.558C8.333 23.988 8.74 24 12 24s3.667-.015 4.947-.072c1.277-.06 2.148-.262 2.913-.558.788-.306 1.459-.718 2.126-1.384.666-.667 1.079-1.335 1.384-2.126.296-.765.499-1.636.558-2.913.06-1.28.072-1.687.072-4.947s-.015-3.667-.072-4.947c-.06-1.277-.262-2.149-.558-2.913-.306-.789-.718-1.459-1.384-2.126C21.319 1.347 20.651.935 19.86.63c-.765-.297-1.636-.499-2.913-.558C15.667.012 15.26 0 12 0zm0 2.16c3.203 0 3.585.016 4.85.071 1.17.055 1.805.249 2.227.415.562.217.96.477 1.382.896.419.42.679.819.896 1.381.164.422.36 1.057.413 2.227.057 1.266.07 1.646.07 4.85s-.015 3.585-.074 4.85c-.061 1.17-.256 1.805-.421 2.227-.224.562-.479.96-.899 1.382-.419.419-.824.679-1.38.896-.42.164-1.065.36-2.235.413-1.274.057-1.649.07-4.859.07-3.211 0-3.586-.015-4.859-.074-1.171-.061-1.816-.256-2.236-.421-.569-.224-.96-.479-1.379-.899-.421-.419-.69-.824-.9-1.38-.165-.42-.359-1.065-.42-2.235-.045-1.26-.061-1.649-.061-4.844 0-3.196.016-3.586.061-4.861.061-1.17.255-1.814.42-2.234.21-.57.479-.96.9-1.381.419-.419.81-.689 1.379-.898.42-.166 1.051-.361 2.221-.421 1.275-.045 1.65-.06 4.859-.06l.045.03zm0 3.678c-3.405 0-6.162 2.76-6.162 6.162 0 3.405 2.76 6.162 6.162 6.162 3.405 0 6.162-2.76 6.162-6.162 0-3.405-2.76-6.162-6.162-6.162zM12 16c-2.21 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm7.846-10.405c0 .795-.646 1.44-1.44 1.44-.795 0-1.44-.646-1.44-1.44 0-.794.646-1.439 1.44-1.439.793-.001 1.44.645 1.44 1.439z"/></svg>
```

partials/icons/social/instapaper.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.766 20.259c0 1.819.271 2.089 2.934 2.292V24H6.301v-1.449c2.666-.203 2.934-.473 2.934-2.292V3.708c0-1.784-.27-2.089-2.934-2.292V0h11.398v1.416c-2.662.203-2.934.506-2.934 2.292v16.551z"/></svg>
```

partials/icons/social/intercom.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21 0H3C1.343 0 0 1.343 0 3v18c0 1.658 1.343 3 3 3h18c1.658 0 3-1.342 3-3V3c0-1.657-1.342-3-3-3zm-5.801 4.399c0-.44.36-.8.802-.8.44 0 .8.36.8.8v10.688c0 .442-.36.801-.8.801-.443 0-.802-.359-.802-.801V4.399zM11.2 3.994c0-.44.357-.799.8-.799s.8.359.8.799v11.602c0 .44-.357.8-.8.8s-.8-.36-.8-.8V3.994zm-4 .405c0-.44.359-.8.799-.8.443 0 .802.36.802.8v10.688c0 .442-.36.801-.802.801-.44 0-.799-.359-.799-.801V4.399zM3.199 6c0-.442.36-.8.802-.8.44 0 .799.358.799.8v7.195c0 .441-.359.8-.799.8-.443 0-.802-.36-.802-.8V6zM20.52 18.202c-.123.105-3.086 2.593-8.52 2.593-5.433 0-8.397-2.486-8.521-2.593-.335-.288-.375-.792-.086-1.128.285-.334.79-.375 1.125-.09.047.041 2.693 2.211 7.481 2.211 4.848 0 7.456-2.186 7.479-2.207.334-.289.839-.25 1.128.086.289.336.25.84-.086 1.128zm.281-5.007c0 .441-.36.8-.801.8-.441 0-.801-.36-.801-.8V6c0-.442.361-.8.801-.8.441 0 .801.357.801.8v7.195z"/></svg>
```

partials/icons/social/invision.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.825 0H2.175C.975 0 0 .975 0 2.175v19.65C0 23.025.975 24 2.175 24h19.65c1.2 0 2.175-.975 2.175-2.175V2.175C24 .975 23.025 0 21.825 0zM8.02 4.667c.798 0 1.468.63 1.468 1.44 0 .82-.67 1.444-1.468 1.444v.027c-.803 0-1.454-.65-1.454-1.455s.65-1.455 1.455-1.455zm9.816 13.815c-1.484 0-2.204-.885-2.204-2.09 0-.346.044-.713.15-1.08l.71-2.545c.088-.28.11-.54.11-.775 0-.82-.5-1.315-1.296-1.315-1.013 0-1.68.727-2.025 2.13l-1.38 5.535H9.487l.432-1.74c-.708 1.166-1.695 1.885-2.91 1.885-1.467 0-2.157-.842-2.157-2.113.004-.365.047-.73.13-1.085v.002l1.1-4.49H4.375l.518-1.905h4.1l-1.62 6.405c-.105.41-.15.75-.15.986 0 .41.202.53.517.604.195.04 1.725.012 2.56-1.84l1.06-4.25H9.637l.52-1.875h3.72l-.48 2.16c.647-1.2 1.937-2.355 3.212-2.355 1.35 0 2.475.975 2.475 2.82 0 .534-.08 1.065-.24 1.575l-.69 2.476c-.06.254-.104.465-.104.66 0 .434.18.645.494.645s.735-.24 1.2-1.56l.943.36c-.555 1.964-1.576 2.774-2.85 2.774z"/></svg>
```

partials/icons/social/javascript.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0V0zm22.034 18.276c-.175-1.095-.888-2.015-3.003-2.873-.736-.345-1.554-.585-1.797-1.14-.091-.33-.105-.51-.046-.705.15-.646.915-.84 1.515-.66.39.12.75.42.976.9 1.034-.676 1.034-.676 1.755-1.125-.27-.42-.404-.601-.586-.78-.63-.705-1.469-1.065-2.834-1.034l-.705.089c-.676.165-1.32.525-1.71 1.005-1.14 1.291-.811 3.541.569 4.471 1.365 1.02 3.361 1.244 3.616 2.205.24 1.17-.87 1.545-1.966 1.41-.811-.18-1.26-.586-1.755-1.336l-1.83 1.051c.21.48.45.689.81 1.109 1.74 1.756 6.09 1.666 6.871-1.004.029-.09.24-.705.074-1.65l.046.067zm-8.983-7.245h-2.248c0 1.938-.009 3.864-.009 5.805 0 1.232.063 2.363-.138 2.711-.33.689-1.18.601-1.566.48-.396-.196-.597-.466-.83-.855-.063-.105-.11-.196-.127-.196l-1.825 1.125c.305.63.75 1.172 1.324 1.517.855.51 2.004.675 3.207.405.783-.226 1.458-.691 1.811-1.411.51-.93.402-2.07.397-3.346.012-2.054 0-4.109 0-6.179l.004-.056z"/></svg>
```

partials/icons/social/jira.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.323 11.33L13.001 1 12 0 4.225 7.775.67 11.33a.96.96 0 0 0 0 1.347l7.103 7.103L12 24l7.771-7.771.121-.121 3.431-3.431a.945.945 0 0 0 0-1.347zM12 15.551L8.449 12 12 8.453 15.548 12 12 15.551z"/></svg>
```

partials/icons/social/joomla.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.719 14.759L14.22 17.26l-2.37 2.37-.462.466c-1.368 1.365-3.297 1.83-5.047 1.397-.327 1.424-1.604 2.49-3.13 2.49C1.438 23.983 0 22.547 0 20.772c0-1.518 1.055-2.789 2.469-3.123-.446-1.76.016-3.705 1.396-5.08l.179-.18 2.37 2.37-.184.181c-.769.779-.769 2.024 0 2.789.771.78 2.022.78 2.787 0l.465-.465 2.367-2.371 2.502-2.506 2.368 2.372zm.924 6.652c-1.822.563-3.885.12-5.328-1.318l-.18-.185 2.365-2.369.18.184c.771.768 2.018.768 2.787 0 .765-.765.769-2.01-.004-2.781l-.466-.465-2.365-2.37-2.502-2.503 2.37-2.369 2.499 2.505 2.367 2.37.464.464c1.365 1.36 1.846 3.278 1.411 5.021 1.56.224 2.759 1.56 2.759 3.18 0 1.784-1.439 3.21-3.209 3.21-1.545 0-2.851-1.096-3.135-2.565l-.013-.009zM6.975 9.461l2.508-2.505 2.37-2.369.462-.461C13.74 2.7 15.772 2.251 17.58 2.79c.212-1.561 1.555-2.775 3.179-2.775 1.772 0 3.211 1.437 3.211 3.209 0 1.631-1.216 2.978-2.79 3.186.519 1.799.068 3.816-1.35 5.234l-.182.184-2.369-2.369.184-.184c.769-.77.769-2.016 0-2.783-.766-.766-2.011-.768-2.781.003l-.462.461-2.37 2.369-2.505 2.502-2.37-2.366zm-2.653 2.647l-.461-.462C2.43 10.215 1.986 8.17 2.529 6.358 1.1 6.029.03 4.754.03 3.224.03 1.454 1.47.015 3.24.015c1.596 0 2.92 1.166 3.17 2.691 1.73-.405 3.626.065 4.979 1.415l.184.185-2.37 2.37-.183-.181c-.77-.765-2.016-.765-2.785 0-.771.781-.77 2.025-.005 2.79l.465.466 2.37 2.369 2.505 2.505-2.367 2.37-2.51-2.505-2.371-2.37v-.012z"/></svg>
```

partials/icons/social/jquery.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M1.534 5.874c-2.123 3.05-1.86 7.017-.237 10.256.037.079.078.154.118.229.023.052.049.1.077.149.013.028.031.057.047.083.026.052.054.102.081.152l.157.265c.029.049.057.097.09.146.055.094.12.187.177.281.026.039.05.078.079.117a6.36 6.36 0 0 0 .31.444c.078.107.156.211.24.315.027.038.057.076.085.114l.221.269c.027.031.054.067.083.099.098.118.202.233.306.349 0 .002.003.004.005.007a3.13 3.13 0 0 0 .424.44c.08.082.16.164.245.244l.101.097c.111.104.222.208.339.308.002 0 .003.002.005.003l.057.05c.102.089.205.178.31.26l.125.105c.085.068.173.133.26.2l.136.104c.093.07.192.139.287.207.035.025.07.05.106.073l.029.023.281.185.12.08c.147.094.293.183.438.271.042.021.084.044.123.068.108.062.22.125.329.183.06.034.122.063.184.094.075.042.153.083.233.125a.324.324 0 0 1 .056.023c.033.015.064.031.096.047.12.06.245.117.375.174.024.01.05.02.076.034.144.063.288.123.437.182.034.01.07.027.105.04.135.051.274.103.411.152l.05.018c.153.052.304.102.459.15.036.01.073.023.111.033.159.048.313.105.473.136 10.26 1.87 13.242-6.169 13.242-6.169-2.505 3.262-6.95 4.122-11.16 3.165-.156-.036-.312-.086-.469-.132a13.522 13.522 0 0 1-.567-.181l-.062-.024c-.136-.046-.267-.097-.4-.148a1.613 1.613 0 0 0-.11-.041c-.147-.059-.29-.12-.432-.183-.031-.01-.057-.024-.088-.036a23.41 23.41 0 0 1-.361-.17c-.037-.016-.07-.033-.106-.052-.094-.044-.188-.094-.28-.142a3.942 3.942 0 0 1-.187-.096c-.113-.06-.226-.125-.339-.187-.034-.024-.073-.044-.112-.066a15.902 15.902 0 0 1-.438-.269 2.104 2.104 0 0 1-.118-.079 6.002 6.002 0 0 1-.312-.206c-.035-.023-.067-.048-.103-.073a9.541 9.541 0 0 1-.294-.212c-.042-.034-.087-.066-.132-.1-.088-.069-.177-.135-.265-.208l-.118-.094a10.58 10.58 0 0 1-.334-.281.258.258 0 0 0-.037-.03l-.347-.316-.1-.094c-.082-.083-.166-.163-.25-.245l-.097-.1a9.07 9.07 0 0 1-.309-.323l-.015-.016c-.106-.116-.209-.234-.313-.354-.027-.031-.052-.064-.08-.097l-.226-.277a21.248 21.248 0 0 1-.34-.448C2.16 11.786 1.315 7.386 3.184 3.777"/><path d="M8.121 3.305c-1.539 2.209-1.452 5.163-.254 7.499a9.1 9.1 0 0 0 .677 1.132c.23.33.484.72.792.986.107.122.223.24.344.359l.09.09c.114.11.231.218.35.325l.015.013a9.855 9.855 0 0 0 .414.342c.034.023.063.05.096.073.14.108.281.212.427.315l.015.009c.062.045.128.086.198.13.028.018.06.042.09.06.106.068.21.132.317.197.017.007.032.016.048.023.09.055.188.108.282.157.033.02.065.035.099.054.067.033.133.068.197.102l.032.014c.135.066.273.128.408.19.034.013.063.024.092.038.111.048.224.094.335.137.05.017.097.037.144.052.102.038.209.073.31.108l.14.045c.146.045.294.104.448.129 7.92 1.313 9.754-4.787 9.754-4.787-1.651 2.376-4.846 3.508-8.251 2.624a8.03 8.03 0 0 1-.448-.13c-.048-.013-.09-.028-.136-.042-.104-.036-.211-.071-.312-.109l-.144-.054c-.112-.045-.226-.087-.335-.135-.034-.015-.065-.025-.091-.04-.14-.063-.281-.125-.417-.192l-.206-.107-.119-.06c-.092-.048-.177-.098-.265-.15a.62.62 0 0 1-.062-.034c-.106-.066-.216-.13-.317-.198-.034-.019-.065-.042-.097-.062l-.208-.136c-.144-.1-.285-.208-.427-.312-.032-.029-.063-.053-.094-.079-1.497-1.177-2.678-2.786-3.238-4.608-.59-1.894-.46-4.018.559-5.742"/><path d="M13.66 1.384c-.908 1.332-.995 2.986-.37 4.455.664 1.56 2.022 2.785 3.604 3.365.065.025.128.046.195.07l.088.027c.092.029.185.063.28.084 4.376.844 5.56-2.247 5.879-2.701-1.042 1.496-2.789 1.855-4.932 1.334a4.844 4.844 0 0 1-.516-.16 6.344 6.344 0 0 1-.617-.254 6.521 6.521 0 0 1-1.08-.66c-1.92-1.454-3.109-4.23-1.857-6.491"/></svg>
```

partials/icons/social/jsfiddle.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.078 11.251c.01-.141.021-.278.021-.419 0-3.883-3.193-7.031-7.135-7.031-2.738-.01-5.24 1.548-6.441 4.009-.575-.442-1.28-.681-2.007-.681-1.82 0-3.295 1.45-3.295 3.24 0 .338.053.663.15.967C.908 12.181.004 13.739 0 15.429c0 2.602 2.124 4.717 4.759 4.755h14.25c.09 0 .18.015.27.015 2.609 0 4.723-2.083 4.723-4.662-.012-1.886-1.16-3.579-2.91-4.286h-.014zM6.44 16.602c-.479-.434-.779-.959-.898-1.58-.041-.216-.061-.434-.061-.652 0-.885.322-1.613.967-2.188.645-.576 1.462-.864 2.455-.864 1.02 0 1.979.383 2.831 1.146.21.189.417.404.614.641l1.091 1.284c.188.259.389.48.6.671.563.504 1.17.756 1.686.756.438 0 .801-.135 1.094-.402.248-.229.402-.539.434-.875l.008-.148c.002-.141-.021-.281-.064-.416-.227-.619-.824-1.023-1.484-1.001-.543 0-1.082.183-1.672.755l-.967-1.139-.105-.129c.855-.829 1.695-1.139 2.834-1.139 1.004 0 1.828.284 2.441.854l.016.015c.646.569.959 1.305.959 2.208 0 .21-.016.435-.059.63-.121.614-.42 1.124-.885 1.559-.477.435-1.07.717-1.709.81-.225.03-.449.045-.705.045-1.033 0-2.008-.375-2.832-1.124-.234-.212-.449-.443-.645-.689l-1.094-1.275c-.171-.244-.366-.471-.585-.674-.555-.51-1.17-.75-1.709-.75-.156 0-.313.021-.465.061-.235.06-.452.178-.629.345-.279.259-.438.623-.436 1.005 0 .389.135.719.42.988l.016.016c.3.27.675.404 1.109.404.555 0 1.094-.194 1.678-.764l.96 1.124.104.119c-.869.84-1.708 1.154-2.803 1.154-1.004 0-1.828-.284-2.458-.854l-.052.073z"/></svg>
```

partials/icons/social/justgiving.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.716 9.925H15.33l-4.898 4.919h6.727c-.885 1.975-2.865 3.061-5.16 3.061-3.104 0-5.639-2.67-5.639-5.771C6.36 9.02 8.896 6.42 12 6.42c1.134 0 2.189.295 3.061.871l4.542-4.561C17.541 1.031 14.893 0 12 0 5.37 0 0 5.367 0 12c0 6.623 5.37 12 12 12s12-5.115 12-11.738c0-.896-.103-1.35-.284-2.337z"/></svg>
```

partials/icons/social/khanacademy.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.469 22.395S-1.229 13.553 5.401 6.96C11.415.969 20.5.041 22.076 0c0 0 2.438 8.006-3.651 17.081-6.083 9.075-14.521 6.614-14.521 6.614s8.336-10.626 7.332-10.561c-.701.041-5.076 4.856-8.768 9.263"/></svg>
```

partials/icons/social/kickstarter.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.168 0c-3.2 0-5.797 2.579-5.797 5.758v12.484C1.371 21.42 3.968 24 7.168 24c1.981 0 3.716-.978 4.768-2.479l.794.79c2.26 2.245 5.943 2.245 8.203 0a5.724 5.724 0 001.696-4.075 5.724 5.724 0 00-1.696-4.074l-2.182-2.168 2.182-2.156a5.724 5.724 0 001.696-4.074 5.724 5.724 0 00-1.696-4.074c-2.26-2.246-5.942-2.246-8.203 0l-.794.789A5.797 5.797 0 007.168 0Z"/></svg>
```

partials/icons/social/kik.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.482 16.752c-.01.688-.56 1.242-1.238 1.242-.689 0-1.23-.541-1.244-1.23h-.016v-6.243H9v-.029c0-.693.556-1.256 1.237-1.256s1.236.563 1.236 1.258v.045h.016v6.225h-.016l.009-.012zm11.137-4.889c.75 0 1.381.618 1.381 1.377 0 .76-.631 1.375-1.381 1.375-.766 0-1.395-.615-1.395-1.379 0-.766.615-1.381 1.379-1.381l.016.008zm-2.084 4.186c.121.195.193.432.193.686 0 .703-.553 1.26-1.244 1.26-.463 0-.869-.256-1.08-.631l-2.053-2.746-.631.586v1.635h-.014c-.039.652-.57 1.168-1.225 1.168-.674 0-1.221-.553-1.221-1.238v-.025h-.016v-9.45h.027v-.047c0-.69.551-1.253 1.23-1.253.674 0 1.225.562 1.225 1.253v.07h.016l.01 4.597 2.311-2.261c.229-.255.559-.405.928-.405.689 0 1.248.57 1.248 1.26 0 .346-.133.646-.344.871l.012.015-1.621 1.605 2.281 3.061-.016.016-.016-.027zm-13.246 0c.12.195.195.432.195.686 0 .703-.555 1.26-1.244 1.26-.466 0-.871-.256-1.081-.631l-2.054-2.746-.63.586v1.631H2.46c-.036.654-.57 1.17-1.221 1.17-.676 0-1.225-.555-1.225-1.238v-.027H0V7.29h.031c-.004-.015-.004-.029-.004-.044 0-.69.551-1.252 1.23-1.252.675 0 1.225.559 1.225 1.25v.07h.016l.01 4.6 2.311-2.261c.23-.255.562-.405.931-.405.687 0 1.245.57 1.245 1.26 0 .33-.131.646-.346.871l.016.015-1.627 1.605 2.271 3.061-.016.016-.004-.027z"/></svg>
```

partials/icons/social/kofi.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.881 8.948c-.773-4.085-4.859-4.593-4.859-4.593H.723c-.604 0-.679.798-.679.798s-.082 7.324-.022 11.822c.164 2.424 2.586 2.672 2.586 2.672s8.267-.023 11.966-.049c2.438-.426 2.683-2.566 2.658-3.734 4.352.24 7.422-2.831 6.649-6.916zm-11.062 3.511c-1.246 1.453-4.011 3.976-4.011 3.976s-.121.119-.31.023c-.076-.057-.108-.09-.108-.09-.443-.441-3.368-3.049-4.034-3.954-.709-.965-1.041-2.7-.091-3.71.951-1.01 3.005-1.086 4.363.407 0 0 1.565-1.782 3.468-.963 1.904.82 1.832 3.011.723 4.311zm6.173.478c-.928.116-1.682.028-1.682.028V7.284h1.77s1.971.551 1.971 2.638c0 1.913-.985 2.667-2.059 3.015z"/></svg>
```

partials/icons/social/lastfm.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M10.599 17.211l-.881-2.393s-1.433 1.596-3.579 1.596c-1.9 0-3.249-1.652-3.249-4.296 0-3.385 1.708-4.596 3.388-4.596 2.418 0 3.184 1.568 3.845 3.578l.871 2.751c.871 2.672 2.523 4.818 7.285 4.818 3.41 0 5.722-1.045 5.722-3.801 0-2.227-1.276-3.383-3.635-3.935l-1.757-.384c-1.217-.274-1.577-.771-1.577-1.597 0-.936.736-1.487 1.952-1.487 1.323 0 2.028.495 2.147 1.679l2.749-.33c-.225-2.479-1.937-3.494-4.745-3.494-2.479 0-4.897.936-4.897 3.934 0 1.873.902 3.058 3.185 3.605l1.862.443c1.397.33 1.863.916 1.863 1.713 0 1.021-.992 1.441-2.869 1.441-2.779 0-3.936-1.457-4.597-3.469l-.901-2.75c-1.156-3.574-3.004-4.896-6.669-4.896C2.147 5.327 0 7.879 0 12.235c0 4.179 2.147 6.445 6.003 6.445 3.108 0 4.596-1.457 4.596-1.457v-.012z"/></svg>
```

partials/icons/social/line.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.365 9.863c.349 0 .63.285.63.631 0 .345-.281.63-.63.63H17.61v1.125h1.755c.349 0 .63.283.63.63 0 .344-.281.629-.63.629h-2.386c-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63h2.386c.346 0 .627.285.627.63 0 .349-.281.63-.63.63H17.61v1.125h1.755zm-3.855 3.016c0 .27-.174.51-.432.596-.064.021-.133.031-.199.031-.211 0-.391-.09-.51-.25l-2.443-3.317v2.94c0 .344-.279.629-.631.629-.346 0-.626-.285-.626-.629V8.108c0-.27.173-.51.43-.595.06-.023.136-.033.194-.033.195 0 .375.104.495.254l2.462 3.33V8.108c0-.345.282-.63.63-.63.345 0 .63.285.63.63v4.771zm-5.741 0c0 .344-.282.629-.631.629-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63.346 0 .628.285.628.63v4.771zm-2.466.629H4.917c-.345 0-.63-.285-.63-.629V8.108c0-.345.285-.63.63-.63.348 0 .63.285.63.63v4.141h1.756c.348 0 .629.283.629.63 0 .344-.282.629-.629.629M24 10.314C24 4.943 18.615.572 12 .572S0 4.943 0 10.314c0 4.811 4.27 8.842 10.035 9.608.391.082.923.258 1.058.59.12.301.079.766.038 1.08l-.164 1.02c-.045.301-.24 1.186 1.049.645 1.291-.539 6.916-4.078 9.436-6.975C23.176 14.393 24 12.458 24 10.314"/></svg>
```

partials/icons/social/linkedin.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
```

partials/icons/social/livestream.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.987 6.248l.041.002.039.006.04.011.039.015.038.02.039.022.035.03.035.029.037.045.046.045.03.045.044.045.075.119.029.06.029.075.03.074.031.074.028.074.029.09.029.09.03.09.031.089.029.104.028.104.031.105.03.104.029.104.029.104.03.12.03.118.029.135.015.12.029.134.03.134.017.135.028.149.015.148.015.149.031.149.015.149.016.148.015.165.015.164.015.163.015.165.015.164.016.179.015.343.016.179.015.179.015.18.015.18.015.193.015.193.015.193.016.195.015.193v.388l.016.209.015.209v.403l.015.208v.611l.015.419.015.625v1.269l.015.373.03.269.046.179.043.119.047.104.059.09.045.044.045.045.044.045.062.029.089.046.089.029.096.03.142.029.193.011.269-.016h.1v2.253l-.239.029-.566.026-.61-.029-.448-.067-.344-.089-.254-.089-.237-.119-.236-.15-.208-.184-.134-.134-.136-.149-.17-.269-.15-.313-.119-.342-.082-.403-.054-.456-.015-.508v-1.938l-.015-.418v-.865l-.015-.402v-.287l-.016-.199v-.397l-.015-.194v-.193l-.008-.193-.015-.194-.014-.179-.003-.18-.015-.179-.015-.183v-.178l-.015-.18-.017-.179-.012-.179-.014-.17-.017-.17-.015-.164-.015-.169-.015-.16-.014-.163-.015-.164-.017-.15-.015-.148-.016-.158-.015-.141-.015-.135-.044-.278-.016-.134-.015-.135-.03-.125-.026-.135-.029-.118-.03-.12-.031-.119-.034-.103-.029-.104-.025-.103-.045-.09-.029-.104-.029-.089-.022-.09-.029-.089-.031-.09-.03-.074-.029-.076-.029-.074-.03-.059-.03-.061-.029-.06-.044-.06-.03-.045-.036-.045-.031-.044-.041-.03-.028-.029-.046-.03-.028-.015-.046-.016-.049-.012-.044-.016-.03-.015h-.03 2.552l-.051.031zM.008 3.082l1.169.021 1.089.026.97.015.851.03.73.029.642.029.567.03.506.029.463.046.418.044.387.046.357.044.329.046.313.044.283.061.27.059.252.059.24.06.223.06.209.06.194.075.194.059.179.074.163.076.166.074.148.074.164.074.148.09.135.09.135.09.119.088.119.09.119.09.119.09.104.09.104.104.104.09.105.104.09.104.09.104.104.105.09.104.09.104.074.104.09.105.074.119.074.104.074.119.075.12.074.119.074.12.06.119.061.119.074.119.06.119.06.119.06.119.06.12.045.118.048.12.06.135.05.118.06.135.06.119.044.119.061.135.054.135.044.119.051.134.045.12.045.133.045.135.045.135.045.134.044.135.03.134.045.135.039.135.029.133.039.135.029.135.041.134.029.134.045.135.029.119.045.135v.014l.029.12.031.127.029.134.029.135.03.119.03.135.029.133.045.12.029.134.03.119.03.135.029.119.029.119.03.12.03.119.029.12.03.119.03.119.029.119.029.119.03.119.03.119.014.12.03.104.046.223.029.105.029.104.03.104.022.104.029.104.016.104.029.104.03.104.015.104.029.105.03.09.03.097.015.089.03.09.015.09.015.089.015.09.015.075.016.09.015.085.016.075.014.074.016.078.024.074.015.074.015.075.015.068.016.06.023.074.023.061.016.065.015.06.016.06.015.06.015.06.015.06.015.045.03.051.015.045.015.045.016.044.029.046.015.044.038.075.015.038.03.061.015.029.015.03.015.029.016.03.015.015.015.015.015.015.016.015.015.016.029.016.016.004.015.015h.03-7.027l-.051-.015-.057-.016-.057-.014-.06-.016-.06-.015h-.016l-.052-.024-.056-.015-.057-.031-.061-.03-.044-.029-.06-.03-.045-.029-.061-.03-.044-.045-.044-.045-.061-.045-.045-.045-.06-.044-.06-.06-.06-.056-.044-.06-.061-.054-.06-.045-.06-.06-.061-.06-.044-.06-.062-.005-.059-.06-.045-.068-.054-.065-.119-.148-.059-.075-.045-.074-.061-.09-.059-.074-.061-.09-.06-.075-.06-.088-.06-.09-.06-.09-.061-.09-.059-.09-.061-.09-.06-.089-.06-.104-.059-.09-.046-.104-.06-.105-.06-.104-.06-.105-.061-.104-.059-.104-.06-.104-.06-.104-.061-.104-.059-.104-.061-.104-.059-.104-.061-.119-.06-.12-.06-.119-.061-.12-.059-.119-.061-.119-.059-.119-.06-.119-.135-.028-.049-.126-.059-.123-.061-.123-.059-.125-.064-.125-.06-.127-.06-.119-.064-.119-.06-.119-.063-.119-.06-.119-.06-.15-.06-.134-.063-.119-.063-.12-.06-.134-.063-.119-.061-.135-.06-.119-.06-.135-.06-.134-.06-.134-.058-.134-.059-.135-.061-.119-.059-.134-.059-.133-.059-.135-.06-.135-.06-.134-.119-.268-.06-.149-.06-.12-.059-.134-.061-.12-.06-.119-.073-.118-.06-.135-.074-.12-.06-.118-.074-.12-.061-.119-.059-.12-.06-.119-.06-.119-.059-.137-.12-.239-.06-.119-.061-.119-.074-.119-.074-.119-.135-.229-.058-.119-.074-.11-.076-.12-.059-.112-.061-.104-.125-.208-.074-.106-.061-.103-.058-.105-.061-.089-.06-.105-.063-.104-.066-.09-.059-.09-.074-.09-.076-.088-.059-.089-.075-.09-.088-.117-.067-.076-.069-.078-.059-.074-.058-.1-.074-.074-.066-.06-.075-.069-.062-.065-.075-.081-.065-.06-.065-.06-.068-.058-.067-.053-.069-.045-.07-.045L.672 3.4l-.075-.046-.06-.044-.074-.044-.067-.03-.068-.03-.07-.03-.071-.03-.068-.031-.059-.023L0 3.086h.008v-.004z"/></svg>
```

partials/icons/social/mailchimp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.98 11.341c.165-.021.332-.021.497 0 .089-.205.104-.558.024-.942-.12-.571-.28-.917-.613-.863-.333.054-.346.468-.226 1.039.067.321.186.596.319.766zM15.12 11.793c.239.105.385.174.442.114.037-.038.026-.11-.03-.203-.118-.193-.36-.388-.617-.497a1.677 1.677 0 0 0-1.634.196c-.16.117-.31.28-.29.378.008.032.031.056.087.064.132.015.591-.217 1.12-.25.374-.023.684.094.922.199zm-.48.274c-.31.05-.481.152-.591.247-.094.082-.152.173-.152.237l.024.057.051.02c.07 0 .228-.064.228-.064a1.975 1.975 0 0 1 1-.104c.155.018.23.028.263-.026.01-.015.023-.049-.008-.1-.073-.118-.387-.317-.814-.266zM17.015 13.073c.21.104.442.063.518-.09.076-.155-.034-.364-.245-.467-.21-.104-.442-.063-.518.09-.076.155.034.364.245.467zm1.355-1.186c-.171-.003-.314.185-.317.421-.004.235.131.428.302.431.171.003.314-.185.318-.42.003-.235-.132-.428-.303-.432zM6.866 16.13c-.042-.053-.112-.037-.18-.021a.646.646 0 0 1-.16.022.347.347 0 0 1-.292-.148c-.078-.12-.073-.299.012-.504l.04-.092c.138-.308.368-.825.11-1.317-.194-.37-.511-.602-.892-.65a1.145 1.145 0 0 0-.983.355c-.379.418-.438.988-.364 1.19.027.073.069.094.099.098.065.009.16-.038.22-.2l.017-.052c.026-.085.076-.243.157-.37a.688.688 0 0 1 .953-.2c.266.175.368.5.255.811-.059.161-.154.468-.133.72.043.512.357.717.638.74.274.01.466-.145.514-.258.03-.066.005-.107-.01-.125v.001z"/><path d="M22.691 15.194c-.01-.037-.078-.286-.172-.586l-.19-.51c.375-.563.381-1.066.332-1.35-.054-.353-.2-.654-.496-.964-.295-.312-.9-.63-1.75-.868l-.445-.124c-.002-.018-.023-1.053-.043-1.497-.013-.32-.041-.822-.196-1.315-.185-.669-.507-1.253-.91-1.627 1.11-1.152 1.803-2.422 1.801-3.511-.003-2.095-2.571-2.73-5.736-1.416l-.67.285a666.1 666.1 0 0 0-1.23-1.207C9.376-2.65-1.905 9.912 1.701 12.964l.789.668a3.885 3.885 0 0 0-.22 1.793c.085.84.517 1.644 1.218 2.266.665.59 1.54.965 2.389.964 1.403 3.24 4.61 5.228 8.37 5.34 4.034.12 7.42-1.776 8.84-5.182.093-.24.486-1.317.486-2.267 0-.956-.539-1.352-.882-1.352zm-16.503 2.55a1.94 1.94 0 0 1-.374.027c-1.218-.033-2.534-1.131-2.665-2.435-.145-1.44.59-2.548 1.89-2.81a2.22 2.22 0 0 1 .547-.04c.729.04 1.803.6 2.048 2.191.217 1.408-.128 2.843-1.446 3.068zm-1.36-6.08c-.81.157-1.524.617-1.96 1.252-.261-.218-.747-.64-.833-.804-.697-1.325.76-3.902 1.778-5.357C6.33 3.159 10.268.437 12.093.931c.296.084 1.278 1.224 1.278 1.224s-1.823 1.013-3.514 2.426c-2.278 1.757-3.999 4.311-5.03 7.083zm12.787 5.542a.072.072 0 0 0 .042-.071.067.067 0 0 0-.074-.06s-1.908.283-3.711-.379c.196-.639.718-.408 1.508-.344a11.01 11.01 0 0 0 3.64-.394c.816-.235 1.888-.698 2.722-1.356.28.618.38 1.298.38 1.298s.217-.039.399.073c.171.106.297.326.211.895-.175 1.063-.626 1.926-1.384 2.72a5.698 5.698 0 0 1-1.663 1.244 7.018 7.018 0 0 1-1.085.46c-2.858.935-5.784-.093-6.727-2.3a3.582 3.582 0 0 1-.19-.522c-.401-1.455-.06-3.2 1.007-4.299.065-.07.132-.153.132-.256 0-.087-.055-.178-.102-.243-.373-.542-1.666-1.466-1.406-3.254.186-1.285 1.308-2.189 2.353-2.135l.265.015c.453.027.848.085 1.222.101.624.027 1.185-.064 1.85-.619.224-.187.404-.35.708-.401.032-.005.111-.034.27-.026a.892.892 0 0 1 .456.146c.533.355.608 1.215.636 1.845.016.36.059 1.228.074 1.478.034.57.183.65.486.75.17.057.329.099.562.164.705.199 1.123.4 1.387.659.158.161.23.333.253.497.084.608-.47 1.359-1.938 2.041-1.605.746-3.55.935-4.895.785l-.471-.053c-1.076-.145-1.689 1.247-1.044 2.201.416.615 1.55 1.015 2.683 1.015 2.6 0 4.598-1.111 5.341-2.072l.06-.085c.036-.055.006-.085-.04-.054-.607.416-3.304 2.069-6.19 1.571 0 0-.35-.057-.67-.182-.254-.099-.786-.344-.85-.891 2.328.721 3.793.039 3.793.039zm-3.688-.436l.001.001v-.002zM9.473 6.74c.895-1.036 1.996-1.936 2.982-2.441.034-.017.07.02.052.053-.079.142-.23.447-.277.677a.04.04 0 0 0 .061.042c.614-.419 1.681-.868 2.618-.925.04-.003.06.049.027.074-.154.119-.293.258-.411.413a.04.04 0 0 0 .031.064c.657.005 1.584.235 2.188.575.04.023.012.102-.034.092-.914-.21-2.41-.37-3.964.01-1.387.339-2.446.862-3.218 1.425-.04.029-.086-.023-.055-.06z"/></svg>
```

partials/icons/social/makerbot.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.055 7.328c-.604-1.428-1.47-2.714-2.569-3.813C19.382 2.414 18.1 1.551 16.672.944 15.189.315 13.619 0 12 0c-1.62 0-3.19.318-4.672.945-1.428.604-2.711 1.47-3.813 2.57C2.414 4.615 1.551 5.9.943 7.328.315 8.81 0 10.38 0 12c0 1.619.318 3.189.945 4.671.604 1.429 1.47 2.714 2.569 3.814 1.103 1.1 2.386 1.964 3.813 2.57C8.81 23.686 10.38 24 12 24c1.619 0 3.189-.314 4.671-.944 1.429-.601 2.711-1.471 3.814-2.564 1.1-1.095 1.964-2.386 2.57-3.811.63-1.47.944-3.045.944-4.665 0-1.619-.314-3.18-.944-4.664v-.024zM12 22.335C6.293 22.335 1.665 17.707 1.665 12S6.293 1.665 12 1.665 22.335 6.293 22.335 12 17.707 22.335 12 22.335zm3.242-18.214H8.757c-.922 0-1.7.324-2.333.975-.635.644-.953 1.425-.953 2.334v10.182c0 .449.135.81.4 1.095.267.269.615.42 1.051.42.445 0 .805-.135 1.079-.405.272-.271.409-.63.409-1.08V7.08h2.141v10.529c0 .445.131.806.391 1.08.259.273.611.411 1.059.411.446 0 .799-.138 1.059-.411.26-.274.39-.635.39-1.08V7.08h2.142v10.529c0 .445.135.806.408 1.08.275.273.635.411 1.08.411.435 0 .783-.141 1.05-.423.268-.28.401-.638.401-1.069V7.426c0-.91-.318-1.688-.953-2.336-.633-.648-1.41-.975-2.334-.975v.006z"/></svg>
```

partials/icons/social/mastercard.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.343 18.031c.058.049.12.098.181.146-1.177.783-2.59 1.238-4.107 1.238C3.32 19.416 0 16.096 0 12c0-4.095 3.32-7.416 7.416-7.416 1.518 0 2.931.456 4.105 1.238-.06.051-.12.098-.165.15C9.6 7.489 8.595 9.688 8.595 12c0 2.311 1.001 4.51 2.748 6.031zm5.241-13.447c-1.52 0-2.931.456-4.105 1.238.06.051.12.098.165.15C14.4 7.489 15.405 9.688 15.405 12c0 2.31-1.001 4.507-2.748 6.031-.058.049-.12.098-.181.146 1.177.783 2.588 1.238 4.107 1.238C20.68 19.416 24 16.096 24 12c0-4.094-3.32-7.416-7.416-7.416zM12 6.174c-.096.075-.189.15-.28.231C10.156 7.764 9.169 9.765 9.169 12c0 2.236.987 4.236 2.551 5.595.09.08.185.158.28.232.096-.074.189-.152.28-.232 1.563-1.359 2.551-3.359 2.551-5.595 0-2.235-.987-4.236-2.551-5.595-.09-.08-.184-.156-.28-.231z"/></svg>
```

partials/icons/social/mastodon.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.193 7.879c0-5.206-3.411-6.732-3.411-6.732C18.062.357 15.108.025 12.041 0h-.076c-3.068.025-6.02.357-7.74 1.147 0 0-3.411 1.526-3.411 6.732 0 1.192-.023 2.618.015 4.129.124 5.092.934 10.109 5.641 11.355 2.17.574 4.034.695 5.535.612 2.722-.15 4.25-.972 4.25-.972l-.09-1.975s-1.945.613-4.129.539c-2.165-.074-4.449-.233-4.799-2.891a5.499 5.499 0 0 1-.048-.745s2.125.52 4.817.643c1.646.075 3.19-.097 4.758-.283 3.007-.359 5.625-2.212 5.954-3.905.517-2.665.475-6.507.475-6.507zm-4.024 6.709h-2.497V8.469c0-1.29-.543-1.944-1.628-1.944-1.2 0-1.802.776-1.802 2.312v3.349h-2.483v-3.35c0-1.536-.602-2.312-1.802-2.312-1.085 0-1.628.655-1.628 1.944v6.119H4.832V8.284c0-1.289.328-2.313.987-3.07.68-.758 1.569-1.146 2.674-1.146 1.278 0 2.246.491 2.886 1.474L12 6.585l.622-1.043c.64-.983 1.608-1.474 2.886-1.474 1.104 0 1.994.388 2.674 1.146.658.757.986 1.781.986 3.07v6.304z"/></svg>
```

partials/icons/social/medium.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.846 6.36c.03-.295-.083-.586-.303-.784l-2.24-2.7v-.403H7.26l5.378 11.795 4.728-11.795H24v.403l-1.917 1.837c-.165.126-.247.333-.213.538v13.5c-.034.204.048.41.213.537l1.87 1.837v.403h-9.41v-.403l1.937-1.882c.19-.19.19-.246.19-.538V7.794l-5.39 13.688h-.727L4.278 7.794v9.174c-.052.386.076.774.347 1.053l2.52 3.06v.402H0v-.403l2.52-3.06c.27-.278.39-.67.326-1.052V6.36z"/></svg>
```

partials/icons/social/meetup.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.978 20.238c-.304-1.931-3.874-.444-4.096-2.559-.313-2.998 4.15-9.459 3.797-11.972-.313-2.255-1.841-2.73-3.165-2.756-1.284-.02-1.623.182-2.058.435-.253.146-.612.435-1.112-.041-.334-.318-.557-.536-.905-.819-.182-.142-.466-.324-.945-.395-.476-.071-1.098 0-1.492.167-.395.172-.702.466-1.026.749-.323.283-1.147 1.198-1.911.859-.335-.145-1.458-.706-2.272-1.055-1.563-.677-3.822.42-4.636 1.866C2.944 6.866.557 15.32.193 16.432c-.809 2.502 1.032 4.54 3.509 4.424 1.052-.051 1.75-.43 2.412-1.638.384-.693 3.979-10.087 4.248-10.543.197-.323.844-.753 1.39-.475.551.283.662.869.581 1.421-.136.895-2.669 6.629-2.771 7.275-.162 1.103.359 1.714 1.507 1.774.784.041 1.567-.237 2.184-1.41.349-.652 4.349-8.666 4.702-9.202.39-.586.703-.779 1.103-.758.309.015.799.096.678 1.016-.122.905-3.343 6.78-3.676 8.221-.456 1.927.602 3.874 2.341 4.728 1.112.546 5.97 1.476 5.577-1.027z"/></svg>
```

partials/icons/social/messenger.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.373 0 0 4.974 0 11.111c0 3.498 1.744 6.614 4.469 8.654V24l4.088-2.242c1.092.3 2.246.464 3.443.464 6.627 0 12-4.975 12-11.11S18.627 0 12 0zm1.191 14.963l-3.055-3.26-5.963 3.26L10.732 8l3.131 3.259L19.752 8l-6.561 6.963z"/></svg>
```

partials/icons/social/microblog.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.4 17.7c-2 2.6-1 4.8-.3 5.9.3.4-.1.4-.3.4a6 6 0 0 1-4-2.7c-.2-.1-.3-.2-.5-.1-1.4.4-2.8.7-4.3.6C5.4 21.8 0 17 0 11 0 5 5.4 0 12 0s12 4.9 12 11c0 2.5-1 4.8-2.6 6.7zM12 14l3.2 2.2a.4.4 0 0 0 .6-.4L14.6 12l3.1-2.4a.4.4 0 0 0-.2-.6h-3.9l-1.3-3.8a.4.4 0 0 0-.6 0L10.4 9h-4a.4.4 0 0 0-.1.7l3 2.4-1 3.7a.4.4 0 0 0 .5.4L12 14z"/></svg>
```

partials/icons/social/net.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M3.1672 7.5655v8.749H4.19v-6.325a8.979 8.979 0 0 0-.0488-1.1998h.0384a2.9082 2.9082 0 0 0 .2784.5473l4.4973 6.9774h1.2569V7.5655H9.1904v6.1526a9.2574 9.2574 0 0 0 .0619 1.286h-.0234c-.0544-.1056-.173-.3002-.3553-.585L4.4964 7.5656zm9.315 0v8.749h4.65l.0048-.9599h-3.6087v-3.0331h3.1579V11.4h-3.1579V8.4916h3.3884v-.926zm5.4374 0v.926h2.5149v7.823h1.0216v-7.823H24v-.926zM.6534 15.067a.643.643 0 0 0-.4565.2062A.6719.6719 0 0 0 0 15.753a.6623.6623 0 0 0 .1968.4799.6479.6479 0 0 0 .4799.2015.6623.6623 0 0 0 .4799-.2015.6575.6575 0 0 0 .2015-.48.667.667 0 0 0-.2015-.4798.6575.6575 0 0 0-.4799-.2062.643.643 0 0 0-.0234 0z"/></svg>
```

partials/icons/social/netflix.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M5.39.004l4.75 13.46v-.007l.376 1.06c2.088 5.908 3.21 9.075 3.216 9.082.004 0 .32.02.702.04 1.156.05 2.59.18 3.676.31.25.03.466.04.48.03l-4.71-13.36-.436-1.23-2.423-6.85c-.46-1.3-.85-2.408-.87-2.45L10.12 0H5.395z"/><path d="M13.898.012l-.01 5.306-.008 5.306-.437-1.232V9.39l-.565 11.81c.555 1.567.852 2.403.855 2.407.004.004.32.024.702.042 1.157.05 2.59.18 3.68.31.25.03.467.04.48.03s.02-5.42.017-12.01L18.604.01h-4.706zM5.39.002v11.99c0 6.594.007 11.995.015 12.003s.416-.03.907-.086c.49-.06 1.17-.13 1.51-.16.518-.05 2.068-.15 2.248-.15.052 0 .056-.27.063-5.08l.008-5.08.38 1.06.13.376.57-11.8-.19-.546-.88-2.44-.03-.087H5.39z"/></svg>
```

partials/icons/social/netlify.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path class="a" d="M16.934 8.519a1.044 1.044 0 0 1 .303.23l2.349-1.045-2.192-2.171-.491 2.954zM12.06 6.546a1.305 1.305 0 0 1 .209.574l3.497 1.482a1.044 1.044 0 0 1 .355-.177l.574-3.55-2.13-2.234-2.505 3.852v.053zm11.933 5.491l-3.748-3.748-2.548 1.044 6.264 2.662s.053.042.032.042zm-.627.606l-6.013-2.569a1.044 1.044 0 0 1-.7.407l-.647 3.957a1.044 1.044 0 0 1 .303.731l3.633.762 3.33-3.31v-.062zM15.4 9.25L12.132 7.86a1.2 1.2 0 0 1-1.044.543h-.199L8.185 12.58l7.225-3.132v.01a.887.887 0 0 1 0-.167.052.052 0 0 0-.01-.041zm3.967 7.308l-3.195-.658a1.096 1.096 0 0 1-.46.344l-.761 4.72 4.437-4.396s-.01.02-.021.02zm-4.469-.324a1.044 1.044 0 0 1-.616-.71l-5.95-1.222-.084.136 5.398 7.81.323-.324.919-5.67s.031.022.01.011zm-6.441-2.652l5.878 1.211a1.044 1.044 0 0 1 .824-.522l.637-3.894-.135-.115-7.308 3.132a1.817 1.817 0 0 1 .104.188zm-2.464.981l-.125-.125-2.537 1.044 1.232 1.222 1.399-2.172zm1.67.397a1.368 1.368 0 0 1-.563.125 1.389 1.389 0 0 1-.45-.073l-1.544 2.245 6.765 6.702 1.19-1.18zm-.95-2.641a1.702 1.702 0 0 1 .314 0 1.378 1.378 0 0 1 .344 0l2.735-4.25a1.19 1.19 0 0 1-.334-.824 1.242 1.242 0 0 1 0-.271l-3.32-1.535-2.672 2.6zm.303-7.402l3.237 1.378a1.242 1.242 0 0 1 .835-.282 1.357 1.357 0 0 1 .397.063l2.526-3.947L11.923.041 7.016 4.854s-.01.052 0 .063zm-1.21 8.164a1.566 1.566 0 0 1 .24-.334L3.278 8.613 0 11.797l5.804 1.284zm-.262.7L.533 12.735l2.203 2.235 2.777-1.18z"/></svg>
```

partials/icons/social/nintendoswitch.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.176 24h3.674c3.376 0 6.15-2.774 6.15-6.15V6.15C24 2.775 21.226 0 17.85 0H14.1c-.074 0-.15.074-.15.15v23.7c-.001.076.075.15.226.15zm4.574-13.199c1.351 0 2.399 1.125 2.399 2.398 0 1.352-1.125 2.4-2.399 2.4-1.35 0-2.4-1.049-2.4-2.4-.075-1.349 1.05-2.398 2.4-2.398zM11.4 0H6.15C2.775 0 0 2.775 0 6.15v11.7C0 21.226 2.775 24 6.15 24h5.25c.074 0 .15-.074.15-.149V.15c.001-.076-.075-.15-.15-.15zM9.676 22.051H6.15c-2.326 0-4.201-1.875-4.201-4.201V6.15c0-2.326 1.875-4.201 4.201-4.201H9.6l.076 20.102zM3.75 7.199c0 1.275.975 2.25 2.25 2.25s2.25-.975 2.25-2.25c0-1.273-.975-2.25-2.25-2.25s-2.25.977-2.25 2.25z"/></svg>
```

partials/icons/social/notion.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.459 4.208c.746.606 1.026.56 2.428.466l13.215-.793c.28 0 .047-.28-.046-.326L17.86 1.968c-.42-.326-.981-.7-2.055-.607L3.01 2.295c-.466.046-.56.28-.374.466zm.793 3.08v13.904c0 .747.373 1.027 1.214.98l14.523-.84c.841-.046.935-.56.935-1.167V6.354c0-.606-.233-.933-.748-.887l-15.177.887c-.56.047-.747.327-.747.933zm14.337.745c.093.42 0 .84-.42.888l-.7.14v10.264c-.608.327-1.168.514-1.635.514-.748 0-.935-.234-1.495-.933l-4.577-7.186v6.952L12.21 19s0 .84-1.168.84l-3.222.186c-.093-.186 0-.653.327-.746l.84-.233V9.854L7.822 9.76c-.094-.42.14-1.026.793-1.073l3.456-.233 4.764 7.279v-6.44l-1.215-.139c-.093-.514.28-.887.747-.933zM1.936 1.035l13.31-.98c1.634-.14 2.055-.047 3.082.7l4.249 2.986c.7.513.934.653.934 1.213v16.378c0 1.026-.373 1.634-1.68 1.726l-15.458.934c-.98.047-1.448-.093-1.962-.747l-3.129-4.06c-.56-.747-.793-1.306-.793-1.96V2.667c0-.839.374-1.54 1.447-1.632z"/></svg>
```

partials/icons/social/npm.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 7.334v8h6.666v1.332H12v-1.332h12v-8H0zm6.666 6.664H5.334v-4H3.999v4H1.335V8.667h5.331v5.331zm4 0v1.336H8.001V8.667h5.334v5.332h-2.669v-.001zm12.001 0h-1.33v-4h-1.336v4h-1.335v-4h-1.33v4h-2.671V8.667h8.002v5.331z"/><path d="M10.665 10H12v2.667h-1.335V10z"/></svg>
```

partials/icons/social/nvidia.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M8.948 8.798v-1.43a6.7 6.7 0 0 1 .424-.018c3.922-.124 6.493 3.374 6.493 3.374s-2.774 3.851-5.75 3.851c-.398 0-.787-.062-1.158-.185v-4.346c1.528.185 1.837.857 2.747 2.385l2.04-1.714s-1.492-1.952-4-1.952a6.016 6.016 0 0 0-.796.035m0-4.735v2.138l.424-.027c5.45-.185 9.01 4.47 9.01 4.47s-4.08 4.964-8.33 4.964c-.37 0-.733-.035-1.095-.097v1.325c.3.035.61.062.91.062 3.957 0 6.82-2.023 9.593-4.408.459.371 2.34 1.263 2.73 1.652-2.633 2.208-8.772 3.984-12.253 3.984-.335 0-.653-.018-.971-.053v1.864H24V4.063zm0 10.326v1.131c-3.657-.654-4.673-4.46-4.673-4.46s1.758-1.944 4.673-2.262v1.237H8.94c-1.528-.186-2.73 1.245-2.73 1.245s.68 2.412 2.739 3.11M2.456 10.9s2.164-3.197 6.5-3.533V6.201C4.153 6.59 0 10.653 0 10.653s2.35 6.802 8.948 7.42v-1.237c-4.84-.6-6.492-5.936-6.492-5.936z"/></svg>
```

partials/icons/social/oculus.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.135 13.949c-.319.221-.675.355-1.057.416s-.761.049-1.142.049H8.063c-.382 0-.762.014-1.145-.049-.381-.063-.734-.195-1.057-.416-.643-.451-1.027-1.17-1.027-1.951 0-.796.387-1.515 1.029-1.95.314-.225.674-.359 1.049-.42s.75-.061 1.141-.061h7.875c.375 0 .765-.014 1.14.046s.735.194 1.051.405c.645.434 1.02 1.17 1.02 1.949 0 .78-.391 1.5-1.035 1.95l.031.032zm3.174-7.555c-.845-.678-1.812-1.146-2.865-1.398-.6-.146-1.203-.211-1.822-.23-.449-.015-.899-.01-1.364-.01H8.76c-.457 0-.915-.005-1.372.01-.618.021-1.222.083-1.825.23-1.051.254-2.025.723-2.865 1.4C.99 7.761 0 9.82 0 12c0 2.182.99 4.241 2.689 5.606.846.678 1.815 1.146 2.865 1.4.603.146 1.206.211 1.823.229.45.016.9.012 1.365.012h6.496c.449 0 .914.004 1.364-.012.615-.018 1.215-.082 1.814-.229 1.05-.256 2.011-.723 2.866-1.402C23.01 16.24 24 14.18 24 12c0-2.181-.99-4.241-2.691-5.606z"/></svg>
```

partials/icons/social/odnoklassniki.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.505 17.44c1.275-.29 2.493-.794 3.6-1.49.834-.558 1.058-1.686.5-2.52-.536-.802-1.604-1.044-2.435-.553-2.55 1.595-5.79 1.595-8.34 0-.847-.534-1.965-.28-2.5.565 0 .002 0 .004-.002.005-.534.847-.28 1.966.567 2.5l.002.002c1.105.695 2.322 1.2 3.596 1.488l-3.465 3.465c-.707.695-.72 1.83-.028 2.537l.03.03c.344.354.81.53 1.274.53.465 0 .93-.176 1.275-.53L12 20.065l3.404 3.406c.72.695 1.87.676 2.566-.045.678-.703.678-1.818 0-2.52l-3.465-3.466zM12 12.388c3.42-.004 6.19-2.774 6.195-6.193C18.195 2.78 15.415 0 12 0S5.805 2.78 5.805 6.197c.005 3.42 2.776 6.19 6.195 6.192zm0-8.757c1.416.002 2.563 1.15 2.564 2.565 0 1.416-1.148 2.563-2.564 2.565-1.415-.002-2.562-1.148-2.565-2.564C9.437 4.78 10.585 3.633 12 3.63z"/></svg>
```

partials/icons/social/origin.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.588 3.11c1.189.071 2.352.384 3.417.919 1.031.514 1.95 1.225 2.706 2.094.751.865 1.322 1.853 1.715 2.963.391 1.109.548 2.278.464 3.502-.033.636-.135 1.252-.306 1.848-.167.588-.393 1.159-.674 1.703-.439.849-.929 1.652-1.47 2.412-.538.759-1.125 1.465-1.762 2.118-.638.653-1.313 1.254-2.032 1.802-.719.544-1.471 1.038-2.254 1.479l-.037.026c-.033.018-.071.026-.109.023-.063-.015-.118-.048-.159-.097-.041-.05-.063-.111-.062-.173 0-.029.004-.059.012-.085.008-.023.021-.044.037-.062.277-.393.506-.806.686-1.235.181-.434.303-.885.368-1.359 0-.032-.015-.064-.038-.085-.021-.025-.053-.038-.085-.038-.264.032-.528.053-.795.062-.266.009-.532-.003-.796-.037-1.189-.071-2.353-.385-3.418-.918-1.031-.515-1.949-1.226-2.705-2.095-.754-.87-1.336-1.875-1.715-2.963-.394-1.123-.552-2.314-.465-3.502.033-.636.135-1.252.306-1.848.171-.598.396-1.155.675-1.68.439-.864.931-1.676 1.469-2.436.539-.757 1.125-1.464 1.761-2.118.639-.652 1.314-1.252 2.033-1.8.72-.546 1.47-1.039 2.253-1.479l.038-.025c.033-.02.07-.027.109-.025.065.016.119.051.158.098.043.051.062.106.062.174.001.027-.003.057-.012.084-.007.023-.02.043-.036.061-.273.386-.505.801-.687 1.237-.181.433-.3.885-.366 1.358 0 .033.012.063.036.086.022.024.054.037.085.037.262-.033.527-.053.795-.061.272-.009.536.003.798.035zm-.807 12.367c.922.079 1.838-.231 2.521-.855.72-.639 1.109-1.438 1.176-2.4.078-.928-.232-1.846-.856-2.535-.601-.708-1.472-1.131-2.4-1.162-.927-.078-1.845.232-2.534.855-.709.602-1.132 1.473-1.164 2.4-.078.926.228 1.842.846 2.535.628.725 1.432 1.115 2.411 1.162z"/></svg>
```

partials/icons/social/overcast.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 24C5.389 24.018.017 18.671 0 12.061V12C0 5.35 5.351 0 12 0s12 5.35 12 12c0 6.649-5.351 12-12 12zm0-4.751l.9-.899-.9-3.45-.9 3.45.9.899zm-1.15-.05L10.4 20.9l1.05-1.052-.6-.649zm2.3 0l-.6.601 1.05 1.051-.45-1.652zm.85 3.102L12 20.3l-2 2.001c.65.1 1.3.199 2 .199s1.35-.05 2-.199zM12 1.5C6.201 1.5 1.5 6.201 1.5 12c-.008 4.468 2.825 8.446 7.051 9.899l2.25-8.35c-.511-.372-.809-.968-.801-1.6 0-1.101.9-2.001 2-2.001s2 .9 2 2.001c0 .649-.301 1.2-.801 1.6l2.25 8.35c4.227-1.453 7.06-5.432 7.051-9.899 0-5.799-4.701-10.5-10.5-10.5zm6.85 15.7c-.255.319-.714.385-1.049.15-.313-.207-.4-.628-.194-.941.014-.021.028-.04.044-.06 0 0 1.35-1.799 1.35-4.35s-1.35-4.35-1.35-4.35c-.239-.289-.198-.719.091-.957.02-.016.039-.031.06-.044.335-.235.794-.169 1.049.15.1.101 1.65 2.15 1.65 5.2S18.949 17.1 18.85 17.2zm-3.651-1.95c-.3-.3-.249-.85.051-1.15 0 0 .75-.799.75-2.1s-.75-2.051-.75-2.1c-.3-.301-.3-.801-.051-1.15.232-.303.666-.357.969-.125.029.022.056.047.082.074C16.301 8.75 17.5 10 17.5 12s-1.199 3.25-1.25 3.301c-.301.299-.75.25-1.051-.051zm-6.398 0c-.301.301-.75.35-1.051.051C7.699 15.199 6.5 14 6.5 12s1.199-3.199 1.25-3.301c.301-.299.801-.299 1.051.051.3.3.249.85-.051 1.15 0 .049-.75.799-.75 2.1s.75 2.1.75 2.1c.3.3.351.799.051 1.15zm-2.602 2.101c-.335.234-.794.169-1.05-.15C5.051 17.1 3.5 15.05 3.5 12s1.551-5.1 1.649-5.2c.256-.319.715-.386 1.05-.15.313.206.4.628.194.941-.013.02-.028.04-.043.059C6.35 7.65 5 9.449 5 12s1.35 4.35 1.35 4.35c.25.3.15.75-.151 1.001z"/></svg>
```

partials/icons/social/patreon.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.386.524c-4.764 0-8.64 3.876-8.64 8.64 0 4.75 3.876 8.613 8.64 8.613 4.75 0 8.614-3.864 8.614-8.613C24 4.4 20.136.524 15.386.524M.003 23.537h4.22V.524H.003"/></svg>
```

partials/icons/social/paypal.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M6.908 24H3.804c-.664 0-1.086-.529-.936-1.18l.149-.674h2.071c.666 0 1.336-.533 1.482-1.182l1.064-4.592c.15-.648.816-1.18 1.48-1.18h.883c3.789 0 6.734-.779 8.84-2.34s3.16-3.6 3.16-6.135c0-1.125-.195-2.055-.588-2.789 0-.016-.016-.031-.016-.046l.135.075c.75.465 1.32 1.064 1.711 1.814.404.75.598 1.68.598 2.791 0 2.535-1.049 4.574-3.164 6.135-2.1 1.545-5.055 2.324-8.834 2.324h-.9c-.66 0-1.334.525-1.484 1.186L8.39 22.812c-.149.645-.81 1.17-1.47 1.17L6.908 24zm-2.677-2.695H1.126c-.663 0-1.084-.529-.936-1.18L4.563 1.182C4.714.529 5.378 0 6.044 0h6.465c1.395 0 2.609.098 3.648.289 1.035.189 1.92.519 2.684.99.736.465 1.322 1.072 1.697 1.818.389.748.584 1.68.584 2.797 0 2.535-1.051 4.574-3.164 6.119-2.1 1.561-5.056 2.326-8.836 2.326h-.883c-.66 0-1.328.524-1.478 1.169L5.7 20.097c-.149.646-.817 1.172-1.485 1.172l.016.036zm7.446-17.369h-1.014c-.666 0-1.332.529-1.48 1.178l-.93 4.02c-.15.648.27 1.179.93 1.179h.766c1.664 0 2.97-.343 3.9-1.021.929-.686 1.395-1.654 1.395-2.912 0-.83-.301-1.445-.9-1.84-.6-.404-1.5-.605-2.686-.605l.019.001z"/></svg>
```

partials/icons/social/periscope.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.135 24c1.875 0 9.314-8.439 9.314-14.096C21.449 4.49 17.22 0 12.135 0 6.78 0 2.551 4.488 2.551 9.904 2.551 15.56 9.99 24 12.135 24zM10.639 3.846c.485-.12.995-.185 1.524-.185 3 0 5.581 2.551 5.581 5.865 0 2.985-2.581 5.535-5.596 5.535-3.345 0-5.925-2.55-5.925-5.535 0-1.396.45-2.64 1.229-3.63v.03c0 1.245 1.006 2.234 2.25 2.234C10.948 8.161 12 7.14 12 5.896c0-.919-.56-1.708-1.359-2.053l-.002.003z"/></svg>
```

partials/icons/social/pinboard.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.352 14.585l-4.509 4.614.72-4.062L3.428 7.57 0 7.753 7.58 0v2.953l7.214 6.646 4.513-1.105-4.689 4.982L24 24l-10.648-9.415z"/></svg>
```

partials/icons/social/pingdom.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.96 17.804l7.959-3.396-7.049 7.241c-.124-1.315-.432-2.61-.91-3.844v-.001zM24 11.118c-5.101-.236-10.208.414-15.087 1.92 1.024 1.073 1.881 2.292 2.535 3.621 4.042-2.25 9.646-5.123 12.552-5.531v-.015.005zm-12.574.275l.207-.06c1.538-.459 3.049-1.015 4.523-1.656 1.492-.585 2.896-1.38 4.159-2.367 1.345-1.069 2.355-2.499 2.915-4.122.12-.267.211-.549.267-.837-2.024 2.76-10.041 3.048-10.041 3.048l1.89-1.734C9.84 3.684 4.47 5.424 0 8.645c3.03.322 5.877 1.596 8.139 3.634 1.086-.336 2.196-.576 3.286-.879v-.006l.001-.001z"/></svg>
```

partials/icons/social/pinterest.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.162-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.741.099.12.112.225.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.401.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.354-.629-2.758-1.379l-.749 2.848c-.269 1.045-1.004 2.352-1.498 3.146 1.123.345 2.306.535 3.55.535 6.607 0 11.985-5.365 11.985-11.987C23.97 5.39 18.592.026 11.985.026L12.017 0z"/></svg>
```

partials/icons/social/playerme.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.981 0a8.957 8.957 0 0 0-8.956 8.957v.363C3.283 15.828 10.082 24 10.082 24V13.205c-1.638-.747-2.756-2.369-2.756-4.253a4.66 4.66 0 1 1 6.152 4.416l-.033.01v4.427c4.296-.713 7.531-4.401 7.531-8.845A8.959 8.959 0 0 0 12.017.001h-.038.002z"/></svg>
```

partials/icons/social/plex.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.643 0H4.68l7.679 12L4.68 24h6.963l7.677-12-7.677-12"/></svg>
```

partials/icons/social/pocket.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.813 10.259l-5.646 5.419c-.32.305-.73.458-1.141.458-.41 0-.821-.153-1.141-.458l-5.646-5.419c-.657-.628-.677-1.671-.049-2.326.63-.657 1.671-.679 2.325-.05l4.511 4.322 4.517-4.322c.66-.631 1.697-.607 2.326.049.631.645.615 1.695-.045 2.326l-.011.001zm5.083-7.546c-.299-.858-1.125-1.436-2.041-1.436H2.179c-.9 0-1.717.564-2.037 1.405-.094.25-.142.511-.142.774v7.245l.084 1.441c.348 3.277 2.047 6.142 4.682 8.139.045.036.094.07.143.105l.03.023c1.411 1.03 2.989 1.728 4.694 2.072.786.158 1.591.24 2.389.24.739 0 1.481-.067 2.209-.204.088-.029.176-.045.264-.06.023 0 .049-.015.074-.029 1.633-.36 3.148-1.036 4.508-2.025l.029-.031.135-.105c2.627-1.995 4.324-4.862 4.686-8.148L24 10.678V3.445c0-.251-.031-.5-.121-.742l.017.01z"/></svg>
```

partials/icons/social/podcasts.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.93 24s2.633 0 2.633-7.794c0-1.451-1.18-2.633-2.633-2.633s-2.634 1.182-2.634 2.633C9.296 24 11.93 24 11.93 24zm3.23-2.656c.115-.447.205-.896.275-1.351l.053-.36c.115-.05.23-.098.346-.15 1.828-.828 3.367-2.243 4.348-3.993.447-.803.777-1.67.973-2.572.227-1.008.285-2.059.166-3.088-.105-.963-.361-1.904-.77-2.787-.465-1.039-1.111-1.986-1.924-2.784-.828-.827-1.807-1.505-2.875-1.972-1.098-.496-2.303-.752-3.52-.782-1.22-.03-2.438.166-3.582.603-1.098.419-2.106 1.037-2.979 1.834-.827.752-1.534 1.67-2.046 2.678-.437.858-.736 1.776-.902 2.723-.166.979-.166 1.986-.016 2.98.135.872.391 1.73.768 2.543.888 1.881 2.393 3.444 4.258 4.394.226.104.451.21.692.314.015.121.046.256.06.392.075.438.166.889.271 1.325-.406-.136-.813-.287-1.204-.468-2.152-.976-3.972-2.662-5.101-4.754-.512-.947-.873-1.955-1.098-3.01-.257-1.158-.302-2.377-.15-3.566.15-1.112.466-2.211.933-3.22.556-1.188 1.339-2.286 2.271-3.204.916-.916 2.06-1.684 3.31-2.211C9.02.311 10.42.018 11.828.001c1.412-.015 2.824.24 4.139.758 1.266.498 2.434 1.238 3.43 2.166.965.895 1.76 1.962 2.346 3.139.496.993.842 2.076 1.008 3.175.18 1.144.18 2.317-.016 3.446-.166 1.053-.512 2.091-.979 3.053-1.053 2.122-2.799 3.868-4.92 4.922-.527.256-1.084.481-1.655.661l-.021.023zm.52-4.295l.01-.47c0-.316 0-.632-.046-.943-.015-.121-.045-.226-.075-.346.557-.451 1.023-1.023 1.369-1.67.256-.481.451-1.008.557-1.551.121-.602.15-1.233.061-1.865-.074-.557-.227-1.098-.451-1.61-.285-.616-.677-1.188-1.158-1.67-.497-.481-1.054-.872-1.686-1.159-.692-.3-1.445-.48-2.197-.496-.752-.015-1.52.121-2.227.392-.632.256-1.219.617-1.73 1.083-.513.466-.934 1.008-1.235 1.624-.257.496-.436 1.024-.542 1.58-.105.572-.119 1.159-.045 1.73.075.557.226 1.099.451 1.609.346.768.857 1.445 1.49 2.002l-.091.406c-.06.316-.045.617-.045.947v.422c-1.054-.646-1.927-1.58-2.513-2.663-.347-.617-.587-1.279-.723-1.972-.166-.768-.195-1.564-.09-2.347.09-.707.286-1.399.572-2.032.346-.781.857-1.504 1.459-2.121.617-.617 1.339-1.113 2.121-1.459.873-.391 1.82-.602 2.769-.632.964-.016 1.927.15 2.813.497.813.315 1.551.781 2.197 1.368.631.587 1.174 1.278 1.564 2.047.316.632.557 1.309.678 2.001.121.723.15 1.459.045 2.182-.09.707-.285 1.399-.588 2.046-.586 1.31-1.594 2.438-2.828 3.176l.114-.106zm-3.75-9.575c1.465 0 2.654 1.188 2.654 2.656 0 1.473-1.189 2.662-2.654 2.662-1.467 0-2.655-1.189-2.655-2.648s1.188-2.649 2.655-2.649v-.021z"/></svg>
```

partials/icons/social/processwire.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.939 5.27C21.211 4.183 20 2.941 18.784 2.137 16.258.407 13.332-.207 10.744.061c-2.699.291-5.01 1.308-6.91 3.004C2.074 4.637.912 6.559.4 8.392c-.518 1.833-.449 3.53-.264 4.808.195 1.297.841 2.929.841 2.929.132.313.315.44.41.493.472.258 1.247.031 1.842-.637.03-.041.046-.098.03-.146-.166-.639-.226-1.12-.285-1.492-.135-.736-.195-1.969-.105-3.109.045-.617.165-1.277.375-1.969.406-1.367 1.262-2.794 2.6-3.98 1.441-1.277 3.289-2.066 5.046-2.27.616-.074 1.788-.145 3.199.203.301.075 1.593.412 2.975 1.348 1.006.684 1.816 1.528 2.374 2.363.568.797 1.185 2.141 1.366 3.125.256 1.12.256 2.307.074 3.463-.225 1.158-.631 2.284-1.262 3.275-.435.768-1.337 1.783-2.403 2.545-.961.676-2.058 1.164-3.184 1.434-.57.135-1.142.221-1.728.24-.521.016-1.212 0-1.697-.082-.721-.115-.871-.299-1.036-.549 0 0-.115-.18-.147-.662.011-4.405.009-3.229.009-5.516 0-.646-.021-1.232-.015-1.764.03-.873.104-1.473.728-2.123.451-.479 1.082-.768 1.777-.768.211 0 .938.01 1.577.541.685.572.8 1.354.827 1.563.156 1.223-.652 2.134-.962 2.365-.384.288-.729.428-.962.51-.496.166-1.041.214-1.531.182-.075-.005-.143.044-.158.119l-.165.856c-.161.65.2.888.41.972.671.207 1.266.293 1.971.24 1.081-.076 2.147-.502 3.052-1.346.77-.732 1.209-1.635 1.359-2.645.15-1.121-.045-2.328-.556-3.35-.562-1.127-1.532-2.068-2.81-2.583-1.291-.508-2.318-.526-3.642-.188l-.015.005c-.86.296-1.596.661-2.362 1.452-.525.546-.955 1.207-1.217 1.953-.26.752-.33 1.313-.342 2.185-.016.646.015 1.246.015 1.808v3.701c0 1.184-.04 1.389 0 1.998.022.404.078.861.255 1.352.182.541.564 1.096.826 1.352.367.391.834.705 1.293.9 1.051.467 2.478.541 3.635.496.766-.029 1.536-.135 2.291-.314 1.51-.359 2.96-1.012 4.235-1.918 1.367-.963 2.555-2.277 3.211-3.393.841-1.326 1.385-2.814 1.668-4.343.255-1.532.243-3.103-.099-4.612-.27-1.4-.991-2.936-1.823-4.176l.038.037z"/></svg>
```

partials/icons/social/producthunt.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.604 8.4h-3.405V12h3.405c.995 0 1.801-.806 1.801-1.801 0-.993-.805-1.799-1.801-1.799z"/><path d="M12 0C5.372 0 0 5.372 0 12s5.372 12 12 12 12-5.372 12-12S18.628 0 12 0zm1.604 14.4h-3.405V18H7.801V6h5.804c2.319 0 4.2 1.88 4.2 4.199 0 2.321-1.881 4.201-4.201 4.201z"/></svg>
```

partials/icons/social/protoio.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 11.997c-.728 0-1.316-.59-1.316-1.317S11.272 9.363 12 9.363s1.316.589 1.316 1.316-.588 1.318-1.316 1.318zm2.916-.021c0-2.828-1.109-5.397-2.916-7.298-1.807 1.9-2.916 4.47-2.916 7.298 0 1.297.234 2.535.66 3.683-.618.9-1.074 2.16-1.275 3.616.639-.767 1.422-1.306 2.292-1.591.363.555.78 1.096 1.239 1.574.461-.494.876-1.02 1.239-1.59.87.271 1.653.826 2.29 1.576-.199-1.456-.655-2.716-1.275-3.615.427-1.155.66-2.385.66-3.69l.002.037z"/><path d="M12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10-4.477 10-10 10zm0-22C5.373 0 0 5.373 0 12s5.373 12 12 12 12-5.373 12-12S18.627 0 12 0z"/></svg>
```

partials/icons/social/python.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.31.18l.9.2.73.26.59.3.45.32.34.34.25.34.16.33.1.3.04.26.02.2-.01.13V8.5l-.05.63-.13.55-.21.46-.26.38-.3.31-.33.25-.35.19-.35.14-.33.1-.3.07-.26.04-.21.02H8.83l-.69.05-.59.14-.5.22-.41.27-.33.32-.27.35-.2.36-.15.37-.1.35-.07.32-.04.27-.02.21v3.06H3.23l-.21-.03-.28-.07-.32-.12-.35-.18-.36-.26-.36-.36-.35-.46-.32-.59-.28-.73-.21-.88-.14-1.05L0 11.97l.06-1.22.16-1.04.24-.87.32-.71.36-.57.4-.44.42-.33.42-.24.4-.16.36-.1.32-.05.24-.01h.16l.06.01h8.16v-.83H6.24l-.01-2.75-.02-.37.05-.34.11-.31.17-.28.25-.26.31-.23.38-.2.44-.18.51-.15.58-.12.64-.1.71-.06.77-.04.84-.02 1.27.05 1.07.13zm-6.3 1.98l-.23.33-.08.41.08.41.23.34.33.22.41.09.41-.09.33-.22.23-.34.08-.41-.08-.41-.23-.33-.33-.22-.41-.09-.41.09-.33.22z"/><path d="M21.1 6.11l.28.06.32.12.35.18.36.27.36.35.35.47.32.59.28.73.21.88.14 1.04.05 1.23-.06 1.23-.16 1.04-.24.86-.32.71-.36.57-.4.45-.42.33-.42.24-.4.16-.36.09-.32.05-.24.02-.16-.01h-8.22v.82h5.84l.01 2.76.02.36-.05.34-.11.31-.17.29-.25.25-.31.24-.38.2-.44.17-.51.15-.58.13-.64.09-.71.07-.77.04-.84.01-1.27-.04-1.07-.14-.9-.2-.73-.25-.59-.3-.45-.33-.34-.34-.25-.34-.16-.33-.1-.3-.04-.25-.02-.2.01-.13v-5.34l.05-.64.13-.54.21-.46.26-.38.3-.32.33-.24.35-.2.35-.14.33-.1.3-.06.26-.04.21-.02.13-.01h5.84l.69-.05.59-.14.5-.21.41-.28.33-.32.27-.35.2-.36.15-.36.1-.35.07-.32.04-.28.02-.21V6.07h2.09l.14.01.21.03zm-6.47 14.25l-.23.33-.08.41.08.41.23.33.33.23.41.08.41-.08.33-.23.23-.33.08-.41-.08-.41-.23-.33-.33-.23-.41-.08-.41.08-.33.23z"/></svg>
```

partials/icons/social/quantopian.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M1.5 0h21c.828 0 1.5.672 1.5 1.5v21c0 .828-.672 1.5-1.5 1.5h-21C.672 24 0 23.328 0 22.5v-21C0 .672.672 0 1.5 0zM3 3v18h18V3H3zm2.4 10.8h2.4v4.8H5.4v-4.8zM9 9h2.4v9.6H9V9zm3.6 2.4H15v7.2h-2.4v-7.2zm3.599-6h2.4v13.2h-2.4V5.4z"/></svg>
```

partials/icons/social/quip.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.154 22.154H12a10.06 10.06 0 01-7.4-3.201C2.66 16.89 1.69 14.19 1.868 11.35c.315-5.091 4.39-9.168 9.482-9.484.22-.014.44-.02.657-.02A10.058 10.059 0 0118.952 4.6a10.058 10.059 0 013.202 7.4zm-1.938-18.9C17.778.963 14.59-.186 11.236.024 5.218.399.398 5.219.024 11.237c-.207 3.353.94 6.543 3.231 8.98A12.047 12.048 0 0012 24h11.077c.51 0 .923-.413.923-.922V12a12.047 12.048 0 00-3.784-8.745m-4.062 11.976H7.846a.923.923 0 000 1.846h8.308a.923.923 0 000-1.846M7.846 8.77h8.308a.923.923 0 000-1.847H7.846a.923.923 0 000 1.847m-2.769 2.308a.923.923 0 000 1.845h13.846a.923.923 0 000-1.846H5.077Z"/></svg>
```

partials/icons/social/quora.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.738 18.701c-.831-1.635-1.805-3.287-3.708-3.287-.362 0-.727.061-1.059.209l-.646-1.289c.786-.678 2.058-1.214 3.693-1.214 2.544 0 3.851 1.229 4.888 2.792.613-1.335.904-3.14.904-5.375 0-5.582-1.744-8.447-5.822-8.447-4.018 0-5.757 2.865-5.757 8.447 0 5.553 1.739 8.389 5.757 8.389.64 0 1.22-.069 1.75-.225zm.996 1.947c-.881.237-1.817.366-2.743.366-5.352 0-10.59-4.269-10.59-10.478C.402 4.271 5.639 0 10.991 0c5.441 0 10.628 4.238 10.628 10.537 0 3.504-1.635 6.351-4.01 8.191.764 1.148 1.543 1.914 2.652 1.914 1.199 0 1.68-.915 1.77-1.649h1.557c.092.974-.402 5.007-4.766 5.007-2.652 0-4.047-1.528-5.096-3.328l.008-.024z"/></svg>
```

partials/icons/social/raspberrypi.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.111 17.338c-.857.989-1.334 2.79-.709 3.371.596.449 2.201.391 3.385-1.23.86-1.08.569-2.893.081-3.372-.73-.555-1.778.164-2.757 1.243v-.012zm-8.057.3c-.908-1.04-2.088-1.658-2.851-1.199-.51.382-.605 1.685.123 2.967 1.078 1.524 2.596 1.679 3.221 1.307.659-.488.3-2.137-.493-3.075zm4.105 3.145c-1.103-.026-2.798.439-2.776 1.032-.018.403 1.331 1.572 2.705 1.513 1.326.03 2.699-1.139 2.682-1.649-.004-.523-1.498-.927-2.607-.884l-.004-.012zm-.075-13.944c-1.275-.032-2.502.933-2.502 1.493-.004.68 1.008 1.376 2.51 1.394 1.543.01 2.518-.559 2.532-1.26.016-.794-1.394-1.639-2.518-1.627h-.022zm-3.071.532c-2.135-.345-3.913.9-3.842 3.192.07.884 4.63-3.041 3.843-3.177l-.001-.015zm9.749 3.251c.071-2.277-1.709-3.521-3.844-3.176-.787.135 3.772 4.061 3.844 3.176zm.364.824c-1.239-.329-.42 5.049.588 4.615 1.109-.869 1.466-3.446-.588-4.6v-.015zM4.228 16.121c1.007.45 1.827-4.929.589-4.6-2.053 1.153-1.698 3.73-.589 4.615v-.015zm9.415-5.948c-1.146.75-1.354 2.428-.461 3.746.891 1.318 2.543 1.813 3.691 1.078 1.146-.733 1.353-2.412.462-3.746-.892-1.333-2.545-1.813-3.692-1.063v-.015zm-3.096.135c-1.146-.734-2.799-.254-3.689 1.064-.892 1.334-.686 3.012.461 3.761s2.799.269 3.691-1.064c.885-1.318.675-2.997-.465-3.745l.002-.016zm4.369 7.162c-.009-1.393-1.252-2.518-2.781-2.502-1.527.016-2.761 1.139-2.754 2.532v.029c.01 1.394 1.254 2.517 2.783 2.502 1.527 0 2.756-1.138 2.742-2.517v-.029l.01-.015zm3.209-15.133c-2.307 1.184-3.652 2.128-4.389 2.938.377 1.498 2.344 1.558 3.063 1.512-.147-.06-.271-.149-.315-.269.18-.12.821-.016 1.268-.255-.171-.03-.252-.061-.329-.195.419-.135.875-.24 1.141-.465-.143 0-.278.03-.467-.09.377-.194.778-.359 1.095-.658-.196 0-.406 0-.466-.075.346-.21.635-.435.877-.704-.272.045-.39.016-.454-.03.261-.255.593-.479.749-.81-.203.076-.391.09-.522 0 .091-.194.47-.314.69-.779-.215.03-.441.046-.486 0 .098-.389.269-.613.435-.854-.457 0-1.15 0-1.117-.029l.283-.285c-.448-.12-.904.015-1.236.12-.149-.105 0-.255.185-.405-.39.061-.733.135-1.034.256-.164-.15.105-.285.24-.436-.599.12-.839.27-1.094.42-.18-.165-.015-.314.104-.449-.449.164-.674.374-.914.568-.09-.104-.209-.179-.06-.449-.314.18-.554.39-.734.629-.194-.134-.119-.299-.119-.449-.33.27-.54.54-.794.811-.061-.031-.105-.15-.135-.346-.779.75-1.889 2.623-.285 3.356 1.349-1.094 2.981-1.903 4.779-2.503l.041-.075zm-12.259 0c1.798.6 3.419 1.408 4.777 2.518 1.596-.75.493-2.623-.282-3.356-.041.194-.085.329-.135.359-.255-.27-.462-.54-.788-.81 0 .15.077.33-.117.45-.175-.239-.41-.45-.725-.63.149.256.025.33-.056.449-.24-.225-.465-.434-.899-.599.12.149.3.3.12.465-.239-.149-.494-.3-1.078-.42.135.149.404.3.238.45-.315-.122-.66-.212-1.035-.258.181.15.342.289.192.405-.345-.12-.806-.255-1.255-.135l.284.284c.03.037-.659.03-1.121.035.165.225.337.449.435.854-.045.045-.27.016-.483 0 .225.449.599.57.688.765-.135.096-.314.075-.523 0 .164.314.494.539.748.81-.074.044-.18.074-.464.037.239.26.524.494.869.704-.06.07-.271.069-.479.075.314.304.719.464 1.094.663-.195.136-.33.105-.465.105.255.225.72.329 1.139.464-.09.135-.164.165-.344.195.449.254 1.078.135 1.258.27-.045.119-.164.209-.314.27.719.045 2.697-.015 3.072-1.514-.736-.807-2.084-1.752-4.391-2.921l.04.016zM7.6.103c.236-.007.436.135.652.201.529-.17.65.063.91.159.577-.12.752.141 1.029.419l.322-.009c.869.507 1.305 1.536 1.457 2.065.152-.529.584-1.559 1.457-2.065l.321.007c.277-.283.453-.539 1.029-.418.261-.105.38-.33.911-.166.33-.104.62-.375 1.057-.045.368-.149.726-.195 1.045.09.495-.06.653.061.774.21.108 0 .809-.104 1.132.36.81-.09 1.064.464.774.988.165.255.337.494-.05.975.15.269.062.553-.27.913.091.374-.074.63-.374.839.06.51-.48.81-.629.914-.061.3-.181.584-.795.734-.089.449-.464.523-.824.614 1.185.675 2.188 1.558 2.188 3.731l.181.299c1.349.809 2.562 3.402.674 5.514-.119.659-.329 1.124-.511 1.648-.269 2.113-2.082 3.101-2.561 3.221-.689.525-1.438 1.02-2.442 1.363-.942.961-1.976 1.336-2.994 1.336h-.092c-1.033 0-2.063-.375-3.012-1.335-1.007-.344-1.754-.838-2.447-1.363-.479-.12-2.283-1.107-2.562-3.221-.187-.524-.394-1.004-.518-1.662-1.894-2.113-.681-4.705.666-5.515l.172-.3c0-2.172 1.005-3.057 2.188-3.73-.359-.09-.72-.165-.823-.615-.615-.15-.735-.434-.795-.734-.15-.105-.689-.404-.629-.928-.3-.211-.465-.465-.375-.854-.314-.346-.404-.645-.27-.915-.39-.479-.209-.733-.045-.974C3.236 1.329 3.491.76 4.3.85 4.614.385 5.32.491 5.423.491c.121-.15.285-.285.779-.225.314-.285.675-.24 1.049-.102.151-.12.286-.164.406-.164L7.6.103z"/></svg>
```

partials/icons/social/redbubble.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.633 16.324h-3.199a.321.321 0 0 1-.32-.322V7.974a.32.32 0 0 1 .32-.32H16.4c2.226 0 2.693 1.31 2.693 2.408 0 .636-.169 1.14-.504 1.511.816.337 1.256 1.096 1.256 2.194 0 1.601-1.201 2.557-3.212 2.557m-4.644 0H5.345a.32.32 0 0 1-.32-.322V7.974a.32.32 0 0 1 .32-.32h3.103c1.939 0 3.096 1.043 3.096 2.791 0 1.163-.585 2.077-1.527 2.448l2.21 2.897a.322.322 0 0 1-.24.533M12 0C5.373 0 0 5.373 0 12s5.373 12 12 12c6.628 0 12-5.373 12-12S18.63 0 12.001 0"/></svg>
```

partials/icons/social/reddit.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0zm5.01 4.744c.688 0 1.25.561 1.25 1.249a1.25 1.25 0 0 1-2.498.056l-2.597-.547-.8 3.747c1.824.07 3.48.632 4.674 1.488.308-.309.73-.491 1.207-.491.968 0 1.754.786 1.754 1.754 0 .716-.435 1.333-1.01 1.614a3.111 3.111 0 0 1 .042.52c0 2.694-3.13 4.87-7.004 4.87-3.874 0-7.004-2.176-7.004-4.87 0-.183.015-.366.043-.534A1.748 1.748 0 0 1 4.028 12c0-.968.786-1.754 1.754-1.754.463 0 .898.196 1.207.49 1.207-.883 2.878-1.43 4.744-1.487l.885-4.182a.342.342 0 0 1 .14-.197.35.35 0 0 1 .238-.042l2.906.617a1.214 1.214 0 0 1 1.108-.701zM9.25 12C8.561 12 8 12.562 8 13.25c0 .687.561 1.248 1.25 1.248.687 0 1.248-.561 1.248-1.249 0-.688-.561-1.249-1.249-1.249zm5.5 0c-.687 0-1.248.561-1.248 1.25 0 .687.561 1.248 1.249 1.248.688 0 1.249-.561 1.249-1.249 0-.687-.562-1.249-1.25-1.249zm-5.466 3.99a.327.327 0 0 0-.231.094.33.33 0 0 0 0 .463c.842.842 2.484.913 2.961.913.477 0 2.105-.056 2.961-.913a.361.361 0 0 0 .029-.463.33.33 0 0 0-.464 0c-.547.533-1.684.73-2.512.73-.828 0-1.979-.196-2.512-.73a.326.326 0 0 0-.232-.095z"/></svg>
```

partials/icons/social/riot.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M5.918 0c-2.067 0-3.76 1.623-3.76 3.63-.003 5.526.001 11.483 0 16.743 0 2.006 1.693 3.627 3.76 3.627 2.067 0 3.762-1.62 3.762-3.627v-3.071l1.984-.002 3.63 4.98c.673.924 1.746 1.419 2.836 1.419.686 0 1.378-.196 1.983-.603 1.564-1.054 1.943-3.13.846-4.635l-2.322-3.19c1.97-1.593 3.224-3.977 3.224-6.621 0-4.773-4.037-8.65-8.98-8.65zm1.42.603h5.543c4.63 0 8.38 3.613 8.38 8.047 0 2.444-1.156 4.652-2.98 6.136l-1.648-2.263c1.078-.97 1.768-2.338 1.768-3.873 0-2.942-2.48-5.322-5.52-5.322H9.367a3.215 3.215 0 0 0-.597-1.606A3.405 3.405 0 0 0 7.338.602zM9.365 3.93h3.516c2.727 0 4.919 2.115 4.919 4.719 0 1.335-.588 2.53-1.518 3.39l-.211-.29a3.463 3.463 0 0 0-2.2-1.36c.636-.34 1.071-.992 1.071-1.74 0-1.103-.933-1.994-2.061-1.994H9.079v3.992l2.706-.002a3.28 3.28 0 0 0-1.979 2.727l-3.587.004V6.93a3.515 3.515 0 0 0 1.7-.575 3.296 3.296 0 0 0 1.425-2.148c.017-.092.012-.184.02-.276zM2.759 4.959c.092.201.204.394.338.578.606.833 1.543 1.303 2.522 1.39v13.446c-.02.42.62.42.6 0v-6.395l3.59-.004c.054.555.238 1.106.594 1.595l.824 1.13-2.148.002v3.672c0 1.669-1.406 3.026-3.161 3.026-1.754 0-3.16-1.357-3.16-3.026-.002-5.124 0-10.7 0-15.414zm6.92 2.298h3.202c.814 0 1.459.629 1.459 1.393 0 .725-.588 1.34-1.357 1.39a1.595 1.595 0 0 1-.106.003l-3.197.002Z"/></svg>
```

partials/icons/social/runkeeper.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.475 16.634c1.887-.257 3.258-1.114 4.537-2.57 1.5-1.757 1.93-4.112 1.327-6.34-.6-2.143-2.31-3.814-4.54-4.116-2.757-.426-5.618.9-7.638 2.704-.045.04-.165.126-.21.21-.21-.384-.482-.77-.77-1.07-.385-.557-1.24-1.458-1.285-1.5-.17-.214-.47-.257-.64-.342-.527-.113-.888-.29-1.114-.42-.012-.018-.027-.034-.045-.054L.914.824C.7.65.44.61.227.824c-.17.214-.214.472 0 .686L2.37 3.824l.02.02.03-.002c.077.136.348.362.453.83.045.21.166.466.377.767 0 0 1.506 1.625 2.108 2.725.558 1.114.693 1.46.768 1.67 0 .03-.557-.646-1.204-1.113-2.485 2.83-4.293 6.22-4.82 9.894-.557 3.765 1.506 4.76 3.043 4.714 1.234 0 3.81-1.325 5.18-4.623C9.65 15.5 9.44 11.81 8.1 8.6c1.28-1.294 3.644-2.83 5.948-2.785 1.716 0 2.575 1.49 2.696 1.627 1.324 2.394-.227 4.548-.227 4.548-.858 1.295-2.35 1.898-3.133 2.107-.587.166-1.702.12-1.973 0-.164-.045-.21-.136-.21-.256 0-.18.136-.255.256-.255.166 0 .256.12.256.256v.138c.437.12 1.28.03 1.627 0-.272-.644-.86-.987-1.643-.987h-.036c-1.01.008-1.823.833-1.815 1.844 0 .77.437 1.415 1.07 1.67.332.13 1.326.258 2.56.13zm-6.82-.427c-.86 3.772-3.256 5.1-3.9 4.884-.642-.213-.856-2.1.428-5.27.216-.47 1.5-3.427 3.172-5.27-.045.086.943 2.872.3 5.657z"/><path d="M23.186 16.938L24 13.85c.03-.256-.09-.557-.348-.6-.256-.043-.557.088-.586.344l-.81 2.977h-.095c-.017.022-.03.044-.044.066-.12.214-.346.558-.678.814-.256.214-.377.47-.377.47-.12.128-.978 2.83-3.673 2.957-3.18.128-3.81-3.427-3.855-3.727-.678.127-2.048-.174-2.606-.43.166 1.97 1.115 4.327 2.786 5.442 1.928 1.328 4.926 1.328 6.988 0 1.19-.815 1.973-1.843 2.484-3.172l.045-.11.015-.033c.016-.037.016-.074.046-.113v-.045c-.03 0 0-.257-.075-.513-.164-.683-.03-1.113-.03-1.24z"/></svg>
```

partials/icons/social/saucelabs.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.93 15.475l6.396.004-3.582 6.758C2.178 20.057.002 16.18 0 12 0 5.383 5.383 0 12 0c1.761 0 3.436.381 4.94 1.064L5.428 12.58h10.25l-7.539 7.614 3.115-5.876H3.795C3.455 13.164 3.477 12 3.477 12c.006-4.713 3.831-8.529 8.544-8.523.093 0 .187.002.28.005l1.094-1.099c-.455-.065-.915-.098-1.375-.098-5.356 0-9.73 4.357-9.73 9.715-.001 0-.061 1.719.64 3.475zM18.255 1.764C21.82 3.943 23.997 7.82 24 12c0 6.616-5.384 12-12 12-1.704.003-3.389-.36-4.941-1.065l11.426-11.513H8.205l7.656-7.616-3.115 5.876h7.46c.319 1.079.319 2.318.319 2.318-.008 4.714-3.834 8.529-8.547 8.522-.105 0-.21-.002-.314-.006l-1.084 1.096c5.314.777 10.256-2.901 11.032-8.218.067-.461.103-.928.103-1.395 0-1.189-.22-2.369-.647-3.479h-6.394l3.581-6.756z"/></svg>
```

partials/icons/social/sellfy.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.179.818C15.533-.273 8.406-.273.8.818-.266 8.377-.266 15.424.8 22.946 4.511 23.491 8.22 24 12.005 24c3.748 0 7.459-.51 11.17-1.017 1.1-7.56 1.1-14.607 0-22.165h.004zm-11.54 18.314c-2.055 0-4.226-.689-5.179-1.199l.807-3.126c1.064.705 2.682 1.395 4.446 1.395 1.395 0 2.24-.436 2.24-1.305 0-.615-.435-.975-1.575-1.26l-2.279-.631c-2.416-.66-3.557-1.891-3.557-3.855 0-2.365 1.83-4.256 5.619-4.256 1.99 0 3.973.545 5.07 1.092l-.951 2.976c-1.104-.615-2.79-1.125-4.226-1.125-1.365 0-1.95.436-1.95 1.092 0 .619.404.87 1.291 1.092l2.488.734c2.566.736 3.707 1.966 3.707 3.885-.076 2.701-2.461 4.517-5.957 4.517l.006-.026z"/></svg>
```

partials/icons/social/shopify.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.337 23.979l7.216-1.561s-2.604-17.613-2.625-17.73c-.018-.116-.114-.192-.211-.192s-1.929-.136-1.929-.136-1.275-1.274-1.439-1.411c-.045-.037-.075-.057-.121-.074l-.914 21.104h.023zM11.71 11.305s-.81-.424-1.774-.424c-1.447 0-1.504.906-1.504 1.141 0 1.232 3.24 1.715 3.24 4.629 0 2.295-1.44 3.76-3.406 3.76-2.354 0-3.54-1.465-3.54-1.465l.646-2.086s1.245 1.066 2.28 1.066c.675 0 .975-.545.975-.932 0-1.619-2.654-1.694-2.654-4.359-.034-2.237 1.571-4.416 4.827-4.416 1.257 0 1.875.361 1.875.361l-.945 2.715-.02.01zM11.17.83c.136 0 .271.038.405.135-.984.465-2.064 1.639-2.508 3.992-.656.213-1.293.405-1.889.578C7.697 3.75 8.951.84 11.17.84V.83zm1.235 2.949v.135c-.754.232-1.583.484-2.394.736.466-1.777 1.333-2.645 2.085-2.971.193.501.309 1.176.309 2.1zm.539-2.234c.694.074 1.141.867 1.429 1.755-.349.114-.735.231-1.158.366v-.252c0-.752-.096-1.371-.271-1.871v.002zm2.992 1.289c-.02 0-.06.021-.078.021s-.289.075-.714.21c-.423-1.233-1.176-2.37-2.508-2.37h-.115C12.135.209 11.669 0 11.265 0 8.159 0 6.675 3.877 6.21 5.846c-1.194.365-2.063.636-2.16.674-.675.213-.694.232-.772.87-.075.462-1.83 14.063-1.83 14.063L15.009 24l.927-21.166z"/></svg>
```

partials/icons/social/skype.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.069 18.874c-4.023 0-5.82-1.979-5.82-3.464 0-.765.561-1.296 1.333-1.296 1.723 0 1.273 2.477 4.487 2.477 1.641 0 2.55-.895 2.55-1.811 0-.551-.269-1.16-1.354-1.429l-3.576-.895c-2.88-.724-3.403-2.286-3.403-3.751 0-3.047 2.861-4.191 5.549-4.191 2.471 0 5.393 1.373 5.393 3.199 0 .784-.688 1.24-1.453 1.24-1.469 0-1.198-2.037-4.164-2.037-1.469 0-2.292.664-2.292 1.617s1.153 1.258 2.157 1.487l2.637.587c2.891.649 3.624 2.346 3.624 3.944 0 2.476-1.902 4.324-5.722 4.324m11.084-4.882l-.029.135-.044-.24c.015.045.044.074.059.12.12-.675.181-1.363.181-2.052 0-1.529-.301-3.012-.898-4.42-.569-1.348-1.395-2.562-2.427-3.596-1.049-1.033-2.247-1.856-3.595-2.426-1.318-.631-2.801-.93-4.328-.93-.72 0-1.444.07-2.143.204l.119.06-.239-.033.119-.025C8.91.274 7.829 0 6.731 0c-1.789 0-3.47.698-4.736 1.967C.729 3.235.032 4.923.032 6.716c0 1.143.292 2.265.844 3.258l.02-.124.041.239-.06-.115c-.114.645-.172 1.299-.172 1.955 0 1.53.3 3.017.884 4.416.568 1.362 1.378 2.576 2.427 3.609 1.034 1.05 2.247 1.857 3.595 2.442 1.394.6 2.877.898 4.404.898.659 0 1.334-.06 1.977-.179l-.119-.062.24.046-.135.03c1.002.569 2.126.871 3.294.871 1.783 0 3.459-.69 4.733-1.963 1.259-1.259 1.962-2.951 1.962-4.749 0-1.138-.299-2.262-.853-3.266"/></svg>
```

partials/icons/social/slack.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M5.042 15.165a2.528 2.528 0 0 1-2.52 2.523A2.528 2.528 0 0 1 0 15.165a2.527 2.527 0 0 1 2.522-2.52h2.52v2.52zM6.313 15.165a2.527 2.527 0 0 1 2.521-2.52 2.527 2.527 0 0 1 2.521 2.52v6.313A2.528 2.528 0 0 1 8.834 24a2.528 2.528 0 0 1-2.521-2.522v-6.313zM8.834 5.042a2.528 2.528 0 0 1-2.521-2.52A2.528 2.528 0 0 1 8.834 0a2.528 2.528 0 0 1 2.521 2.522v2.52H8.834zM8.834 6.313a2.528 2.528 0 0 1 2.521 2.521 2.528 2.528 0 0 1-2.521 2.521H2.522A2.528 2.528 0 0 1 0 8.834a2.528 2.528 0 0 1 2.522-2.521h6.312zM18.956 8.834a2.528 2.528 0 0 1 2.522-2.521A2.528 2.528 0 0 1 24 8.834a2.528 2.528 0 0 1-2.522 2.521h-2.522V8.834zM17.688 8.834a2.528 2.528 0 0 1-2.523 2.521 2.527 2.527 0 0 1-2.52-2.521V2.522A2.527 2.527 0 0 1 15.165 0a2.528 2.528 0 0 1 2.523 2.522v6.312zM15.165 18.956a2.528 2.528 0 0 1 2.523 2.522A2.528 2.528 0 0 1 15.165 24a2.527 2.527 0 0 1-2.52-2.522v-2.522h2.52zM15.165 17.688a2.527 2.527 0 0 1-2.52-2.523 2.526 2.526 0 0 1 2.52-2.52h6.313A2.527 2.527 0 0 1 24 15.165a2.528 2.528 0 0 1-2.522 2.523h-6.313z"/></svg>
```

partials/icons/social/slickpic.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.483 18.308L6.056 14.085l2.52-9.201L24 9.104l-2.517 9.204zm-13.414-5.37l12.263 3.354 1.654-6.033L9.72 6.9l-1.65 6.034v.004zM8.526 15.795l-4.891 1.311-1.625-6.045 4.146-1.11.501-1.835L0 9.902l2.478 9.215 9.178-2.467"/></svg>
```

partials/icons/social/smashingmagazine.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.734 12.002c.766.524 1.662 1.01 2.708 1.443 1.785.742 2.985 1.387 3.601 1.936.615.547.928 1.248.928 2.104-.005 1.457-1.023 2.189-3.076 2.189-1.977 0-3.75-.627-5.326-1.875l-1.871 4.186c1.422.761 2.58 1.257 3.475 1.496l.141.033-1.798.416c-1.271.292-2.539-.503-2.832-1.771L.061 6.5c-.291-1.271.5-2.539 1.773-2.835l4.375-1.009c-.158.155-.307.316-.441.485l-.018.021c-.753.949-1.131 2.115-1.131 3.505 0 2.101 1.03 3.87 3.079 5.296l.046.029-.01.01zm10.358.072c-.84-.672-1.904-1.268-3.24-1.786-1.98-.784-3.271-1.41-3.871-1.872-.6-.465-.914-.981-.914-1.557 0-1.459.914-2.19 2.76-2.19 2.041 0 3.646.494 4.786 1.476l1.515-4.08c-1.095-.556-2.235-.96-3.405-1.216l-.06-.015c-.256-.061-.525-.12-.811-.164l2.625-.602c1.275-.285 2.535.511 2.836 1.771l3.63 15.647c.284 1.274-.51 2.551-1.784 2.835l-2.985.69c.824-1.051 1.245-2.34 1.245-3.87 0-1.575-.437-2.911-1.306-4.021-.285-.346-.615-.676-1.006-1.006l-.044-.029.029-.011z"/></svg>
```

partials/icons/social/snapchat.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.206.793c.99 0 4.347.276 5.93 3.821.529 1.193.403 3.219.299 4.847l-.003.06c-.012.18-.022.345-.03.51.075.045.203.09.401.09.3-.016.659-.12 1.033-.301.165-.088.344-.104.464-.104.182 0 .359.029.509.09.45.149.734.479.734.838.015.449-.39.839-1.213 1.168-.089.029-.209.075-.344.119-.45.135-1.139.36-1.333.81-.09.224-.061.524.12.868l.015.015c.06.136 1.526 3.475 4.791 4.014.255.044.435.27.42.509 0 .075-.015.149-.045.225-.24.569-1.273.988-3.146 1.271-.059.091-.12.375-.164.57-.029.179-.074.36-.134.553-.076.271-.27.405-.555.405h-.03c-.135 0-.313-.031-.538-.074-.36-.075-.765-.135-1.273-.135-.3 0-.599.015-.913.074-.6.104-1.123.464-1.723.884-.853.599-1.826 1.288-3.294 1.288-.06 0-.119-.015-.18-.015h-.149c-1.468 0-2.427-.675-3.279-1.288-.599-.42-1.107-.779-1.707-.884-.314-.045-.629-.074-.928-.074-.54 0-.958.089-1.272.149-.211.043-.391.074-.54.074-.374 0-.523-.224-.583-.42-.061-.192-.09-.389-.135-.567-.046-.181-.105-.494-.166-.57-1.918-.222-2.95-.642-3.189-1.226-.031-.063-.052-.15-.055-.225-.015-.243.165-.465.42-.509 3.264-.54 4.73-3.879 4.791-4.02l.016-.029c.18-.345.224-.645.119-.869-.195-.434-.884-.658-1.332-.809-.121-.029-.24-.074-.346-.119-1.107-.435-1.257-.93-1.197-1.273.09-.479.674-.793 1.168-.793.146 0 .27.029.383.074.42.194.789.3 1.104.3.234 0 .384-.06.465-.105l-.046-.569c-.098-1.626-.225-3.651.307-4.837C7.392 1.077 10.739.807 11.727.807l.419-.015h.06z"/></svg>
```

partials/icons/social/songkick.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M6.55 18.779c-1.855 0-3.372-.339-4.598-1.602l1.92-1.908c.63.631 1.74.853 2.715.853 1.186 0 1.739-.391 1.739-1.089 0-.291-.06-.529-.239-.717-.15-.154-.404-.273-.795-.324l-1.455-.205c-1.064-.152-1.891-.51-2.43-1.072-.555-.578-.84-1.395-.84-2.434C2.536 8.066 4.2 6.45 6.96 6.45c1.74 0 3.048.407 4.086 1.448L9.171 9.77c-.765-.766-1.77-.715-2.295-.715-1.039 0-1.465.597-1.465 1.125 0 .152.051.375.24.561.15.153.404.307.832.359l1.467.203c1.09.153 1.875.495 2.385 1.005.645.63.9 1.53.9 2.655 0 2.47-2.127 3.819-4.68 3.819l-.005-.003zM20.813 2.651C19.178 1.432 17.37.612 15.089.237v10.875l3.261-4.539h3.565l-4.095 5.72s.944 1.51 1.515 2.405c.586.899 1.139 1.14 1.965 1.14h.57v2.806h-.872c-1.812 0-2.9-.33-3.72-1.575-.504-.811-2.175-3.436-2.175-3.436v4.995H12.12V-.001H12c-3.852 0-6.509.931-8.811 2.652C-.132 5.137.001 8.451.001 11.997c0 3.547-.133 6.867 3.188 9.352C5.491 23.074 8.148 24 12 24s6.51-.927 8.812-2.651C24.131 18.865 24 15.544 24 11.997c0-3.546.132-6.859-3.188-9.346h.001z"/></svg>
```

partials/icons/social/soundcloud.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M1.175 12.225c-.051 0-.094.046-.101.1l-.233 2.154.233 2.105c.007.058.05.098.101.098.05 0 .09-.04.099-.098l.255-2.105-.27-2.154c0-.057-.045-.1-.09-.1m-.899.828c-.06 0-.091.037-.104.094L0 14.479l.165 1.308c0 .055.045.094.09.094s.089-.045.104-.104l.21-1.319-.21-1.334c0-.061-.044-.09-.09-.09m1.83-1.229c-.061 0-.12.045-.12.104l-.21 2.563.225 2.458c0 .06.045.12.119.12.061 0 .105-.061.121-.12l.254-2.474-.254-2.548c-.016-.06-.061-.12-.121-.12m.945-.089c-.075 0-.135.06-.15.135l-.193 2.64.21 2.544c.016.077.075.138.149.138.075 0 .135-.061.15-.15l.24-2.532-.24-2.623c0-.075-.06-.135-.135-.135l-.031-.017zm1.155.36c-.005-.09-.075-.149-.159-.149-.09 0-.158.06-.164.149l-.217 2.43.2 2.563c0 .09.075.157.159.157.074 0 .148-.068.148-.158l.227-2.563-.227-2.444.033.015zm.809-1.709c-.101 0-.18.09-.18.181l-.21 3.957.187 2.563c0 .09.08.164.18.164.094 0 .174-.09.18-.18l.209-2.563-.209-3.972c-.008-.104-.088-.18-.18-.18m.959-.914c-.105 0-.195.09-.203.194l-.18 4.872.165 2.548c0 .12.09.209.195.209.104 0 .194-.089.21-.209l.193-2.548-.192-4.856c-.016-.12-.105-.21-.21-.21m.989-.449c-.121 0-.211.089-.225.209l-.165 5.275.165 2.52c.014.119.104.225.225.225.119 0 .225-.105.225-.225l.195-2.52-.196-5.275c0-.12-.105-.225-.225-.225m1.245.045c0-.135-.105-.24-.24-.24-.119 0-.24.105-.24.24l-.149 5.441.149 2.503c.016.135.121.24.256.24s.24-.105.24-.24l.164-2.503-.164-5.456-.016.015zm.749-.134c-.135 0-.255.119-.255.254l-.15 5.322.15 2.473c0 .15.12.255.255.255s.255-.12.255-.27l.15-2.474-.165-5.307c0-.148-.12-.27-.271-.27m1.005.166c-.164 0-.284.135-.284.285l-.103 5.143.135 2.474c0 .149.119.277.284.277.149 0 .271-.12.284-.285l.121-2.443-.135-5.112c-.012-.164-.135-.285-.285-.285m1.184-.945c-.045-.029-.105-.044-.165-.044s-.119.015-.165.044c-.09.054-.149.15-.149.255v.061l-.104 6.048.115 2.449v.008c.008.06.03.135.074.18.058.061.142.104.234.104.08 0 .158-.044.209-.09.058-.06.091-.135.091-.225l.015-.24.117-2.203-.135-6.086c0-.104-.061-.193-.135-.239l-.002-.022zm1.006-.547c-.045-.045-.09-.061-.15-.061-.074 0-.149.016-.209.061-.075.061-.119.15-.119.24v.029l-.137 6.609.076 1.215.061 1.185c0 .164.148.314.328.314.181 0 .33-.15.33-.329l.15-2.414-.15-6.637c0-.12-.074-.221-.165-.277m8.934 3.777c-.405 0-.795.086-1.139.232-.24-2.654-2.46-4.736-5.188-4.736-.659 0-1.305.135-1.889.359-.225.09-.27.18-.285.359v9.368c.016.18.15.33.33.345h8.185C22.681 17.218 24 15.914 24 14.28s-1.319-2.952-2.938-2.952"/></svg>
```

partials/icons/social/sparkpost.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.2 9c-1.351.9-1.8 2.7-1.65 3.9-2.25-2.25 3.45-8.55-3-12.9C15.15 5.4 6 9.75 6 17.4c0 3 1.95 5.701 6 6.6 4.05-.898 6-3.6 6-6.6 0-4.5-2.7-6-1.8-8.4zM12 20.852c-1.8 0-3.45-1.5-3.45-3.451 0-1.801 1.5-3.45 3.45-3.45 1.8 0 3.45 1.5 3.45 3.45-.15 1.951-1.65 3.451-3.45 3.451z"/></svg>
```

partials/icons/social/spotify.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.4 0 0 5.4 0 12s5.4 12 12 12 12-5.4 12-12S18.66 0 12 0zm5.521 17.34c-.24.359-.66.48-1.021.24-2.82-1.74-6.36-2.101-10.561-1.141-.418.122-.779-.179-.899-.539-.12-.421.18-.78.54-.9 4.56-1.021 8.52-.6 11.64 1.32.42.18.479.659.301 1.02zm1.44-3.3c-.301.42-.841.6-1.262.3-3.239-1.98-8.159-2.58-11.939-1.38-.479.12-1.02-.12-1.14-.6-.12-.48.12-1.021.6-1.141C9.6 9.9 15 10.561 18.72 12.84c.361.181.54.78.241 1.2zm.12-3.36C15.24 8.4 8.82 8.16 5.16 9.301c-.6.179-1.2-.181-1.38-.721-.18-.601.18-1.2.72-1.381 4.26-1.26 11.28-1.02 15.721 1.621.539.3.719 1.02.419 1.56-.299.421-1.02.599-1.559.3z"/></svg>
```

partials/icons/social/squarespace.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.655 8.719c-1.802-1.801-4.726-1.801-6.564 0l-7.351 7.35c-.45.45-.45 1.2 0 1.65.45.449 1.2.449 1.65 0l7.351-7.351c.899-.899 2.362-.899 3.264 0 .9.9.9 2.364 0 3.264l-7.239 7.239c.9.899 2.362.899 3.263 0l5.589-5.589c1.836-1.838 1.836-4.763.037-6.563zm-2.475 2.437c-.451-.45-1.201-.45-1.65 0l-7.354 7.389c-.9.899-2.361.899-3.262 0-.45-.45-1.2-.45-1.65 0s-.45 1.2 0 1.649c1.801 1.801 4.726 1.801 6.564 0l7.351-7.35c.449-.487.449-1.239.001-1.688zm-2.439-7.35c-1.801-1.801-4.726-1.801-6.564 0l-7.351 7.351c-.45.449-.45 1.199 0 1.649s1.2.45 1.65 0l7.395-7.351c.9-.899 2.371-.899 3.27 0 .451.45 1.201.45 1.65 0 .421-.487.421-1.199-.029-1.649h-.021zm-2.475 2.437c-.45-.45-1.2-.45-1.65 0l-7.351 7.389c-.899.9-2.363.9-3.265 0-.9-.899-.9-2.363 0-3.264l7.239-7.239c-.9-.9-2.362-.9-3.263 0L1.35 8.719c-1.8 1.8-1.8 4.725 0 6.563 1.801 1.801 4.725 1.801 6.564 0l7.35-7.351c.451-.488.451-1.238 0-1.688h.002z"/></svg>
```

partials/icons/social/stackoverflow.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.986 21.865v-6.404h2.134V24H1.844v-8.539h2.13v6.404h15.012zM6.111 19.731H16.85v-2.137H6.111v2.137zm.259-4.852l10.48 2.189.451-2.07-10.478-2.187-.453 2.068zm1.359-5.056l9.705 4.53.903-1.95-9.706-4.53-.902 1.936v.014zm2.715-4.785l8.217 6.855 1.359-1.62-8.216-6.853-1.35 1.617-.01.001zM15.751 0l-1.746 1.294 6.405 8.604 1.746-1.294L15.749 0h.002z"/></svg>
```

partials/icons/social/steam.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.979 0C5.678 0 .511 4.86.022 11.037l6.432 2.658c.545-.371 1.203-.59 1.912-.59.063 0 .125.004.188.006l2.861-4.142V8.91c0-2.495 2.028-4.524 4.524-4.524 2.494 0 4.524 2.031 4.524 4.527s-2.03 4.525-4.524 4.525h-.105l-4.076 2.911c0 .052.004.105.004.159 0 1.875-1.515 3.396-3.39 3.396-1.635 0-3.016-1.173-3.331-2.727L.436 15.27C1.862 20.307 6.486 24 11.979 24c6.627 0 11.999-5.373 11.999-12S18.605 0 11.979 0zM7.54 18.21l-1.473-.61c.262.543.714.999 1.314 1.25 1.297.539 2.793-.076 3.332-1.375.263-.63.264-1.319.005-1.949s-.75-1.121-1.377-1.383c-.624-.26-1.29-.249-1.878-.03l1.523.63c.956.4 1.409 1.5 1.009 2.455-.397.957-1.497 1.41-2.454 1.012H7.54zm11.415-9.303c0-1.662-1.353-3.015-3.015-3.015-1.665 0-3.015 1.353-3.015 3.015 0 1.665 1.35 3.015 3.015 3.015 1.663 0 3.015-1.35 3.015-3.015zm-5.273-.005c0-1.252 1.013-2.266 2.265-2.266 1.249 0 2.266 1.014 2.266 2.266 0 1.251-1.017 2.265-2.266 2.265-1.253 0-2.265-1.014-2.265-2.265z"/></svg>
```

partials/icons/social/strava.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M15.387 17.944l-2.089-4.116h-3.065L15.387 24l5.15-10.172h-3.066m-7.008-5.599l2.836 5.598h4.172L10.463 0l-7 13.828h4.169"/></svg>
```

partials/icons/social/stripe.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.976 9.15c-2.172-.806-3.356-1.426-3.356-2.409 0-.831.683-1.305 1.901-1.305 2.227 0 4.515.858 6.09 1.631l.89-5.494C18.252.975 15.697 0 12.165 0 9.667 0 7.589.654 6.104 1.872 4.56 3.147 3.757 4.992 3.757 7.218c0 4.039 2.467 5.76 6.476 7.219 2.585.92 3.445 1.574 3.445 2.583 0 .98-.84 1.545-2.354 1.545-1.875 0-4.965-.921-6.99-2.109l-.9 5.555C5.175 22.99 8.385 24 11.714 24c2.641 0 4.843-.624 6.328-1.813 1.664-1.305 2.525-3.236 2.525-5.732 0-4.128-2.524-5.851-6.594-7.305h.003z"/></svg>
```

partials/icons/social/ted.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.431 9.886H0V7.665h7.53v2.221H5.1v6.45H2.431v-6.45zm5.514-2.221h7.31v2.221h-4.638v1.083h4.638v2.063h-4.638v1.08h4.638v2.225h-7.31V7.665zm10.43 6.451h1.046c1.664 0 1.907-1.352 1.907-2.166 0-.545-.179-2.063-2.115-2.063h-.854v4.23l.016-.001zm-2.67-6.451h4.384C22.98 7.665 24 9.8 24 11.985c0 2.66-1.409 4.351-4.434 4.351h-3.861V7.663v.002z"/></svg>
```

partials/icons/social/telegram.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M9.028 20.837c-.714 0-.593-.271-.839-.949l-2.103-6.92L22.263 3.37"/><path d="M9.028 20.837c.552 0 .795-.252 1.105-.553l2.941-2.857-3.671-2.214"/><path d="M9.403 15.213l8.89 6.568c1.015.56 1.748.271 2-.942l3.62-17.053c.372-1.487-.564-2.159-1.534-1.72L1.125 10.263c-1.45.582-1.443 1.392-.264 1.753l5.455 1.7L18.94 5.753c.595-.36 1.143-.167.694.232"/></svg>
```

partials/icons/social/tencentqq.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.395 15.035a39.548 39.548 0 0 0-.803-2.264l-1.079-2.695c.001-.032.014-.562.014-.836C19.526 4.632 17.351 0 12 0S4.474 4.632 4.474 9.241c0 .274.013.804.014.836l-1.08 2.695a38.97 38.97 0 0 0-.802 2.264c-1.021 3.283-.69 4.643-.438 4.673.54.065 2.103-2.472 2.103-2.472 0 1.469.756 3.387 2.394 4.771-.612.188-1.363.479-1.845.835-.434.32-.379.646-.301.778.343.578 5.883.369 7.482.189 1.6.18 7.14.389 7.483-.189.078-.132.132-.458-.301-.778-.483-.356-1.233-.646-1.846-.836 1.637-1.384 2.393-3.302 2.393-4.771 0 0 1.563 2.537 2.103 2.472.251-.03.581-1.39-.438-4.673zM12.662 4.846c.039-1.052.659-1.878 1.385-1.846s1.281.912 1.242 1.964c-.039 1.051-.659 1.878-1.385 1.846s-1.282-.912-1.242-1.964zM9.954 3c.725-.033 1.345.794 1.384 1.846.04 1.052-.517 1.931-1.242 1.963-.726.033-1.346-.794-1.385-1.845C8.672 3.912 9.228 3.033 9.954 3zM7.421 8.294c.194-.43 2.147-.908 4.566-.908h.026c2.418 0 4.372.479 4.566.908a.14.14 0 0 1 .014.061c0 .031-.01.059-.026.083-.163.238-2.333 1.416-4.553 1.416h-.026c-2.221 0-4.39-1.178-4.553-1.416a.136.136 0 0 1-.014-.144zm10.422 8.622c-.22 3.676-2.403 5.987-5.774 6.021h-.137c-3.37-.033-5.554-2.345-5.773-6.021-.081-1.35.001-2.496.147-3.43.318.063.638.122.958.176v3.506s1.658.334 3.318.103v-3.225c.488.027.96.04 1.406.034h.025c1.678.021 3.714-.204 5.683-.594.146.934.227 2.08.147 3.43z"/><path d="M10.48 5.804c.313-.041.542-.409.508-.825-.033-.415-.314-.72-.629-.679-.313.04-.541.409-.508.824.034.417.315.72.629.68zM14.479 5.156c.078.037.221.042.289-.146.035-.095.025-.165-.009-.214-.023-.033-.133-.118-.371-.176-.904-.22-1.341.384-1.405.499-.04.072-.012.176.056.227.067.051.139.037.179-.006.58-.628 1.21-.208 1.261-.184z"/></svg>
```

partials/icons/social/themighty.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19.178.001h-4.432L12.05 13.988 9.309.001H4.856c.216.219.334.634.39 1.072v21.21c0 .621-.105 1.383-.425 1.717 1.014-.214 2.307-.416 3.414-.611V9.375l2.489 12.375c.07.46.135 1.084-.021 1.198.847-.129 1.694-.252 2.544-.366-.105-.16-.064-.652-.005-1.061L15.696 9.15v13.095c1.054-.123 2.366-.24 3.47-.349l.012-.008c-.324-.328-.43-1.1-.43-1.724V1.726c0-.627.105-1.396.43-1.726v.001z"/></svg>
```

partials/icons/social/threads.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.186 24h-.007c-3.581-.024-6.334-1.205-8.184-3.509C2.35 18.44 1.5 15.586 1.472 12.01v-.017c.03-3.579.879-6.43 2.525-8.482C5.845 1.205 8.6.024 12.18 0h.014c2.746.02 5.043.725 6.826 2.098 1.677 1.29 2.858 3.13 3.509 5.467l-2.04.569c-1.104-3.96-3.898-5.984-8.304-6.015-2.91.022-5.11.936-6.54 2.717C4.307 6.504 3.616 8.914 3.589 12c.027 3.086.718 5.496 2.057 7.164 1.43 1.783 3.631 2.698 6.54 2.717 2.623-.02 4.358-.631 5.8-2.045 1.647-1.613 1.618-3.593 1.09-4.798-.31-.71-.873-1.3-1.634-1.75-.192 1.352-.622 2.446-1.284 3.272-.886 1.102-2.14 1.704-3.73 1.79-1.202.065-2.361-.218-3.259-.801-1.063-.689-1.685-1.74-1.752-2.964-.065-1.19.408-2.285 1.33-3.082.88-.76 2.119-1.207 3.583-1.291a13.853 13.853 0 0 1 3.02.142c-.126-.742-.375-1.332-.75-1.757-.513-.586-1.308-.883-2.359-.89h-.029c-.844 0-1.992.232-2.721 1.32L7.734 7.847c.98-1.454 2.568-2.256 4.478-2.256h.044c3.194.02 5.097 1.975 5.287 5.388.108.046.216.094.321.142 1.49.7 2.58 1.761 3.154 3.07.797 1.82.871 4.79-1.548 7.158-1.85 1.81-4.094 2.628-7.277 2.65Zm1.003-11.69c-.242 0-.487.007-.739.021-1.836.103-2.98.946-2.916 2.143.067 1.256 1.452 1.839 2.784 1.767 1.224-.065 2.818-.543 3.086-3.71a10.5 10.5 0 0 0-2.215-.221z"/></svg>
```

partials/icons/social/tiktok.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.53.02C13.84 0 15.14.01 16.44 0c.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.15 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"/></svg>
```

partials/icons/social/tinder.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.188.047c-.246-.105-.521.078-.508.339.009.14.014.282.014.39 0 3.679-2.295 6.838-5.576 8.213-.565-.757-.732-2.11-.782-2.906-.017-.277-.346-.426-.576-.26-2.557 1.854-4.205 4.817-4.18 8.153.042 5.58 4.818 10.093 10.586 10.006 5.679-.085 10.254-4.567 10.254-10.082v-.097c0-6.135-3.792-11.412-9.232-13.756z"/></svg>
```

partials/icons/social/trakt.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 24C5.385 24 0 18.615 0 12S5.385 0 12 0s12 5.385 12 12-5.385 12-12 12zm0-22.789C6.05 1.211 1.211 6.05 1.211 12S6.05 22.79 12 22.79 22.79 17.95 22.79 12 17.95 1.211 12 1.211zm-7.11 17.32c1.756 1.92 4.294 3.113 7.11 3.113 1.439 0 2.801-.313 4.027-.876l-6.697-6.68-4.44 4.443zm14.288-.067c1.541-1.71 2.484-3.99 2.484-6.466 0-3.885-2.287-7.215-5.568-8.76l-6.089 6.076 9.164 9.15h.009zm-9.877-8.429L4.227 15.09l-.679-.68 5.337-5.336 6.23-6.225c-.978-.328-2.02-.509-3.115-.509C6.663 2.337 2.337 6.663 2.337 12c0 2.172.713 4.178 1.939 5.801l5.056-5.055.359.329 7.245 7.245c.15-.082.285-.164.42-.266L9.33 12.05l-4.854 4.855-.679-.679 5.535-5.535.359.331 8.46 8.437c.135-.1.255-.215.375-.316L9.39 10.027l-.083.015-.006-.007zm3.047 1.028l-.678-.676 4.788-4.79.679.689-4.789 4.785v-.008zm4.542-6.578l-5.52 5.52-.68-.679 5.521-5.52.679.684v-.005z"/></svg>
```

partials/icons/social/trello.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21 0H3C1.343 0 0 1.343 0 3v18c0 1.656 1.343 3 3 3h18c1.656 0 3-1.344 3-3V3c0-1.657-1.344-3-3-3zM10.44 18.18c0 .795-.645 1.44-1.44 1.44H4.56c-.795 0-1.44-.646-1.44-1.44V4.56c0-.795.645-1.44 1.44-1.44H9c.795 0 1.44.645 1.44 1.44v13.62zm10.44-6c0 .794-.645 1.44-1.44 1.44H15c-.795 0-1.44-.646-1.44-1.44V4.56c0-.795.646-1.44 1.44-1.44h4.44c.795 0 1.44.645 1.44 1.44v7.62z"/></svg>
```

partials/icons/social/tumblr.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M14.563 24c-5.093 0-7.031-3.756-7.031-6.411V9.747H5.116V6.648c3.63-1.313 4.512-4.596 4.71-6.469C9.84.051 9.941 0 9.999 0h3.517v6.114h4.801v3.633h-4.82v7.47c.016 1.001.375 2.371 2.207 2.371h.09c.631-.02 1.486-.205 1.936-.419l1.156 3.425c-.436.636-2.4 1.374-4.156 1.404h-.178l.011.002z"/></svg>
```

partials/icons/social/twilio.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.381-.008.008 5.352 0 11.971V12c0 6.64 5.359 12 12 12 6.64 0 12-5.36 12-12 0-6.641-5.36-12-12-12zm0 20.801c-4.846.015-8.786-3.904-8.801-8.75V12c-.014-4.846 3.904-8.786 8.75-8.801H12c4.847-.014 8.786 3.904 8.801 8.75V12c.015 4.847-3.904 8.786-8.75 8.801H12zm5.44-11.76c0 1.359-1.12 2.479-2.481 2.479-1.366-.007-2.472-1.113-2.479-2.479 0-1.361 1.12-2.481 2.479-2.481 1.361 0 2.481 1.12 2.481 2.481zm0 5.919c0 1.36-1.12 2.48-2.481 2.48-1.367-.008-2.473-1.114-2.479-2.48 0-1.359 1.12-2.479 2.479-2.479 1.361-.001 2.481 1.12 2.481 2.479zm-5.919 0c0 1.36-1.12 2.48-2.479 2.48-1.368-.007-2.475-1.113-2.481-2.48 0-1.359 1.12-2.479 2.481-2.479 1.358-.001 2.479 1.12 2.479 2.479zm0-5.919c0 1.359-1.12 2.479-2.479 2.479-1.367-.007-2.475-1.112-2.481-2.479 0-1.361 1.12-2.481 2.481-2.481 1.358 0 2.479 1.12 2.479 2.481z"/></svg>
```

partials/icons/social/twitch.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M2.089 0L.525 4.175v16.694h5.736V24h3.132l3.127-3.132h4.695l6.26-6.258V0H2.089zm2.086 2.085H21.39v11.479l-3.652 3.652H12l-3.127 3.127v-3.127H4.175V2.085z"/><path d="M9.915 12.522H12v-6.26H9.915v6.26zm5.735 0h2.086v-6.26H15.65v6.26z"/></svg>
```

partials/icons/social/twitter.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.954 4.569c-.885.389-1.83.654-2.825.775 1.014-.611 1.794-1.574 2.163-2.723-.951.555-2.005.959-3.127 1.184-.896-.959-2.173-1.559-3.591-1.559-2.717 0-4.92 2.203-4.92 4.917 0 .39.045.765.127 1.124C7.691 8.094 4.066 6.13 1.64 3.161c-.427.722-.666 1.561-.666 2.475 0 1.71.87 3.213 2.188 4.096-.807-.026-1.566-.248-2.228-.616v.061c0 2.385 1.693 4.374 3.946 4.827-.413.111-.849.171-1.296.171-.314 0-.615-.03-.916-.086.631 1.953 2.445 3.377 4.604 3.417-1.68 1.319-3.809 2.105-6.102 2.105-.39 0-.779-.023-1.17-.067 2.189 1.394 4.768 2.209 7.557 2.209 9.054 0 13.999-7.496 13.999-13.986 0-.209 0-.42-.015-.63.961-.689 1.8-1.56 2.46-2.548l-.047-.02z"/></svg>
```

partials/icons/social/twoo.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M10.116 16.877c.064-.054.129-.109.189-.168-1.209 1.176-2.756 1.756-4.291 1.735h-.023c-1.545-.025-3.08-.656-4.245-1.894-.733-.78-1.233-1.708-1.507-2.691v-.007c-.604-2.199-.065-4.674 1.605-6.406 2.346-2.434 6.072-2.492 8.459-.205l1.215 1.275.543.57 4.228 4.484h.018c.045.046.09.076.119.121.855.779 2.162.75 2.986-.105.869-.9.9-2.37.047-3.285-.092-.105-.197-.195-.303-.27l-.24-.166c-.824-.449-1.875-.3-2.58.42-.105.105-.195.226-.27.346-.301.465-.406 1.02-.346 1.561l-1.514-1.529-1.756-1.665c.286-.563.657-1.095 1.114-1.569.105-.105.211-.21.318-.307-.064.055-.129.111-.189.168 1.209-1.176 2.756-1.754 4.291-1.734h.023c1.545.025 3.08.656 4.246 1.895.732.779 1.232 1.707 1.506 2.693v.006c.605 2.197.066 4.676-1.605 6.405-2.346 2.434-6.072 2.494-8.459.205l-1.214-1.286-.543-.581-4.225-4.501-.004-.015c-.016 0-.016-.015-.016-.015-.045-.046-.09-.09-.121-.136-.854-.78-2.16-.765-2.984.105-.87.9-.9 2.37-.045 3.271.09.105.195.18.3.27l.24.15c.825.436 1.876.3 2.58-.436.105-.104.196-.225.271-.345.301-.465.404-1.034.345-1.575l1.515 1.561 1.758 1.771c-.285.564-.657 1.096-1.115 1.569-.104.105-.21.21-.318.306l-.003.004z"/></svg>
```

partials/icons/social/udacity.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M8.01.138L0 4.68v10.458c-.015 4.803 3.915 8.71 8.775 8.725 1.604.004 3.115-.418 4.414-1.154l6.487-3.686c2.561-1.306 4.313-3.946 4.323-6.991V1.096L22.409.18l-6.503 3.631v11.373c-.003.482-.025.836-.153 1.435-.216.915-.521 1.561-.574 1.665-.511-.03-1.546-.314-2.386-.81-.42-.24-.914-.601-1.364-1.021-.3-.285-.556-.615-.78-.945-.24-.345-.435-.704-.585-1.079-.165-.391-.284-.78-.375-1.185-.09-.421-.104-.855-.104-1.275L9.6 1.051 8.01.143V.138zm3.687 21.583c-.436.179-.889.316-1.35.41-.477.094-.916.141-1.403.141-.488 0-.978-.053-1.452-.151-.461-.092-.915-.234-1.35-.417-.424-.179-.836-.404-1.219-.659-.99-.691-1.5-1.291-1.941-1.936-.26-.39-.48-.795-.66-1.215-.183-.435-.322-.886-.416-1.335-.09-.465-.104-.961-.104-1.439V5.58l6-3.621V11.97c0 3.806 2.819 6.979 6.45 7.747-.135.165-.24.331-.391.48-.33.322-.675.624-1.064.877-.375.257-.645.465-1.065.644l-.035.003zm10.405-8.408c-.087.404-.211.803-.375 1.186-.439.955-1.148 1.77-1.74 2.294-1.216 1.101-2.725 1.44-2.898 1.44.362-.948.608-1.965.611-3.039V4.725L22.204 2l.003 10.009c0 .431-.018.879-.105 1.296v.008z"/></svg>
```

partials/icons/social/udemy.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.58 13.38a.66.66 0 0 0-.28-.14c-.6.61-1.35 1.25-2 1.68-.31.2-.7.3-.95.3-.59 0-.84-.55-.91-1.44a54.8 54.8 0 0 1-.17-4.83c0-2.26-.52-3.8-1.88-3.92l-.18-.01c-.83 0-1.24.43-1.77 1.52-.46.94-1.17 2.3-2.48 4.9a34.72 34.72 0 0 1-3.5 5.58c-.31.38-.55.64-.78.8a.8.8 0 0 1-.44.14c-.43 0-.75-.36-.85-1.21a5.46 5.46 0 0 1-.04-.69c0-1.75.66-4.6 1.8-8.78.83-3.05.48-5.13-1.34-5.13h-.03c-.41 0-.75.16-1.08.42-.33.25-.65.81-.96 1.56-.34.84-2.42 5.03-5.74 7.2-.04.81.42 1.63 1.37 1.73.85.08 1.46-.28 2.24-.81l-.16.73a31.56 31.56 0 0 0-.5 2.6c-.46 4.2 1.47 6.27 3.74 6.27.38 0 .76-.05 1.13-.15 2.5-.63 4.9-3.51 7.75-10.13a18.8 18.8 0 0 0-.01 2.02c.19 3.8 1.68 4.93 3.8 4.93 1.6 0 3.09-.83 3.85-1.87a3.7 3.7 0 0 0 .79-2.19c-.02-.49-.17-.88-.42-1.08z"/></svg>
```

partials/icons/social/unsplash.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M7.5 6.75V0h9v6.75h-9zm9 3.75H24V24H0V10.5h7.5v6.75h9V10.5z"/></svg>
```

partials/icons/social/upwork.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.561 13.158c-1.102 0-2.135-.467-3.074-1.227l.228-1.076.008-.042c.207-1.143.849-3.06 2.839-3.06 1.492 0 2.703 1.212 2.703 2.703-.001 1.489-1.212 2.702-2.704 2.702zm0-8.14c-2.539 0-4.51 1.649-5.31 4.366-1.22-1.834-2.148-4.036-2.687-5.892H7.828v7.112c-.002 1.406-1.141 2.546-2.547 2.548-1.405-.002-2.543-1.143-2.545-2.548V3.492H0v7.112c0 2.914 2.37 5.303 5.281 5.303 2.913 0 5.283-2.389 5.283-5.303v-1.19c.529 1.107 1.182 2.229 1.974 3.221l-1.673 7.873h2.797l1.213-5.71c1.063.679 2.285 1.109 3.686 1.109 3 0 5.439-2.452 5.439-5.45 0-3-2.439-5.439-5.439-5.439z"/></svg>
```

partials/icons/social/vimeo.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.977 6.416c-.105 2.338-1.739 5.543-4.894 9.609-3.268 4.247-6.026 6.37-8.29 6.37-1.409 0-2.578-1.294-3.553-3.881L5.322 11.4C4.603 8.816 3.834 7.522 3.01 7.522c-.179 0-.806.378-1.881 1.132L0 7.197c1.185-1.044 2.351-2.084 3.501-3.128C5.08 2.701 6.266 1.984 7.055 1.91c1.867-.18 3.016 1.1 3.447 3.838.465 2.953.789 4.789.971 5.507.539 2.45 1.131 3.674 1.776 3.674.502 0 1.256-.796 2.265-2.385 1.004-1.589 1.54-2.797 1.612-3.628.144-1.371-.395-2.061-1.614-2.061-.574 0-1.167.121-1.777.391 1.186-3.868 3.434-5.757 6.762-5.637 2.473.06 3.628 1.664 3.493 4.797l-.013.01z"/></svg>
```

partials/icons/social/vine.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.521 11.922c-.618.143-1.217.206-1.758.206-3.028 0-5.361-2.116-5.361-5.794 0-1.801.706-2.731 1.696-2.731.946 0 1.562.841 1.562 2.552 0 .975-.256 2.041-.45 2.672 0 0 .93 1.636 3.481 1.125.54-1.201.842-2.762.842-4.127C22.533 2.146 20.657 0 17.219 0c-3.543-.017-5.615 2.7-5.615 6.288 0 3.55 1.659 6.597 4.395 7.985-1.15 2.301-2.614 4.328-4.142 5.856-2.769-3.351-5.273-7.82-6.302-16.541H1.467c1.889 14.526 7.517 19.149 9.004 20.035.84.504 1.566.48 2.336.049 1.215-.688 4.848-4.315 6.859-8.563.84-.003 1.861-.1 2.867-.328v-2.865l-.012.006z"/></svg>
```

partials/icons/social/visa.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.445 8.623c-.387-.146-.99-.301-1.74-.301-1.92 0-3.275.968-3.285 2.355-.012 1.02.964 1.594 1.701 1.936.757.35 1.01.57 1.008.885-.005.477-.605.693-1.162.693-.766 0-1.186-.107-1.831-.375l-.239-.111-.271 1.598c.466.195 1.306.362 2.175.375 2.041 0 3.375-.961 3.391-2.439.016-.813-.51-1.43-1.621-1.938-.674-.33-1.094-.551-1.094-.886 0-.296.359-.612 1.109-.612.645-.01 1.096.129 1.455.273l.18.081.271-1.544-.047.01zm4.983-.17h-1.5c-.467 0-.816.127-1.021.591l-2.885 6.534h2.041l.408-1.07 2.49.002c.061.25.24 1.068.24 1.068H24l-1.572-7.125zM9.66 8.393h1.943l-1.215 7.129H8.444L9.66 8.391v.002zm-4.939 3.929l.202.99 1.901-4.859h2.059l-3.061 7.115H3.768l-1.68-6.026c-.035-.103-.078-.173-.18-.237C1.34 9.008.705 8.766 0 8.598l.025-.15h3.131c.424.016.766.15.883.604l.682 3.273v-.003zm15.308.727l.775-1.994c-.01.02.16-.412.258-.68l.133.615.449 2.057h-1.615v.002z"/></svg>
```

partials/icons/social/vk.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.701 18.771h1.437s.433-.047.654-.284c.21-.221.21-.63.21-.63s-.031-1.927.869-2.21c.887-.281 2.012 1.86 3.211 2.683.916.629 1.605.494 1.605.494l3.211-.044s1.682-.105.887-1.426c-.061-.105-.451-.975-2.371-2.76-2.012-1.861-1.742-1.561.676-4.787 1.469-1.965 2.07-3.166 1.875-3.676-.166-.48-1.26-.361-1.26-.361l-3.602.031s-.27-.031-.465.09c-.195.119-.314.391-.314.391s-.572 1.529-1.336 2.82c-1.623 2.729-2.268 2.879-2.523 2.699-.604-.391-.449-1.58-.449-2.432 0-2.641.404-3.75-.781-4.035-.39-.091-.681-.15-1.685-.166-1.29-.014-2.378.01-2.995.311-.405.203-.72.652-.539.675.24.03.779.146 1.064.537.375.506.359 1.636.359 1.636s.211 3.116-.494 3.503c-.495.262-1.155-.28-2.595-2.756-.735-1.26-1.291-2.67-1.291-2.67s-.105-.256-.299-.406c-.227-.165-.557-.225-.557-.225l-3.435.03s-.51.016-.689.24c-.166.195-.016.615-.016.615s2.686 6.287 5.732 9.453c2.79 2.902 5.956 2.715 5.956 2.715l-.05-.055z"/></svg>
```

partials/icons/social/vsco.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0C5.376 0 0 5.376 0 12s5.376 12 12 12 12-5.376 12-12S18.624 0 12 0zm11.52 12c0 .408-.023.792-.072 1.176l-2.04-.24c.024-.312.05-.624.05-.936 0-.288-.025-.6-.05-.888l2.04-.24c.072.384.072.744.072 1.128zM.479 12c0-.384.024-.769.049-1.152l2.04.24c-.024.312-.047.6-.047.912s.023.6.047.912l-2.04.24C.479 12.769.479 12.384.479 12zm20.472-3.096l1.921-.72c.264.72.433 1.464.552 2.232l-2.04.24c-.097-.6-.24-1.2-.433-1.752zM21 12c0 .6-.072 1.176-.167 1.752l-2.017-.455c.071-.409.119-.841.119-1.297s-.048-.912-.119-1.344l2.017-.457c.118.577.167 1.177.167 1.801zm-9 6.456C8.435 18.455 5.545 15.565 5.544 12 5.545 8.435 8.435 5.545 12 5.544c3.565.001 6.455 2.891 6.456 6.456.008 3.559-2.871 6.448-6.429 6.456H12zM12.216 21v-2.064c.885-.029 1.756-.224 2.568-.575l.888 1.872c-1.09.482-2.264.742-3.456.767zm-3.936-.791l.912-1.873c.792.359 1.656.575 2.568.6V21c-1.202-.023-2.386-.293-3.48-.791zM3 12c0-.624.072-1.224.192-1.824l2.016.456c-.098.45-.146.908-.144 1.368 0 .432.048.864.12 1.272l-2.016.455C3.051 13.159 2.994 12.58 3 12zm8.76-9v2.064c-.877.029-1.74.224-2.544.576l-.888-1.871C9.411 3.291 10.577 3.03 11.76 3zm3.935.792l-.911 1.872c-.809-.363-1.682-.559-2.568-.576V3.024c1.248 0 2.424.288 3.479.768zm5.088 4.656c-.231-.56-.513-1.098-.84-1.608l1.681-1.152c.407.648.768 1.32 1.056 2.04l-1.897.72zm-.07 1.296l-2.018.456c-.23-.85-.621-1.648-1.151-2.352l1.632-1.295c.72.959 1.248 2.015 1.537 3.191zm-3.457-2.256c-.572-.667-1.264-1.22-2.04-1.633l.912-1.871c1.056.549 1.993 1.299 2.76 2.208l-1.632 1.296zm-.6-3.744l.96-1.824c.672.384 1.295.816 1.896 1.32L18.145 4.8c-.461-.401-.959-.754-1.489-1.056zm-.408-.216c-.54-.266-1.102-.483-1.68-.648l.504-1.992c.744.216 1.464.48 2.159.84l-.983 1.8zm-2.16-.768c-.6-.144-1.2-.216-1.824-.239V.479c.793.024 1.584.12 2.328.289l-.504 1.992zm-2.28-.239c-.605.021-1.207.094-1.8.216L9.528.744c.72-.168 1.487-.265 2.28-.265v2.042zm-2.28.334c-.586.167-1.156.384-1.704.649l-.96-1.824c.691-.343 1.415-.616 2.16-.816l.504 1.991zm-2.112.865c-.529.294-1.027.64-1.488 1.032L4.56 3.216c.6-.504 1.224-.936 1.896-1.319l.96 1.823zm.48.264l.888 1.871c-.792.408-1.464.96-2.04 1.608L5.136 6.168c.775-.895 1.711-1.636 2.76-2.184zM4.848 6.552l1.608 1.295c-.53.705-.921 1.503-1.152 2.353l-2.016-.456c.312-1.2.84-2.28 1.56-3.192zM3.24 8.4l-1.92-.72c.287-.72.648-1.416 1.08-2.04l1.68 1.176c-.341.494-.623 1.025-.84 1.584zm-.168.455c-.192.577-.36 1.152-.432 1.776L.6 10.393c.12-.769.288-1.537.553-2.257l1.919.719zm-.456 4.513c.096.6.239 1.2.432 1.776l-1.92.72c-.271-.728-.456-1.485-.552-2.257l2.04-.239zm.624 2.208c.239.576.528 1.104.84 1.607L2.4 18.336c-.435-.629-.797-1.306-1.08-2.016l1.92-.744zm.024-1.392l2.017-.456c.216.864.624 1.681 1.128 2.376L4.8 17.4c-.725-.957-1.247-2.051-1.536-3.216zm3.432 2.28c.577.672 1.272 1.248 2.064 1.656l-.912 1.872c-1.063-.557-2.009-1.315-2.784-2.232l1.632-1.296zm.72 3.815l-.96 1.825c-.674-.376-1.31-.819-1.896-1.321l1.368-1.535c.456.407.936.744 1.488 1.031zm.408.217c.528.264 1.104.48 1.705.647l-.504 1.992c-.747-.196-1.471-.469-2.16-.815l.959-1.824zm2.16.768c.576.12 1.176.193 1.8.217v2.039c-.774-.026-1.544-.114-2.305-.264l.505-1.992zm2.28.216c.605-.021 1.207-.094 1.801-.217l.479 1.992c-.749.168-1.513.264-2.28.287V21.48zm2.257-.336c.586-.165 1.155-.382 1.703-.647l.96 1.824c-.688.35-1.412.623-2.159.815l-.504-1.992zm2.086-.865c.528-.287 1.032-.647 1.488-1.031l1.369 1.535c-.588.502-1.223.945-1.896 1.321l-.961-1.825zm-.479-.263l-.888-1.871c.788-.414 1.489-.977 2.064-1.656l1.606 1.296c-.778.91-1.722 1.668-2.782 2.231zm3.071-2.592l-1.607-1.296c.532-.708.916-1.517 1.128-2.376l2.017.456c-.311 1.157-.831 2.248-1.538 3.216zM20.76 15.6l1.92.721c-.288.72-.648 1.392-1.079 2.04l-1.682-1.177c.337-.504.624-1.032.841-1.584zm.168-.455c.192-.553.336-1.152.433-1.752l2.039.239c-.11.761-.294 1.508-.551 2.232l-1.921-.719zm.456-9.841l-1.681 1.152c-.358-.49-.76-.947-1.199-1.368l1.368-1.536c.552.552 1.056 1.128 1.512 1.752zM4.2 3.528l1.368 1.536c-.456.408-.84.864-1.2 1.368l-1.68-1.176c.431-.636.94-1.216 1.512-1.728zM2.664 18.744l1.68-1.152c.36.48.769.937 1.2 1.369l-1.368 1.535c-.548-.545-1.054-1.131-1.512-1.752zm17.16 1.729l-1.368-1.537c.432-.407.841-.863 1.199-1.344l1.682 1.176c-.457.6-.961 1.175-1.513 1.705z"/></svg>
```

partials/icons/social/wechat.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M23.541 12.748c-.609-1.38-1.758-2.476-3.092-3.151-2.354-1.192-5.281-1.185-7.629.03-1.631.837-2.993 2.337-3.379 4.162-.318 1.344-.033 2.791.68 3.961 1.061 1.762 2.979 2.887 4.971 3.248 1.443.293 2.936.119 4.338-.285.842.326 1.592.854 2.408 1.246-.211-.707-.436-1.406-.676-2.102.916-.65 1.746-1.461 2.244-2.479.744-1.415.789-3.171.135-4.63zm-9.924-9.466c-2.495-1.404-5.602-1.615-8.286-.645-1.764.635-3.36 1.815-4.346 3.42-.895 1.45-1.23 3.258-.799 4.917.433 1.84 1.711 3.383 3.262 4.413-.3.85-.585 1.699-.855 2.555.975-.51 1.95-1.043 2.926-1.561 1.17.375 2.415.559 3.66.518-.33-.943-.405-1.965-.255-2.951.225-1.371.975-2.625 1.994-3.554 1.726-1.615 4.171-2.296 6.496-2.131-.436-2.135-1.936-3.939-3.824-4.98h.027zm1.733 9.989c-.209.652-1.156.848-1.615.352-.506-.459-.309-1.418.355-1.623.734-.31 1.582.537 1.26 1.271zm4.795.092c-.256.586-1.141.723-1.576.27-.209-.191-.27-.479-.344-.73.104-.458.42-.933.93-.955.705-.098 1.336.773.975 1.416h.015zM12.99 6.909c.008.961-1.275 1.561-1.995.909-.747-.535-.535-1.837.342-2.106.785-.315 1.713.344 1.651 1.185l.002.012zm-6.059.244c-.172.835-1.291 1.238-1.946.678-.759-.535-.546-1.861.345-2.131.873-.336 1.865.55 1.601 1.453z"/></svg>
```

partials/icons/social/weibo.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M10.098 20.323c-3.977.391-7.414-1.406-7.672-4.02-.259-2.609 2.759-5.047 6.74-5.441 3.979-.394 7.413 1.404 7.671 4.018.259 2.6-2.759 5.049-6.737 5.439l-.002.004zM9.05 17.219c-.384.616-1.208.884-1.829.602-.612-.279-.793-.991-.406-1.593.379-.595 1.176-.861 1.793-.601.622.263.82.972.442 1.592zm1.27-1.627c-.141.237-.449.353-.689.253-.236-.09-.313-.361-.177-.586.138-.227.436-.346.672-.24.239.09.315.36.18.601l.014-.028zm.176-2.719c-1.893-.493-4.033.45-4.857 2.118-.836 1.704-.026 3.591 1.886 4.21 1.983.64 4.318-.341 5.132-2.179.8-1.793-.201-3.642-2.161-4.149zm7.563-1.224c-.346-.105-.57-.18-.405-.615.375-.977.42-1.804 0-2.404-.781-1.112-2.915-1.053-5.364-.03 0 0-.766.331-.571-.271.376-1.217.315-2.224-.27-2.809-1.338-1.337-4.869.045-7.888 3.08C1.309 10.87 0 13.273 0 15.348c0 3.981 5.099 6.395 10.086 6.395 6.536 0 10.888-3.801 10.888-6.82 0-1.822-1.547-2.854-2.915-3.284v.01zm1.908-5.092c-.766-.856-1.908-1.187-2.96-.962-.436.09-.706.511-.616.932.09.42.511.691.932.602.511-.105 1.067.044 1.442.465.376.421.466.977.316 1.473-.136.406.089.856.51.992.405.119.857-.105.992-.512.33-1.021.12-2.178-.646-3.035l.03.045zm2.418-2.195c-1.576-1.757-3.905-2.419-6.054-1.968-.496.104-.812.587-.706 1.081.104.496.586.813 1.082.707 1.532-.331 3.185.15 4.296 1.383 1.112 1.246 1.429 2.943.947 4.416-.165.48.106 1.007.586 1.157.479.165.991-.104 1.157-.586.675-2.088.241-4.478-1.338-6.235l.03.045z"/></svg>
```

partials/icons/social/whatsapp.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.498 14.382c-.301-.15-1.767-.867-2.04-.966-.273-.101-.473-.15-.673.15-.197.295-.771.964-.944 1.162-.175.195-.349.21-.646.075-.3-.15-1.263-.465-2.403-1.485-.888-.795-1.484-1.77-1.66-2.07-.174-.3-.019-.465.13-.615.136-.135.301-.345.451-.523.146-.181.194-.301.297-.496.1-.21.049-.375-.025-.524-.075-.15-.672-1.62-.922-2.206-.24-.584-.487-.51-.672-.51-.172-.015-.371-.015-.571-.015-.2 0-.523.074-.797.359-.273.3-1.045 1.02-1.045 2.475s1.07 2.865 1.219 3.075c.149.195 2.105 3.195 5.1 4.485.714.3 1.27.48 1.704.629.714.227 1.365.195 1.88.121.574-.091 1.767-.721 2.016-1.426.255-.705.255-1.29.18-1.425-.074-.135-.27-.21-.57-.345m-5.446 7.443h-.016c-1.77 0-3.524-.48-5.055-1.38l-.36-.214-3.75.975 1.005-3.645-.239-.375c-.99-1.576-1.516-3.391-1.516-5.26 0-5.445 4.455-9.885 9.942-9.885 2.654 0 5.145 1.035 7.021 2.91 1.875 1.859 2.909 4.35 2.909 6.99-.004 5.444-4.46 9.885-9.935 9.885M20.52 3.449C18.24 1.245 15.24 0 12.045 0 5.463 0 .104 5.334.101 11.893c0 2.096.549 4.14 1.595 5.945L0 24l6.335-1.652c1.746.943 3.71 1.444 5.71 1.447h.006c6.585 0 11.946-5.336 11.949-11.896 0-3.176-1.24-6.165-3.495-8.411"/></svg>
```

partials/icons/social/wikipedia.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12.09 13.119c-.936 1.932-2.217 4.548-2.853 5.728-.616 1.074-1.127.931-1.532.029-1.406-3.321-4.293-9.144-5.651-12.409-.251-.601-.441-.987-.619-1.139-.181-.15-.554-.24-1.122-.271C.103 5.033 0 4.982 0 4.898v-.455l.052-.045c.924-.005 5.401 0 5.401 0l.051.045v.434c0 .119-.075.176-.225.176l-.564.031c-.485.029-.727.164-.727.436 0 .135.053.33.166.601 1.082 2.646 4.818 10.521 4.818 10.521l.136.046 2.411-4.81-.482-1.067-1.658-3.264s-.318-.654-.428-.872c-.728-1.443-.712-1.518-1.447-1.617-.207-.023-.313-.05-.313-.149v-.468l.06-.045h4.292l.113.037v.451c0 .105-.076.15-.227.15l-.308.047c-.792.061-.661.381-.136 1.422l1.582 3.252 1.758-3.504c.293-.64.233-.801.111-.947-.07-.084-.305-.22-.812-.24l-.201-.021c-.052 0-.098-.015-.145-.051-.045-.031-.067-.076-.067-.129v-.427l.061-.045c1.247-.008 4.043 0 4.043 0l.059.045v.436c0 .121-.059.178-.193.178-.646.03-.782.095-1.023.439-.12.186-.375.589-.646 1.039l-2.301 4.273-.065.135 2.792 5.712.17.048 4.396-10.438c.154-.422.129-.722-.064-.895-.197-.172-.346-.273-.857-.295l-.42-.016c-.061 0-.105-.014-.152-.045-.043-.029-.072-.075-.072-.119v-.436l.059-.045h4.961l.041.045v.437c0 .119-.074.18-.209.18-.648.03-1.127.18-1.443.421-.314.255-.557.616-.736 1.067 0 0-4.043 9.258-5.426 12.339-.525 1.007-1.053.917-1.503-.031-.571-1.171-1.773-3.786-2.646-5.71l.053-.036z"/></svg>
```

partials/icons/social/wire.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 14.475c.009 4.084-3.296 7.401-7.38 7.41h-.016c-1.637-.015-3.222-.58-4.5-1.605-3.269 2.544-7.981 1.957-10.524-1.313-1-1.286-1.555-2.862-1.58-4.492V2.82h1.41v11.655c-.002 3.314 2.683 6.002 5.996 6.004 1.293.001 2.552-.416 3.589-1.189-1.163-1.335-1.806-3.043-1.815-4.814v-9.54c0-1.557 1.263-2.82 2.82-2.82s2.82 1.263 2.82 2.82v9.54c.006 1.766-.623 3.474-1.77 4.814 2.674 1.957 6.429 1.371 8.383-1.304.745-1.019 1.149-2.248 1.157-3.511V2.82H24v11.655zm-10.59-9.54c0-.778-.632-1.41-1.41-1.41-.779 0-1.41.631-1.41 1.41v9.54c.002 1.41.501 2.776 1.41 3.855.908-1.079 1.408-2.445 1.41-3.855v-9.54z"/></svg>
```

partials/icons/social/wordpress.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M21.469 6.825c.84 1.537 1.318 3.3 1.318 5.175 0 3.979-2.156 7.456-5.363 9.325l3.295-9.527c.615-1.54.82-2.771.82-3.864 0-.405-.026-.78-.07-1.11m-7.981.105c.647-.03 1.232-.105 1.232-.105.582-.075.514-.93-.067-.899 0 0-1.755.135-2.88.135-1.064 0-2.85-.15-2.85-.15-.585-.03-.661.855-.075.885 0 0 .54.061 1.125.09l1.68 4.605-2.37 7.08L5.354 6.9c.649-.03 1.234-.1 1.234-.1.585-.075.516-.93-.065-.896 0 0-1.746.138-2.874.138-.2 0-.438-.008-.69-.015C4.911 3.15 8.235 1.215 12 1.215c2.809 0 5.365 1.072 7.286 2.833-.046-.003-.091-.009-.141-.009-1.06 0-1.812.923-1.812 1.914 0 .89.513 1.643 1.06 2.531.411.72.89 1.643.89 2.977 0 .915-.354 1.994-.821 3.479l-1.075 3.585-3.9-11.61.001.014zM12 22.784c-1.059 0-2.081-.153-3.048-.437l3.237-9.406 3.315 9.087c.024.053.05.101.078.149-1.12.393-2.325.609-3.582.609M1.211 12c0-1.564.336-3.05.935-4.39L7.29 21.709C3.694 19.96 1.212 16.271 1.211 12M12 0C5.385 0 0 5.385 0 12s5.385 12 12 12 12-5.385 12-12S18.615 0 12 0"/></svg>
```

partials/icons/social/x.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M18.901 1.153h3.68l-8.04 9.19L24 22.846h-7.406l-5.8-7.584-6.638 7.584H.474l8.6-9.83L0 1.154h7.594l5.243 6.932ZM17.61 20.644h2.039L6.486 3.24H4.298Z"/></svg>
```

partials/icons/social/xbox.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M4.102 21.033C6.211 22.881 8.977 24 12 24c3.026 0 5.789-1.119 7.902-2.967 1.877-1.912-4.316-8.709-7.902-11.417-3.582 2.708-9.779 9.505-7.898 11.417zm11.16-14.406c2.5 2.961 7.484 10.313 6.076 12.912C23.002 17.48 24 14.861 24 12.004c0-3.34-1.365-6.362-3.57-8.536 0 0-.027-.022-.082-.042-.063-.022-.152-.045-.281-.045-.592 0-1.985.434-4.805 3.246zM3.654 3.426c-.057.02-.082.041-.086.042C1.365 5.642 0 8.664 0 12.004c0 2.854.998 5.473 2.661 7.533-1.401-2.605 3.579-9.951 6.08-12.91-2.82-2.813-4.216-3.245-4.806-3.245-.131 0-.223.021-.281.046v-.002zM12 3.551S9.055 1.828 6.755 1.746c-.903-.033-1.454.295-1.521.339C7.379.646 9.659 0 11.984 0H12c2.334 0 4.605.646 6.766 2.085-.068-.046-.615-.372-1.52-.339C14.946 1.828 12 3.545 12 3.545v.006z"/></svg>
```

partials/icons/social/youtube.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path class="a" d="M23.495 6.205a3.007 3.007 0 0 0-2.088-2.088c-1.87-.501-9.396-.501-9.396-.501s-7.507-.01-9.396.501A3.007 3.007 0 0 0 .527 6.205a31.247 31.247 0 0 0-.522 5.805 31.247 31.247 0 0 0 .522 5.783 3.007 3.007 0 0 0 2.088 2.088c1.868.502 9.396.502 9.396.502s7.506 0 9.396-.502a3.007 3.007 0 0 0 2.088-2.088 31.247 31.247 0 0 0 .5-5.783 31.247 31.247 0 0 0-.5-5.805zM9.609 15.601V8.408l6.264 3.602z"/></svg>
```

partials/icons/social/youtubemusic.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M9.818182 15.136364l5.318182-3.272728-5.318182-3zM12 6.278182c3.155455 0 5.721818 2.566363 5.721818 5.721818S15.155455 17.721818 12 17.721818 6.278182 15.155455 6.278182 12 8.844545 6.278182 12 6.278182m0-.550909C8.535 5.727273 5.727273 8.535 5.727273 12S8.535 18.272727 12 18.272727 18.272727 15.465 18.272727 12 15.465 5.727273 12 5.727273zM24 12a12 12 0 01-12 12A12 12 0 010 12 12 12 0 0112 0a12 12 0 0112 12"/></svg>
```

partials/icons/social/zendesk.hbs
```
1 | <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M11.085 21.095H0L11.085 7.712v13.383zm12.915 0H12.915c0-3.063 2.479-5.543 5.543-5.543 3.063 0 5.542 2.482 5.542 5.543zm-11.085-4.804V2.905H24L12.915 16.291zm-1.83-13.386c0 3.061-2.481 5.544-5.543 5.544C2.482 8.449 0 5.968 0 2.907h11.085v-.002z"/></svg>
```

partials/images/archive_image.hbs
```
1 | <picture>
2 | 	<source srcset="{{img_url archive_image size="s" format="webp"}} 300w,
3 | 					{{img_url archive_image size="m" format="webp"}} 600w"
4 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px"
5 | 	type="image/webp">
6 | 	<img srcset="{{img_url archive_image size="s"}} 300w, 
7 | 				 {{img_url archive_image size="m"}} 600w"
8 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px"
9 | 	src="{{img_url archive_image size="m"}}"
10 | 	alt="{{name}}">
11 | </picture>
```

partials/images/background_cover.hbs
```
1 | {{^is "author,tag"}}{{#if custom_cover}}<div class="global-cover{{#if is_membership}} is-membership{{else if is_featured}} is-featured{{/if}}" style="background-image:url({{{img_url custom_cover size="xl" format="webp"}}})"></div>{{/if}}{{/is}}
2 | {{#is "author"}}{{{block "cover_image"}}}{{/is}}
3 | {{#is "tag"}}{{{block "feature_image"}}}{{/is}}
```

partials/images/loop_image.hbs
```
1 | {{#if is_first}}
2 | <picture>
3 | 	<source srcset="{{img_url feature_image size="s" format="webp"}} 300w,
4 | 					{{img_url feature_image size="m" format="webp"}} 600w,
5 | 					{{img_url feature_image size="xl" format="webp"}} 1600w"
6 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px, 1600px"
7 | 	type="image/webp">
8 | 	<img srcset="{{img_url feature_image size="s"}} 300w, 
9 | 				 {{img_url feature_image size="m"}} 600w,
10 | 				 {{img_url feature_image size="xl"}} 1600w"
11 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px, 1600px"
12 | 	src="{{img_url feature_image size="xl"}}"
13 | 	loading="lazy"
14 | 	alt="{{title}}">
15 | </picture>
16 | {{else}}
17 | <picture>
18 | 	<source srcset="{{img_url feature_image size="s" format="webp"}} 300w,
19 | 					{{img_url feature_image size="m" format="webp"}} 600w"
20 | 	sizes="(max-width:480px) 300px, 600px"
21 | 	type="image/webp">
22 | 	<img srcset="{{img_url feature_image size="s"}} 300w, 
23 | 				 {{img_url feature_image size="m"}} 600w"
24 | 	sizes="(max-width:480px) 300px, 600px"
25 | 	src="{{img_url feature_image size="m"}}"
26 | 	loading="lazy"
27 | 	alt="{{title}}">
28 | </picture>
29 | {{/if}}
```

partials/images/other_image.hbs
```
1 | <picture>
2 | 	<source srcset="{{img_url other_image size="s" format="webp"}} 300w"
3 | 	sizes="300px"
4 | 	type="image/webp">
5 | 	<img srcset="{{img_url other_image size="s"}} 300w"
6 | 	sizes="300px"
7 | 	src="{{img_url other_image size="s"}}"
8 | 	{{#if lazy}}loading="lazy"{{/if}}
9 | 	alt="{{alt}}">
10 | </picture>
```

partials/images/post_image.hbs
```
1 | <picture>
2 | 	<source srcset="{{img_url feature_image size="s" format="webp"}} 300w,
3 | 					{{img_url feature_image size="m" format="webp"}} 600w,
4 | 					{{img_url feature_image size="l" format="webp"}} 1200w,
5 | 					{{img_url feature_image size="xxl" format="webp"}} 2000w"
6 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px, (max-width:1024px) 1200px, 2000px"
7 | 	type="image/webp">
8 | 	<img srcset="{{img_url feature_image size="s"}} 300w, 
9 | 				 {{img_url feature_image size="m"}} 600w,
10 | 				 {{img_url feature_image size="l"}} 1200w,
11 | 				 {{img_url feature_image size="xxl"}} 2000w"
12 | 	sizes="(max-width:480px) 300px, (max-width:768px) 600px, (max-width:1024px) 1200px, 2000px"
13 | 	src="{{img_url feature_image size="xxl"}}"
14 | 	alt="{{#if feature_image_alt}}{{feature_image_alt}}{{else}}{{title}}{{/if}}">
15 | </picture>
```

partials/item.hbs
```
1 | {{^if is_widget}}
2 | <article class="item{{#if is_top}} is-top{{#if is_first}} is-first{{/if}}{{else if is_special}} is-special{{/if}}">
3 | 	{{#if is_featured}}
4 | 	<a href="{{url}}" class="global-link" aria-label="{{title}}"></a>
5 | 	{{/if}}
6 | 	{{#if feature_image}}
7 | 	<a href="{{url}}" class="item-image global-image global-image-orientation global-radius">
8 | 		{{>images/loop_image}}
9 | 	</a>
10 | 	{{/if}}
11 | 	<div class="item-content">
12 | 		{{^if is_special}}
13 | 		{{^if is_featured}}
14 | 		<div class="item-tags global-tags">
15 | 			{{>members/visibility_label}}{{#if tags}}
16 | 				<div class="post-tags">
17 | 					{{#foreach tags}}
18 | 						{{^has slug="rough-notes"}}
19 | 							<a href="{{url}}" class="post-tag">{{name}}</a>
20 | 						{{/has}}
21 | 					{{/foreach}}
22 | 				</div>
23 | 			{{/if}}
24 | 		</div>
25 | 		{{/if}}
26 | 		{{/if}}
27 | 		<h2 class="item-title"><a href="{{url}}">{{title}}</a></h2>
28 | 		{{^if is_special}}
29 | 		{{^if is_featured}}
30 | 		{{#has any="excerpt,custom_excerpt"}}
31 | 		{{#unless feature_image}}
32 | 		<p class="item-excerpt global-excerpt no-image">
33 | 			{{#if custom_excerpt}}{{custom_excerpt}}{{else if excerpt}}{{excerpt}}...{{/if}}
34 | 		</p>
35 | 		{{else if show_excerpt}}
36 | 		<p class="item-excerpt global-excerpt">
37 | 			{{#if custom_excerpt}}{{custom_excerpt}}{{else if excerpt}}{{excerpt}}...{{/if}}
38 | 		</p>
39 | 		{{/unless}}
40 | 		{{/has}}
41 | 		{{/if}}
42 | 		{{/if}}
43 | 		{{>meta}}
44 | 	</div>
45 | </article>
46 | {{else}}
47 | <a href="{{url}}" class="item global-image-orientation global-radius{{#if is_authors}} is-portrait{{/if}}">
48 | 	<h2 class="item-title">{{name}}</h2>
49 | 	<div class="widget-image global-image">
50 | 		{{#if other_image}}
51 | 		{{>images/other_image}}
52 | 		{{/if}}
53 | 	</div>
54 | </a>
55 | {{/if}}
```

partials/logo.hbs
```
1 | {{#match @custom.color_scheme "Dark"}}
2 | 	{{#if @custom.logo_for_dark_version}}
3 | 	{{>logo_mode is_dark=true}}
4 | 	{{else}}
5 | 	{{>logo_mode is_light=true}}
6 | 	{{/if}}
7 | {{else match @custom.color_scheme "Auto: Light/Dark"}}
8 | 	{{#if @custom.logo_for_dark_version}}
9 | 	{{>logo_mode is_dark=true is_auto=true}}
10 | 	{{/if}}
11 | 	{{>logo_mode is_light=true}}
12 | {{else match @custom.color_scheme "Auto: Sepia/Dark"}}
13 | 	{{#if @custom.logo_for_dark_version}}
14 | 	{{>logo_mode is_dark=true is_auto=true}}
15 | 	{{/if}}
16 | 	{{>logo_mode is_light=true}}
17 | {{else}}
18 | 	{{>logo_mode is_light=true}}
19 | {{/match}}
```

partials/logo_mode.hbs
```
1 | {{#if is_light}}
2 | {{#if @site.logo}}
3 | <a href="{{@site.url}}" class="is-logo"><img src="{{@site.logo}}" alt="{{@site.title}} home"></a>
4 | {{else}}
5 | <a href="{{@site.url}}" class="is-title">{{@site.title}}</a>
6 | {{/if}}
7 | {{else if is_dark}}
8 | <a href="{{@site.url}}" class="is-logo{{#if is_auto}} is-auto{{/if}}"><img src="{{@custom.logo_for_dark_version}}" alt="{{@site.title}} home"></a>
9 | {{/if}}
```

partials/loop.hbs
```
1 | <div class="loop-section global-padding">
2 | 	{{#if is_archive}}
3 | 	{{^if label}}
4 | 	<small class="global-subtitle">{{#if is_featured}}{{plural pagination.total empty=(t "No posts") singular=(t "1 featured post") plural=(t "% featured posts")}}{{else}}{{plural pagination.total empty=(t "No posts") singular=(t "1 post") plural=(t "% posts")}}{{/if}}</small>
5 | 	{{/if}}
6 | 	{{#if label}}
7 | 	<small class="global-subtitle">{{label}}</small>
8 | 	{{/if}}
9 | 	<div class="loop-wrap">
10 | 		{{#foreach posts}}
11 | 		{{>item show_excerpt=true}}
12 | 		{{/foreach}}
13 | 	</div>
14 | 	{{else}}
15 | 	{{^is "paged"}}
16 | 	<small class="global-subtitle">{{t "What’s new?"}}</small>
17 | 	<div class="loop-wrap is-top">
18 | 		{{#foreach posts to="1"}}
19 | 		{{>item show_excerpt=true show_all_option=true is_first=true is_top=true}}
20 | 		{{/foreach}}
21 | 		{{^match @custom.hero_options "Subscribe form"}}
22 | 		{{>members/subscribe_form is_box=true}}
23 | 		{{/match}}
24 | 		{{#foreach posts from="2" to="3"}}
25 | 		{{#if @site.members_enabled}}
26 | 		{{#if @member}}
27 | 		{{>item show_excerpt=true is_top=true}}
28 | 		{{else}}
29 | 		{{^match @custom.hero_options "Subscribe form"}}
30 | 		{{>item show_excerpt=false is_top=true}}
31 | 		{{else}}
32 | 		{{>item show_excerpt=true is_top=true}}
33 | 		{{/match}}
34 | 		{{/if}}
35 | 		{{else}}
36 | 		{{>item show_excerpt=true is_top=true}}
37 | 		{{/if}}
38 | 		{{/foreach}}
39 | 	</div>
40 | 	{{>featured}}
41 | 	{{#foreach posts from="3" to="4"}}
42 | 	<small class="loop-subtitle global-subtitle">{{t "Previous posts"}}</small>
43 | 	{{/foreach}}
44 | 	<div class="loop-wrap">
45 | 		{{#foreach posts from="4"}}
46 | 		{{>item show_excerpt=true}}
47 | 		{{/foreach}}
48 | 	</div>
49 | 	{{else}}
50 | 	<div class="loop-wrap">
51 | 		{{#foreach posts}}
52 | 		{{>item show_excerpt=true}}
53 | 		{{/foreach}}
54 | 	</div>
55 | 	{{/is}}
56 | 	{{/if}}
57 | </div>
```

partials/members/cta.hbs
```
1 | {{#has visibility="paid"}}
2 | <div class="members-cta global-radius">
3 | 	<h2>{{t "This post is for paying subscribers only"}}</h2>
4 | 	{{#if @member}}
5 | 	<p class="global-excerpt">{{t "Upgrade your account to read the post and get access to the full library of posts for paying subscribers only."}}</p>
6 | 	<a href="javascript:" class="global-button is-cta" data-portal="account/plans">{{t "See plans"}}</a>
7 | 	{{else}}
8 | 	<p class="global-excerpt">{{t "Sign up now and upgrade your account to read the post and get access to the full library of posts for paying subscribers only."}}</p>
9 | 	<a class="global-button is-cta" href="{{@site.url}}/signup/">{{t "Sign up now"}}</a>
10 | 	<small class="global-question is-cta"><span>{{t "Already have an account?"}}</span> <a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></small>
11 | 	{{/if}}
12 | </div>
13 | {{else has visibility="tiers"}}
14 | <div class="members-cta global-radius">
15 | 	<h2>{{plural tiers.length empty=(t "No tiers") singular=(t "This post is for subscribers with the tier:") plural=(t "This post is for subscribers with any of the tiers:")}} {{tiers lastSeparator=(t "or") suffix=""}}</h2>
16 | 	{{#if @member}}
17 | 	<p class="global-excerpt">{{t "Upgrade your account to get access to the post."}}</p>
18 | 	<a href="javascript:" class="global-button is-cta" data-portal="account/plans">{{t "See plans"}}</a>
19 | 	{{else}}
20 | 	<p class="global-excerpt">{{t "Sign up now and upgrade your account to get access to the post."}}</p>
21 | 	<a class="global-button is-cta" href="{{@site.url}}/signup/">{{t "Sign up now"}}</a>
22 | 	<small class="global-question is-cta"><span>{{t "Already have an account?"}}</span> <a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></small>
23 | 	{{/if}}
24 | </div>
25 | {{else has visibility="members"}}
26 | <div class="members-cta global-radius">
27 | 	<h2>{{t "This post is for subscribers only"}}</h2>
28 | 	<p class="global-excerpt">{{t "Sign up now to read the post and get access to the full library of posts for subscribers only."}}</p>
29 | 	<a class="global-button is-cta" href="{{@site.url}}/signup/">{{t "Sign up now"}}</a>
30 | 	<small class="global-question is-cta"><span>{{t "Already have an account?"}}</span> <a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></small>
31 | </div>
32 | {{/has}}
```

partials/members/login_panel.hbs
```
1 | {{#if @site.members_enabled}}
2 | {{#if @member}}
3 | <li class="account"><a href="{{@site.url}}/account/" class="global-button no-color">{{t "Account"}}</a></li>
4 | {{else}}
5 | <li class="signin"><a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></li>
6 | <li class="signup"><a href="{{@site.url}}{{#if @custom.slug_for_become_a_subscriber_button}}{{@custom.slug_for_become_a_subscriber_button}}{{else}}/signup/{{/if}}" class="global-button">{{t "Subscribe"}}</a></li>
7 | {{/if}}
8 | {{/if}}
```

partials/members/notifications.hbs
```
1 | <div id="notifications" class="global-notification">
2 | 	<div class="subscribe">{{t "You’ve successfully subscribed to {site-title}" site-title=@site.title}}</div>
3 | 	<div class="signin">{{t "Welcome back! You’ve successfully signed in."}}</div>
4 | 	<div class="signup">{{t "Great! You’ve successfully signed up."}}</div>
5 | 	<div class="update-email">{{t "Success! Your email is updated."}}</div>
6 | 	<div class="expired">{{t "Your link has expired"}}</div>
7 | 	{{#if @member}}
8 | 	<div class="checkout-success">{{t "Success! You now have access to additional content."}}</div>
9 | 	{{else}}
10 | 	<div class="checkout-success">{{t "Success! Check your email for magic link to sign-in."}}</div>
11 | 	{{/if}}
12 | </div>
13 | {{#contentFor "script_js"}}
14 | <script>
15 | !function(){"use strict";const p=new URLSearchParams(window.location.search),isAction=p.has("action"),isStripe=p.has("stripe"),success=p.get("success"),action=p.get("action"),stripe=p.get("stripe"),n=document.getElementById("notifications"),a="is-subscribe",b="is-signin",c="is-signup",f="is-update-email",d="is-expired",e="is-checkout-success";p&&(isAction&&(action=="subscribe"&&success=="true"&&n.classList.add(a),action=="signup-paid"&&success=="true"&&n.classList.add(a),action=="signin"&&success=="true"&&n.classList.add(b),action=="signup"&&success=="true"&&n.classList.add(c),action=="updateEmail"&&success=="true"&&n.classList.add(f),success=="false"&&n.classList.add(d)),isStripe&&stripe=="success"&&n.classList.add(e),(isAction||isStripe)&&setTimeout(function(){window.history.replaceState(null,null,window.location.pathname),n.classList.remove(a,b,c,d,e,f)},5000))}();
16 | </script>
17 | {{/contentFor}}
```

partials/members/sidebar_form.hbs
```
1 | {{>members/subscribe_form}}
```

partials/members/subscribe_form.hbs
```
1 | {{#if @site.members_enabled}}
2 | {{^if @member}}
3 | {{#if is_hero}}
4 | {{#match @custom.hero_options "Subscribe form"}}
5 | <div class="subscribe-wrap is-hero">
6 | 	<form data-members-form="subscribe" data-members-autoredirect="false">
7 | 		<input data-members-email type="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
8 | 		<button class="global-button" type="submit">{{t "Subscribe"}}</button>
9 | 	</form>
10 | 	<div class="subscribe-alert">
11 | 		<span class="alert-loading global-alert">{{t "Processing your application"}}</span>
12 | 		<span class="alert-success global-alert">{{t "Please check your inbox and click the link to confirm your subscription."}}</span>
13 | 		<span class="alert-error global-alert">{{t "There was an error sending the email"}}</span>
14 | 	</div>
15 | </div>
16 | {{/match}}
17 | {{/if}}
18 | {{#if is_box}}
19 | {{#if is_footer}}
20 | <div class="global-padding">
21 | 	<small class="subscribe-form-subtitle global-subtitle">{{t "Newsletter"}}</small>
22 | 	{{/if}}
23 | 	<div class="subscribe-form global-radius{{#if is_sticky}} is-sticky{{/if}}">
24 | 		<div class="global-dynamic-color">
25 | 			{{^if is_footer}}
26 | 			<small class="global-subtitle">{{t "Newsletter"}}</small>
27 | 			{{/if}}
28 | 			<h3 class="subscribe-title">{{#if label}}{{label}}{{else}}{{t "Want to receive my work as I publish it?"}}{{/if}}</h3>
29 | 		</div>
30 | 		<div class="subscribe-wrap">
31 | 			<form data-members-form="subscribe" data-members-autoredirect="false">
32 | 				<input data-members-email type="email" placeholder="{{t "Your email"}}" aria-label="{{t "Your email"}}" required>
33 | 				<button class="global-button no-color" type="submit">{{#if button}}{{button}}{{else}}{{t "Subscribe"}}{{/if}}</button>
34 | 			</form>
35 | 			<div class="subscribe-alert global-dynamic-color">
36 | 				<span class="alert-loading global-alert">{{t "Processing the subscription"}}</span>
37 | 				<span class="alert-success global-alert">{{t "Please check your inbox and click the link to confirm your subscription."}}</span>
38 | 				<span class="alert-error global-alert">{{t "There was an error sending the email"}}</span>
39 | 			</div>
40 | 		</div>
41 | 	</div>
42 | 	{{#if is_footer}}
43 | </div>
44 | {{/if}}
45 | {{/if}}
46 | {{#if is_button}}
47 | <div class="footer-subscribe">
48 | 	<a href="{{@site.url}}{{#if @custom.slug_for_become_a_subscriber_button}}{{@custom.slug_for_become_a_subscriber_button}}{{else}}/signup/{{/if}}" class="global-button">{{t "Invite me to your inbox →"}}</a>
49 | 	<small>{{t "Want to stay up to date?"}}</small>
50 | </div>
51 | {{/if}}
52 | {{/if}}
53 | {{/if}}
```

partials/members/tiers.hbs
```
1 | <div class="membership-section global-padding">
2 | 	<small class="global-subtitle">{{t "See pricing plans"}}</small>
3 | 	<div class="membership-wrap global-radius">
4 | 		{{>images/background_cover custom_cover=feature_image is_membership=true}}
5 | 		{{#if @site.paid_members_enabled}}
6 | 		<div class="membership-switch" data-active-price="{{@site.portal_default_plan}}" data-active-price-plans="{{@site.portal_plans}}"{{#get "tiers" limit="all" filter="visibility:public+type:paid" as |public_paid_tiers|}} data-active-public-paid-tiers="{{#if public_paid_tiers}}true{{else}}false{{/if}}"{{/get}}>
7 | 			<button data-price="monthly">{{t "Monthly"}}</button>
8 | 			<button data-price="yearly">{{t "Yearly"}}</button>
9 | 		</div>
10 | 		{{/if}}
11 | 		<div class="membership-cards">
12 | 			{{^if @member}}
13 | 			{{#if membership_page}}
14 | 			{{#get "tiers" filter="visibility:public+type:free" include="benefits"}}
15 | 			{{#foreach tiers}}
16 | 			<div class="membership-card global-radius">
17 | 				<div class="membership-card-content">
18 | 					<small>{{name}}</small>
19 | 					<h2 class="membership-card-price"><sup>{{t "$"}}</sup>0</h2>
20 | 					{{#if description}}<p class="membership-card-excerpt global-excerpt">{{description}}</p>{{/if}}
21 | 					{{#if benefits}}
22 | 					<div class="membership-card-list">
23 | 						<ul>
24 | 							{{#foreach benefits as |benefit|}}
25 | 							<li>{{benefit}}</li>
26 | 							{{/foreach}}
27 | 						</ul>
28 | 					</div>
29 | 					{{/if}}
30 | 				</div>
31 | 				<a href="{{@site.url}}/signup/" class="membership-button global-button">{{t "Sign up for free"}}</a>
32 | 			</div>
33 | 			{{/foreach}}
34 | 			{{/get}}
35 | 			{{/if}}
36 | 			{{/if}}
37 | 			{{#if @site.paid_members_enabled}}
38 | 			{{#get "tiers" limit="all" filter="visibility:public+type:paid" include="monthly_price,yearly_price,benefits"}}
39 | 			{{#foreach tiers}}
40 | 			<div class="membership-card global-radius">
41 | 				<div class="membership-card-content">
42 | 					<small>{{name}}</small>
43 | 					<h2 class="membership-card-price" data-monthly>{{#if monthly_price}}<sup>{{price currency=currency}}</sup>{{price monthly_price}}{{else}}<sup>{{t "$"}}</sup>0{{/if}}<span>/{{t "month"}}</span></h2>
44 | 					<h2 class="membership-card-price" data-yearly>{{#if yearly_price}}<sup>{{price currency=currency}}</sup>{{price yearly_price}}{{else}}<sup>{{t "$"}}</sup>0{{/if}}<span>/{{t "year"}}</span></h2>
45 | 					{{#if description}}<p class="membership-card-excerpt global-excerpt">{{description}}</p>{{/if}}
46 | 					{{#if benefits}}
47 | 					<div class="membership-card-list">
48 | 						<ul>
49 | 							{{#foreach benefits as |benefit|}}
50 | 							<li>{{benefit}}</li>
51 | 							{{/foreach}}
52 | 						</ul>
53 | 					</div>
54 | 					{{/if}}
55 | 				</div>
56 | 				<a href="javascript:" data-portal="signup/{{id}}/monthly" class="membership-button global-button" data-monthly>{{#if trial_days}}{{t "Start {trial}-day free trial" trial=trial_days}}{{else}}{{t "Sign up now"}}{{/if}}</a>
57 | 				<a href="javascript:" data-portal="signup/{{id}}/yearly" class="membership-button global-button" data-yearly>{{#if trial_days}}{{t "Start {trial}-day free trial" trial=trial_days}}{{else}}{{t "Sign up now"}}{{/if}}</a>
58 | 			</div>
59 | 			{{/foreach}}
60 | 			{{/get}}
61 | 			{{/if}}
62 | 		</div>
63 | 	</div>
64 | 	{{^if @member}}
65 | 	{{#if membership_page}}
66 | 	<small class="global-question"><span>{{t "Already have an account?"}}</span> <a href="{{@site.url}}/signin/">{{t "Sign in"}}</a></small>
67 | 	{{/if}}
68 | 	{{/if}}
69 | </div>
70 | {{#contentFor "script_js"}}
71 | <script>
72 | !function(){const c=document.querySelector(".membership-switch"),t=document.querySelectorAll(".membership-switch button");c&&t.forEach(e=>{e.addEventListener("click",t=>{c.setAttribute("data-active-price",e.getAttribute("data-price"))})})}();
73 | </script>
74 | {{/contentFor}}
```

partials/members/visibility_label.hbs
```
1 | {{^has visibility="public"}}
2 | <small class="global-dynamic-color">{{#has visibility="paid"}}{{t "Paid-members"}}{{else has visibility="tiers"}}{{tiers lastSeparator=", " suffix=""}}{{else has visibility="members"}}{{t "Members"}}{{/has}}</small>
3 | {{/has}}
```

partials/meta.hbs
```
1 | {{#if show_all_option}}
2 | <div class="global-meta is-full-meta{{#is "post"}} is-post{{/is}}">
3 | 	{{#if @custom.show_author}}
4 | 	<div class="global-meta-wrap">
5 | 		<div>
6 | 			{{#foreach authors}}
7 | 			<a href="{{url}}" class="global-meta-avatar{{#if profile_image}} is-image global-image{{/if}}">
8 | 				{{#if profile_image}}
9 | 				{{>images/other_image other_image=profile_image alt=name lazy=true}}
10 | 				{{else}}
11 | 				<span>{{name}}</span>
12 | 				{{/if}}
13 | 			</a>
14 | 			{{/foreach}}
15 | 		</div>
16 | 	</div>
17 | 	{{/if}}
18 | 	<div class="global-meta-content">
19 | 		{{#if @custom.show_author}}
20 | 		<div>
21 | 			{{t "by"}}
22 | 			{{#has author="count:1"}}
23 | 			{{authors}}
24 | 			{{else has author="count:2"}}
25 | 			{{authors separator=(t "&")}}
26 | 			{{else has author="count:3"}}
27 | 			{{authors to="2"}}{{t "and"}}{{authors from="3"}}
28 | 			{{else has author="count:>3"}}
29 | 			{{authors}}
30 | 			{{/has}}
31 | 		</div>
32 | 		{{/if}}
33 | 		{{#is "post"}}
34 | 		<time datetime="{{date format="YYYY-MM-DD"}}"><span>{{date published_at format="LL"}} ∙ </span>{{reading_time minute=(t "1 minute read") minutes=(t "% minutes read")}}</time>
35 | 		{{else}}
36 | 		{{#if @custom.show_author}}
37 | 		<time datetime="{{date format="YYYY-MM-DD"}}"><span>{{date published_at format="LL"}} ∙ </span>{{reading_time minute=(t "1 minute read") minutes=(t "% minutes read")}}</time>
38 | 		{{/if}}
39 | 		{{/is}}
40 | 	</div>
41 | </div>
42 | {{else}}
43 | {{#if @custom.show_author}}
44 | <div class="global-meta">
45 | 	<div class="global-meta-content">
46 | 		{{t "by"}}
47 | 		{{#has author="count:1"}}
48 | 		{{authors}}
49 | 		{{else has author="count:2"}}
50 | 		{{authors separator=(t "&")}}
51 | 		{{else has author="count:>2"}}
52 | 		{{authors limit="1"}}
53 | 		{{t "and others"}}
54 | 		{{/has}}
55 | 	</div>
56 | </div>
57 | {{/if}}
58 | {{/if}}
```

partials/navigation.hbs
```
1 | {{! Header navigation }}
2 | 
3 | {{^if isSecondary}}
4 | <ul>
5 | 	{{#foreach navigation to="5"}}
6 | 	<li><a href="{{url absolute="true"}}"{{#if current}} class="is-active"{{/if}}>{{label}}</a></li>
7 | 	{{/foreach}}
8 | 	{{#foreach navigation from="6"}}
9 | 	{{#if @first}}
10 | 	<li class="is-dropdown">
11 | 		<span>{{>icons/site/dots}}</span>
12 | 		<ul>
13 | 			{{/if}}
14 | 			<li><a href="{{url absolute="true"}}"{{#if current}} class="is-active"{{/if}}>{{label}}</a></li>
15 | 			{{#if @last}}
16 | 		</ul>
17 | 	</li>
18 | 	{{/if}}
19 | 	{{/foreach}}
20 | </ul>
21 | <ul>
22 | 	{{>search is_desktop=true}}
23 | 	{{>members/login_panel}}
24 | </ul>
25 | {{else}}
26 | 
27 | 
28 | {{! Footer navigation }}
29 | 
30 | 
31 | {{#foreach navigation limit="4"}}
32 | {{#if @first}}
33 | <div class="footer-nav-column">
34 | 	<small>{{t "Column 1"}}</small>
35 | 	<ul>
36 | 		{{/if}}
37 | 		<li><a href="{{url absolute="true"}}">{{label}}</a></li>
38 | 		{{#if @last}}
39 | 	</ul>
40 | </div>
41 | {{/if}}
42 | {{/foreach}}
43 | 
44 | {{#foreach navigation limit="4" from="5"}}
45 | {{#if @first}}
46 | <div class="footer-nav-column">
47 | 	<small>{{t "Column 2"}}</small>
48 | 	<ul>
49 | 		{{/if}}
50 | 		<li><a href="{{url absolute="true"}}">{{label}}</a></li>
51 | 		{{#if @last}}
52 | 	</ul>
53 | </div>
54 | {{/if}}
55 | {{/foreach}}
56 | 
57 | {{#foreach navigation limit="4" from="9"}}
58 | {{#if @first}}
59 | <div class="footer-nav-column">
60 | 	<small>{{t "Column 3"}}</small>
61 | 	<ul>
62 | 		{{/if}}
63 | 		<li><a href="{{url absolute="true"}}">{{label}}</a></li>
64 | 		{{#if @last}}
65 | 	</ul>
66 | </div>
67 | {{/if}}
68 | {{/foreach}}
69 | 
70 | {{#foreach navigation limit="4" from="13"}}
71 | {{#if @first}}
72 | <div class="footer-nav-column">
73 | 	<small>{{t "Column 4"}}</small>
74 | 	<ul>
75 | 		{{/if}}
76 | 		<li><a href="{{url absolute="true"}}">{{label}}</a></li>
77 | 		{{#if @last}}
78 | 	</ul>
79 | </div>
80 | {{/if}}
81 | {{/foreach}}
82 | 
83 | {{#foreach navigation from="17"}}
84 | {{#if @first}}
85 | <div class="footer-nav-column">
86 | 	<small>{{t "Column 5"}}</small>
87 | 	<ul>
88 | 		{{/if}}
89 | 		<li><a href="{{url absolute="true"}}">{{label}}</a></li>
90 | 		{{#if @last}}
91 | 	</ul>
92 | </div>
93 | {{/if}}
94 | {{/foreach}}
95 | {{/if}}
```

partials/pagination.hbs
```
1 | {{#if next}}
2 | <div class="pagination-section">
3 | 	<a href="{{page_url next}}" aria-label="Load more"></a>
4 | 	<button class="global-button">{{t "Load more"}}</button>
5 | </div>
6 | {{/if}}
```

partials/posts/comments.hbs
```
1 | {{#if comments}}
2 | <div class="comments-section global-padding">
3 | 	<div class="comments-wrap global-radius">
4 | 		<div class="comments-content">
5 | 			<div class="comments-header">
6 | 				<h3>{{t "Member discussion"}}</h3>
7 | 				{{comment_count empty=(t "0 comments") singular=(t "comment") plural=(t "comments") autowrap="span"}}
8 | 			</div>
9 | 			{{comments title="" count=false mode="auto"}}
10 | 		</div>
11 | 	</div>
12 | </div>
13 | {{/if}}
```

partials/posts/header.hbs
```
1 | <div class="post-header">
2 | 	<div class="post-header-wrap global-padding{{#if is_custom}} is-center{{/if}}{{#if custom_image}} is-archive-image{{/if}}">
3 | 		<div class="post-header-content">
4 | 			{{^if is_custom}}
5 | 			{{^has visibility="public"}}<div class="post-tags global-tags">{{>members/visibility_label}}</div>{{/has}}
6 | 			{{/if}}
7 | 			{{#if custom_image}}
8 | 			<div class="archive-image global-image">
9 | 				{{>images/other_image other_image=custom_image alt=name}}
10 | 			</div>
11 | 			{{/if}}
12 | 			<h1 class="post-title global-title">{{title}}</h1>
13 | 			{{#if archive_page}}
14 | 			{{#has any="location,website,facebook,twitter"}}
15 | 			<div class="archive-social">
16 | 				{{#if location}}
17 | 				<span>{{>icons/site/pin}}{{location}}</span>
18 | 				{{/if}}
19 | 				{{#if website}}
20 | 				<a href="{{website}}" target="_blank" rel="noopener">{{>icons/site/link}}{{t "Website"}}</a>
21 | 				{{/if}}
22 | 				{{#if facebook}}
23 | 				<a href="{{facebook_url}}" target="_blank" rel="noopener">{{>icons/social/facebook}}Facebook</a>
24 | 				{{/if}}
25 | 				{{#if twitter}}
26 | 				<a href="{{twitter_url}}" target="_blank" rel="noopener">{{>icons/social/x}}X/Twitter</a>
27 | 				{{/if}}
28 | 			</div>
29 | 			{{/has}}
30 | 			{{/if}}
31 | 			{{#if custom_excerpt}}
32 | 			<p class="post-excerpt global-excerpt">{{custom_excerpt}}</p>
33 | 			{{else if featured_page}}
34 | 			<p class="post-excerpt global-excerpt">{{t "A curated list of the most interesting thoughts, stories and ideas"}}</p>
35 | 			{{else if membership_page}}
36 | 			<p class="post-excerpt global-excerpt">{{t "Unlock full access to {site-title} and see the entire library of subscribers-only content & updates" site-title=@site.title}}</p>
37 | 			{{/if}}
38 | 			{{#if tags}}<div class="post-tags global-tags">{{tags limit="all" separator=""}}</div>{{/if}}
39 | 			{{^if archive_page}}
40 | 			{{^is "page"}}
41 | 			<div class="post-meta-wrap">
42 | 				{{>meta show_all_option=true}}
43 | 				{{>posts/share is_header=true}}
44 | 			</div>
45 | 			{{/is}}
46 | 			{{/if}}
47 | 		</div>
48 | 		{{^if is_custom}}
49 | 		{{^match @custom.feature_image_orientation "Disable"}}
50 | 		{{#if feature_image}}
51 | 		<div class="post-header-image{{#match @custom.feature_image_orientation "Landscape wide"}} is-wide{{else match @custom.feature_image_orientation "Natural wide"}} is-wide{{else match @custom.feature_image_orientation "Panoramic wide"}} is-wide{{/match}}">
52 | 			<figure>
53 | 				<div class="global-image global-image-orientation global-radius{{#match @custom.feature_image_orientation "Natural"}} is-natural{{else match @custom.feature_image_orientation "Panoramic"}} is-panoramic{{/match}}{{#match @custom.feature_image_orientation "Natural wide"}} is-natural{{else match @custom.feature_image_orientation "Panoramic wide"}} is-panoramic{{/match}}">
54 | 				{{>images/post_image}}
55 | 				</div>
56 | 				{{#if feature_image_caption}}
57 | 				<figcaption>{{feature_image_caption}}</figcaption>
58 | 				{{/if}}
59 | 			</figure>
60 | 		</div>
61 | 		{{/if}}
62 | 		{{/match}}
63 | 		{{/if}}
64 | 	</div>
65 | </div>
```

partials/posts/navigation.hbs
```
1 | <aside class="navigation-section global-padding">
2 | 	<div class="navigation-wrap">
3 | 		{{#next_post}}
4 | 		<a href="{{url}}" class="navigation-next">
5 | 			<small class="global-subtitle">{{t "Newer post"}}</small>
6 | 			<div>
7 | 				{{#if feature_image}}
8 | 				<div class="navigation-image global-image-orientation global-image global-radius is-square">
9 | 					{{>images/other_image other_image=feature_image alt="" lazy=true}}
10 | 				</div>
11 | 				{{/if}}
12 | 				<div class="navigation-title">
13 | 					<div><h3>{{title}}</h3></div>
14 | 				</div>
15 | 			</div>
16 | 		</a>
17 | 		{{/next_post}}
18 | 		{{#prev_post}}
19 | 		<a href="{{url}}" class="navigation-prev">
20 | 			<small class="global-subtitle">{{t "Older post"}}</small>
21 | 			<div>
22 | 				<div class="navigation-title">
23 | 					<div><h3>{{title}}</h3></div>
24 | 				</div>
25 | 				{{#if feature_image}}
26 | 				<div class="navigation-image global-image-orientation global-image global-radius is-square">
27 | 					{{>images/other_image other_image=feature_image alt="" lazy=true}}
28 | 				</div>
29 | 				{{/if}}
30 | 			</div>
31 | 		</a>
32 | 		{{/prev_post}}
33 | 	</div>
34 | </aside>
```

partials/posts/share.hbs
```
1 | {{^if is_header}}
2 | <div class="post-share">
3 | 	{{/if}}
4 | 	<div class="post-share-wrap">
5 | 		<a href="https://x.com/intent/tweet?text={{encode title}}&amp;url={{url absolute="true"}}" target="_blank" rel="noopener" aria-label="Share on X">{{>icons/social/x}}</a>
6 | 		<a href="https://www.facebook.com/sharer/sharer.php?u={{url absolute="true"}}" target="_blank" rel="noopener" aria-label="Share on Facebook">{{>icons/social/facebook}}</a>
7 | 		<a href="https://www.linkedin.com/shareArticle?mini=true&amp;title={{encode title}}&amp;url={{url absolute="true"}}" target="_blank" rel="noopener" aria-label="Share on Linkedin">{{>icons/social/linkedin}}</a>
8 | 		{{^if is_header}}
9 | 		<a href="javascript:" class="post-share-link" id="copy" data-clipboard-target="#copy-link" aria-label="Copy link">{{>icons/site/copy}}</a>
10 | 		<small class="share-link-info global-alert">{{t "The link has been copied!"}}</small>
11 | 		{{/if}}
12 | 	</div>
13 | 	{{^if is_header}}
14 | 	<input type="text" value="{{url absolute="true"}}" id="copy-link" aria-label="Copy link input">
15 | </div>
16 | {{/if}}
```

partials/posts/sidebar.hbs
```
1 | {{#if feature_image}}
2 | {{#if @custom.show_author}}
3 | {{^match @custom.feature_image_orientation "Disable"}}
4 | <div class="is-authors">
5 | 	<small class="global-subtitle">{{t "Written by"}}</small>
6 | 	{{#foreach authors}}
7 | 	<a href="{{url}}"{{^if bio}} class="no-bio"{{/if}}>
8 | 		{{#if profile_image}}
9 | 		{{>images/other_image other_image=profile_image alt="" lazy=true}}
10 | 		{{/if}}
11 | 		<div>
12 | 			<h3 class="post-sidebar-title">{{name}}</h3>
13 | 			{{#if bio}}<p>{{bio}}</p>{{/if}}
14 | 		</div>
15 | 	</a>
16 | 	{{/foreach}}
17 | </div>
18 | {{/match}}
19 | {{/if}}
20 | {{/if}}
21 | {{#get "posts" limit="3" filter="id:-{{id}}+featured:true+feature_image:-null" as |featured|}}
22 | {{#if featured}}
23 | <div class="is-featured">
24 | 	<small class="global-subtitle">{{t "Editor’s Choice"}}</small>
25 | 	{{#foreach featured}}
26 | 	<a href="{{url}}">
27 | 		{{#if feature_image}}
28 | 		{{>images/other_image other_image=feature_image alt="" lazy=true}}
29 | 		{{/if}}
30 | 		<div>
31 | 			<h3 class="post-sidebar-title">{{title}}</h3>
32 | 		</div>
33 | 	</a>
34 | 	{{/foreach}}
35 | </div>
36 | {{/if}}
37 | {{/get}}
```

partials/related.hbs
```
1 | <div class="special-section global-padding">
2 | 	<small class="global-subtitle">{{label}}</small>
3 | 	<div class="special-wrap">
4 | 		{{#foreach posts}}
5 | 		{{>item is_special=true}}
6 | 		{{/foreach}}
7 | 	</div>
8 | </div>
```

partials/search.hbs
```
1 | {{#if @custom.content_api_key_for_search}}
2 | {{#if is_search_core}}
3 | <div class="search-section">
4 | 	<div class="search-wrap">
5 | 		<div class="search-content global-radius">
6 | 			<form class="search-form" onsubmit="return false">
7 | 				<input class="search-input" type="text" placeholder="{{t "Search"}}">
8 | 				<div class="search-meta">
9 | 					<span class="search-info">{{t "Please enter at least 3 characters"}}</span>
10 | 					<span class="search-counter is-hide">
11 | 						{{{t "{counter} results for your search" counter="<span>0</span>"}}}
12 | 					</span>
13 | 				</div>
14 | 				<span class="search-close">{{>icons/site/close}}</span>
15 | 			</form>
16 | 			<div class="search-results global-image"></div>
17 | 		</div>
18 | 	</div>
19 | 	<div class="search-overlay"></div>
20 | </div>
21 | {{#contentFor "script_js"}}
22 | <script>
23 | const options = {
24 | 	api:'{{@site.url}}/ghost/api/content/posts/?key='+"{{@custom.content_api_key_for_search}}"+'&limit=all&fields=url,title,feature_image,published_at,custom_excerpt,visibility,html',
25 | 	threshold: 0.1,
26 | 	ignoreLocation: true,
27 | 	keys: ['title','custom_excerpt','html'],
28 | 	images: true,
29 | 	limit: 30
30 | }
31 | </script>
32 | {{/contentFor}}
33 | {{/if}}
34 | {{/if}}
35 | {{#if is_mobile}}
36 | <span class="header-search search-open is-mobile"{{^if @custom.content_api_key_for_search}} data-ghost-search{{/if}}>{{>icons/site/search}}</span>
37 | {{else if is_desktop}}
38 | <li class="header-search search-open is-desktop"{{^if @custom.content_api_key_for_search}} data-ghost-search{{/if}}>{{>icons/site/search}}</li>
39 | {{/if}}
40 | {{#if is_hero}}
41 | {{#match @custom.hero_options "Search box (Flat style)"}}
42 | <div class="hero-search is-flat{{#if @custom.content_api_key_for_search}} search-open"{{else}}" data-ghost-search{{/if}}>
43 | 	<span>{{#if @custom.content_api_key_for_search}}{{t "Search for essays"}}{{else}}{{t "Search for essays, rough notes, and more"}}{{/if}}</span><span class="global-dynamic-color">{{>icons/site/search}}</span>
44 | </div>
45 | {{else match @custom.hero_options "Search box (Shadow style)"}}
46 | <div class="hero-search is-shadow{{#if @custom.content_api_key_for_search}} search-open"{{else}}" data-ghost-search{{/if}}>
47 | 	<span>{{#if @custom.content_api_key_for_search}}{{t "Search for essays"}}{{else}}{{t "Search for essays, rough notes"}}{{/if}}</span><span class="global-dynamic-color">{{>icons/site/search}}</span>
48 | </div>
49 | {{else match @custom.hero_options "Search box (Linear style)"}}
50 | <div class="hero-search is-linear{{#if @custom.content_api_key_for_search}} search-open"{{else}}" data-ghost-search{{/if}}>
51 | 	<span>{{#if @custom.content_api_key_for_search}}{{t "Search for essays"}}{{else}}{{t "Search for essays, rough notes"}}{{/if}}</span><span class="global-dynamic-color">{{>icons/site/search}}</span>
52 | </div>
53 | {{/match}}
54 | {{/if}}
```

partials/sections.hbs
```
1 | {{#match @custom.tags_for_special_section}}
2 | {{#get "posts" limit="5" filter="tag:[{{@custom.tags_for_special_section}}]" include="authors" as |special_posts|}}
3 | 	{{#if special_posts}}
4 | 		{{>related label=(t "Rough Notes")}}
5 | 	{{/if}}
6 | {{/get}}
7 | {{else}}
8 | {{#foreach posts limit="1"}}
9 | {{#if primary_tag}}
10 | {{#get "posts" limit="5" filter="tag:{{primary_tag.slug}}+id:-{{id}}" include="authors" as |special_posts|}}
11 | 	{{#if special_posts}}
12 | 		{{>related label=(t "Rough Notes")}}
13 | 	{{/if}}
14 | {{/get}}
15 | {{/if}}
16 | {{/foreach}}
17 | {{/match}}
```

partials/services/google_fonts.hbs
```
1 | {{#match @custom.fonts "Archivo + System fonts"}} 
2 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
3 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
4 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Archivo:ital,wght@0,300;0,800;1,300;1,800&display=swap">
5 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Archivo:ital,wght@0,300;0,800;1,300;1,800&display=swap">
6 | {{#contentFor "fonts_css"}}
7 | <style>
8 | :root {
9 | 	--font-family-one: 'Archivo', sans-serif;
10 | 	--font-weight-one-light: 300;
11 | 	--font-weight-one-bold: 800;
12 | 
13 | 	--font-family-two: 'Archivo', sans-serif;
14 | 	--font-weight-two-bold: 800;
15 | }
16 | </style>
17 | {{/contentFor}}
18 | {{/match}}
19 | 
20 | {{#match @custom.fonts "Figtree + Inter"}}
21 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
22 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
23 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Figtree:wght@300;700&family=Inter:wght@400;500;700&display=swap">
24 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Figtree:wght@300;700&family=Inter:wght@400;500;700&display=swap">
25 | {{#contentFor "fonts_css"}}
26 | <style>
27 | :root {
28 | 	--font-family-one: 'Figtree', sans-serif;
29 | 	--font-weight-one-light: 300;
30 | 	--font-weight-one-bold: 700;
31 | 
32 | 	--font-family-two: 'Figtree', sans-serif;
33 | 	--font-weight-two-bold: 700;
34 | 
35 | 	--font-family-three: 'Inter', sans-serif;
36 | 	--font-weight-three-regular: 400;
37 | 	--font-weight-three-medium: 500;
38 | 	--font-weight-three-bold: 700;
39 | 
40 | 	--letter-spacing: -.01em;
41 | }
42 | </style>
43 | {{/contentFor}}
44 | {{/match}}
45 | 
46 | {{#match @custom.fonts "Fraunces + System fonts"}} 
47 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
48 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
49 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,350;0,9..144,680;1,9..144,350;1,9..144,680&display=swap">
50 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,350;0,9..144,680;1,9..144,350;1,9..144,680&display=swap">
51 | {{#contentFor "fonts_css"}}
52 | <style>
53 | :root {
54 | 	--font-family-one: 'Fraunces', serif;
55 | 	--font-weight-one-light: 350;
56 | 	--font-weight-one-bold: 680;
57 | }
58 | </style>
59 | {{/contentFor}}
60 | {{/match}}
61 | 
62 | {{#match @custom.fonts "IBM Plex Sans"}}
63 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
64 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
65 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap">
66 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap">
67 | {{#contentFor "fonts_css"}}
68 | <style>
69 | :root {
70 | 	--font-family-one: 'IBM Plex Sans', sans-serif;
71 | 	--font-weight-one-light: 400;
72 | 	--font-weight-one-bold: 700;
73 | 
74 | 	--font-family-two: 'IBM Plex Sans', sans-serif;
75 | 	--font-weight-two-bold: 700;
76 | 
77 | 	--font-family-three: 'IBM Plex Sans', sans-serif;
78 | 	--font-weight-three-regular: 400;
79 | 	--font-weight-three-medium: 500;
80 | 	--font-weight-three-bold: 700;
81 | }
82 | </style>
83 | {{/contentFor}}
84 | {{/match}}
85 | 
86 | {{#match @custom.fonts "Inter"}} 
87 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
88 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
89 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;700&display=swap">
90 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;700&display=swap">
91 | {{#contentFor "fonts_css"}}
92 | <style>
93 | :root {
94 | 	--font-family-one: 'Inter', sans-serif;
95 | 	--font-weight-one-light: 300;
96 | 	--font-weight-one-bold: 700;
97 | 
98 | 	--font-family-two: 'Inter', sans-serif;
99 | 	--font-weight-two-bold: 700;
100 | 
101 | 	--font-family-three: 'Inter', sans-serif;
102 | 	--font-weight-three-regular: 400;
103 | 	--font-weight-three-medium: 500;
104 | 	--font-weight-three-bold: 700;
105 | 
106 | 	--letter-spacing: -.01em;
107 | }
108 | </style>
109 | {{/contentFor}}
110 | {{/match}}
111 | 
112 | {{#match @custom.fonts "Libre Franklin + System fonts"}}
113 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
114 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
115 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Libre+Franklin:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">
116 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Libre+Franklin:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">
117 | {{#contentFor "fonts_css"}}
118 | <style>
119 | :root {
120 | 	--font-family-one: 'Libre Franklin', sans-serif;
121 | 	--font-weight-one-light: 400;
122 | 	--font-weight-one-bold: 700;
123 | 
124 | 	--font-family-two: 'Libre Franklin', sans-serif;
125 | 	--font-weight-two-bold: 700;
126 | }
127 | </style>
128 | {{/contentFor}}
129 | {{/match}}
130 | 
131 | {{#match @custom.fonts "Livvic + System fonts"}}
132 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
133 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
134 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Livvic:ital,wght@0,400;0,700;1,400;1,700&display=swap">
135 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Livvic:ital,wght@0,400;0,700;1,400;1,700&display=swap">
136 | {{#contentFor "fonts_css"}}
137 | <style>
138 | :root {
139 | 	--font-family-one: 'Livvic', sans-serif;
140 | 	--font-weight-one-light: 400;
141 | 	--font-weight-one-bold: 700;
142 | 
143 | 	--font-family-two: 'Livvic', sans-serif;
144 | 	--font-weight-two-bold: 700;
145 | }
146 | </style>
147 | {{/contentFor}}
148 | {{/match}}
149 | 
150 | {{#match @custom.fonts "Lora + System fonts"}} 
151 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
152 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
153 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,700;1,400;1,700&display=swap">
154 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,700;1,400;1,700&display=swap">
155 | {{#contentFor "fonts_css"}}
156 | <style>
157 | :root {
158 | 	--font-family-one: 'Lora', serif;
159 | 	--font-weight-one-light: 400;
160 | 	--font-weight-one-bold: 700;
161 | 
162 | 	--font-family-two: 'Lora', serif;
163 | 	--font-weight-two-bold: 700;
164 | }
165 | </style>
166 | {{/contentFor}}
167 | {{/match}}
168 | 
169 | {{#match @custom.fonts "Manrope + System fonts"}}
170 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
171 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
172 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;800&display=swap" rel="stylesheet">
173 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;800&display=swap" rel="stylesheet">
174 | {{#contentFor "fonts_css"}}
175 | <style>
176 | :root {
177 | 	--font-family-one: 'Manrope', sans-serif;
178 | 	--font-weight-one-light: 400;
179 | 	--font-weight-one-bold: 800;
180 | 
181 | 	--font-family-two: 'Manrope', sans-serif;
182 | 	--font-weight-two-bold: 800;
183 | }
184 | </style>
185 | {{/contentFor}}
186 | {{/match}}
187 | 
188 | {{#match @custom.fonts "Nunito"}} 
189 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
190 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
191 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,400;0,600;0,900;1,400;1,600;1,900&display=swap">
192 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,400;0,600;0,900;1,400;1,600;1,900&display=swap">
193 | {{#contentFor "fonts_css"}}
194 | <style>
195 | :root {
196 | 	--font-family-one: 'Nunito', sans-serif;
197 | 	--font-weight-one-light: 400;
198 | 	--font-weight-one-bold: 900;
199 | 
200 | 	--font-family-two: 'Nunito', sans-serif;
201 | 	--font-weight-two-bold: 900;
202 | 
203 | 	--font-family-three: 'Nunito', sans-serif;
204 | 	--font-weight-three-regular: 400;
205 | 	--font-weight-three-medium: 600;
206 | 	--font-weight-three-bold: 900;
207 | }
208 | </style>
209 | {{/contentFor}}
210 | {{/match}}
211 | 
212 | {{#match @custom.fonts "Nunito Sans"}} 
213 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
214 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
215 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Nunito+Sans:ital,wght@0,400;0,600;0,800;1,400;1,600;1,800&display=swap">
216 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Nunito+Sans:ital,wght@0,400;0,600;0,800;1,400;1,600;1,800&display=swap">
217 | {{#contentFor "fonts_css"}}
218 | <style>
219 | :root {
220 | 	--font-family-one: 'Nunito Sans', sans-serif;
221 | 	--font-weight-one-light: 400;
222 | 	--font-weight-one-bold: 800;
223 | 
224 | 	--font-family-two: 'Nunito Sans', sans-serif;
225 | 	--font-weight-two-bold: 800;
226 | 
227 | 	--font-family-three: 'Nunito Sans', sans-serif;
228 | 	--font-weight-three-regular: 400;
229 | 	--font-weight-three-medium: 600;
230 | 	--font-weight-three-bold: 800;
231 | }
232 | </style>
233 | {{/contentFor}}
234 | {{/match}}
235 | 
236 | {{#match @custom.fonts "Oswald + Roboto"}} 
237 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
238 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
239 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Oswald:wght@300;700&family=Roboto:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap">
240 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Oswald:wght@300;700&family=Roboto:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap">
241 | {{#contentFor "fonts_css"}}
242 | <style>
243 | :root {
244 | 	--font-family-one: 'Oswald', sans-serif;
245 | 	--font-weight-one-light: 300;
246 | 	--font-weight-one-bold: 700;
247 | 
248 | 	--font-family-two: 'Oswald', sans-serif;
249 | 	--font-weight-two-bold: 700;
250 | 
251 | 	--font-family-three: 'Roboto', sans-serif;
252 | 	--font-weight-three-regular: 400;
253 | 	--font-weight-three-medium: 500;
254 | 	--font-weight-three-bold: 700;
255 | }
256 | </style>
257 | {{/contentFor}}
258 | {{/match}}
259 | 
260 | {{#match @custom.fonts "Playfair + System fonts"}} 
261 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
262 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
263 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,900;1,400;1,900&display=swap">
264 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,900;1,400;1,900&display=swap">
265 | {{#contentFor "fonts_css"}}
266 | <style>
267 | :root {
268 | 	--font-family-one: 'Playfair Display', serif;
269 | 	--font-weight-one-light: 400;
270 | 	--font-weight-one-bold: 900;
271 | }
272 | </style>
273 | {{/contentFor}}
274 | {{/match}}
275 | 
276 | {{#match @custom.fonts "Poppins + Inter"}} 
277 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
278 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
279 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,400;0,700;1,400;1,700&family=Inter:wght@400;500;700&display=swap">
280 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,400;0,700;1,400;1,700&family=Inter:wght@400;500;700&display=swap">
281 | {{#contentFor "fonts_css"}}
282 | <style>
283 | :root {
284 | 	--font-family-one: 'Poppins', sans-serif;
285 | 	--font-weight-one-light: 400;
286 | 	--font-weight-one-bold: 700;
287 | 
288 | 	--font-family-two: 'Poppins', sans-serif;
289 | 	--font-weight-two-bold: 700;
290 | 
291 | 	--font-family-three: 'Inter', sans-serif;
292 | 	--font-weight-three-regular: 400;
293 | 	--font-weight-three-medium: 500;
294 | 	--font-weight-three-bold: 700;
295 | 
296 | 	--letter-spacing: -.01em;
297 | }
298 | </style>
299 | {{/contentFor}}
300 | {{/match}}
301 | 
302 | {{#match @custom.fonts "Radio Canada + System fonts"}}
303 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
304 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
305 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Radio+Canada:ital,wght@0,400;0,700;1,400;1,700&display=swap">
306 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Radio+Canada:ital,wght@0,400;0,700;1,400;1,700&display=swap">
307 | {{#contentFor "fonts_css"}}
308 | <style>
309 | :root {
310 | 	--font-family-one: 'Radio Canada', sans-serif;
311 | 	--font-weight-one-light: 400;
312 | 	--font-weight-one-bold: 700;
313 | 
314 | 	--font-family-two: 'Radio Canada', sans-serif;
315 | 	--font-weight-two-bold: 700;
316 | }
317 | </style>
318 | {{/contentFor}}
319 | {{/match}}
320 | 
321 | {{#match @custom.fonts "Readex Pro + System fonts"}}
322 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
323 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
324 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Readex+Pro:wght@300;700&display=swap">
325 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Readex+Pro:wght@300;700&display=swap">
326 | {{#contentFor "fonts_css"}}
327 | <style>
328 | :root {
329 | 	--font-family-one: 'Readex Pro', sans-serif;
330 | 	--font-weight-one-light: 300;
331 | 	--font-weight-one-bold: 700;
332 | 
333 | 	--font-family-two: 'Readex Pro', sans-serif;
334 | 	--font-weight-two-bold: 700;
335 | }
336 | </style>
337 | {{/contentFor}}
338 | {{/match}}
339 | 
340 | {{#match @custom.fonts "Roboto"}} 
341 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
342 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
343 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap">
344 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap">
345 | {{#contentFor "fonts_css"}}
346 | <style>
347 | :root {
348 | 	--font-family-one: 'Roboto', sans-serif;
349 | 	--font-weight-one-light: 300;
350 | 	--font-weight-one-bold: 700;
351 | 
352 | 	--font-family-two: 'Roboto', sans-serif;
353 | 	--font-weight-two-bold: 700;
354 | 
355 | 	--font-family-three: 'Roboto', sans-serif;
356 | 	--font-weight-three-regular: 400;
357 | 	--font-weight-three-medium: 500;
358 | 	--font-weight-three-bold: 700;
359 | }
360 | </style>
361 | {{/contentFor}}
362 | {{/match}}
363 | 
364 | {{#match @custom.fonts "Space Grotesk + Inter"}} 
365 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
366 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
367 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;700&family=Inter:wght@400;500;700&display=swap">
368 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;700&family=Inter:wght@400;500;700&display=swap">
369 | {{#contentFor "fonts_css"}}
370 | <style>
371 | :root {
372 | 	--font-family-one: 'Space Grotesk', sans-serif;
373 | 	--font-weight-one-light: 300;
374 | 	--font-weight-one-bold: 700;
375 | 
376 | 	--font-family-two: 'Space Grotesk', sans-serif;
377 | 	--font-weight-two-bold: 700;
378 | 
379 | 	--font-family-three: 'Inter', sans-serif;
380 | 	--font-weight-three-regular: 400;
381 | 	--font-weight-three-medium: 500;
382 | 	--font-weight-three-bold: 700;
383 | 
384 | 	--letter-spacing: -.01em;
385 | }
386 | </style>
387 | {{/contentFor}}
388 | {{/match}}
389 | 
390 | {{#match @custom.fonts "Source Serif Pro + Inter"}} 
391 | <link rel="preconnect" href="https://fonts.googleapis.com"> 
392 | <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
393 | <link rel="preload" as="style" href="https://fonts.googleapis.com/css2?family=Source+Serif+Pro:ital,wght@0,400;0,700;1,400;1,700&family=Inter:wght@400;500;700&display=swap">
394 | <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Source+Serif+Pro:ital,wght@0,400;0,700;1,400;1,700&family=Inter:wght@400;500;700&display=swap">
395 | {{#contentFor "fonts_css"}}
396 | <style>
397 | :root {
398 | 	--font-family-one: 'Source Serif Pro', serif;
399 | 	--font-weight-one-light: 400;
400 | 	--font-weight-one-bold: 700;
401 | 
402 | 	--font-family-three: 'Inter', sans-serif;
403 | 	--font-weight-three-regular: 400;
404 | 	--font-weight-three-medium: 500;
405 | 	--font-weight-three-bold: 700;
406 | }
407 | </style>
408 | {{/contentFor}}
409 | {{/match}}
```

partials/widgets.hbs
```
1 | {{#match @custom.widgets "Popular tags"}}
2 | {{#if @custom.slugs_for_selected_tags_or_authors}}
3 | {{#get "tags" limit="7" filter="slug:[{{@custom.slugs_for_selected_tags_or_authors}}]+visibility:public+feature_image:-null" include="count.posts" as |widget|}}
4 | {{#if widget}}
5 | <div class="widget-section global-padding">
6 | 	<small class="global-subtitle">{{t "Popular tags"}}</small>
7 | 	<div class="widget-wrap is-tags">
8 | 		{{#foreach widget}}
9 | 		{{#if count.posts}}
10 | 		{{>item is_widget=true is_topics=true other_image=feature_image alt=""}}
11 | 		{{/if}}
12 | 		{{/foreach}}
13 | 	</div>
14 | </div>
15 | {{/if}}
16 | {{/get}}
17 | {{else}}
18 | {{#get "tags" limit="7" filter="visibility:public+feature_image:-null" include="count.posts" order="count.posts desc" as |widget|}}
19 | {{#if widget}}
20 | <div class="widget-section global-padding">
21 | 	<small class="global-subtitle">{{t "Popular tags"}}</small>
22 | 	<div class="widget-wrap is-tags">
23 | 		{{#foreach widget}}
24 | 		{{#if count.posts}}
25 | 		{{>item is_widget=true is_topics=true other_image=feature_image alt=""}}
26 | 		{{/if}}
27 | 		{{/foreach}}
28 | 	</div>
29 | </div>
30 | {{/if}}
31 | {{/get}}
32 | {{/if}}
33 | {{else match @custom.widgets "Best authors"}}
34 | {{#if @custom.slugs_for_selected_tags_or_authors}}
35 | {{#get "authors" limit="8" filter="slug:[{{@custom.slugs_for_selected_tags_or_authors}}]+visibility:public+profile_image:-null" include="count.posts" as |widget|}}
36 | {{#if widget}}
37 | <div class="widget-section global-padding">
38 | 	<small class="global-subtitle">{{t "Best authors"}}</small>
39 | 	<div class="widget-wrap is-authors">
40 | 		{{#foreach widget}}
41 | 		{{#if count.posts}}
42 | 		{{>item is_widget=true is_authors=true other_image=profile_image alt=""}}
43 | 		{{/if}}
44 | 		{{/foreach}}
45 | 	</div>
46 | </div>
47 | {{/if}}
48 | {{/get}}
49 | {{else}}
50 | {{#get "authors" limit="8" filter="visibility:public+profile_image:-null" include="count.posts" order="count.posts desc" as |widget|}}
51 | {{#if widget}}
52 | <div class="widget-section global-padding">
53 | 	<small class="global-subtitle">{{t "Best authors"}}</small>
54 | 	<div class="widget-wrap is-authors">
55 | 		{{#foreach widget}}
56 | 		{{#if count.posts}}
57 | 		{{>item is_widget=true is_authors=true other_image=profile_image alt=""}}
58 | 		{{/if}}
59 | 		{{/foreach}}
60 | 	</div>
61 | </div>
62 | {{/if}}
63 | {{/get}}
64 | {{/if}}
65 | {{/match}}
```

post-card.hbs
```
1 | <article class="post-card {{#has tag="rough-notes"}}rough-notes-post-card{{/has}}"></article>
2 |   <header class="post-card-header">
3 |     <h2 class="post-card-title">
4 |       <a href="{{url}}">{{title}}</a>
5 |     </h2>
6 |     <time class="post-card-date" datetime="{{date format="YYYY-MM-DD"}}">{{date format="MMMM DD, YYYY"}}</time>
7 |   </header>
8 |   
9 |   {{#if feature_image}}
10 |     <img class="post-card-image" src="{{feature_image}}" alt="{{title}}">
11 |   {{/if}}
12 |   
13 |   <section class="post-card-excerpt">
14 |     <p>{{excerpt words="30"}}...</p>
15 |   </section>
16 |   
17 |   <footer class="post-card-footer">
18 |     {{#if tags}}
19 |       <div class="post-card-tags">
20 |         {{#foreach tags}}
21 |           <span class="post-card-tag">{{name}}</span>
22 |         {{/foreach}}
23 |       </div>
24 |     {{/if}}
25 |     
26 |     {{#if reading_time}}
27 |       <span class="post-card-reading-time">{{reading_time minute="1 min read" minutes="% min read"}}</span>
28 |     {{/if}}
29 |   </footer>
30 | </article>
```

post.hbs
```
1 | {{!< default}}
2 | {{#post}}
3 | {{^is "page"}}
4 | {{#if access}}<progress class="post-progress"></progress>{{/if}}
5 | {{/is}}
6 | <article class="post-section{{^is "page"}}{{^match @custom.sidebar "Disable"}} is-sidebar{{/match}}{{/is}}">
7 | 	{{#match @page.show_title_and_feature_image}}
8 | 	{{>posts/header}}
9 | 	{{/match}}
10 | 	<div class="post-wrap global-padding">
11 | 		{{^is "page"}}
12 |         {{#match @custom.sidebar "Without Subscription form"}}
13 | 		<div class="post-sidebar">
14 | 			{{>posts/sidebar}}
15 | 		</div>
16 | 		{{/match}}
17 | 		{{#match @custom.sidebar "With Subscription form"}}
18 | 		<div class="post-sidebar">
19 | 		{{#if access}}
20 | 		{{>posts/sidebar}}
21 | 		{{>members/sidebar_form is_box=true}}
22 | 		{{else if html}}
23 | 		{{>posts/sidebar}}
24 | 		{{/if}}
25 | 		</div>
26 | 		{{/match}}
27 |         {{#match @custom.sidebar "With sticky Subscription form"}}
28 | 		<div class="post-sidebar">
29 | 		{{#if access}}
30 | 		{{>posts/sidebar}}
31 | 		{{>members/sidebar_form is_box=true is_sticky=true}}
32 | 		{{else if html}}
33 | 		{{>posts/sidebar}}
34 | 		{{/if}}
35 | 		</div>
36 | 		{{/match}}
37 | 		{{/is}}
38 | 		<div class="post-content">
39 | 			{{#if access}}
40 | 			{{content}}
41 | 			{{^is "page"}}
42 | 			{{>posts/share}}
43 | 			{{/is}}
44 | 			{{else}}
45 | 			{{#if html}}
46 | 			<div class="members-cta-teaser">
47 | 				{{{html}}}
48 | 			</div>
49 | 			{{/if}}
50 | 			{{>members/cta}}
51 | 			{{/if}}
52 | 		</div>
53 | 	</div>
54 | </article>
55 | {{^is "page"}}
56 | {{>posts/navigation}}
57 | {{>posts/comments}}
58 | {{#if primary_tag}}
59 | {{#get "posts" limit="5" filter="tags:{{primary_tag.slug}}+id:-{{id}}" include="authors" as |special_posts|}}
60 | 	{{#if special_posts}}
61 | 		{{>related label=(t "You might also like")}}
62 | 	{{/if}}
63 | {{/get}}
64 | {{/if}}
65 | {{/is}}
66 | {{/post}}
```

rough-notes.hbs
```
1 | {{!< default}}
2 | 
3 | <div class="rough-notes-page global-padding">
4 |   <div class="global-content">
5 |     {{#page.rough-notes}}
6 |       <h1 class="global-title">{{title}}</h1>
7 |       <p class="global-description">
8 |         {{content}}
9 |       </p>
10 |     {{/page.rough-notes}}
11 | 
12 |     <div class="loop-section global-padding">
13 |       <small class="global-subtitle">{{t "Rough Notes Posts"}}</small>
14 |       <div class="loop-wrap">
15 |         {{#get "posts" limit="all" filter="tag:rough-notes" include="authors,tags" as |posts|}}
16 |           {{#foreach posts}}
17 |             {{> "item" show_excerpt=true}}
18 |           {{/foreach}}
19 |         {{/get}}
20 |       </div>
21 |     </div>
22 |   </div>
23 | </div>
```

tag.hbs
```
1 | {{!< default}}
2 | {{#tag}}
3 | {{#contentFor "feature_image"}}
4 | {{#if feature_image}}
5 | <div class="global-cover" style="background-image:url({{{img_url feature_image size="xl" format="webp"}}})"></div>
6 | {{else if @site.cover_image}}
7 | <div class="global-cover" style="background-image:url({{{img_url @site.cover_image size="xl" format="webp"}}})"></div>
8 | {{/if}}
9 | {{/contentFor}}
10 | {{>posts/header archive_page=true is_custom=true title=name custom_excerpt=description custom_image=feature_image}}
11 | {{/tag}}
12 | {{>loop is_archive=true}}
13 | {{pagination}}
```

