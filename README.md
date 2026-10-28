# Sales_analysis
I don't trust videos where "AI builds a dashboard by itself in 5 minutes." So I tested it for real: I built a full sales dashboard together with Claude. Here is what it actually looked like.

Some context: I'm moving into business analysis (BA/BI) from finance, banking and sales. I wanted a project I could show, not just a list of courses.

What I built: an interactive 6-page sales dashboard covering overview, sales team, product categories, products, suppliers and customers. Filters by year, category and employee. Click an employee and you see which categories they are strong in and where they fall behind.

How we worked:
→ Data: a training sales database (8 tables, star schema) in my local MySQL. I exported the tables to CSV so the database never had to be exposed.
→ Claude can't drive Power BI directly, so the dashboard is an HTML page, and my earlier Power BI report served as the reference.
→ I set the goals and decided which metrics matter. Claude wrote the code and turned edits around fast.
→ We checked the data together and spotted an odd category name and a sharp jump in average order value after a certain date. That is the part AI doesn't replace.

My takeaway: AI speeds up the routine, but understanding the data model, the business logic and validating the results stay with the analyst.
