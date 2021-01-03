# Bootstrap 4 From Scratch With 5 Projects

Master Bootstrap 4 and build 5 real world themes while learning HTML5 semantics & CSS3

# Bootstrap/ basic file structure

```
├── css/
│ ├── bootstrap.css
│ ├── bootstrap.css.map
│ ├── bootstrap.min.css
│ ├── bootstrap-theme.css
│ ├── bootstrap-theme.css.map
│ └── bootstrap-theme.min.css
├── js/
│ ├── bootstrap.js
│ └── bootstrap.min.js
└── fonts/
├── glyphicons-halflings-regular.eot
├── glyphicons-halflings-regular.svg
├── glyphicons-halflings-regular.ttf
├── glyphicons-halflings-regular.woff
└── glyphicons-halflings-regular.woff2
```

# About bootstrap

- Open source front-end framework for fast web development.
- Pre-made HTML/CSS templates and classes.
- Javascript widgets and plugins.
- Mobile first responsive layout.

# How to install /Use Bootstrap

- Include the CDN.
- Download & Include Files
- Package mangaers - NPM/ Yarn

# UI Utiliteis

- Grid System
- Text & typography
- Positioning
- Spacing
- Sizing
- Alighnment
- Colors
- images
- Responsive Layouts
- shadows

# CSS Components

- Forms & Input Groups
- Tables
- List Groups
- Cards
- Progress Bars
- Alerts
- Navbar & menus
- Buttons an Buttons groups
- Paginations
- Media objects
- Jumbotron
- badges

# Javascript Widjets

- Carousel Slider
- Collpsible Accordion
- modals
- Toolpits
- Popovers
- ScrollSpy

# Improved Grid system and layouts Compared to Previous version of Bootstrap.

- Changes in the underlying architeture
- rem & em units instead of pixels.
- New -xl tier for extra large scrrens
- Grid noow uses flexbox.

# Flexbox

- Include flexbox utilities
- Use flexbox to manage grids, navigation,components and more
- Display utilities can trenform childern into flex items.
- <div class="d-flex p-2">I'm a flexbox container!</div>

# cards

- Cards replace Panels, wells and thumnails
- Uses flexbox
- get same behaviour with modifiers
- .card-body instead of .well
- Use .card-title for titles
- Image headings

# Changes to Navbar

- Wrapping .navbar with .navbar-expand{-sm|-md|-lg|-xl} for responsive collapse

# Form Changes

- Dropped the .form-horizonal class.
- Forms using grids require the .row class abd can use .col-form-label for labels
- Use .form-control-lg and .form-control-sm to increase and decrease size of input control.

# rem vs em

- 1 rem = 16px

# Bootstrap screen sizes

- Bootsrap has basicall four diffrent screen sizes
  1.  sm - Small
  2.  md - Medium
  3.  lg - large
  4.  xl - xtra large

# Important Notes

- clearfix will claer the float in between.
- If we want to change the color for links , the class should be in the link.

# list group badges and breadcrums are important topics

