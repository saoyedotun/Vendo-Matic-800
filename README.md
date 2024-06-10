---


---

<h1 id="module-1-capstone---vending-machine-software--v-1.0.0">Module 1 Capstone - Vending Machine Software  (V 1.0.0)</h1>
<p>You’re developing an application for the newest vending machine distributor, Umbrella Corp. They’ve released a new vending machine, Vendo-Matic 800, that’s integrated with everyone’s bank accounts, allowing customers to purchase products from their computers for their convenience.</p>
<p>Classes require to develop the vending machine software as well as their Unit Test classes.</p>

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
<td>Lorem ipsor dolor sit ammet</td>
</tr>
<tr>
<td><code>Product</code></td>
<td>Represents an item in the vending machine</td>
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
<td><code>ProductTest</code></td>
<td>Test cases for Product  Class</td>
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
<p>The core of this application consists of 4 packages, product, report, transaction, and vendingmachine and their respective 7 Classes, which you’ll create in the main package <code>com.techelevator</code>. Make sure to read through the requirements for each class before writing any code.</p>
<h3 id="step-one-create-the-producttype-enum-class-in-the-com.techelevator.product-package">Step One: Create the <code>ProductType</code> Enum class in the <code>com.techelevator.product</code> package</h3>
<p>Create a new enum class called <code>ProductType.java</code> with the following requirements.</p>
<h4 id="properties">Properties</h4>

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
<td><code>message</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>Lorem ipsor dolor sit ammet</td>
</tr>
</tbody>
</table><h4 id="constructors">Constructors</h4>
<p><code>Project</code> must have one constructor that accepts four parameters: <code>name</code>, <code>type</code>, <code>slot</code>, and <code>price</code>.</p>
<h3 id="step-two-create-the-product-class-in-the-com.techelevator.product-package">Step Two: Create the <code>Product</code> class in the <code>com.techelevator.product</code> package</h3>
<p>Create a new class called <code>Product.java</code> with the following requirements.</p>
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
<td><code>name</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>The display name of the vending machine product</td>
</tr>
<tr>
<td><code>type</code></td>
<td><code>ProductType</code></td>
<td>X</td>
<td></td>
<td>The product type for this row</td>
</tr>
<tr>
<td><code>slot</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>The slot location in the vending machine</td>
</tr>
<tr>
<td><code>price</code></td>
<td><code>double</code></td>
<td>X</td>
<td></td>
<td>The purchase price for the product</td>
</tr>
<tr>
<td><code>quantity</code></td>
<td><code>int</code></td>
<td>X</td>
<td></td>
<td>Total amount of product in a slot</td>
</tr>
</tbody>
</table><h4 id="static-constants">Static constants</h4>
<p>The default maximum amount for all product is 5 and is stored in a static constant variable of type <code>int</code>.</p>
<h4 id="constructors-1">Constructors</h4>
<p><code>Project</code> must have one constructor that accepts four parameters: <code>name</code>, <code>type</code>, <code>slot</code>, and <code>price</code>.</p>
<blockquote>
<p>Note: Make sure to initialize <code>slot</code> to the static constant you created. You can do this in the constructor.</p>
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
<td><code>dispense</code></td>
<td><code>void</code></td>
<td>none</td>
</tr>
<tr>
<td><code>isSoldOut</code></td>
<td><code>boolean</code></td>
<td>none</td>
</tr>
</tbody>
</table><p>The <code>dispense</code> method doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>isSoldOut</code> method returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<h3 id="step-two-create-the-vendingmachine-class">Step Two: Create the <code>VendingMachine</code> class</h3>
<p>Create a new class called <code>VendingMachine.java</code> with the following requirements.</p>
<h4 id="properties-2">Properties</h4>

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
<td><code>inventory</code></td>
<td><code>Map&lt;String, Product&gt;</code></td>
<td>X</td>
<td></td>
<td>Lorem ipsum dolor sit.</td>
</tr>
<tr>
<td><code>balance</code></td>
<td><code>double</code></td>
<td>X</td>
<td></td>
<td>Lorem ipsum dolor sit.</td>
</tr>
</tbody>
</table><h4 id="constructors-2">Constructors</h4>
<p><code>VendingMachine</code> has one constructor:</p>
<ul>
<li>It accepts a <code>String</code> parameter filepath.</li>
<li>This constructor calls the method readInventory(filepath).</li>
</ul>
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
<tr>
<td><code>printMessage</code></td>
<td><code>void</code></td>
<td>type</td>
</tr>
</tbody>
</table><p>The <code>readInventory</code> method doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>displayItems</code> method returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<p>The <code>feedMoney</code> method doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>selectProduct</code> method returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<p>The <code>finishTransaction</code> method doesn’t return any value. If there are items left in the vending machine, decrements the <code>quantity</code> of the product by one when it’s dispensed.</p>
<p>The <code>printMessage</code> method returns a boolean value (<code>true</code> or <code>false</code>). if the <code>quantity</code> of the product is equal to 0, it returns <code>true</code> eelse <code>false</code>.</p>
<h3 id="step-three-create-the-salesreport-class">Step Three: Create the <code>SalesReport</code> class</h3>
<p>Create a new class called <code>SalesReport.java</code> with the following requirements.</p>
<h3 id="step-four-create-the-transaction-class">Step Four: Create the <code>Transaction</code> class</h3>
<p>Create a new class called <code>Transaction.java</code> with the following requirements.</p>
<h3 id="step-five-create-the-application-class">Step Five: Create the <code>Application</code> class</h3>
<p>Create a new class called <code>Application.java</code> with the following requirements.</p>
<h3 id="step-six-create-the-invventory-class">Step Six: Create the <code>Invventory</code> class</h3>
<p>Create a new class called <code>Invventory.java</code> with the following requirements.</p>
<h3 id="step-seven-update-the-unittest1-class">Step Seven: Update the <code>UnitTest1</code> class</h3>
<p>Update the class called <code>UnitTest1.java</code> with the following requirements.</p>

