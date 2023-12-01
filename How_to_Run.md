## How to Run the Web App

1. Open the terminal and navigate to the MedAdvisor folder.

2. Create a virtual environment:
   ```bash
   python -m venv env   # For Python 3.x
   ```

3. Activate the virtual environment:
   - For Linux/macOS:
     ```bash
     source env/bin/activate
     ```
   - For Windows:
     ```bash
     .\env\Scripts\activate
     ```
4. Install dependencies from `requirements.txt`:
   ```bash
   pip install -r requirements.txt  # for windows
   pip install -r requirements_os.txt  # for linux/macos
   ```

5. Navigate to the backend directory:
   ```bash
   cd backend
   ```

6. Run the Django development server:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   python manage.py runserver
   ```

   - For unit testing:
     ```bash
     python manage.py test
     ```

7. Open a new terminal in the same directory (MedAdvisor).

8. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

9. Serve/Start the React app:
   ```bash
   serve -s build
   ```

10. To Run Develpoment the React app:
   ```bash
   npm start
   ```

if somehow react app doest start ( error on npm start or on serve -s build ) 
- run these commands ( iff error shows on 9th or 10th step )
   ```bash
   rm -rf node_modules
   npm install
   npm start
   ```
