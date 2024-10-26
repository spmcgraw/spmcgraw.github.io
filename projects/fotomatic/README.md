# Fotomatic Project

The purpose of the project was to fix bugs on an existing webpage to make it responsive, and style it according to the [provided spec sheet](fotomatic_spec_landing_v3_.png).

Initial step was to review the HTML index.html file to ensure structure was complete.

Missing/Errornous items in HTML:

1. Missing lang in `<html>` element.
2. The `<head>` section was missing:
    1. Link to style.css file.
    2. The viewport meta tag for response design.
    3. The `<title>` element.
3. The `<body>` section was missing:
    1. Correct src links to images in the Features Section.
    2. The Quote Section comment was missing the proper closure.

CSS Corrections:

1. Universal Section:

    ```css
        .image-container img {
            max-width: 100%;
        }
    ```

2. Header Section:

    ```css
        header {
            z-index: 100;
        }

        header .content {
            height: 5.3125rem;
            padding: 0 1.875rem;
        }

        header .logo {
            color: #4a4a4a;
            font-size: 1.5rem;
            font-family: "Roboto Mono";
        }
    ```

3. Sign Up Section:

    ```css
        #sign-up-section {
            background-image: url("../images/banner-landingpage.jpg");
            background-position: bottom;
            background-size: cover;
            background-repeat: no-repeat;
        }

        #sign-up-cta {
            position: relative;
            top: 10.625rem;
            left: 10%;
        }
    ```

4. Feature Section Media >760px:

    ```css
        .feature .content {
            padding: 1.25rem 0 1.875rem 0;
        }
    ```

5. Filters Section:

    ```css
        #filters-section .content h2 {
            opacity: 100%;
        }

        #filters-section .images-container {
            display: flex;
        }
    ```

6. Quote Section (several of the classes were missing a **.**):

    ```css
        quotes-section .content {
            padding: 5rem 0;
        }

        #quotes-section .quote-citation {
            padding-left: 1.875rem;
        }
    ```