```
Here are all the classes from Bootstrap 3 (version 3.1.1).

Method of extraction:

1.  Download Bootstrap 3 and rename bootstrap.css as "bootstrap.html"
2.  Add the following 24 lines of code to the very bottom of the bootstrap.html file:

    <script src="http://code.jquery.com/jquery-1.11.0.min.js"></script>
    <script src="http://cdnjs.cloudflare.com/ajax/libs/lodash.js/2.4.1/lodash.min.js"></script>
    <script>
        $("script").empty();  //use jQuery remove script element text before analysis
        var bootstrapCSS = $("body").text(); //grab all text on the page (all bootstrap css)
        bootstrapCSS = bootstrapCSS.replace(
                /(\/\*([^*]|[\r\n]|(\*+([^*\/]|[\r\n])))*\*+\/)|(\/\/.*)/g, ""
        ); // remove comments from the css
        bootstrapCSS = bootstrapCSS.replace(
                /(@media.*\{)/g, ""
        ); // remove media query lines up to and including first open brace
        bootstrapCSS = bootstrapCSS.replace(
                /(\{[^}]+\})/g, ""
        ); // remove all css in between braces
        var res = bootstrapCSS.match(
             /([\.][\w]+([-][\w]*)*)/g
        ); // match .classnames with any number of dashes
        res = _.uniq(res); //use lo-dash uniq() method to pull out duplicates
        res = res.sort(); //sort alphabetically (not case sensitive, but no real need)
        $("body").empty(); //empty the page before redisplay
        for (var i = 0; i < res.length; i++) {
            $("body").append(res[i]+"<br>"); //append each unique class name back to DOM
        }
    </script>

3.  Open the bootstrap.html file in a modern browser (tested in Chrome).


.active
.affix
.alert
.alert-danger
.alert-dismissable
.alert-info
.alert-link
.alert-success
.alert-warning
.arrow
.badge
.bg-danger
.bg-info
.bg-primary
.bg-success
.bg-warning
.blockquote-reverse
.bottom
.bottom-left
.bottom-right
.breadcrumb
.btn
.btn-block
.btn-danger
.btn-default
.btn-group
.btn-group-justified
.btn-group-lg
.btn-group-sm
.btn-group-vertical
.btn-group-xs
.btn-info
.btn-lg
.btn-link
.btn-primary
.btn-sm
.btn-success
.btn-toolbar
.btn-warning
.btn-xs
.caption
.caret
.carousel
.carousel-caption
.carousel-control
.carousel-indicators
.carousel-inner
.center-block
.checkbox
.checkbox-inline
.clearfix
.close
.col-lg-1
.col-lg-10
.col-lg-11
.col-lg-12
.col-lg-2
.col-lg-3
.col-lg-4
.col-lg-5
.col-lg-6
.col-lg-7
.col-lg-8
.col-lg-9
.col-lg-offset-0
.col-lg-offset-1
.col-lg-offset-10
.col-lg-offset-11
.col-lg-offset-12
.col-lg-offset-2
.col-lg-offset-3
.col-lg-offset-4
.col-lg-offset-5
.col-lg-offset-6
.col-lg-offset-7
.col-lg-offset-8
.col-lg-offset-9
.col-lg-pull-0
.col-lg-pull-1
.col-lg-pull-10
.col-lg-pull-11
.col-lg-pull-12
.col-lg-pull-2
.col-lg-pull-3
.col-lg-pull-4
.col-lg-pull-5
.col-lg-pull-6
.col-lg-pull-7
.col-lg-pull-8
.col-lg-pull-9
.col-lg-push-0
.col-lg-push-1
.col-lg-push-10
.col-lg-push-11
.col-lg-push-12
.col-lg-push-2
.col-lg-push-3
.col-lg-push-4
.col-lg-push-5
.col-lg-push-6
.col-lg-push-7
.col-lg-push-8
.col-lg-push-9
.col-md-1
.col-md-10
.col-md-11
.col-md-12
.col-md-2
.col-md-3
.col-md-4
.col-md-5
.col-md-6
.col-md-7
.col-md-8
.col-md-9
.col-md-offset-0
.col-md-offset-1
.col-md-offset-10
.col-md-offset-11
.col-md-offset-12
.col-md-offset-2
.col-md-offset-3
.col-md-offset-4
.col-md-offset-5
.col-md-offset-6
.col-md-offset-7
.col-md-offset-8
.col-md-offset-9
.col-md-pull-0
.col-md-pull-1
.col-md-pull-10
.col-md-pull-11
.col-md-pull-12
.col-md-pull-2
.col-md-pull-3
.col-md-pull-4
.col-md-pull-5
.col-md-pull-6
.col-md-pull-7
.col-md-pull-8
.col-md-pull-9
.col-md-push-0
.col-md-push-1
.col-md-push-10
.col-md-push-11
.col-md-push-12
.col-md-push-2
.col-md-push-3
.col-md-push-4
.col-md-push-5
.col-md-push-6
.col-md-push-7
.col-md-push-8
.col-md-push-9
.col-sm-1
.col-sm-10
.col-sm-11
.col-sm-12
.col-sm-2
.col-sm-3
.col-sm-4
.col-sm-5
.col-sm-6
.col-sm-7
.col-sm-8
.col-sm-9
.col-sm-offset-0
.col-sm-offset-1
.col-sm-offset-10
.col-sm-offset-11
.col-sm-offset-12
.col-sm-offset-2
.col-sm-offset-3
.col-sm-offset-4
.col-sm-offset-5
.col-sm-offset-6
.col-sm-offset-7
.col-sm-offset-8
.col-sm-offset-9
.col-sm-pull-0
.col-sm-pull-1
.col-sm-pull-10
.col-sm-pull-11
.col-sm-pull-12
.col-sm-pull-2
.col-sm-pull-3
.col-sm-pull-4
.col-sm-pull-5
.col-sm-pull-6
.col-sm-pull-7
.col-sm-pull-8
.col-sm-pull-9
.col-sm-push-0
.col-sm-push-1
.col-sm-push-10
.col-sm-push-11
.col-sm-push-12
.col-sm-push-2
.col-sm-push-3
.col-sm-push-4
.col-sm-push-5
.col-sm-push-6
.col-sm-push-7
.col-sm-push-8
.col-sm-push-9
.col-xs-1
.col-xs-10
.col-xs-11
.col-xs-12
.col-xs-2
.col-xs-3
.col-xs-4
.col-xs-5
.col-xs-6
.col-xs-7
.col-xs-8
.col-xs-9
.col-xs-offset-0
.col-xs-offset-1
.col-xs-offset-10
.col-xs-offset-11
.col-xs-offset-12
.col-xs-offset-2
.col-xs-offset-3
.col-xs-offset-4
.col-xs-offset-5
.col-xs-offset-6
.col-xs-offset-7
.col-xs-offset-8
.col-xs-offset-9
.col-xs-pull-0
.col-xs-pull-1
.col-xs-pull-10
.col-xs-pull-11
.col-xs-pull-12
.col-xs-pull-2
.col-xs-pull-3
.col-xs-pull-4
.col-xs-pull-5
.col-xs-pull-6
.col-xs-pull-7
.col-xs-pull-8
.col-xs-pull-9
.col-xs-push-0
.col-xs-push-1
.col-xs-push-10
.col-xs-push-11
.col-xs-push-12
.col-xs-push-2
.col-xs-push-3
.col-xs-push-4
.col-xs-push-5
.col-xs-push-6
.col-xs-push-7
.col-xs-push-8
.col-xs-push-9
.collapse
.collapsing
.container
.container-fluid
.control-label
.danger
.disabled
.divider
.dl-horizontal
.dropdown
.dropdown-backdrop
.dropdown-header
.dropdown-menu
.dropdown-menu-left
.dropdown-menu-right
.dropdown-toggle
.dropup
.fade
.form-control
.form-control-feedback
.form-control-static
.form-group
.form-horizontal
.form-inline
.glyphicon
.glyphicon-adjust
.glyphicon-align-center
.glyphicon-align-justify
.glyphicon-align-left
.glyphicon-align-right
.glyphicon-arrow-down
.glyphicon-arrow-left
.glyphicon-arrow-right
.glyphicon-arrow-up
.glyphicon-asterisk
.glyphicon-backward
.glyphicon-ban-circle
.glyphicon-barcode
.glyphicon-bell
.glyphicon-bold
.glyphicon-book
.glyphicon-bookmark
.glyphicon-briefcase
.glyphicon-bullhorn
.glyphicon-calendar
.glyphicon-camera
.glyphicon-certificate
.glyphicon-check
.glyphicon-chevron-down
.glyphicon-chevron-left
.glyphicon-chevron-right
.glyphicon-chevron-up
.glyphicon-circle-arrow-down
.glyphicon-circle-arrow-left
.glyphicon-circle-arrow-right
.glyphicon-circle-arrow-up
.glyphicon-cloud
.glyphicon-cloud-download
.glyphicon-cloud-upload
.glyphicon-cog
.glyphicon-collapse-down
.glyphicon-collapse-up
.glyphicon-comment
.glyphicon-compressed
.glyphicon-copyright-mark
.glyphicon-credit-card
.glyphicon-cutlery
.glyphicon-dashboard
.glyphicon-download
.glyphicon-download-alt
.glyphicon-earphone
.glyphicon-edit
.glyphicon-eject
.glyphicon-envelope
.glyphicon-euro
.glyphicon-exclamation-sign
.glyphicon-expand
.glyphicon-export
.glyphicon-eye-close
.glyphicon-eye-open
.glyphicon-facetime-video
.glyphicon-fast-backward
.glyphicon-fast-forward
.glyphicon-file
.glyphicon-film
.glyphicon-filter
.glyphicon-fire
.glyphicon-flag
.glyphicon-flash
.glyphicon-floppy-disk
.glyphicon-floppy-open
.glyphicon-floppy-remove
.glyphicon-floppy-save
.glyphicon-floppy-saved
.glyphicon-folder-close
.glyphicon-folder-open
.glyphicon-font
.glyphicon-forward
.glyphicon-fullscreen
.glyphicon-gbp
.glyphicon-gift
.glyphicon-glass
.glyphicon-globe
.glyphicon-hand-down
.glyphicon-hand-left
.glyphicon-hand-right
.glyphicon-hand-up
.glyphicon-hd-video
.glyphicon-hdd
.glyphicon-header
.glyphicon-headphones
.glyphicon-heart
.glyphicon-heart-empty
.glyphicon-home
.glyphicon-import
.glyphicon-inbox
.glyphicon-indent-left
.glyphicon-indent-right
.glyphicon-info-sign
.glyphicon-italic
.glyphicon-leaf
.glyphicon-link
.glyphicon-list
.glyphicon-list-alt
.glyphicon-lock
.glyphicon-log-in
.glyphicon-log-out
.glyphicon-magnet
.glyphicon-map-marker
.glyphicon-minus
.glyphicon-minus-sign
.glyphicon-move
.glyphicon-music
.glyphicon-new-window
.glyphicon-off
.glyphicon-ok
.glyphicon-ok-circle
.glyphicon-ok-sign
.glyphicon-open
.glyphicon-paperclip
.glyphicon-pause
.glyphicon-pencil
.glyphicon-phone
.glyphicon-phone-alt
.glyphicon-picture
.glyphicon-plane
.glyphicon-play
.glyphicon-play-circle
.glyphicon-plus
.glyphicon-plus-sign
.glyphicon-print
.glyphicon-pushpin
.glyphicon-qrcode
.glyphicon-question-sign
.glyphicon-random
.glyphicon-record
.glyphicon-refresh
.glyphicon-registration-mark
.glyphicon-remove
.glyphicon-remove-circle
.glyphicon-remove-sign
.glyphicon-repeat
.glyphicon-resize-full
.glyphicon-resize-horizontal
.glyphicon-resize-small
.glyphicon-resize-vertical
.glyphicon-retweet
.glyphicon-road
.glyphicon-save
.glyphicon-saved
.glyphicon-screenshot
.glyphicon-sd-video
.glyphicon-search
.glyphicon-send
.glyphicon-share
.glyphicon-share-alt
.glyphicon-shopping-cart
.glyphicon-signal
.glyphicon-sort
.glyphicon-sort-by-alphabet
.glyphicon-sort-by-alphabet-alt
.glyphicon-sort-by-attributes
.glyphicon-sort-by-attributes-alt
.glyphicon-sort-by-order
.glyphicon-sort-by-order-alt
.glyphicon-sound-5-1
.glyphicon-sound-6-1
.glyphicon-sound-7-1
.glyphicon-sound-dolby
.glyphicon-sound-stereo
.glyphicon-star
.glyphicon-star-empty
.glyphicon-stats
.glyphicon-step-backward
.glyphicon-step-forward
.glyphicon-stop
.glyphicon-subtitles
.glyphicon-tag
.glyphicon-tags
.glyphicon-tasks
.glyphicon-text-height
.glyphicon-text-width
.glyphicon-th
.glyphicon-th-large
.glyphicon-th-list
.glyphicon-thumbs-down
.glyphicon-thumbs-up
.glyphicon-time
.glyphicon-tint
.glyphicon-tower
.glyphicon-transfer
.glyphicon-trash
.glyphicon-tree-conifer
.glyphicon-tree-deciduous
.glyphicon-unchecked
.glyphicon-upload
.glyphicon-usd
.glyphicon-user
.glyphicon-volume-down
.glyphicon-volume-off
.glyphicon-volume-up
.glyphicon-warning-sign
.glyphicon-wrench
.glyphicon-zoom-in
.glyphicon-zoom-out
.h1
.h2
.h3
.h4
.h5
.h6
.has-error
.has-feedback
.has-success
.has-warning
.help-block
.hidden
.hidden-lg
.hidden-md
.hidden-print
.hidden-sm
.hidden-xs
.hide
.icon-bar
.icon-next
.icon-prev
.img-circle
.img-responsive
.img-rounded
.img-thumbnail
.in
.info
.initialism
.input-group
.input-group-addon
.input-group-btn
.input-group-lg
.input-group-sm
.input-lg
.input-sm
.invisible
.item
.jumbotron
.label
.label-danger
.label-default
.label-info
.label-primary
.label-success
.label-warning
.lead
.left
.list-group
.list-group-item
.list-group-item-danger
.list-group-item-heading
.list-group-item-info
.list-group-item-success
.list-group-item-text
.list-group-item-warning
.list-inline
.list-unstyled
.media
.media-body
.media-heading
.media-list
.media-object
.modal
.modal-backdrop
.modal-body
.modal-content
.modal-dialog
.modal-footer
.modal-header
.modal-lg
.modal-open
.modal-sm
.modal-title
.nav
.nav-divider
.nav-justified
.nav-pills
.nav-stacked
.nav-tabs
.nav-tabs-justified
.navbar
.navbar-brand
.navbar-btn
.navbar-collapse
.navbar-default
.navbar-fixed-bottom
.navbar-fixed-top
.navbar-form
.navbar-header
.navbar-inverse
.navbar-left
.navbar-link
.navbar-nav
.navbar-right
.navbar-static-top
.navbar-text
.navbar-toggle
.next
.open
.page-header
.pager
.pagination
.pagination-lg
.pagination-sm
.panel
.panel-body
.panel-collapse
.panel-danger
.panel-default
.panel-footer
.panel-group
.panel-heading
.panel-info
.panel-primary
.panel-success
.panel-title
.panel-warning
.popover
.popover-content
.popover-title
.pre-scrollable
.prev
.previous
.progress
.progress-bar
.progress-bar-danger
.progress-bar-info
.progress-bar-success
.progress-bar-warning
.progress-striped
.pull-left
.pull-right
.radio
.radio-inline
.right
.row
.show
.small
.sr-only
.success
.tab-content
.tab-pane
.table
.table-bordered
.table-condensed
.table-hover
.table-responsive
.table-striped
.text-center
.text-danger
.text-hide
.text-info
.text-justify
.text-left
.text-muted
.text-primary
.text-right
.text-success
.text-warning
.thumbnail
.tooltip
.tooltip-arrow
.tooltip-inner
.top
.top-left
.top-right
.visible-lg
.visible-md
.visible-print
.visible-sm
.visible-xs
.warning
.well
.well-lg
.well-sm
```
