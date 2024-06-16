---


---

<h1 id="module-1-capstone---vending-machine-software--v-1.0.0">Module 1 Capstone - Vending Machine Software  (V 1.0.0)</h1>
<p>You’re developing an application for the newest vending machine distributor, Umbrella Corp. They’ve released a new vending machine, Vendo-Matic 800, that’s integrated with everyone’s bank accounts, allowing customers to purchase products from their computers for their convenience.</p>
<p>See: <a href="https://docs.google.com/document/d/1XaVVdYm9wQ1N09_7VvX2BDrTVYbfGDa0tWz2zNUwDrU/edit">User Stories</a>, <a href="https://trello.com/invite/b/dDOmyVq9/ATTI3c72f8159df94a0b48e0645c265d4ee3546DA34C/vending-machine-software">Trello Board</a></p>
<p>Classes require to develop the vending machine software as well as their Test classes.</p>

<table>
<thead>
<tr>
<th>Property</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>ProductType</code></td>
<td>Manages the type associated with each product</td>
</tr>
<tr>
<td><code>Product</code></td>
<td>Represents an item in the vending machine</td>
</tr>
<tr>
<td><code>Quantity</code></td>
<td>The default maximum quantity a slot holds per product</td>
</tr>
<tr>
<td><code>AbstractVendingMachine</code></td>
<td>Manages the inventory and operations of the vending machine</td>
</tr>
<tr>
<td><code>StandardVendingMachine</code></td>
<td>Manages the inventory and operations of the vending machine</td>
</tr>
<tr>
<td><code>SalesReport</code></td>
<td>Generates sales reports</td>
</tr>
<tr>
<td><code>Transaction</code></td>
<td>Manages logging of transactions</td>
</tr>
<tr>
<td><code>Application</code></td>
<td>The main class to run the application</td>
</tr>
<tr>
<td></td>
<td></td>
</tr>
<tr>
<td><code>SalesReportTest</code></td>
<td>Test cases for SalesReport Class</td>
</tr>
<tr>
<td><code>TransactionTest</code></td>
<td>Test cases for Transaction  Class</td>
</tr>
<tr>
<td><code>StandardVendingMachineTest</code></td>
<td>Test cases for VendingMachine Class</td>
</tr>
</tbody>
</table><h2 id="classes">Classes</h2>
<p>The core of this application consists of <code>4 packages</code>, <code>product</code>, <code>report</code>, <code>transaction</code>, and <code>vendingmachine</code> and their respective <code>Classes</code> see above. These classes, including an <code>Enum</code> and an <code>Abstract Class</code> will be created in the subclasses of the main package <code>com.techelevator</code>. Make sure to read through the requirements for each class before writing any code.</p>
<h3 id="step-one-create-the-producttype-enum-class-in-the-com.techelevator.product-package">Step One: Create the <code>ProductType</code> Enum class in the <code>com.techelevator.product</code> package</h3>
<p>Create a new enum class called <code>ProductType.java</code> with the following requirements. The enum has 4 constants. Each constant represents a type of product.</p>
<h4 id="enum-constants">Enum Constants</h4>
<p><code>CHIP</code>, <code>CANDY</code>, <code>DRINK</code>, <code>GUM</code></p>
<h4 id="properties">Properties</h4>

<table>
<thead>
<tr>
<th>Property</th>
<th>Data Type</th>
<th>Get</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>message</code></td>
<td><code>String</code></td>
<td>X</td>
<td>This variable holds the message each enum type</td>
</tr>
</tbody>
</table><h4 id="constructors">Constructors</h4>
<p><code>ProjectType</code> must have one constructor that accepts one parameter: <code>message</code></p>
<h3 id="step-two-create-the-product-class-in-the-com.techelevator.product-package">Step Two: Create the <code>Product</code> class in the <code>com.techelevator.product</code> package</h3>
<p>Create a new class called <code>Product.java</code> with the following requirements. The Product has 4 variables.</p>
<h4 id="properties-1">Properties</h4>

