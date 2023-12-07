---
layout: page
title: FFXI ReShade Preset
subtitle: "This is a subtitle"  
permalink: /ffxireshadepreset/         # Set a permalink your your page
hide: false                           # Prevent the page title to appear in the navbar
tags: [reshade,ffxi]
---

Some Content about reshade.


{% for i in (0..25) %}
<div class="mainSection">
        <div id="comp{{i}}" class="bal-container">
            <div class="bal-after">
                <img src="/ElfyLab2/img/beforeafter/{{i+1}}.jpg">
                <div class="bal-afterPosition afterLabel">
                    After
                </div>
            </div>
            <div class="bal-before">
                <div class="bal-before-inset">
                    <img src="/ElfyLab2/img/beforeafter/{{i}}.png">
                    <div class="bal-beforePosition beforeLabel">
                        Before
                    </div>
                </div>
            </div>
            <div class="bal-handle">
                <span class="handle-left-arrow"></span>
                <span class="handle-right-arrow"></span>
            </div>
        </div>
    </div>
 {% assign i = i+1 %}
{% endfor %}

<script src="/ElfyLab2/assets/js/imagecomparison.js"></script>

<script>
        new BeforeAfter({
            id: '#one'
        });
        new BeforeAfter({
            id: '#two'
        });
</script>
