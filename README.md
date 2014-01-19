Guitar-tabs to songtex.js
======================

JS script to convert raw text tabs to tex file for the songbook package (see https://github.com/crep4ever/songbook)

Demo
-------------
http://jsbin.com/OyaGEzaQ/1

Usage
-------------
Just call the plainTab2tex.parse() function with an array of lines, it will return an array of lines

  
    function parse_id(src_id, dst_id) {
        var src = document.getElementById(src_id),
            dst = document.getElementById(dst_id),
            raw_textlines = src.value.split(/\r\n|\r|\n/g);
    
        dst.innerHTML = plainTab2tex.parse(raw_textlines).join('<br/>');
    }