<table>
<thead>
<tr>
<th>Property</th>
<th>Data Type</th>
<th>Get</th>
<th>Set</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>slot</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>The slot location in the vending machine</td>
</tr>
<tr>
<td><code>name</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>The display name of the vending machine product</td>
</tr>
<tr>
<td><code>price</code></td>
<td><code>double</code></td>
<td>X</td>
<td></td>
<td>The purchase price for the product</td>
</tr>
<tr>
<td><code>type</code></td>
<td><code>ProductType</code></td>
<td>X</td>
<td></td>
<td>The product type for this row</td>
</tr>
</tbody>
</table><h4 id="constructors-1">Constructors</h4>
<p><code>Project</code> must have one constructor that accepts four parameters: <code>slot</code>, <code>name</code>, <code>price</code>, and <code>type</code>.</p>
<h3 id="step-three-create-the-quantity-class-in-the-com.techelevator.transaction-package">Step Three: Create the <code>Quantity</code> class in the <code>com.techelevator.transaction</code> package</h3>
<p>Create a new class called <code>Quantity.java</code> with the following requirements.</p>
<blockquote>
<p>The The <code>Quantity</code> class’s <code>getDefaultMaximumQuantity</code> method returns 5.</p>
</blockquote>
<h4 id="methods">Methods</h4>

<table>
<thead>
<tr>
<th>Method Name</th>
<th>Return Type</th>
<th>Parameters</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>getDefaultMaximumQuantity</code></td>
<td><code>int</code></td>
<td></td>
</tr>
</tbody>
</table><h3 id="step-four-create-the-transaction-class-in-the-com.techelevator.transaction-package">Step Four: Create the <code>Transaction</code> class in the <code>com.techelevator.transaction</code> package</h3>
<p>Create a new class called <code>Transaction.java</code> with the following requirements.</p>
<blockquote>
<p>The <code>Transaction</code> class’s <code>logTransaction</code> method logs a message to a file named <code>Log.txt</code>, prefixed with a timestamp. It uses the <code>SimpleDateFormat</code> class to format the timestamp and handles file writing with <code>PrintWriter</code> and <code>FileWriter</code> in a try-with-resources statement to ensure proper resource management. If an IOException occurs, it is caught and printed to the standard error stream.</p>
</blockquote>
<h4 id="methods-1">Methods</h4>

<table>
<thead>
<tr>
<th>Method Name</th>
<th>Return Type</th>
<th>Parameters</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>logTransaction</code></td>
<td><code>void</code></td>
<td>message</td>
</tr>
</tbody>
</table><h3 id="step-five-create-the-salesreport-class-in-the-com.techelevator.report-package">Step Five: Create the <code>SalesReport</code> class in the <code>com.techelevator.report</code> package</h3>
<p>Create a new class called <code>SalesReport.java</code> with the following requirements.</p>
<blockquote>
<p>The <code>SalesReport</code> class’s <code>generateReport</code> method generates a sales report file named with a timestamp. It iterates over the provided <code>inventory</code> of products, writes each product’s name and quantity sold to the file, calculates the total sales amount, and writes the total sales to the file. It handles file writing with a try-with-resources statement to ensure proper resource management, and it catches and prints any <code>IOExceptions</code> that occur.</p>
</blockquote>
<h4 id="methods-2">Methods</h4>

<table>
<thead>
<tr>
<th>Method Name</th>
<th>Return Type</th>
<th>Parameters</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>generateReport</code></td>
<td><code>void</code></td>
<td>message</td>
</tr>
</tbody>
</table><h3 id="step-six-create-the-abstractvendingmachine-class-in-the-com.techelevator.vendingmachine-package">Step Six: Create the <code>AbstractVendingMachine</code> class in the <code>com.techelevator.vendingmachine</code> package</h3>
<p>Create a new abstract class called <code>AbstractVendingMachine.java</code> with the following requirements.</p>
<blockquote>
<p>The <code>AbstractVendingMachine</code> class provides a blueprint for creating vending machine implementations by defining essential properties and methods that need to be implemented. It ensures that any subclass will have a consistent set of functionalities for handling products, money transactions, and displaying items, while leaving the specific details of these operations to be defined in the subclasses.</p>
</blockquote>
<h4 id="properties-2">Properties</h4>

