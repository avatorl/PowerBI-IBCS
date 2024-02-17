Visualization design is based on IBCS guidlines: https://www.ibcs.com/ibcs-standards-1-2/

Not produced, not certified, not authorized, not endorsed by IBCS® https://www.ibcs.com/

### Bug: some charts are broken (e.g. missisng red/green bars, but text labels are visible)

If in you Language and Region settings decimal separator is a comma (e.g. European countries) and not a dot (e.g. the United States), update DAX measures to ensure only whole numbers (makes sense for pixels, but it makes sense to keep one decimal digit for % values) or only numbers with a dot decimal separator are being included into SVG code.

You can add <locale_name> parameter to ensure FORMAT function always uses the US format, e.g. FORMAT ( _WidthValue, "0.0%", "en-US" )

![image](https://github.com/avatorl/IBCS-for-Power-BI/assets/59934292/6f26e246-d797-4e90-a8ef-77aa8ae9aa0a)

