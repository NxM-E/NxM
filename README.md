🌐 Publier votre site web en ligne

Je vais vous montrer 3 méthodes simples et gratuites pour publier votre site :
Méthode 1 : Netlify (La plus facile) ⭐
Étape 1 : Préparez votre fichier
Créez un dossier ecommerce
Dedans, créez un fichier index.html avec le code complet
Zippez le dossier
Étape 2 : Uploadez sur Netlify
Allez sur netlify.com
Cliquez sur "Sign up" (inscrivez-vous gratuitement)
Cliquez sur "Drag and drop your site"
Glissez-déposez votre dossier ecommerce
✅ Votre site est en ligne !

Vous recevrez une URL comme : https://clever-gandalf-xyz123.netlify.app

Méthode 2 : GitHub Pages (Gratuit & Professionnel)
Étape 1 : Créez un compte GitHub
Allez sur github.com
Inscrivez-vous gratuitement
Cliquez sur "New Repository"
Étape 2 : Créez le repository
Repository name: [votre-nom].github.io
Description: Mon E-Commerce ShopHub
☑ Public
☑ Add a README file
Créer le repository
Étape 3 : Uploadez votre fichier
Cliquez sur "Add file" → "Upload files"
Uploadez votre index.html
Cliquez sur "Commit changes"
Étape 4 : Activez GitHub Pages
Allez dans Settings
Allez dans Pages (menu de gauche)
Sous "Source", sélectionnez "main branch"
Cliquez Save

✅ Votre site sera accessible à : https://[votre-nom].github.io

Méthode 3 : Vercel (Très rapide)

Allez sur vercel.com
Cliquez "Sign Up" avec GitHub
Cliquez "Create a Project"
Sélectionnez votre repository GitHub
Cliquez "Deploy"

✅ Déployé automatiquement !

Voici le code HTML complet à publier :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopHub - Votre E-Commerce</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #6366f1;
            --secondary: #ec4899;
            --dark: #1f2937;
            --light: #f9fafb;
            --border: #e5e7eb;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .nav-center {
            display: flex;
            gap: 2rem;
        }

        .nav-center a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-center a:hover {
            color: var(--primary);
        }

        .nav-right {
            display: flex;
            gap: 1.5rem;
            align-items: center;
        }

        .search-bar {
            display: flex;
            align-items: center;
            background: var(--light);
            padding: 0.5rem 1rem;
            border-radius: 25px;
            border: 1px solid var(--border);
        }

        .search-bar input {
            border: none;
            background: none;
            outline: none;
            width: 200px;
            font-size: 0.9rem;
        }

        .search-bar input::placeholder {
            color: #9ca3af;
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 1.3rem;
            transition: color 0.3s;
        }

        .cart-icon:hover {
            color: var(--primary);
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background: var(--secondary);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.7rem;
            font-weight: bold;
        }

        .hero {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 4rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .btn-primary {
            background: white;
            color: var(--primary);
            padding: 0.75rem 2rem;
            border: none;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            font-size: 1rem;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        .btn-secondary {
            background: var(--secondary);
            color: white;
            padding: 0.75rem 2rem;
            border: none;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s, background 0.3s;
            font-size: 1rem;
            margin-left: 1rem;
        }

        .btn-secondary:hover {
            background: #d1347a;
            transform: translateY(-2px);
        }

        .filters {
            background: white;
            padding: 2rem;
            max-width: 1200px;
            margin: -2rem auto 2rem;
            border-radius: 15px;
            display: flex;
            gap: 2rem;
            flex-wrap: wrap;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
        }

        .filter-group {
            display: flex;
            flex-direction: column;
            gap: 0.5rem;
        }

        .filter-group label {
            font-weight: 600;
            color: var(--dark);
        }

        .filter-group select,
        .filter-group input {
            padding: 0.5rem 1rem;
            border: 1px solid var(--border);
            border-radius: 8px;
            font-size: 0.9rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        .section-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .product-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }

        .product-image {
            width: 100%;
            height: 250px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
            position: relative;
            overflow: hidden;
        }

        .product-image.cat {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
        }

        .product-image.tech {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
        }

        .product-image.sport {
            background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
        }

        .badge {
            position: absolute;
            top: 10px;
            right: 10px;
            background: var(--secondary);
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }

        .product-info {
            padding: 1.5rem;
        }

        .product-name {
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }

        .product-desc {
            font-size: 0.85rem;
            color: #6b7280;
            margin-bottom: 1rem;
            line-height: 1.4;
        }

        .product-rating {
            color: #f59e0b;
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }

        .product-price {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1rem;
        }

        .price {
            font-size: 1.3rem;
            font-weight: bold;
            color: var(--primary);
        }

        .original-price {
            text-decoration: line-through;
            color: #9ca3af;
            font-size: 0.9rem;
        }

        .btn-add-cart {
            width: 100%;
            padding: 0.75rem;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn-add-cart:hover {
            background: #4f46e5;
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0,0,0,0.5);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: white;
            border-radius: 15px;
            width: 90%;
            max-width: 500px;
            padding: 2rem;
            max-height: 80vh;
            overflow-y: auto;
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
            border-bottom: 2px solid var(--border);
            padding-bottom: 1rem;
        }

        .modal-header h2 {
            font-size: 1.5rem;
        }

        .close-btn {
            font-size: 1.5rem;
            cursor: pointer;
            background: none;
            border: none;
            color: var(--dark);
        }

        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
            border-bottom: 1px solid var(--border);
        }

        .cart-item-info h4 {
            margin-bottom: 0.3rem;
        }

        .cart-item-price {
            font-weight: bold;
            color: var(--primary);
        }

        .remove-item {
            background: #ef4444;
            color: white;
            border: none;
            padding: 0.3rem 0.8rem;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.8rem;
        }

        .cart-summary {
            margin-top: 2rem;
            border-top: 2px solid var(--border);
            padding-top: 1rem;
        }

        .summary-row {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.5rem;
        }

        .summary-row.total {
            font-size: 1.3rem;
            font-weight: bold;
            color: var(--primary);
        }

        .checkout-btn {
            width: 100%;
            padding: 1rem;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-weight: bold;
            font-size: 1rem;
            margin-top: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }

        .checkout-btn:hover {
            background: #4f46e5;
        }

        .empty-cart {
            text-align: center;
            padding: 2rem;
            color: #6b7280;
        }

        footer {
            background: var(--dark);
            color
