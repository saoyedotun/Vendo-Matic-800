---


---

<h1 id="module-1-capstone---vending-machine-software">Module 1 Capstone - Vending Machine Software</h1>
<p>You’re developing an application for the newest vending machine distributor, Umbrella Corp. They’ve released a new vending machine, Vendo-Matic 800, that’s integrated with everyone’s bank accounts, allowing customers to purchase products from their computers for their convenience.</p>
<h2 id="classes">Classes</h2>
<p>The core of this application consists of x classes, which you’ll create in the main package <code>corp.umbrella</code>. Make sure to read through the requirements for each class before writing any code.</p>
<h3 id="step-one-create-the-product-class">Step One: Create the <code>Product</code> class</h3>
<p>Create a new class called <code>Product.java</code> with the following requirements.</p>
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
<td><code>name</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>Name of the product.</td>
</tr>
<tr>
<td><code>type</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>Type of the product.</td>
</tr>
<tr>
<td><code>slot</code></td>
<td><code>String</code></td>
<td>X</td>
<td></td>
<td>A slot contains up to 5 products.</td>
</tr>
<tr>
<td><code>price</code></td>
<td><code>double</code></td>
<td>X</td>
<td></td>
<td>Price of the product.</td>
</tr>
<tr>
<td><code>quantity</code></td>
<td><code>int</code></td>
<td>X</td>
<td></td>
<td>Total amount of product in a slot.</td>
</tr>
</tbody>
</table><h4 id="static-constants">Static constants</h4>
<p>The default maximum amount for all product is 5 and is stored in a static constant variable of type <code>double</code>.</p>
<h4 id="constructors">Constructors</h4>
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

