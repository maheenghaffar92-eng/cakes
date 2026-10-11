Cake Shop Website

Live site:https://maheenghaffar92-eng.github.io/Faizas-Cake/

About

A responsive website for a cake shop in Defence Phase 5, Clifton. Visitors can see the cakes and place an order by email.

Built with

HTML and CSS js only. Hosted on GitHub Pages. Fonts from Google Fonts.

#	Task	What AI did	What went wrong	How I checked and fixed it
1	Add to cart	Wrote the button HTML, cart CSS and beginner JavaScript	The button was placed inside the image box (.ph), so it was hidden behind the image	Used Inspect to find it, then moved the button outside .ph, after the price
2	Prices in PKR	Added a formatPKR() function and told me to change the total line	The old dollar cart stayed saved in localStorage, so old prices still showed	Changed the prices and total line, then clicked Clear cart
3	Cart total	Wrote the add and total logic	All 4 buttons still had data-name="Choco Cake" data-price="98", so every click added 98	Gave each button its own name and price, then tested: one of each should total ₨ 9,800
4	Code review	Read my HTML and spotted problems	#cup, #cake and #slice are used but never defined in the SVG block, so those spots can show empty	Checked the hero and about sections for blank areas
5	Phone numbers	(Fill in if AI wrote them)	The header says +10 783 346 4378 but the footer says 913-473-7000, and both look like placeholders	Replace both with the real number
6	Responsive design	Reviewed against the lab’s 5-point check	My CSS uses max-width media queries (desktop-first), and some fixed values like section h2 { font-size: 50px !important; } and min-height: 680px on the hero	Run the squeeze test from 1200px down to 320px, then fix with clamp() before adding more breakpoints