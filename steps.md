![github-header-image-6](https://github.com/user-attachments/assets/d71d9de6-6474-42e4-a51e-a47e4946c9c4)


<div align="left">

# Setting Up the NBA Data Lake

Follow these step-by-step instructions to set up and execute the NBA Data Lake project.

## 1. Open CloudShell
- On the console Home, navigate to the very bottom left corner and click **CloudShell**.
<img src="https://github.com/user-attachments/assets/3a08a0c3-de88-472a-8356-80c93ae03ffd" alt="image" width="400">

## 2. Create a Python File
- In CloudShell, type the following command to open a new file:
<img src="https://github.com/user-attachments/assets/c32d8e60-9d5e-4361-9d4a-e6d81e345cd3" alt="image" width="600">

  ```bash
  nano setup_nba_data_lake.py
  ```
  
- Copy and paste the provided `.py` code into the `nano` editor.
<img src="https://github.com/user-attachments/assets/d9775702-d3a2-45cf-8282-d91c05f55a97" alt="image" width="1500">

- Make the following changes in the script:
  - Update the **bucket name** as required.
  - Add your **API key** in the appropriate field.
  <img src="https://github.com/user-attachments/assets/7fc37e4f-9fb4-4348-9a20-94ae538eedb0" alt="image" width="900">

## 3. Configure the `.env` File
- Open the `.env` file in CloudShell:
  ```bash
  nano .env
  ```
<img src="https://github.com/user-attachments/assets/9dafc349-4334-49e3-b240-07d90bc224b4" alt="image" width="900">

- Copy and paste the following template into your `.env` file, replacing `<YOUR_API_KEY>` with your actual API key:
  ```env
  API_KEY=<YOUR_API_KEY>
  ```
  <img src="https://github.com/user-attachments/assets/93521765-01ea-46a2-8963-d4593d93c0ca" alt="image" width="900">

## 4. Install Required Dependencies
If the `dotenv` module is not installed in your environment, follow these steps:
<img src="https://github.com/user-attachments/assets/34c62356-cea5-424d-ab1b-e8a69c3b7273" alt="image" width="900">

- Install the `python-dotenv` module:
  ```bash
  pip install python-dotenv
  ```
- Verify the installation:
  ```bash
  pip show python-dotenv
  ```

- If you are using a virtual environment:
  ```bash
  source /path/to/venv/bin/activate
  pip install python-dotenv
  ```

- Run the Python script to set up the data lake:
  ```bash
  python setup_nba_data_lake.py
  ```
<img src="https://github.com/user-attachments/assets/f17e8cee-6a2d-46e8-a23a-aafe1c52a374" alt="image" width="700">

## 5. Verify the Bucket Creation
- Check the bucket that was created in your cloud storage service.
<img src="https://github.com/user-attachments/assets/af600ea3-43c3-4ae4-9f51-b84f24104dc5" alt="image" width="900">

- Verify that the bucket includes the following contents:
  - **Raw data** files.
  - A `.json` file.
  <img src="https://github.com/user-attachments/assets/bf770039-a917-4150-8c7b-fc09d5b39e76" alt="image" width="900">
  <img src="https://github.com/user-attachments/assets/d6d58753-9c94-4b84-9132-dcd91a2e39ca" alt="image" width="900">

## 6. Inspect the JSON File
- Open the `.json` file that was created and review its contents to ensure accuracy.
  <img src="https://github.com/user-attachments/assets/3b9b989b-d5bf-4e6f-a04f-1d75dd605ec8" alt="image" width="500">

</div>
