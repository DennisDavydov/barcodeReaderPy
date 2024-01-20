
# Barcode Reader Project

This project is a barcode reader application that connects to a MySQL database to store product information. It uses OpenCV for barcode scanning, tkinter for the graphical user interface, and pygame for sound effects. The project allows you to scan barcodes, view product details, and add or remove products from the database.

This project is primarily made to work with my [inventory server](https://github.com/DennisDavydov/homeinventory), but is useable as a standalone application too.


## Features

- Barcode scanning using a webcam.
- Display product details based on the scanned barcode.
- Add new products to the database.
- Remove products from the database.
- Calendar widget for selecting expiration dates.

## Technologies Used

- Python
- OpenCV (cv2)
- PyZbar (barcode decoding)
- Tkinter (GUI)
- MySQL database
- Pygame (sound effects)
- Pillow (PIL) for image manipulation
- tkcalendar (for the calendar widget)

## Setup

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/barcode-reader-project.git
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up a MySQL database and configure the connection details in `barcodeRead.py` and `dbFunctions.py`.

4. Run the `barcodeRead.py` script to start the application:

   ```bash
   python barcodeRead.py
   ```

## Usage

- Launch the application and use your webcam to scan product barcodes.
- Product details will be displayed on the screen if the barcode is found in the database.
- You can add new products by filling in the product details and clicking the "Add" button.
- To remove a product, scan its barcode and click the "Remove" button.
- Use the calendar widget to select expiration dates.

## Database Functions

- `insert_data`: Inserts product data into the database.
- `check_database`: Checks if a product with the given barcode exists in the database.
- `select_data`: Retrieves product details from the database based on the barcode.
- `remove_product`: Removes a product from the database based on the barcode and, optionally, the expiration date.

## Acknowledgments

- This project uses various open-source libraries and tools, including OpenCV, PyZbar, Tkinter, and more.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## Author

- [DennisDavydov](https://github.com/DennisDavydov)
