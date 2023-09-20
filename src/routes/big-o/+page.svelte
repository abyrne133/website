<article>
	<h3>Big O Notation</h3>
	<article>
		<h6>Why is it useful?</h6>
		<p>Categorise and compare the efficiency of algorithms as the input scales up.</p>
		<ul>
			<li>consider time and space (memory) efficiency</li>
			<li>consider trade offs between time and space efficiency</li>
			<li>interested in behaviour for very large inputs</li>
		</ul>
	</article>
	<article>
		<h6>Simplified Time Example</h6>
		<p>
			Delivering a letter to a friend by foot has <i>contstant</i> runtime, notated as O(1) or "big oh
			of 1" with respect to the size of the message.
		</p>
		<p>
			Sending the same message over a computer network has <i>linear</i> runtime, notated as O(n) with
			respect to the size of the message.
		</p>
		<p>
			Which is faster? It depends on the size of the file. For a small file the network will
			probably win, but for a really large file it might be faster to walk! The takeaway is that for
			some large input the linear (network) runtime will exceed the constant (walking) runtime.
		</p>
	</article>
	<article>
		<p>There are different measurements of efficiency to consider:</p>
		<ul>
			<li>
				<strong>Best Case</strong> describes the runtime in the best edge case input scenario, usually
				not considered.
			</li>
			<li><strong>Worst Case</strong> for unlucky inputs! Needs to be considered.</li>
			<li><strong>Expected Case</strong> describes what usually happens. Interested.</li>
		</ul>
	</article>
	<article>
		<h6>Amortized Time</h6>
		<p>
			Some algorithms will deviate from the expected runtime but in known situations. When a java
			ArrayList gets full, the library creates a new array with double the size and copies the
			records over. This is an example of a space-time trade off or balance. Space is saved when the
			arrary is not full, but time is lost upon creating a larger array and copying over.
		</p>
	</article>
	<article><h6>Space Complexity</h6></article>
	<p>
		It get's harder, because measurements can be applied to different actions like sorting,
		inserting, searching..! One approach is to practice classifiying the time and space complexity
		of different algorithms instead of memorizing them. Gayle Laakmann McDowell provides great
		exercises in her well known <a href="https://www.crackingthecodinginterview.com/"
			>Cracking the Coding Interview</a
		> book.
	</p>
	<p>
		If you'd like a reference or a place to memorise from, go here: <a
			href="https://www.bigocheatsheet.com/">https://www.bigocheatsheet.com/</a
		>
	</p>
</article>

<style>
	ul {
		padding-left: 2.5rem;
	}
</style>
