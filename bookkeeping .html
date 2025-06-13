<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Bookkeeping with Client Ledger Monitoring</title>
  <style>
    /* Reset and base */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: 'Inter', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #121212, #1a1a2e);
      color: #e0e0e0;
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      font-size: 16px;
      transition: background-color 0.4s ease, color 0.4s ease;
      padding: 24px 16px;
    }

    header {
      max-width: 960px;
      margin: 0 auto 32px;
      text-align: center;
      user-select: none;
    }
    header h1 {
      font-weight: 900;
      font-size: 2rem;
      letter-spacing: 0.08em;
      margin: 0;
      background: linear-gradient(135deg, #d3b2ff, #0ff1ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      user-select: text;
      text-shadow: 0 2px 6px rgba(0, 184, 255, 0.5);
    }

    nav {
      max-width: 960px;
      margin: 0 auto 32px;
      display: flex;
      gap: 24px;
      justify-content: center;
      flex-wrap: wrap;
      user-select: none;
    }
    nav button {
      font: 600 1rem 'Inter', sans-serif;
      background: rgba(255 255 255 / 0.2);
      border: none;
      cursor: pointer;
      color: #dfe9ff;
      padding: 10px 22px;
      border-radius: 16px;
      box-shadow:
        inset 0 0 0 1.5px rgba(255 255 255 / 0.4),
        0 2px 6px rgb(30 40 80 / 0.4);
      transition:
        background-color 0.35s cubic-bezier(0.4, 0, 0.2, 1),
        color 0.35s cubic-bezier(0.4, 0, 0.2, 1),
        box-shadow 0.35s cubic-bezier(0.4, 0, 0.2, 1),
        transform 0.2s ease;
      min-width: 140px;
      text-align: center;
    }
    nav button:hover,
    nav button:focus-visible {
      background: #c1eaff;
      color: #18005d;
      box-shadow:
        0 0 10px 3px #00cfff,
        0 8px 15px rgb(0 198 255 / 0.6);
      transform: translateY(-3px);
      outline-offset: 3px;
      outline: 3px solid #0ff1ff;
    }
    nav button[aria-current="page"] {
      background: #0ff1ff;
      color: #18005d;
      cursor: default;
      pointer-events: none;
      box-shadow:
        0 0 8px 1px #a0f3ff,
        0 10px 28px rgb(0 240 255 / 0.6);
      transform: translateY(-1px);
    }

    main {
      max-width: 960px;
      margin: 0 auto;
      flex: 1 0 auto;
      outline: none;
    }

    section {
      background: rgba(14, 14, 26, 0.75);
      padding: 32px 36px;
      border-radius: 24px;
      box-shadow:
        0 8px 28px rgb(78 28 221 / 0.5),
        inset 0 0 40px rgb(24 140 230 / 0.3);
      max-width: 100%;
      margin-bottom: 56px;
      backdrop-filter: saturate(180%) blur(25px);
      -webkit-backdrop-filter: saturate(180%) blur(25px);
      border: 1.5px solid rgba(255 255 255 / 0.08);
      color: #e5e9ff;
    }
    section h2 {
      font-size: 2.25rem;
      font-weight: 900;
      margin-bottom: 28px;
      background: linear-gradient(135deg, #ac88ff 0%, #00e0ff 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-shadow: 0 3px 8px rgb(0, 224, 255, 0.2);
      user-select: text;
    }

    .form-group {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: space-between;
      margin-bottom: 26px;
    }

    .form-field {
      flex: 1 1 260px;
      display: flex;
      flex-direction: column;
    }

    label {
      margin-bottom: 10px;
      font-weight: 700;
      font-size: 1.05rem;
      color: rgba(255 255 255 / 0.85);
      cursor: pointer;
      user-select: text;
      letter-spacing: 0.01em;
    }

    input[type="text"],
    input[type="date"],
    input[type="number"],
    select {
      font-size: 1.1rem;
      padding: 14px 18px;
      border-radius: 16px;
      border: none;
      background-color: #1f1f3c;
      color: #e0e6ff;
      transition: box-shadow 0.4s ease, background-color 0.4s ease;
      outline-offset: 4px;
      outline-color: transparent;
      box-shadow: inset 0 0 8px rgb(40 40 80 / 0.5);
      user-select: text;
    }
    input[type="text"]:focus,
    input[type="date"]:focus,
    input[type="number"]:focus,
    select:focus {
      outline-color: #00f0ff;
      background-color: #222248;
      box-shadow:
        0 0 12px 3px #00e5ff,
        inset 0 0 12px #33ccff;
    }
    input[type="number"] {
      -moz-appearance: textfield;
    }
    input[type=number]::-webkit-inner-spin-button,
    input[type=number]::-webkit-outer-spin-button {
      -webkit-appearance: none;
      margin: 0;
    }

    button[type="submit"], button, input[type="file"] + label {
      background: linear-gradient(135deg, #7e56d9 0%, #00cfff 100%);
      color: #0e0748;
      font-weight: 900;
      font-size: 1.15rem;
      cursor: pointer;
      border: none;
      padding: 14px 30px;
      border-radius: 24px;
      box-shadow:
        0 10px 26px rgb(126 86 217 / 0.7),
        inset 0 0 12px rgb(255 255 255 / 0.3);
      transition:
        background 0.4s ease,
        color 0.4s ease,
        transform 0.25s ease,
        box-shadow 0.25s ease;
      align-self: flex-start;
      margin-top: 12px;
      user-select: none;
      -webkit-tap-highlight-color: transparent;
      display: inline-block;
      text-align: center;
    }
    button[type="submit"]:hover,
    button[type="submit"]:focus-visible,
    button:hover,
    button:focus-visible,
    input[type="file"]:focus + label,
    input[type="file"]:hover + label {
      background: linear-gradient(135deg, #00e5ff 0%, #55ffff 100%);
      color: #072547;
      transform: translateY(-5px) scale(1.05);
      box-shadow:
        0 20px 48px rgb(0 229 255 / 0.9),
        inset 0 0 18px rgb(255 255 255 / 0.6);
      outline-offset: 5px;
      outline-color: #00f4ff;
    }
    button:disabled,
    button[disabled] {
      cursor: not-allowed;
      opacity: 0.4;
      box-shadow: none;
      background: #444666;
      color: #a9a9b9;
      transform: none;
    }

    /* Table styling */
    .table-wrapper {
      border-radius: 20px;
      overflow-x: auto;
      box-shadow:
        inset 0 0 20px rgba(255 255 255 / 0.1),
        0 12px 32px rgba(0 198 255 / 0.2);
      backdrop-filter: saturate(200%) blur(40px);
      -webkit-backdrop-filter: saturate(200%) blur(40px);
      margin-bottom: 56px;
      max-width: 100%;
    }

    table {
      width: 100%;
      border-collapse: separate;
      border-spacing: 0;
      min-width: 720px;
      color: #e0e8ff;
      font-feature-settings: "tnum";
      font-variant-numeric: tabular-nums;
      font-weight: 500;
    }
    thead {
      background: linear-gradient(135deg, #7e56d9, #00e2ff);
      color: #eff4ff;
      user-select: none;
      font-weight: 800;
      letter-spacing: 0.08em;
      font-size: 0.9rem;
    }
    thead th {
      padding: 18px 24px;
      text-align: left;
      position: sticky;
      top: 0;
      user-select: none;
      border-bottom: 2px solid #00aaff;
      box-shadow: inset 0 -3px 6px #00aaff;
      z-index: 10;
    }
    th:first-child {
      border-top-left-radius: 20px;
    }
    th:last-child {
      border-top-right-radius: 20px;
    }

    tbody {
      background: rgba(20, 20, 40, 0.65);
    }
    tbody tr:hover {
      background-color: rgba(79, 44, 255, 0.35);
      cursor: default;
      transition: background-color 0.3s ease;
      font-weight: 600;
      color: #ccf9ff;
      filter: drop-shadow(0 0 8px #4f2cffaa);
    }
    td {
      padding: 16px 22px;
      font-size: 1rem;
      vertical-align: middle;
      border-bottom: 1px solid rgba(255 255 255 / 0.08);
    }
    td:first-child {
      font-weight: 700;
      color: #bad9ff;
    }
    td[style*="text-align:right;"] {
      font-feature-settings: "tnum";
      font-variant-numeric: tabular-nums;
    }
    tbody tr:last-child td {
      border-bottom: none;
    }

    /* Scrollbar for table */
    .table-wrapper::-webkit-scrollbar {
      height: 10px;
    }
    .table-wrapper::-webkit-scrollbar-thumb {
      background: #5dcfffdd;
      border-radius: 20px;
      transition: background-color 0.3s ease;
    }
    .table-wrapper:hover::-webkit-scrollbar-thumb {
      background: #00f7ffdd;
    }
    .table-wrapper::-webkit-scrollbar-track {
      background: transparent;
    }

    /* Accessibility focus outline */
    a:focus,
    button:focus,
    input:focus,
    select:focus,
    textarea:focus {
      outline-offset: 5px;
      outline: 3px solid #0ff0ffcc;
      outline-radius: 10px;
    }

    /* Responsive */
    @media (max-width: 768px) {
      body {
        font-size: 15px;
        padding: 20px 12px;
      }
      header h1 {
        font-size: 1.7rem;
      }
      nav {
        gap: 16px;
      }
      section {
        padding: 24px 20px;
      }
      .form-group {
        flex-direction: column;
      }
      .form-field {
        flex: 1 1 100%;
      }
      table {
        min-width: 100%;
      }
      #ledger-entries-body td:first-child,
      #ledger-entries-body td:last-child {
        min-width: 110px;
      }
    }
  </style>
</head>
<body>
  <header role="banner">
    <h1>Bookkeeping with Client Ledger Monitoring</h1>
  </header>

  <nav role="navigation" aria-label="Main navigation">
    <button id="tab-journal" aria-current="page" aria-controls="section-journal">Journal Entry</button>
    <button id="tab-clients" aria-controls="section-clients">Clients</button>
    <button id="tab-ledger" aria-controls="section-ledger">General Ledger</button>
    <button id="tab-backup" aria-controls="section-backup">Backup &amp; Restore</button>
  </nav>

  <main>
    <!-- Journal Entry Section -->
    <section id="section-journal" role="region" tabindex="-1" aria-labelledby="tab-journal">
      <form id="journal-form" aria-live="polite" novalidate>
        <h2>New Journal Entry</h2>
        <div class="form-group">
          <div class="form-field">
            <label for="entry-date">Date</label>
            <input type="date" id="entry-date" name="date" required aria-required="true" autocomplete="off" />
          </div>
          <div class="form-field" style="flex: 2 1 400px;">
            <label for="entry-description">Description</label>
            <input type="text" id="entry-description" name="description" placeholder="Brief description" required aria-required="true" autocomplete="off" />
          </div>
        </div>
        <div class="form-group" aria-label="Debit, credit accounts and client details">
          <div class="form-field">
            <label for="entry-debit-account">Debit Account</label>
            <select id="entry-debit-account" name="debitAccount" required aria-required="true" aria-describedby="debit-account-help" autocomplete="off">
              <option value="" disabled selected>Select account</option>
              <option value="Cash">Cash</option>
              <option value="Accounts Receivable">Accounts Receivable</option>
              <option value="Supplies">Supplies</option>
              <option value="Equipment">Equipment</option>
              <option value="Rent Expense">Rent Expense</option>
              <option value="Salaries Expense">Salaries Expense</option>
              <option value="Sales Revenue">Sales Revenue</option>
              <option value="Accounts Payable">Accounts Payable</option>
              <option value="Unearned Revenue">Unearned Revenue</option>
              <option value="Capital Stock">Capital Stock</option>
            </select>
            <small id="debit-account-help" style="color: #66ccff;">Select account to debit</small>
          </div>
          <div class="form-field">
            <label for="entry-credit-account">Credit Account</label>
            <select id="entry-credit-account" name="creditAccount" required aria-required="true" aria-describedby="credit-account-help" autocomplete="off">
              <option value="" disabled selected>Select account</option>
              <option value="Cash">Cash</option>
              <option value="Accounts Receivable">Accounts Receivable</option>
              <option value="Supplies">Supplies</option>
              <option value="Equipment">Equipment</option>
              <option value="Rent Expense">Rent Expense</option>
              <option value="Salaries Expense">Salaries Expense</option>
              <option value="Sales Revenue">Sales Revenue</option>
              <option value="Accounts Payable">Accounts Payable</option>
              <option value="Unearned Revenue">Unearned Revenue</option>
              <option value="Capital Stock">Capital Stock</option>
            </select>
            <small id="credit-account-help" style="color: #66ccff;">Select account to credit</small>
          </div>
          <div class="form-field">
            <label for="entry-client">Client</label>
            <select id="entry-client" name="clientId" aria-describedby="client-help" autocomplete="off">
              <option value="" selected>None</option>
            </select>
            <small id="client-help" style="color: #66ccff;">Associate this entry with a client (optional)</small>
          </div>
        </div>
        <div class="form-group" aria-label="Amounts">
          <div class="form-field">
            <label for="entry-debit-amount">Debit Amount</label>
            <input type="number" id="entry-debit-amount" name="debitAmount" min="0.01" step="0.01" placeholder="0.00" required aria-required="true" autocomplete="off" />
          </div>
          <div class="form-field">
            <label for="entry-credit-amount">Credit Amount</label>
            <input type="number" id="entry-credit-amount" name="creditAmount" min="0.01" step="0.01" placeholder="0.00" required aria-required="true" autocomplete="off" />
          </div>
          <div class="form-field" style="flex: 1 1 100%;">&nbsp;</div>
        </div>
        <button type="submit" aria-label="Add journal entry" title="Add new transaction entry">Add Entry</button>
      </form>

      <section aria-labelledby="journal-entries-heading">
        <h2 id="journal-entries-heading" style="margin-bottom: 16px;user-select: text;">Journal Entries</h2>
        <div class="table-wrapper" role="table" aria-label="Journal entries table" tabindex="0" aria-live="polite" aria-relevant="additions">
          <table>
            <thead>
              <tr>
                <th scope="col">Date</th>
                <th scope="col">Description</th>
                <th scope="col">Debit Account</th>
                <th scope="col" style="text-align:right;">Debit Amount</th>
                <th scope="col">Credit Account</th>
                <th scope="col" style="text-align:right;">Credit Amount</th>
                <th scope="col">Client</th>
              </tr>
            </thead>
            <tbody id="journal-entries-body"></tbody>
          </table>
        </div>
      </section>
    </section>

    <!-- Clients Section -->
    <section id="section-clients" role="region" tabindex="-1" aria-labelledby="tab-clients" hidden>
      <h2>Manage Clients</h2>
      <form id="client-form" novalidate aria-live="polite">
        <div class="form-group">
          <div class="form-field" style="flex: 2 1 400px;">
            <label for="client-name">Client Name</label>
            <input type="text" id="client-name" name="name" placeholder="Client full name" required aria-required="true" autocomplete="off" />
          </div>
          <div class="form-field" style="flex: 2 1 400px;">
            <label for="client-company">Company</label>
            <input type="text" id="client-company" name="company" placeholder="Company or organization" autocomplete="off" />
          </div>
        </div>
        <div class="form-group" style="margin-bottom: 0;">
          <div class="form-field" style="flex: 3 1 100%;">
            <label for="client-notes">Notes</label>
            <input type="text" id="client-notes" name="notes" placeholder="Additional info (optional)" autocomplete="off" />
          </div>
        </div>
        <button type="submit" aria-label="Add client">Add Client</button>
      </form>

      <section aria-labelledby="clients-list-heading" style="margin-top: 48px;">
        <h2 id="clients-list-heading" style="color:#bbeeff;">Client List</h2>
        <div class="table-wrapper" tabindex="0" aria-live="polite" aria-relevant="additions removals">
          <table id="clients-list">
            <thead>
              <tr>
                <th scope="col">Client Name</th>
                <th scope="col">Company</th>
                <th scope="col">Notes</th>
                <th scope="col" style="width: 90px;">Actions</th>
              </tr>
            </thead>
            <tbody></tbody>
          </table>
        </div>
      </section>
    </section>

    <!-- General Ledger Section -->
    <section id="section-ledger" role="region" tabindex="-1" aria-labelledby="tab-ledger" hidden>
      <h2>General Ledger - Client Monitoring</h2>
      <div style="margin-bottom: 20px;">
        <label for="ledger-client-filter" style="font-weight:700;">Filter by Client:</label>
        <select id="ledger-client-filter" style="margin-left: 12px; padding: 8px 12px; border-radius: 12px; border:none; min-width:200px; font-size:1rem; background-color:#222248; color:#e0e6ff;">
          <option value="all" selected>All Clients</option>
        </select>
      </div>
      <div class="table-wrapper" role="table" aria-label="General ledger accounts and transactions" tabindex="0" aria-live="polite" aria-relevant="additions">
        <table>
          <thead>
            <tr>
              <th scope="col">Account</th>
              <th scope="col">Date</th>
              <th scope="col">Description</th>
              <th scope="col">Debit</th>
              <th scope="col">Credit</th>
              <th scope="col">Balance</th>
              <th scope="col">Client</th>
            </tr>
          </thead>
          <tbody id="ledger-entries-body"></tbody>
        </table>
      </div>
    </section>

    <!-- Backup Section -->
    <section id="section-backup" role="region" tabindex="-1" aria-labelledby="tab-backup" hidden>
      <h2>Backup &amp; Restore</h2>
      <p>Backup your journal entries and clients data by exporting them to a file. You can restore your data by importing a previously exported backup file.</p>
      <div style="margin-top: 24px; display: flex; gap: 24px; flex-wrap: wrap;">
        <button id="export-btn" aria-label="Export backup file">Export Backup</button>
        <label for="import-file" tabindex="0" role="button" aria-label="Import backup file" style="cursor: pointer; background: linear-gradient(135deg, #7e56d9, #00cfff); color: #0e0748; padding: 12px 28px; border-radius: 20px; font-weight: 900; box-shadow: 0 10px 26px rgb(126 86 217 / 0.7); user-select: none;">Import Backup (JSON)
          <input type="file" id="import-file" accept=".json" />
        </label>
        <button id="export-pdf-btn" aria-label="Export PDF report of journal entries and clients">Export PDF Report</button>
      </div>
      <p id="backup-message" aria-live="polite" style="margin-top: 20px; font-weight: 600;"></p>
    </section>
  </main>

  <!-- jsPDF and autoTable via CDN -->
  <script src="https://cdn.jsdelivr.net/npm/jspdf@2.5.1/dist/jspdf.umd.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/jspdf-autotable@3.5.25/dist/jspdf.plugin.autotable.min.js"></script>

  <script>
    (() => {
      const STORAGE_ENTRIES_KEY = 'bookkeeping-journal-entries';
      const STORAGE_CLIENTS_KEY = 'bookkeeping-clients';

      // Navigation tabs & sections
      const tabs = {
        journal: document.getElementById('tab-journal'),
        clients: document.getElementById('tab-clients'),
        ledger: document.getElementById('tab-ledger'),
        backup: document.getElementById('tab-backup'),
      };
      const sections = {
        journal: document.getElementById('section-journal'),
        clients: document.getElementById('section-clients'),
        ledger: document.getElementById('section-ledger'),
        backup: document.getElementById('section-backup'),
      };

      function switchTab(selected) {
        Object.entries(tabs).forEach(([key, tab]) => {
          if(key === selected) {
            tab.setAttribute('aria-current', 'page');
            sections[key].hidden = false;
            sections[key].focus();
          } else {
            tab.removeAttribute('aria-current');
            sections[key].hidden = true;
          }
        });
      }

      Object.entries(tabs).forEach(([key, tab]) => {
        tab.addEventListener('click', () => switchTab(key));
      });

      // Initialize view to journal
      switchTab('journal');

      // ===== Journal Entries =====
      let journalEntries = JSON.parse(localStorage.getItem(STORAGE_ENTRIES_KEY)) || [];
      const journalEntriesBody = document.getElementById('journal-entries-body');
      const journalForm = document.getElementById('journal-form');
      const clientSelect = document.getElementById('entry-client');

      // ===== Clients Management =====
      let clients = JSON.parse(localStorage.getItem(STORAGE_CLIENTS_KEY)) || [];
      const clientForm = document.getElementById('client-form');
      const clientsListBody = document.querySelector('#clients-list tbody');

      // Ledger elements
      const ledgerFilterClient = document.getElementById('ledger-client-filter');
      const ledgerEntriesBody = document.getElementById('ledger-entries-body');

      // Helpers
      function saveEntries() {
        localStorage.setItem(STORAGE_ENTRIES_KEY, JSON.stringify(journalEntries));
      }

      function saveClients() {
        localStorage.setItem(STORAGE_CLIENTS_KEY, JSON.stringify(clients));
      }

      // Format date YYYY-MM-DD to localized string
      function formatDate(dateStr) {
        const d = new Date(dateStr);
        if (isNaN(d)) return '';
        return d.toLocaleDateString(undefined, { year: 'numeric', month: '2-digit', day: '2-digit' });
      }

      // Format amounts
      function formatAmount(value) {
        if (typeof value !== 'number' && typeof value !== 'string') return '';
        const n = Number(value);
        if (isNaN(n)) return '';
        return n.toLocaleString(undefined, { minimumFractionDigits: 2, maximumFractionDigits: 2 });
      }

      // --- Journal Entries Render ---
      function renderJournalEntries() {
        journalEntriesBody.innerHTML = '';
        if(journalEntries.length === 0) {
          journalEntriesBody.innerHTML = '<tr><td colspan="7" style="text-align:center;color:#7f7f9c;">No journal entries recorded</td></tr>';
          return;
        }
        journalEntries.forEach(({ date, description, debitAccount, debitAmount, creditAccount, creditAmount, clientId }) => {
          // Get client name by id or show blank if none
          const clientName = clients.find(c => c.id === clientId)?.name || '';
          const tr = document.createElement('tr');
          tr.setAttribute('tabindex', '-1');
          tr.setAttribute('role', 'row');
          tr.innerHTML = `
            <td>${formatDate(date)}</td>
            <td>${description}</td>
            <td>${debitAccount}</td>
            <td style="text-align:right;">${formatAmount(debitAmount)}</td>
            <td>${creditAccount}</td>
            <td style="text-align:right;">${formatAmount(creditAmount)}</td>
            <td>${clientName}</td>
          `;
          journalEntriesBody.appendChild(tr);
        });
      }

      // --- Clients Dropdown ---
      function populateClientDropdown() {
        clientSelect.innerHTML = '<option value="" selected>None</option>';
        clients.forEach(client => {
          const opt = document.createElement('option');
          opt.value = client.id;
          opt.textContent = client.name;
          clientSelect.appendChild(opt);
        });

        // Populate ledger client filter as well
        ledgerFilterClient.innerHTML = '<option value="all" selected>All Clients</option>';
        clients.forEach(client => {
          const opt = document.createElement('option');
          opt.value = client.id;
          opt.textContent = client.name;
          ledgerFilterClient.appendChild(opt);
        });
      }

      // --- Clients List Render ---
      function renderClientsList() {
        clientsListBody.innerHTML = '';
        if(clients.length === 0) {
          clientsListBody.innerHTML = '<tr><td colspan="4" style="text-align:center;color:#7f7f9c;">No clients added yet.</td></tr>';
          return;
        }
        clients.forEach(client => {
          const tr = document.createElement('tr');
          tr.innerHTML = `
            <td>${client.name}</td>
            <td>${client.company || ''}</td>
            <td>${client.notes || ''}</td>
            <td class="actions">
              <button aria-label="Delete client ${client.name}" title="Delete client" data-id="${client.id}">&times;</button>
            </td>
          `;
          clientsListBody.appendChild(tr);
        });
      }

      // --- Generate Unique ID ---
      function generateId() {
        return '_' + Math.random().toString(36).substr(2, 9);
      }

      // --- Validate journal entry ---
      function validateJournalEntry(entry) {
        const errors = [];

        if (!entry.date) errors.push('Date is required.');
        if (!entry.description.trim()) errors.push('Description is required.');
        if (!entry.debitAccount) errors.push('Debit account must be selected.');
        if (!entry.creditAccount) errors.push('Credit account must be selected.');
        if (entry.debitAmount <= 0) errors.push('Debit amount must be greater than 0.');
        if (entry.creditAmount <= 0) errors.push('Credit amount must be greater than 0.');
        if (entry.debitAmount !== entry.creditAmount) errors.push('Debit and credit amounts must be equal.');
        if (entry.debitAccount && entry.creditAccount && entry.debitAccount === entry.creditAccount) errors.push('Debit and credit accounts cannot be the same.');

        return errors;
      }

      // --- Validate client ---
      function validateClient(client) {
        const errors = [];
        if (!client.name || client.name.trim() === '') {
          errors.push('Client name is required.');
        }
        return errors;
      }

      // --- Handle journal form submit ---
      journalForm.addEventListener('submit', e => {
        e.preventDefault();

        const formData = new FormData(journalForm);
        const newEntry = {
          date: formData.get('date'),
          description: formData.get('description').trim(),
          debitAccount: formData.get('debitAccount'),
          debitAmount: parseFloat(formData.get('debitAmount')),
          creditAccount: formData.get('creditAccount'),
          creditAmount: parseFloat(formData.get('creditAmount')),
          clientId: formData.get('clientId') || '',
        };

        const errors = validateJournalEntry(newEntry);
        if(errors.length > 0) {
          alert('Please fix the following errors before submitting:\n- ' + errors.join('\n- '));
          return;
        }

        journalEntries.push(newEntry);
        // Sort ascending by date
        journalEntries.sort((a,b) => new Date(a.date) - new Date(b.date));
        saveEntries();
        renderJournalEntries();
        journalForm.reset();
        journalForm.querySelector('input, select').focus();
        // Refresh ledger view if visible
        if (!sections.ledger.hidden) renderGeneralLedger();
      });

      // --- Handle client form submit ---
      clientForm.addEventListener('submit', e => {
        e.preventDefault();

        const formData = new FormData(clientForm);
        const newClient = {
          id: generateId(),
          name: formData.get('name').trim(),
          company: formData.get('company').trim(),
          notes: formData.get('notes').trim()
        };

        const errors = validateClient(newClient);
        if(errors.length > 0) {
          alert('Please fix the following errors before submitting:\n- ' + errors.join('\n- '));
          return;
        }

        clients.push(newClient);
        saveClients();
        renderClientsList();
        populateClientDropdown();
        clientForm.reset();
        clientForm.querySelector('input').focus();
      });

      // --- Handle delete client ---
      document.querySelector('#clients-list tbody').addEventListener('click', e => {
        if(e.target.tagName === 'BUTTON') {
          const id = e.target.dataset.id;
          const client = clients.find(c => c.id === id);
          if(client) {
            const relatedEntries = journalEntries.filter(entry => entry.clientId === id);
            let confirmText = `Are you sure you want to delete client "${client.name}"?`;
            if (relatedEntries.length > 0) {
              confirmText += `\n\nWarning: This client is associated with ${relatedEntries.length} journal entr${relatedEntries.length > 1 ? 'ies' : 'y'}.\nDeleting the client will NOT delete the journal entries, but their client association will be removed.`;
            }
            if(confirm(confirmText)) {
              clients = clients.filter(c => c.id !== id);
              // Remove client association from entries
              journalEntries.forEach(entry => {
                if(entry.clientId === id) entry.clientId = '';
              });
              saveClients();
              saveEntries();
              renderClientsList();
              populateClientDropdown();
              renderJournalEntries();
              // Refresh ledger if visible
              if (!sections.ledger.hidden) renderGeneralLedger();
            }
          }
        }
      });


      // ===== General Ledger Rendering =====
      function renderGeneralLedger() {
        ledgerEntriesBody.innerHTML = '';
        const filterClientId = ledgerFilterClient.value;

        if(journalEntries.length === 0) {
          ledgerEntriesBody.innerHTML = '<tr><td colspan="7" style="text-align:center;color:#7f7f9c;">No ledger entries available</td></tr>';
          return;
        }

        // Filter entries by client if needed
        let filteredEntries = journalEntries;
        if(filterClientId !== 'all') {
          filteredEntries = journalEntries.filter(entry => entry.clientId === filterClientId);
        }

        // Group by account
        const ledgerByAccount = {};

        filteredEntries.forEach(({ date, description, debitAccount, debitAmount, creditAccount, creditAmount, clientId }) => {
          if (!ledgerByAccount[debitAccount]) ledgerByAccount[debitAccount] = [];
          if (!ledgerByAccount[creditAccount]) ledgerByAccount[creditAccount] = [];

          ledgerByAccount[debitAccount].push({
            date,
            description,
            debit: debitAmount,
            credit: 0,
            clientId,
          });

          ledgerByAccount[creditAccount].push({
            date,
            description,
            debit: 0,
            credit: creditAmount,
            clientId,
          });
        });

        // Sort accounts alphabetically
        const accounts = Object.keys(ledgerByAccount).sort();

        // Render rows grouped by accounts with running balance
        accounts.forEach(account => {
          const transactions = ledgerByAccount[account];
          transactions.sort((a, b) => new Date(a.date) - new Date(b.date));
          let runningBalance = 0;
          let firstRow = true;

          transactions.forEach(tx => {
            const debitVal = Number(tx.debit);
            const creditVal = Number(tx.credit);
            runningBalance += debitVal;
            runningBalance -= creditVal;

            const clientName = clients.find(c => c.id === tx.clientId)?.name || '';

            const tr = document.createElement('tr');
            tr.setAttribute('tabindex', '-1');
            tr.setAttribute('role', 'row');
            tr.innerHTML = `
              <td>${firstRow ? account : ''}</td>
              <td>${formatDate(tx.date)}</td>
              <td>${tx.description}</td>
              <td style="text-align:right;">${debitVal !== 0 ? formatAmount(debitVal) : ''}</td>
              <td style="text-align:right;">${creditVal !== 0 ? formatAmount(creditVal) : ''}</td>
              <td style="text-align:right;" class="${runningBalance < 0 ? 'balance negative' : 'balance'}">${formatAmount(runningBalance)}</td>
              <td>${clientName}</td>
            `;
            ledgerEntriesBody.appendChild(tr);
            firstRow = false;
          });
        });
      }

      ledgerFilterClient.addEventListener('change', renderGeneralLedger);

      // ===== Backup & Restore =====
      const exportBtn = document.getElementById('export-btn');
      const importFileInput = document.getElementById('import-file');
      const backupMessage = document.getElementById('backup-message');
      const exportPDFBtn = document.getElementById('export-pdf-btn');

      exportBtn.addEventListener('click', () => {
        const data = {
          journalEntries,
          clients,
          exportedAt: new Date().toISOString()
        };
        const blob = new Blob([JSON.stringify(data, null, 2)], {type:'application/json'});
        const url = URL.createObjectURL(blob);
        const a = document.createElement('a');
        a.href = url;
        a.download = `bookkeeping_backup_${new Date().toISOString().slice(0,10)}.json`;
        document.body.appendChild(a);
        a.click();
        document.body.removeChild(a);
        URL.revokeObjectURL(url);
        backupMessage.textContent = 'Backup exported. Save this file safely.';
      });

      importFileInput.addEventListener('change', e => {
        const file = e.target.files[0];
        if(!file) return;
        const reader = new FileReader();
        reader.onload = (event) => {
          try {
            const jsonData = JSON.parse(event.target.result);
            if(!jsonData.journalEntries || !jsonData.clients) {
              throw new Error('Invalid backup file format.');
            }
            if(confirm('Importing backup will overwrite current data. Proceed?')) {
              if(Array.isArray(jsonData.journalEntries) && Array.isArray(jsonData.clients)) {
                journalEntries.length = 0;
                journalEntries.push(...jsonData.journalEntries);
                clients.length = 0;
                clients.push(...jsonData.clients);
                saveEntries();
                saveClients();
                renderClientsList();
                populateClientDropdown();
                renderJournalEntries();
                renderGeneralLedger();
                backupMessage.textContent = 'Backup successfully restored.';
              } else {
                alert('Backup file content invalid or incomplete.');
              }
            }
          } catch (err) {
            alert('Error reading backup file: ' + err.message);
          }
        };
        reader.readAsText(file);
        importFileInput.value = '';
      });

      // ===== PDF Export =====
      exportPDFBtn.addEventListener('click', () => {
        if(typeof window.jspdf === 'undefined' || typeof window.jspdf.jsPDF === 'undefined') {
          alert('PDF export library not loaded.');
          return;
        }
        const { jsPDF } = window.jspdf;
        const doc = new jsPDF();

        doc.setFont('helvetica', 'bold');
        doc.setFontSize(18);
        doc.setTextColor('#7e56d9');
        doc.text('Bookkeeping Report', 14, 20);

        doc.setFontSize(10);
        doc.setTextColor('#000');
        doc.text(`Generated: ${new Date().toLocaleString()}`, 14, 28);

        // Prepare Journal Entries table for autoTable
        const journalHeaders = ['Date', 'Description', 'Debit Account', 'Debit Amount', 'Credit Account', 'Credit Amount', 'Client'];
        const journalData = journalEntries.map(entry => {
          const clientName = clients.find(c => c.id === entry.clientId)?.name || '';
          return [
            formatDate(entry.date),
            entry.description,
            entry.debitAccount,
            formatAmount(entry.debitAmount),
            entry.creditAccount,
            formatAmount(entry.creditAmount),
            clientName
          ];
        });

        doc.setFontSize(14);
        doc.setTextColor('#0a0a2a');
        doc.text('Journal Entries', 14, 40);

        doc.autoTable({
          startY: 44,
          head: [journalHeaders],
          body: journalData,
          theme: 'grid',
          headStyles: {
            fillColor: [126, 86, 217],
            textColor: 255,
            fontStyle: 'bold',
          },
          alternateRowStyles: { fillColor: [245,245,245] },
          styles: {
            textColor: [0,0,0],
            fontSize: 8,
            cellPadding: 2,
          },
          margin: { left: 14, right: 14 },
          tableLineColor: [126, 86, 217],
          tableLineWidth: 0.15,
          didDrawPage: function(data) {
            if (doc.lastAutoTable.finalY > 235) {
              doc.addPage();
            }
          }
        });

        // Clients section on next page if any clients
        if(clients.length > 0) {
          const lastY = doc.lastAutoTable ? doc.lastAutoTable.finalY + 10 : 250;
          doc.addPage();
          doc.setFontSize(14);
          doc.setTextColor('#0a0a2a');
          doc.text('Clients', 14, 20);

          const clientHeaders = ['Client Name', 'Company', 'Notes'];
          const clientData = clients.map(c => [c.name, c.company || '', c.notes || '']);

          doc.autoTable({
            startY: 24,
            head: [clientHeaders],
            body: clientData,
            theme: 'grid',
            headStyles: {
              fillColor: [126, 86, 217],
              textColor: 255,
              fontStyle: 'bold',
            },
            alternateRowStyles: { fillColor: [245,245,245] },
            styles: {
              textColor: [0,0,0],
              fontSize: 9,
              cellPadding: 2,
            },
            margin: { left: 14, right: 14 },
            tableLineColor: [126, 86, 217],
            tableLineWidth: 0.15,
          });
        }

        doc.save(`bookkeeping_report_${new Date().toISOString().slice(0,10)}.pdf`);
      });

      // Initial rendering
      renderClientsList();
      populateClientDropdown();
      renderJournalEntries();
      renderGeneralLedger();

    })();
  </script>
</body>
</html>

