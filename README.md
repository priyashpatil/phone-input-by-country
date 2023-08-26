# Phone Input by Country

The "Phone Input by Country" is a freely available package that integrates seamlessly with Bootstrap 5. This integration simplifies the process of adding country-specific phone input fields, complete with uncomplicated validation.

<p align="center">
  <img src="marketing/demo.gif" alt="Phone Input by Country Demo">
</p>

## How to Use

To get started, include the following CDN links in the `<head>` section of your HTML document and the JavaScript link just before the closing `</body>` tag:

```html
<link href="https://cdn.jsdelivr.net/gh/priyashpatil/phone-input-by-country@0.0.1/cpi.css" rel="stylesheet" crossorigin="anonymous" referrerpolicy="no-referrer">
```

```html
<script src="https://cdn.jsdelivr.net/gh/priyashpatil/phone-input-by-country@0.0.1/cpi.js" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```

Next, insert the provided HTML code as shown below:

```html
<div class="cpi-input">
    <div class="input-group mb-3 border rounded">
        <button class="btn btn-light dropdown-toggle d-flex align-items-center cpi-drop" type="button" data-bs-toggle="dropdown" aria-expanded="false">
            <span class="me-1">🇮🇳</span>
        </button>
        <div class="dropdown-menu w-100">
            <button type="button" class="dropdown-item" data-cpi-icon="🇮🇳" data-cpi-ext="+91" data-cpi-min-length="10" data-cpi-max-length="10">
                🇮🇳 India (+91)
            </button>
            <button type="button" class="dropdown-item" data-cpi-icon="🇦🇪" data-cpi-ext="+971" data-cpi-min-length="8" data-cpi-max-length="9">
                🇦🇪 United Arab Emirates (+971)
            </button>
        </div>
        <span class="input-group-text bg-white text-muted border-0 cpi-ext-txt">+91</span>
        <input type="text" class="form-control border-0 phone-input flex-shrink-1" style="outline: none;" pattern="[0-9]+" required minlength="10" maxlength="10" title="Enter a valid mobile number">
    </div>
    <input type="hidden" class="country-code-input">
</div>
```

Feel free to customize the appearance and behavior of the dropdown menu as desired. The attributes `cpi-icon` and `cpi-ext` are utilized for rendering data, while `cpi-min-length` and `cpi-max-length` aid in HTML form validation.