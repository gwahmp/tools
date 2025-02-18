---
layout: default
title: Free SEO Writing Assistant Tool - Boost Your Article Score Instantly
description: Analyze your article SEO score with our free SEO writing assistant tool. Get actionable insights, improve keyword rankings, optimize on-page SEO, and enhance your site's visibility on search engines.
date: 2024-12-18
noindex: false
---


<div class="container">
   <div id="seoWriter" class="w-100 p-0 m-0" style="display:none;">
      <div class="row w-100 m-0 p-0">
         <div class="col-md-8 editor p-0 m-0">
            <div class="editor-container bg-light p-0">
               <div class="editor-toolbar bg-white p-1 border border-bottom d-flex align-items-center">
                  <span class="d-flex align-items-center" style="min-width:125px;">
                     <div class="dropdown">
                        <button class="btn btn-secondary bi bi-list me-1 py-0 border-secondary px-2 rounded-0" style="border-color:var(--bs-secondary) ! important;background:var(--bs-secondary) ! important;color:white ! important;" data-bs-toggle="dropdown" aria-expanded="false"></button>
                        <ul class="dropdown-menu shadow-sm">
                           <li><span role="button" class="dropdown-item" id="save"><i class="bi bi-floppy me-2"></i> Save <span class="float-end ms-3 small">Ctrl+S</span></span></li>
                           <li><span role="button" class="dropdown-item" id="run"><i class="bi bi-play me-2"></i> Run <span class="float-end ms-3 small">Ctrl+F5</span></span></li>
                           <li><span role="button" class="dropdown-item" id="print"><i class="bi bi-printer me-2"></i> Print <span class="float-end ms-3 small">Ctrl+P</span></span></li>
                           <li class="border-top mt-2"><span role="button" class="dropdown-item" id="export"><i class="bi bi-upload me-2"></i> Export</span></li>
                           <li><span role="button" class="dropdown-item" id="import"><i class="bi bi-download me-2"></i> <label for="importField" class="form-label">Import</label>
                              <input class="form-control form-control-sm d-none" id="importField" type="file"> <span class="float-end ms-3 small"></span></span>
                           </li>
                           <li><span role="button" class="dropdown-item" id="delete"><i class="bi bi-trash3 me-2"></i> Delete <span class="float-end ms-3 small"></span></span></li>
                           <li class="border-top mt-2"><span role="button" class="dropdown-item" id="exit"><i class="bi bi-x-lg me-2"></i> Exit</span></li>
                        </ul>
                     </div>
                     <ul class="nav nav-pills border border-2 border-primary rounded-0 " id="pills-tab" role="tablist" >
                        <li class="nav-item py-0 visual-tab" role="presentation">
                           <span class="nav-link rounded-0 rounded-top-left btn-sm py-1 px-2 active" id="pills-editor-tab" data-bs-toggle="pill" data-bs-target="#editorContent" type="button" role="tab" aria-controls="pills-editor" aria-selected="true"><i class="bi bi-eye"></i></span>
                        </li>
                        <li class="nav-item py-0 code-tab" role="presentation">
                           <span class="nav-link rounded-0 py-1 px-2" id="pills-html-tab" data-bs-toggle="pill" data-bs-target="#htmlContent" type="button" role="tab" aria-controls="pills-html" aria-selected="false"><i class="bi bi-code"></i></span>
                        </li>
                     </ul>
                  </span>
                  <span class="ms-auto d-flex overflow-y-auto">
                  <button class="bi bi-paragraph format-btn" data-format="p"></button>
                  <button class="bi bi-type-h1 format-btn" data-format="h1"></button>
                  <button class="bi bi-type-h2 format-btn" data-format="h2"></button>
                  <button class="bi bi-type-h3 format-btn" data-format="h3"></button>
                  <button class="bi bi-type-h4 format-btn" data-format="h4"></button>
                  <button class="bi bi-type-h5 format-btn" data-format="h5"></button>            
                  <button class="bi bi-type-h6 format-btn" data-format="h6"></button>
                  <button id="bold-btn" class="bi bi-type-bold" data-format="bold"></button>
                  <button id="italic-btn" class="bi bi-type-italic" data-format="i"></button>
                  <button id="underline-btn" class="bi bi-type-underline" data-format="u"></button>
                  <button class="bi bi-list-ol list-btn"  data-format="ol"></button>
                  <button id="ul-btn" class="bi bi-list-task list-btn"  data-format="ul"></button>
                  <button class="bi bi-quote format-btn"  data-format="blockquote"></button>
                  <button id="link-btn" class="bi bi-link-45deg" data-format="a"></button>
                  <button id="image-btn" class="bi bi-image" data-format="img"></button>
                  </span>
               </div>
               <div class="row w-100 p-0 m-0">
                  <div class="col-4 p-3 bg-light d-none d-lg-block" style="height: calc(100vh - 80px);overflow-y: auto;">
                     <span class="small">
                        <h5 class="text-secondary">SEO Writer</h5>
                        <p class="p-3 bg-warning-subtle border border-warning">This SEO writing tool is only for analysing article blog post having more than 1000 words. Not for small contents like social media post or other one-liners.</p>
                        <p class="p-3 bg-success-subtle border border-success">Just paste your copy here or write it here. Watch your article score raising on realtime.</p>
                        <h5 class="text-secondary lead fw-normal">Useful sub-tools</h5>
                        <p class="p-3 bg-white border"><strong>Case converter</strong>: <a href="https://developer.wikimint.com/p/case-converter-text-formatter-tool.html" target="_blank">Case converter tool</a> helps to immediately and automatically convert text tranformation properties. Like lowercase to uippercase, uppercase to capitalise and so on.</p>
                        <p class="p-3 bg-white border"><strong>Image resizer</strong>: <a href="https://developer.wikimint.com/p/online-image-resizer-tool.html" target="_blank">Image resize tool</a> helps to control the resolution of your article image. It's better to reduce width of the image around the width of the article content element width.</p>
                        <p class="p-3 bg-white border"><strong>Image optimizer</strong>: <a href="https://developer.wikimint.com/p/photo-optimizer-online-image-compressor.html" target="_blank">Image optimizer (compressor) tool</a> helps to reduce the size of the image file keeping the same quality.</p>
                     </span>
                  </div>
                  <div class="col-lg-8 col-12 border-left p-0 m-0">
                     <div class="tab-content" id="pills-tabContent">
                        <div id="editorContent" class="tab-pane fade show active editor-content bg-white p-3 px-4 border-0 border-start float-end" aria-labelledby="pills-html-tab" contenteditable="true">
                           <p>Start writing here...</p>
                        </div>
                        <textarea id="htmlContent" rows="30" class="tab-pane fade p-3 px-4 border-0 border-start float-end" role="tabpanel" aria-labelledby="pills-html-tab" tabindex="0"></textarea>
                     </div>
                  </div>
               </div>
               <div class="bg-white text-dark small py-1 px-2 border-top">
                  Characters : <span id='chars' class="me-2">0</span> 
                  Words : <span id='words' class="me-2">0</span> 
                  Sentences : <span id='sentences' class="me-2">0</span> 
                  Paragraphs : <span id='para' class="me-2">0</span>
               </div>
            </div>
         </div>
         <div id="scorePanel" class="col-md-4 toolbar p-0 m-0 border border-left">
            <div class="sticky-top p-3 py-2 text-dark bg-light border-bottom d-flex align-items-center" style="min-height:45px;"><span class="me-auto">SEO Writing Tool <span class="small bg-white ms-2 p-1 px-2  rounded-2">v1.0.2</span></span><span class="small ms-auto float-end"><i id="closeScore" class="bi bi-x-lg text-secondary d-block d-sm-none" style="font-size:20px;" role="button"></i></span></div>
            <div class="tools h-100 position-absolute" style="width:inherit;">
               <div class="w-100 overflow-y-auto" style="height:calc(100vh - 80px);">
                  <div class="card border-0 rounded-0">
                     <div class="card-body mx-auto">
                        <div class="donut rounded-circle d-flex align-items-center">
                           <span class="donut-content mx-auto">
                           <span class="d-block text-center small">Score</span>
                           <span id="score" class="display-3 fw-bold">0</span>
                           <span class="d-block border-0 border-top text-center">100</span>
                           </span>
                        </div>
                     </div>
                  </div>
                  <ul class="nav nav-tabs rounded-0 border-top mt-3 sticky-top bg-light shadow-sm" id="inputs-analytics-tab" role="tablist" >
                     <li class="nav-item py-0 w-50 text-center" role="presentation">
                        <span class="nav-link rounded-0 rounded-top-left btn-sm py-1 px-2 active" id="pills-inputs-tab" data-bs-toggle="pill" data-bs-target="#inputsTab" type="button" role="tab" aria-controls="pills-inputs" aria-selected="true"><i class="bi bi-pencil-square me-2"></i> Inputs</span>
                     </li>
                     <li class="nav-item py-0 w-50 text-center" role="presentation">
                        <span class="nav-link rounded-0 py-1 px-2" id="pills-analytics-tab" data-bs-toggle="pill" data-bs-target="#analyticsTab" type="button" role="tab" aria-controls="pills-analytics" aria-selected="false"><i class="bi bi-graph-up-arrow me-2"></i> Analytics</span>
                     </li>
                  </ul>
                  <div class="tab-content" id="pills-tabContent">
                     <div id="inputsTab" class="tab-pane bg-light fade show active p-3" aria-labelledby="pills-inputs-tab">
                        <p>Please fill up all below fields for better analysis of your article SEO.</p>
                        <!--Publishing site-->
                        <div class="bg-white p-3 shadow-sm border mb-3">
                           <h5 class="lead fw-normal">Publishing website</h5>
                           <p class="small">Enter website domain, where you are going to publish your article.</p>
                           <div class="input-group mb-3">
                              <span class="input-group-text border-2" id="basic-addon1"><i class="bi bi-globe text-secondary"></i></span>
                              <input type="text" id="pubSite" class="form-control bg-light border-2 shadow-sm" placeholder="https://www.example.com" aria-label="siteURL" aria-describedby="basic-addon1">
                           </div>
                        </div>
                        <!--Meta title-->
                        <div class="bg-white p-3 shadow-sm border mb-3">
                           <h5 class="lead fw-normal">Meta title</h5>
                           <p class="small">Enter SEO meta title for your article with relevant keywords.</p>
                           <div class="small d-block mb-2 text-secondary">SEO meta title (Chars: <span class="title-chars">0</span>)</div>
                           <div class="input-group mb-3">
                              <textarea id="metaTitle" class="form-control bg-light border-2 shadow-sm" placeholder="SEO meta title" max="70" rows="2" aria-label="metaTitle" aria-describedby="basic-addon1"></textarea>
                           </div>
                           <div id="titleProgress" class="progress mb-3" role="progressbar" aria-label="Example 1px high" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100" style="height: 10px">
                              <div class="progress-bar" style="width: 25%"></div>
                           </div>
                        </div>
                        <!--Meta description-->
                        <div class="bg-white p-3 shadow-sm border mb-3">
                           <h5 class="lead fw-normal">Meta description</h5>
                           <p class="small">Enter meta description for your article with relevant keywords.</p>
                           <div class="small d-block mb-2 text-secondary">SEO meta description  (Chars: <span class="desc-chars">0</span>)</div>
                           <div class="input-group mb-3">
                              <textarea id="metaDesc" class="form-control bg-light border-2 shadow-sm" placeholder="SEO meta description" max="300" rows="5" aria-label="metaDesc" aria-describedby="basic-addon1"></textarea>
                           </div>
                           <div id="descProgress" class="progress mb-3" role="progressbar" aria-label="Example 1px high" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100" style="height: 10px">
                              <div class="progress-bar" style="width: 25%"></div>
                           </div>
                        </div>
                        <!--Focus keyphrase-->
                        <div class="bg-white p-3 shadow-sm border mb-3">
                           <h5 class="lead fw-normal">Focus keyphrase</h5>
                           <p class="small">Type your focus keyphrase below for ranking your article.</p>
                           <div class="input-group mb-3">
                              <input type="text" id="keyPhrase" class="form-control bg-light border-2 shadow-sm" placeholder="e.g. best coffee shops" aria-label="keyPhrase" aria-describedby="basic-keyphrase">
                           </div>
                        </div>
                     </div>
                     <div id="analyticsTab" rows="30" class="tab-pane fade" role="tabpanel" aria-labelledby="pills-analytics-tab" tabindex="0">
                        <div class="accordion bg-light" id="accordionExample">
                           <div class="accordion-item bg-light">
                              <h2 class="accordion-header bg-primary-subtle">
                                 <button class="accordion-button  bg-primary-subtle collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#seoAnalysis" aria-expanded="false" aria-controls="seoAnalysis">
                                 SEO analysis
                                 </button>
                              </h2>
                              <div id="seoAnalysis" class="accordion-collapse collapse show">
                                 <div class="accordion-body">
                                    <div class="bad">
                                       <div class="result-title">Problems (<span class="bad-count">0</span>)</div>
                                       <div class="result article-length"><span><strong>Word count</strong>: Your article has only <span class="word-count">0</span> words. Try to increase word count above 1000 words.</span></div>
                                       <div class="result meta-title"><span><strong>Meta title</strong>: You have not yet added meta title. Add meta title.</span></div>
                                       <div class="result meta-desc"><span><strong>Meta description</strong>: You have not yet added meta description. Add meta description.</span></div>
                                       <div class="result internal-links"><span><strong>Internal links</strong>: No internal links found. Link at least 3 posts/pages from your site.</span></div>
                                       <div class="result external-links"><span><strong>Outbound links</strong>: No links to external sites found. Link to atleast 1 posts/pages from any external site.</span>            </div>
                                       <div class="result images"><span><strong>Images</strong>: No image(s) found in your article. Please add relevant image(s).</span>            
                                       </div>
                                       <div class="result h2-heading"><span><strong>Sub-headings H2</strong>: H2 level sub-heading(s) not found in your article. Try to ads sub-heading H2.</span></div>
                                    </div>
                                    <div class="improve">
                                       <div class="result-title">Needs improvement (<span class="improve-count">0</span>)</div>
                                       <div class="result article-length"><span><strong>Word count</strong>: Your article has <span class="word-count">0</span> words. It's better to increase word count above 1000 words.</span></div>
                                       <div class="result meta-title-short"><span><strong>Meta title</strong>: You have added meta title, but it's length is too short. Increase the length to atleast 60 characters.</span></div>
                                       <div class="result meta-title-long"><span><strong>Meta title</strong>: You have added meta title, but it's length is too long. Keep it below 60 characters.</span></div>
                                       <div class="result meta-desc-short"><span><strong>Meta description</strong>: You have added meta description, but it's length is too short. Increase the length to atleast 155 characters.</span></div>
                                       <div class="result meta-desc-long"><span><strong>Meta description</strong>: You have added meta description, but it's length is too long. Keep it below 160 characters.</span></div>
                                       <div class="result h3-heading"><span><strong>Sub-headings H3</strong>: H3 level sub-heading(s) not found in your article. Try to add sub-heading H3.</span></div>
                                       <div class="result external-links"><span><strong>Outbound links</strong>: You have <span class="ext-link-count">0</span> outbound link(s) in your article, but it is very excessive when compared to your article length. Try reduce outbout links to <span class="ext-link-limit">0</span> link(s) maximum.</span></div>
                                    </div>
                                    <div class="good">
                                       <div class="result-title">Good results (<span class="good-count">0</span>)</div>
                                       <div class="result images"><span><strong>Images</strong>: Image(s) found in your article. Great job!</span></div>
                                       <div class="result h2-heading"><span><strong>Sub-headings H2</strong>: Your article has H2 level sub-heading(s). Good job!</span></div>
                                       <div class="result meta-title"><span><strong>Meta title</strong>: You added meta title with good length of characters. Good job!</span></div>
                                       <div class="result meta-desc"><span><strong>Meta description</strong>: You added meta description with good length of characters. Good job!</span></div>
                                       <div class="result h3-heading"><span><strong>Sub-headings H3</strong>: Your article has H3 level sub-heading(s). Good job!</span></div>
                                       <div class="result article-length"><span><strong>Word count</strong>: Your article has <span class="word-count">0</span> words. Good job!</span></div>
                                       <div class="result internal-links"><span><strong>Internal links</strong>: You have <span class="int-link-count">0</span> internal link(s) in your article. Great job!</span></div>
                                       <div class="result external-links"><span><strong>Outbound links</strong>: You have <span class="ext-link-count">0</span> outbound link(s) in your article. Perfect!</span></div>
                                    </div>
                                 </div>
                              </div>
                           </div>
                           <div class="accordion-item">
                              <h2 class="accordion-header bg-primary-subtle">
                                 <button class="accordion-button bg-primary-subtle collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#readAnalysis" aria-expanded="false" aria-controls="readAnalysis">
                                 Readability analysis
                                 </button>
                              </h2>
                              <div id="readAnalysis" class="accordion-collapse collapse show">
                                 <div class="accordion-body">
                                    <div class="bad">
                                       <div class="result-title">Problems (<span class="bad-count">0</span>)</div>
                                       <div class="result para-length"><span><strong>Paragraph length</strong>: Some of your paragraphs are found to be too long. Split them for easier readability.</span></div>
                                       <div class="result sent-words-length"><span><strong>Sentence length</strong>: Some of the sentences are found to be too long. Split them for easier readability.</span></div>
                                       <div class="result transition-words"><span><strong>Transition words</strong>: Usage of transition words is not engough. Try to include more transition words anywhere in the sentences.</span></div>
                                       <div class="result sent-length"><span><strong>Sentence length</strong>: <span class="sent-words">0</span>% of the sentences contain more than 20 words, which is more than the maximum recommended limit of 25%. Try to shorten the sentences.</span></div>
                                       <div class="result passive-voice"><span><strong>Passive voice</strong>: <span class="passive-sent">0</span>% of sentences are found to be passive voice, whice is greater than the maximum recommended limit of 10%. Try to convert them to active voice.</span></div>
                                       <div class="result sub-heading"><span><strong>Sub-heading distribution</strong>: At some places, text content seems to be too lenghty. Try to sub-headings in between them.</span></div>
                                    </div>
                                    <div class="improve">
                                       <div class="result-title">Needs improvement (<span class="improve-count">0</span>)</div>
                                       <div class="result passive-voice"><span><strong>Passive voice</strong>: <span class="passive-sent">0</span>% of sentences are found to be passive voice, whice is greater than the maximum recommended limit of 10%. Try to convert them to active voice.</span></div>
                                       <div class="result transition-words"><span><strong>Transition words</strong>: All the sentences maintain some proportion of transition words. But, it's not engough to make your readers find much clarity while reading. Try to include more transition words anywhere.</span></div>
                                    </div>
                                    <div class="good">
                                       <div class="result-title">Good results (<span class="good-count">0</span>)</div>
                                       <div class="result para-length"><span><strong>Paragraph length</strong>: All your paragraphs are within the maximum limit of 75 words. Good job!</span></div>
                                       <div class="result sub-heading"><span><strong>Sub-heading distribution</strong>: Sub-heading distribution is properly maintained. Well done!</span></div>
                                       <div class="result sent-words-length"><span><strong>Sentence length</strong>: All the sentences are found to have good limit os word count. Good job!</span></div>
                                       <div class="result transition-words"><span><strong>Transition words</strong>: All the sentences maintain a correct proportion of transition words. Thus, your readers will find more clarity. Good job!</span></div>
                                       <div class="result sent-length"><span><strong>Sentence length</strong>: <span class="sent-words">0</span>% of the sentences contain more than 20 words and not exceeds the recommended maximum words of 25%. Great job!</span></div>
                                       <div class="result passive-voice"><span><strong>Passive voice</strong>: All your sentences are found to be maintainig below 10% of passive voice sentences. Perfect!</span></div>
                                    </div>
                                 </div>
                              </div>
                           </div>
                           <div class="accordion-item">
                              <h2 class="accordion-header bg-primary-subtle">
                                 <button class="accordion-button bg-primary-subtle collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#keyAnalysis" aria-expanded="false" aria-controls="keyAnalysis">
                                 Keyword analysis
                                 </button>
                              </h2>
                              <div id="keyAnalysis" class="accordion-collapse collapse show">
                                 <div class="accordion-body">
                                    <div class="bad">
                                       <div class="result-title">Problems (<span class="bad-count">0</span>)</div>
                                       <div class="result key-phrase"><span><strong>Focus key phrase</strong>: You have not set a focus key phrase. Try to set it.</span></div>
                                       <div class="result key-phrase-invalid"><span><strong>Invalid focus key phrase</strong>: Focus key phrase is found, but it is invalid. Key phrase should have atleast 2 words. Try to set it.</span></div>
                                       <div class="result images-focus-alt"><span><strong>Focus keyphrase in images</strong>: Focus keyphrase not appear in alt attribute of <span id="focusAlt">0</span> images. Try to include.</span></div>
                                       <div class="result key-title"><span><strong>Keyphrase in SEO title</strong>: Focus key phrase is not found in the SEO title. Try to include.</span></div>
                                       <div class="result key-desc"><span><strong>Keyphrase in meta description</strong>: Focus key phrase is not found in the SEO meta description. Try to include.</span></div>
                                       <div class="result key-intro"><span><strong>Keyphrase in first paragraph</strong>: Focus key phrase do not found in the first paragraph (introduction) of your article. Try to include.</span></div>
                                       <div class="result key-headings"><span><strong>Keyphrase in sub-headings</strong>: Focus key phrase do not found in any of the sub-headings (H2 and H3). Try to include.</span></div>
                                       <div class="result key-density"><span><strong>Keyphrase density</strong>: Focus key phrase do not found anywhere in your article. Try to include.</span></div>
                                       <div class="result key-density-over"><span><strong>Keyphrase density</strong>: Focus key phrase appears more than required number of times (Over-optimized). Try to remove them and keep your focus phrase count below <span id="densMax">10</span>.</span></div>
                                       <div class="result key-links"><span><strong>Keyphrase in links</strong>: <span id="keyLinksCount">Some of your </span> link(s) has the exact focus key phrase as link text. Try to rewrite the link text.</span></div>
                                    </div>
                                    <div class="improve">
                                       <div class="result-title">Needs improvement (<span class="improve-count">0</span>)</div>
                                       <div class="result key-headings"><span><strong>Keyphrase in sub-headings</strong>: Focus key phrase appears somewhere in the sub-headings (H2 and H3), but it's not sufficient. Try to include focus keyphrase at <span id="keyHeadReq">1</span> more H2 or H3 sub-heading(s).</span></div>
                                       <div class="result key-density"><span><strong>Keyphrase density</strong>: Focus key phrase appears somewhere in your overall article, but it's not sufficient. Try to include focus keyphrase at <span id="densReq">1</span> more places across your article.</span></div>
                                    </div>
                                    <div class="good">
                                       <div class="result-title">Good results (<span class="good-count">0</span>)</div>
                                       <div class="result key-phrase"><span><strong>Focus key phrase</strong>: You have set a valid focus key phrase. Good job!</span></div>
                                       <div class="result images-focus-alt"><span><strong>Focus keyphrase in images</strong>: Focus keyphrase appears in alt attribute of all images. Perfect job!</span></div>
                                       <div class="result key-title"><span><strong>Keyphrase in SEO title</strong>: SEO title has focus key phrase set by you. Good job!</span></div>
                                       <div class="result key-desc"><span><strong>Keyphrase in meta description</strong>: SEO meta description has focus key phrase set by you. Good job!</span></div>
                                       <div class="result key-intro"><span><strong>Keyphrase in first paragraph</strong>: Focus key appears in the first paragraph (introduction). Perfect!</span></div>
                                       <div class="result key-headings"><span><strong>Keyphrase in sub-headings</strong>: Focus key phrase appears in the sub-headings (H2 and H3) in correct proportion. Great job!.</span></div>
                                       <div class="result key-density"><span><strong>Keyphrase density</strong>: Focus key phrase appears in your overall article in a correct proportion. Great job!.</span></div>
                                    </div>
                                 </div>
                              </div>
                           </div>
                           <div class="accordion-item d-none">
                              <h2 class="accordion-header bg-primary-subtle">
                                 <button class="accordion-button bg-primary-subtle collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#internalLinks" aria-expanded="false" aria-controls="internalLinks">
                                 Internal linking suggestions
                                 </button>
                              </h2>
                              <div id="internalLinks" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                 <div class="accordion-body">
                                 </div>
                              </div>
                           </div>
                           <div class="accordion-item d-none">
                              <h2 class="accordion-header bg-primary-subtle">
                                 <button class="accordion-button bg-primary-subtle collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#externalLinks" aria-expanded="false" aria-controls="externalLinks">
                                 External linking suggestions
                                 </button>
                              </h2>
                              <div id="externalLinks" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                 <div class="accordion-body">
                                 </div>
                              </div>
                           </div>
                        </div>
                        <button class="btn btn-light w-100 btn-block border border-top-0 rounded-0 text-start p-3 text-dark d-none">Search engine appearance</button>
                     </div>
                  </div>
               </div>
               <div class="bg-light text-dark small py-1 px-2 border-top text-center">
                  <footer id="copyright">
                     &copy; <script>document.write(new Date().getFullYear());</script>, SEO tool by <a target="_blank" href="https://developer.wikimint.com">Wikimint Developer</a>
                  </footer>
               </div>
            </div>
         </div>
      </div>
   </div>
