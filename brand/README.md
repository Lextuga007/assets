# brand.yml

Following Posit's addition of a [`_brand.yml` file](https://posit-dev.github.io/brand-yml/) 
to help with applying consistent branding across Quarto, Python or R we have set
this up for NHS-R Community branding.

NHS-R Community uses NHS England colours for its slides and books.
Details are in the [branding chapter](https://nhsrway.nhsrcommunity.com/style-guides.html#branding)
of NHS-R Way.

Whilst the NHS blues are the most familiar, NHS-R Community often uses the 
highlight colours.

Although NHS England has possibly checked the accessibility of colours we advise
that you always consider the contrast combination when using the colours and 
check any outputs.

## Logo

If you need to use the NHS-R Community logo (or wish to use another NHS logo for
any official outputs) you will need to remove the comment hashes from the 
`_brand_yml` file and ensure that the logo file is saved wherever the `_brand.yml`
file is.

The NHS-R Community logos can be found in the 
[folder `logo`](https://github.com/nhs-r-community/assets/tree/main/logo) in 
this GitHub repository.

If you'd prefer to link directly using a url, this currently isn't possible to 
do through the `_brand.yml` file but for Quarto can be added to the `_quarto.yml`
file as:

```
# For presentations
format:
  revealjs:
  logo: https://raw.githubusercontent.com/nhs-r-community/assets/main/logo/nhsr-logo.svg
```

## Quarto

If you are using a Quarto file, to apply the branding:

1) Place `_quarto.yml` within a Quarto project (an example
being the [NHS-R Community presentations](https://github.com/nhs-r-community/NHSR-presentations/blob/main/_quarto.yml)). 

2) Then refer to the `_brand.yml` file in the `_quarto.yml` file by adding the code:

```
brand: _brand.yml
```


