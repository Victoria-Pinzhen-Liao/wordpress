# My Blog
[purrgramming.life](https://purrgramming.life/)

# Additional CSS

```css
/* Base styles for the body element */
body {  
    /* Styles for body element go here */
}

/* Automatic heading numbering */
/* Resets counters for nested headings */
h1 { counter-reset: h2counter; } /* Reset counter for h2 elements inside h1 */
h2 { counter-reset: h3counter; } /* Reset counter for h3 elements inside h2 */
h3 { counter-reset: h4counter; } /* Reset counter for h4 elements inside h3 */
h4 { counter-reset: h5counter; } /* Reset counter for h5 elements inside h4 */
h5 { counter-reset: h6counter; } /* Reset counter for h6 elements inside h5 */
h6 { /* Styles for h6 elements go here */ }

/* Adding numbering before each heading */
h2:before { 
    counter-increment: h2counter; 
    content: counter(h2counter) ".\0000a0\0000a0"; /* Number h2 elements and add space */
}
h3:before { 
    counter-increment: h3counter; 
    content: counter(h2counter) "." counter(h3counter) ".\0000a0\0000a0"; /* Number h3 elements and add space */
}
h4:before { 
    counter-increment: h4counter; 
    content: counter(h2counter) "." counter(h3counter) "." counter(h4counter) ".\0000a0\0000a0"; /* Number h4 elements and add space */
}
h5:before { 
    counter-increment: h5counter; 
    content: counter(h2counter) "." counter(h3counter) "." counter(h4counter) "." counter(h5counter) ".\0000a0\0000a0"; /* Number h5 elements and add space */
}
h6:before { 
    counter-increment: h6counter; 
    content: counter(h2counter) "." counter(h3counter) "." counter(h4counter) "." counter(h5counter) "." counter(h6counter) ".\0000a0\0000a0"; /* Number h6 elements and add space */
}

/* Styles for tables, table headers, and table cells */
table,
table th,
table td {
    border-style: solid;
    border-width: 1px;
    border-color: #d3d3d3 !important; /* Apply light gray border color */
}

/* Hide menu */
#menu {
    visibility: hidden;
    display: none; /* Hide the menu element */
}

/* Hide post navigation links */
.post-navigation .nav-links {
    visibility: hidden; /* Hide navigation links in posts */
}

/* Hide category links */
.cat-links {
    display: none; /* Hide category links in posts */
}

/* Hide comments link */
.comments-link {
    display: none; /* Hide comments link in posts */
}



/* Hide entry footer */
.entry-footer {
    display: none; /* Hide entry footer in posts */
}

a {
    color: #a3c1ad; /* Sets the hyperlink color to Cambridge Blue */
}

a:hover {
    color: #88a397; /* Optional: slightly darker shade of Cambridge Blue for hover effect */
}

```
