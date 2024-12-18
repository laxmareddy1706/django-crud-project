# **Django CRUD Application**

This is a simple Django-based CRUD (Create, Read, Update, Delete) application that allows users to manage a list of items. Each item has a name and description, and the app includes basic styling and functionality to perform all CRUD operations.

---

## **Features**
- **Add Items**: Create a new item with a name and description.
- **View Items**: List all existing items with options to edit or delete.
- **Edit Items**: Update the details of an existing item.
- **Delete Items**: Remove an item after confirmation.

---

## **Requirements**
- Python 3.10 or higher
- Django 5.1.4

---

## **Setup Instructions**

### **Step 1: Clone the Repository**
Clone the project repository to your local machine:
```bash
git clone <repository_url>
cd <repository_folder>
```

### **Step 2: Set Up a Virtual Environment**
Create and activate a virtual environment:
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### **Step 3: Install Dependencies**
Install the required Python packages:
```bash
pip install django
```

### **Step 4: Run Migrations**
Set up the database by running migrations:
```bash
python manage.py makemigrations
python manage.py migrate
```

### **Step 5: Start the Development Server**
Run the Django development server:
```bash
python manage.py runserver
```

Visit the app in your browser at [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

---

## **File Structure**
Below is an overview of the key files and folders:

```
assignment/
├── assignment/
│   ├── settings.py         # Project settings
│   ├── urls.py             # Root URL configuration
│   ├── wsgi.py             # WSGI configuration
│
├── items/
│   ├── migrations/         # Database migration files
│   ├── templates/
│   │   ├── items/
│   │   │   ├── item_form.html        # Create/Edit item form
│   │   │   ├── item_list.html        # Item list page
│   │   │   ├── item_confirm_delete.html  # Delete confirmation
│   ├── views.py            # CRUD view logic
│   ├── models.py           # Item model definition
│   ├── forms.py            # Item form
│   ├── urls.py             # URLs for the items app
│
├── templates/
│   ├── base.html           # Base HTML template
│
├── manage.py               # Django project management
```

---

## **How to Use**
1. Navigate to the home page to view a list of all items.
2. Click "Create Item" to add a new item.
3. Use the "Edit" button to update an existing item.
4. Use the "Delete" button to remove an item (confirmation required).

---

## **Future Enhancements**
- Add user authentication for item management.
- Include pagination for the item list.
- Improve the UI with advanced CSS or a framework like Bootstrap.
- Add search functionality for items.

---

