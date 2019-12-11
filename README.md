Note: this file is auto converted from company-posframe.el by [el2org](https://github.com/tumashu/el2org), please do not edit it by hand!!!


# &#30446;&#24405;

1.  [company-posframe README](#org74d467d)
    1.  [What is company-posframe](#org1437d45)
    2.  [How to use company-posframe](#orge5fbefd)
    3.  [Tips](#org2b1e129)
        1.  [Work better with desktop.el](#orge3339a4)
        2.  [Work better with company-quickhelp](#org331ba19)
    4.  [Note](#org685c4a7)


<a id="org74d467d"></a>

# company-posframe README


<a id="org1437d45"></a>

## What is company-posframe

company-posframe is a company extension, which let company use
child frame as its candidate menu.

It has the following feature:

1.  It is fast enough for daily use.
2.  It works well with CJK language.

**At the moment**, company-posframe can not work well with:

1.  company-quickhelp


<a id="orge5fbefd"></a>

## How to use company-posframe

    (require 'company-posframe)
    (company-posframe-mode 1)


<a id="org2b1e129"></a>

## Tips


<a id="orge3339a4"></a>

### Work better with desktop.el

The below code let desktop.el not record the company-posframe-mode

    (require 'desktop) ;this line is needed.
    (push '(company-posframe-mode . nil)
          desktop-minor-mode-table)


<a id="org331ba19"></a>

### Work better with company-quickhelp

    (require 'company-quickhelp)
    (require 'company-posframe)
    (require 'company-posframe-quickhelp)


<a id="org685c4a7"></a>

## Note

company-posframe.el is derived from Clément Pit-Claudel's
company-tooltip.el, which can be found at:

<https://github.com/company-mode/company-mode/issues/745#issuecomment-357138511>