</div>

<link rel="stylesheet" href="assets/css/style.css"/>

<script src="assets/js/script.js"></script>
<script src="assets/js/events.js"></script>
<script src="assets/js/analytics.js"></script>



<div class="container">
   <div class="row py-5 text-center">
      <div class="mx-auto" style="max-width:650px;">
         <h2 class="display-4 fw-normal mb-3 text-dark">SEO Writing Assistant</h2>
         <p class="lead">Write high quality articles and enhance your blog SEO score with 100% free online SEO writing assistant tool.</p>
            <div class="text-center">
      <button id="launch" class="btn btn-primary">Launch SEO Writing</button>
   </div>
      </div>
   </div>
   <div class="row py-5">
      <div class="col-md-6 pb-3">
         <p>Crafting high-quality articles is essential for engaging readers and boosting your website's <a href="https://developer.wikimint.com/2016/10/basics-of-seo-search-engine.html">SEO ranking</a>. Utilizing a free online SEO writing tool can significantly enhance your content's effectiveness. These tools provide valuable insights and suggestions to optimize your articles for search engines while maintaining readability and relevance.</p>
         <h3>Why SEO writing assistant?</h3>
         <p>This SEO tool walk you through SEO guidance through all metrices. All the SEO suggestion adhere to <a href="https://developer.wikimint.com/2023/08/google-algorithm-updates-seo-impacts.html">Google algorith updates</a> and content policies. As you know, Google hate black hat SEO techniques. So, we always suggest you to implement ethical and professionally handled <a href="https://developer.wikimint.com/2017/05/important-seo-techniques-to-increase.html">SEO tweaks</a>.</p>
      </div>
      <div class="col-md-6">
         <img alt="SEO writing assistant - Free article score checker online" width="100%" height="auto" border="0" data-original-height="401" data-original-width="702" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEisGrANs84RK1BdIdeSlf03YloBKKuHm6lwi7TJ4ormYXTzb1hmYbXXXW-aXDAaCs3VkspKAZDcue6kdun3mBgt1yavoAX7_Vwtq1ZJLbWq1QksJp_bsfCAKlHTmvGIvDzXZraQSIt61sHSEwpkHS1COlFooPdVMBAAsCMoXiQANwcvmTohXi0BVonuW-vu/s1600/seo-writing-tool-free-online.JPG"/>
      </div>
   </div>
   <div class="row py-5 text-center middle-content">
      <div class="middle-area mx-auto" style="max-width:650px;">
         <h2>Complete SEO article writing assistant</h2>
         <p>Includes SEO analysis, readability analysis, keyword analysis, search engine and social media preview. Even you could add images, internal links and outbound links.</p>
      </div>
   </div>
   <div class="card p-3">
      <div class="card-body">
         <div class="row">
            <div class="col-md-8 d-flex align-items-center">
               <div>
                  <h3>Developer behind SEO writing tool</h3>
                  <p>Beyond as a <a href="https://developer.wikimint.com/2023/07/full-stack-web-development-step-by-step.html">full-stack developer</a>, Selvakumaran Krishnan has been working with SEO for many freelance as well as personal projects. He conducted several researches and gathered collective knowledge from his experience. As a result, he developed this always free SEO writing tool, <strong>SEO writing assistant</strong> (Article score checking online).</p>
                  <p>Since 2017, he started writing blogs on the topics related to web development and SEO as well as general subject. He came across several writing tools and SEO analytical platforms. Upon finding certain inconvenience, he started developing his own SEO writing tool. Also, he decided to launch this 100% free SEO writing tool for the public usage. Now, SEO professionals, companies, bloggers and everyone could use this always free SEO analysis tool.</p>
                  <blockquote class="blockquote bg-success-subtle p-3 border-success rounded-2">
                     <p>Writing is an art; adhering to streamlined metrics makes it a discipline.</p>
                  </blockquote>
               </div>
            </div>
            <div class="col-md-4 text-center">
               <img alt="Selvakumaran Krishnan - Developer of SEO writing tool" width="100%" height="auto" border="0" data-original-height="501" data-original-width="498" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhI1g9CJxXCihkYdZt1AMtpMKONV7c8meUyCj1YLpGRRlWEdDy-8B1b4Qs97H8Q7Y5E78qF86Fy9k7_7nmNHG5-soLJ9oSvfQsffpIe2TmF45Wrj2Tekz38VcgVzTZDwXqaLc_hMFsefUjak7sD-n1SuQrQzPfSG6g5nkxKHgPbDRpqjmSDmPTESGF48jsG/s1600/Selvakumaran-Krishnan-wikimint-developer-full-stack-web-developer.jpg"/><span class="d-block small text-center"><span class="d-block lead">Selvakumaran Krishnan</span><span class="text-secondary">Full-stack Developer | SEO Specialist</span></span>
            </div>
         </div>
      </div>
   </div>
   <div class="my-5">
      <div class="row text-center">
         <div class="col-md-2"></div>
         <div class="col-md-8 middle-area mx-auto">
            <h2>SEO analysis metrices</h2>
            <p>This SEO writing analysis almost includes all metrices. That includes SEO analysis, readability analysis, keyword analysis, internal links and outbound link suggestions, search and social media appearances, etc.</p>
         </div>
         <div class="col-md-2"></div>
      </div>
      <div class="row mt-3">
         <div class="col-md">
            <div class="alert alert-secondary bg-light" role="alert">
               <span class="small">Analyze</span>   
               <h3 class="alert-heading display-6 fw-thin">SEO Score</h3>
            </div>
         </div>
         <div class="col-md">
            <div class="alert alert-secondary bg-light" role="alert">
               <span class="small">Improve</span>   
               <h3 class="alert-heading display-6 fw-thin">Readability</h3>
            </div>
         </div>
         <div class="col-md">
            <div class="alert alert-secondary bg-light" role="alert">
               <span class="small">Check</span>   
               <h3 class="alert-heading display-6 fw-thin">Appearances</h3>
            </div>
         </div>
         <div class="col-md">
            <div class="alert alert-secondary bg-light" role="alert">
               <span class="small">Complete</span>   
               <h3 class="alert-heading display-6 fw-thin">Writing</h3>
            </div>
         </div>
      </div>
   </div>
</div>