# QR-code-generator
<h4>This project can be used to generate QR code provided link by the user and  the user can also download the QR code </h4>
<h1> Tech-stack used</h1>
<h2>HTML</h2>
<p>Used create the structure of the page</p>
<h2>CSS</h2>
<p>used to give additional design</p>
<h2>Java Script</h2>
<p>use to give the functionality and logic</p>
<h1>Logic used in this project</h1>
<h2>Dom element selection</h2>
<ol>The code begins by selecting various elements from the HTML DOM using document.getElementById and document.querySelector methods. These elements </ol>
<ol>qrText: Input field for entering text or URL.
</ol>
<ol>sizes: Select element for choosing the size of the QR code.
</ol>
<ol>generateBtn: Button for generating the QR code.
</ol>
<ol>downloadBtn: Button for downloading the generated QR code.
</ol>
<ol>qrContainer: Container for displaying the generated QR code.
</ol>
<h2>Event listeners</h2>
<ol>An event listener is added to the generateBtn button. When clicked, it prevents the default behavior (form submission, in this case) and calls the isEmptyInput function.
</ol>
<ol>Another event listener is added to the sizes select element. When the selected size changes, it updates the size variable and calls the isEmptyInput function.
</ol>
<h2>Download Functionality:</h2>
<ol>An event listener is added to the downloadBtn button. When clicked, it checks if an <img> element with the QR code exists in the .qr-body container. If it exists, it retrieves the source attribute (src) of the image and sets it as the download link (href) for the download button.</ol>
<ol>If no <img> element exists (i.e., the QR code is generated as a canvas), it converts the canvas data to a data URL using toDataURL() method and sets it as the download link.</ol>
<h2>Helper Functions:</h2>
<ol>isEmptyInput function checks if the qrText input field is empty or not. If it's not empty, it calls the generateQRCode function. Otherwise, it alerts the user to enter text or a URL.
</ol>
<ol>generateQRCode function clears the content of the qrContainer, then generates a new QR code using the QRCode constructor. It takes the input value from qrText, the selected size from the sizes dropdown, and sets light and dark colors for the QR code.
</ol>

