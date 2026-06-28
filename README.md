# 📚 Archieving  App (Django)

A secure document management system that allows users to:

- Browse and search technical reports
- View PDF files securely using token-based access
- Prevent unauthorized downloading
- Use query filters (company, report type, year, author)
- Support both Arabic and English UI

## 🔐 Secure PDF Viewer

The PDF delivery route ensures:

- Token validation
- No direct file download without permission
- Temporary signed URLs (Django signing module)
- Files stored in protected folder

## 🚀 Features

- Full-text search across title, keywords, references (Arabic + English)
- Secure media handling
- Django + SQL Server optimized queries
- Pagination + Filters + Company-based grouping
- Support for SGS internal library access control

## 🧩 Tech Stack

- **Backend**: Django  
- **Database**: SQL Server  
- **Frontend**: Django Templates  
- **Security**: Signed token access  
- **Language**: Multi-language support with Django locale  

## 🛠 Installation

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
🏗 Folder Structure
bibliodb/
 ├── bibliodb/        # Main Django project
 ├── templates/       # HTML templates
 ├── static/          # Static assets
 ├── media/           # (Ignored) uploaded PDFs
 ├── reports/         # (Ignored) generated reports
 ├── manage.py
 ├── requirements.txt
 ├── run_server.py


🔒 Secure PDF Opening

The application uses:
signing.dumps()
signing.loads()


to generate limited-time access tokens for PDFs stored in media/.

👨‍💻 Author

Ahmed Shehta (https://ahmed-shehta.netlify.app)







