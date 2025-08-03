<h1>📄 Bank Statement Parser (Scanned PDFs & Images)</h1>

<p>
  This project is an intelligent document parser that extracts structured data from scanned <b>bank statements</b> using OCR and LLMs.
  It supports <b>French-language documents</b> and returns the results in clean <code>JSON</code> format.
</p>

<h2>🚀 Features</h2>
<ul>
  <li>✅ Skew correction for scanned documents</li>
  <li>✅ OCR using <code>Tesseract</code></li>
  <li>✅ Natural language understanding using <code>LLama3.2</code> via <code>Ollama</code></li>
  <li>✅ Outputs clean and structured JSON with account, balance, and transaction info</li>
  <li>✅ Supports French-language bank statements</li>
</ul>

<h2>🛠 Technologies Used</h2>
<ul>
  <li>Python</li>
  <li>OpenCV & Pillow</li>
  <li>Pytesseract</li>
  <li>Ollama + LLaMA 3.2 (Locally running LLM)</li>
</ul>

<h2>📂 Output Format</h2>
<pre>
{
  "bank": "Crédit du Nord",
  "account_number": "FR76 3007 6043 3714 9374 0020 033",
  "statement_period": {
    "start_date": "01/12/2019",
    "end_date": "31/12/2019"
  },
  "transactions": [...],
  "totals": {
    "debits": "...",
    "credits": "..."
  },
  "balance": {
    "date": "31/12/2019",
    "amount": "1 566,06"
  }
}
</pre>

<h2>⚙️ How to Run</h2>
<ol>
  <li>Install dependencies:
    <pre>pip install -r requirements.txt</pre>
  </li>
  <li>Run Ollama and pull LLaMA 3.2:
    <pre>ollama run llama3</pre>
  </li>
  <li>Run the main function:
    <pre>python main.py</pre>
  </li>
</ol>

<h2>🧪 Test Cases</h2>
<p>Use sample scanned bank statements (French) in the <code>/data</code> folder to test.</p>

<h2>📄 Report</h2>
<p>A detailed project report is available in <code>Bank_Statement_Parser_Project_Report.docx</code>.</p>

<h2>🤝 Contribution</h2>
<p>Pull requests are welcome. For major changes, please open an issue first.</p>

<h2>📧 Tark Patel</h2>