<table>
<thead>
<tr>
<th>Property</th>
<th>Data Type</th>
<th>Get</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>inventory</code></td>
<td><code>Map&lt;String, Product&gt;</code></td>
<td>X</td>
<td>The inventory of products</td>
</tr>
<tr>
<td><code>balance</code></td>
<td><code>double</code></td>
<td>X</td>
<td>The current balance or amount of money</td>
</tr>
</tbody>
</table><h4 id="constructors-2">Constructors</h4>
<p><code>AbstractVendingMachine</code> has one constructor:</p>
<ul>
<li>It accepts a <code>String</code> parameter filepath.</li>
<li>This constructor calls the method readInventory(filepath).</li>
<li>It throws a FileNotFoundException</li>
</ul>
<blockquote>
<p>This constructor initializes the vending machine by reading its inventory from a specified file. It calls the abstract method <code>readInventory</code> which must be implemented by subclasses.</p>
</blockquote>
<h4 id="methods-3">Methods</h4>

<table>
<thead>
<tr>
<th>Method Name</th>
<th>Return Type</th>
<th>Parameters</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>readInventory</code></td>
<td><code>void</code></td>
<td>filepath</td>
</tr>
<tr>
<td><code>displayItems</code></td>
<td><code>void</code></td>
<td>none</td>
</tr>
<tr>
<td><code>feedMoney</code></td>
<td><code>void</code></td>
<td>amount</td>
</tr>
<tr>
<td><code>selectProduct</code></td>
<td><code>void</code></td>
<td>slot</td>
</tr>
<tr>
<td><code>finishTransaction</code></td>
<td><code>void</code></td>
<td>none</td>
</tr>
</tbody>
</table><p>The <code>readInventory</code> method doesn’t return any value. Reads the inventory from a file and returns a map of products.</p>
<p>The <code>displayItems</code> method returns a boolean value (<code>true</code> or <code>false</code>). Displays the available items in the vending machine.</p>
<p>The <code>feedMoney</code> method doesn’t return any value. It accepts a double parameter <code>balance</code>. It adds  money to the machine’s balance.</p>
<p>The <code>selectProduct</code> method returns a boolean value. It accepts a String parameter <code>slot</code>. It selects a product based on its slot code.</p>
<p>The <code>finishTransaction</code> method doesn’t return any value. It  finalizes the transaction, usually dispensing change and resetting the balance.</p>
<h3 id="step-seven--create-the-standardvendingmachine-class-in-the-com.techelevator.vendingmachine-package">Step Seven : Create the <code>StandardVendingMachine</code> class in the <code>com.techelevator.vendingmachine</code> package</h3>
<p>Create a new class called <code>StandardVendingMachine.java</code> with the following requirements.</p>
<blockquote>
<p>The <code>StandardVendingMachine</code> class is a specific implementation of a vending machine, inheriting from the <code>AbstractVendingMachine</code> class. It provides concrete implementations for the abstract methods, defining how inventory is read, items are displayed, money is fed, products are selected, and transactions are finished. It utilizes the <code>Product</code>, <code>ProductType</code>, and <code>Transaction</code> classes to manage products and log transactions.</p>
</blockquote>
<p>The <code>readInventory</code> method overrides the readInventory in the AbstractVendingMachine abstract class. It doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>displayItems</code> method overrides the displayItems in the AbstractVendingMachine abstract class. It returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<p>The <code>feedMoney</code> method overrides the feedMoney in the AbstractVendingMachine abstract class. It doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>selectProduct</code> method overrides the selectProduct in the AbstractVendingMachine abstract class. It returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<p>The <code>finishTransaction</code> method overrides the finishTransaction in the AbstractVendingMachine abstract class. It doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>

