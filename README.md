# Art Day Discount On Art Work

Professional marketing email template offering a day-specific discount on art work, optimized for various screen sizes.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Art & Entertainment
- **Message Type:** Marketing
- **Tags:** discount, artwork, creative industry

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/art-day-discount-on-art-work.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/art-day-discount-on-art-work/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.art-day-discount-on-art-work',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
