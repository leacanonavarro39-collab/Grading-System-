<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sunflower Grading System - Lea Caño</title>
    <style>
        :root {
            --primary-yellow: #ffcc00;
            --accent-cyan: #00ffe5;
            --glass-bg: rgba(15, 15, 15, 0.95);
            --pass-color: #2ecc71;
            --fail-color: #e74c3c;
            --excel-border: #444;
        }

        body {
            font-family: 'Segoe UI', sans-serif;
            margin: 0;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('https://images.unsplash.com/photo-1470509037663-253afd7f0f51?q=80&w=1974&auto=format&fit=crop') no-repeat center center fixed;
            background-size: cover;
            color: white;
            min-height: 100vh;
        }

        header {
            background: rgba(0, 0, 0, 0.85);
            color: var(--primary-yellow);
            padding: 20px;
            text-align: center;
            font-size: 24px;
            font-weight: 800;
            border-bottom: 4px solid var(--primary-yellow);
            backdrop-filter: blur(10px);
        }

        .container {
            display: flex;
            justify-content: center;
            padding: 40px 20px;
        }

        .calculator-card {
            background: var(--glass-bg);
            padding: 30px;
            border-radius: 20px;
            width: 100%;
            max-width: 450px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 20px 40px rgba(0,0,0,0.5);
        }

        h2 { text-align: center; color: var(--primary-yellow); margin-bottom: 20px; }

        .input-group { display: flex; flex-direction: column; gap: 10px; }

        input, select {
            padding: 12px;
            border-radius: 8px;
            border: 1px solid #444;
            text-align: center;
            font-weight: bold;
            outline: none;
        }

        .grade-row { display: flex; gap: 10px; align-items: center; }
        .grade-row span { flex: 1.5; font-size: 0.9rem; color: #ccc; }
        .grade-row input { flex: 1; background: #fff; color: #000; }

        .compute-btn {
            background: linear-gradient(45deg, #ff7e5f, #feb47b);
            color: white;
            padding: 15px;
            border-radius: 8px;
            border: none;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
            transition: 0.3s;
        }

        .view-btn {
            background: none;
            border: 2px solid var(--accent-cyan);
            color: var(--accent-cyan);
            padding: 10px;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 5px;
        }

        /* EXCEL STYLE MODAL */
        .modal-overlay {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal-content {
            background: #1a1a1a;
            width: 95%;
            max-width: 1200px;
            max-height: 85vh;
            padding: 25px;
            border-radius: 12px;
            border: 1px solid var(--accent-cyan);
            overflow: auto;
            position: relative;
        }

        .close-modal {
            position: absolute;
            top: 10px; right: 20px;
            font-size: 35px; color: #ff4d4d; cursor: pointer;
        }

        /* EXCEL TABLE STYLE */
        .excel-table {
            width: 100%;
            border-collapse: collapse;
            background: #fff;
            color: #222;
            margin-top: 20px;
        }

        .excel-table th {
            background: #2c3e50;
            color: white;
            padding: 12px;
            border: 1px solid var(--excel-border);
            text-transform: uppercase;
            font-size: 0.8rem;
        }

        .excel-table td {
            padding: 10px;
            border: 1px solid #ccc;
            text-align: center;
            font-weight: 500;
        }

        .excel-table tr:nth-child(even) { background: #f9f9f9; }
        .excel-table tr:hover { background: #f1f1f1; }

        .status-pass { background: #d4edda; color: #155724; font-weight: bold; border-radius: 4px; padding: 4px; }
        .status-fail { background: #f8d7da; color: #721c24; font-weight: bold; border-radius: 4px; padding: 4px; }

        .btn-group { display: flex; gap: 4px; justify-content: center; }
        .btn-action { padding: 6px 10px; border-radius: 4px; border: none; cursor: pointer; font-size: 0.75rem; font-weight: bold; }
        .edit { background: #ffc107; color: #000; }
        .del { background: #dc3545; color: #fff; }
        .print { background: #17a2b8; color: #fff; }

        .footer { text-align: center; padding: 20px; color: var(--primary-yellow); font-weight: bold; }
    </style>
</head>
<body>

<header>Sunflower Grading System — Lea Caño BSIT-3A</header>

<div class="container">
    <div class="calculator-card">
        <h2>Add Student Grades</h2>
        <div class="input-group">
            <input type="text" id="studentName" placeholder="Student Full Name">
            
            <div class="grade-row"><span>Programming:</span><input type="number" id="g1" placeholder="0-100" oninput="validate(this)"></div>
            <div class="grade-row"><span>Database:</span><input type="number" id="g2" placeholder="0-100" oninput="validate(this)"></div>
            <div class="grade-row"><span>Networking:</span><input type="number" id="g3" placeholder="0-100" oninput="validate(this)"></div>
            <div class="grade-row"><span>Web Development:</span><input type="number" id="g4" placeholder="0-100" oninput="validate(this)"></div>
            <div class="grade-row"><span>Info Security:</span><input type="number" id="g5" placeholder="0-100" oninput="validate(this)"></div>

            <div style="margin-top:10px; font-weight: bold; text-align: center; color: var(--primary-yellow);">
                AVERAGE: <span id="avgDisplay">0.00</span>
            </div>
            
            <button class="compute-btn" id="saveBtn" onclick="saveRecord()">SAVE TO DATABASE</button>
            <button class="view-btn" onclick="toggleModal(true)">VIEW RECORDS (EXCEL VIEW)</button>
        </div>
    </div>
</div>

<div class="modal-overlay" id="modalOverlay">
    <div class="modal-content">
        <span class="close-modal" onclick="toggleModal(false)">&times;</span>
        <h2 style="color: var(--accent-cyan); text-align: left;">Student Records - Sheet1</h2>
        <div style="overflow-x: auto;">
            <table class="excel-table">
                <thead>
                    <tr>
                        <th rowspan="2">Student Name</th>
                        <th colspan="5">Subjects</th>
                        <th rowspan="2">Average</th>
                        <th rowspan="2">Remarks</th>
                        <th rowspan="2" class="no-print">Actions</th>
                    </tr>
                    <tr>
                        <th>Prog</th>
                        <th>DB</th>
                        <th>Net</th>
                        <th>Web</th>
                        <th>InfoSec</th>
                    </tr>
                </thead>
                <tbody id="recordList"></tbody>
            </table>
        </div>
    </div>
</div>

<div class="footer">DEVELOPED BY: LEA CAÑO | BSIT 3-A</div>

<script>
    let records = JSON.parse(localStorage.getItem("lea_excel_records")) || [];
    let editIndex = null;

    function validate(input) {
        if (input.value > 100) input.value = 100;
        if (input.value < 0) input.value = 0;
        calculateAvg();
    }

    function calculateAvg() {
        let grades = [
            parseFloat(document.getElementById("g1").value) || 0,
            parseFloat(document.getElementById("g2").value) || 0,
            parseFloat(document.getElementById("g3").value) || 0,
            parseFloat(document.getElementById("g4").value) || 0,
            parseFloat(document.getElementById("g5").value) || 0
        ];
        let total = grades.reduce((a, b) => a + b, 0);
        let avg = total / 5;
        document.getElementById("avgDisplay").innerText = avg.toFixed(2);
        return avg.toFixed(2);
    }

    function saveRecord() {
        let name = document.getElementById("studentName").value;
        let avg = calculateAvg();
        let g1 = document.getElementById("g1").value || 0;
        let g2 = document.getElementById("g2").value || 0;
        let g3 = document.getElementById("g3").value || 0;
        let g4 = document.getElementById("g4").value || 0;
        let g5 = document.getElementById("g5").value || 0;

        if(!name || name.trim() === "") { alert("Please enter student name."); return; }

        let remarks = avg >= 75 ? "PASSED" : "FAILED";
        let recordData = { name, grades: [g1, g2, g3, g4, g5], avg, remarks };

        if(editIndex !== null) {
            records[editIndex] = recordData;
            editIndex = null;
            document.getElementById("saveBtn").innerText = "SAVE TO DATABASE";
        } else {
            records.push(recordData);
        }

        localStorage.setItem("lea_excel_records", JSON.stringify(records));
        alert("Data successfully stored!");
        clearForm();
        renderRecords();
    }

    function renderRecords() {
        let list = document.getElementById("recordList");
        list.innerHTML = "";
        
        if (records.length === 0) {
            list.innerHTML = "<tr><td colspan='9'>No data available in sheet.</td></tr>";
            return;
        }

        records.forEach((r, i) => {
            list.innerHTML += `
                <tr>
                    <td style="text-align:left; padding-left:15px;">${r.name}</td>
                    <td>${r.grades[0]}</td>
                    <td>${r.grades[1]}</td>
                    <td>${r.grades[2]}</td>
                    <td>${r.grades[3]}</td>
                    <td>${r.grades[4]}</td>
                    <td style="background:#fff7d1; font-weight:bold;">${r.avg}</td>
                    <td><span class="${r.remarks == 'PASSED' ? 'status-pass' : 'status-fail'}">${r.remarks}</span></td>
                    <td>
                        <div class="btn-group">
                            <button class="btn-action edit" onclick="editRecord(${i})">Edit</button>
                            <button class="btn-action del" onclick="deleteRecord(${i})">Delete</button>
                            <button class="btn-action print" onclick="printReport(${i})">Print</button>
                        </div>
                    </td>
                </tr>`;
        });
    }

    function editRecord(i) {
        let r = records[i];
        document.getElementById("studentName").value = r.name;
        document.getElementById("g1").value = r.grades[0];
        document.getElementById("g2").value = r.grades[1];
        document.getElementById("g3").value = r.grades[2];
        document.getElementById("g4").value = r.grades[3];
        document.getElementById("g5").value = r.grades[4];
        calculateAvg();
        editIndex = i;
        document.getElementById("saveBtn").innerText = "UPDATE DATA";
        toggleModal(false);
    }

    function deleteRecord(i) {
        if(confirm("Confirm deletion of record?")) {
            records.splice(i, 1);
            localStorage.setItem("lea_excel_records", JSON.stringify(records));
            renderRecords();
        }
    }

    function printReport(i) {
        let r = records[i];
        let w = window.open('', '', 'width=800,height=600');
        w.document.write(`
            <html><head><title>Academic Report</title>
            <style>
                body{ font-family: sans-serif; padding: 40px; }
                .header{ text-align: center; border-bottom: 2px solid #000; padding-bottom: 10px; }
                table{ width: 100%; border-collapse: collapse; margin-top: 30px; }
                th, td{ border: 1px solid #000; padding: 12px; text-align: center; }
                .footer{ margin-top: 50px; display: flex; justify-content: space-between; }
            </style></head>
            <body>
                <div class="header">
                    <h2>OFFICIAL STUDENT GRADE REPORT</h2>
                    <p>Generated by Lea Caño Grading System</p>
                </div>
                <p><strong>STUDENT NAME:</strong> ${r.name.toUpperCase()}</p>
                <table>
                    <thead>
                        <tr><th>Subject</th><th>Grade</th></tr>
                    </thead>
                    <tbody>
                        <tr><td>Programming</td><td>${r.grades[0]}</td></tr>
                        <tr><td>Database</td><td>${r.grades[1]}</td></tr>
                        <tr><td>Networking</td><td>${r.grades[2]}</td></tr>
                        <tr><td>Web Development</td><td>${r.grades[3]}</td></tr>
                        <tr><td>Information Security</td><td>${r.grades[4]}</td></tr>
                        <tr style="background:#eee;"><td><strong>AVERAGE</strong></td><td><strong>${r.avg}</strong></td></tr>
                        <tr style="background:#eee;"><td><strong>REMARKS</strong></td><td><strong>${r.remarks}</strong></td></tr>
                    </tbody>
                </table>
                <div class="footer">
                    <div>Date: ${new Date().toLocaleDateString()}</div>
                    <div>Signature: __________________</div>
                </div>
            </body></html>
        `);
        w.document.close();
        w.print();
    }

    function toggleModal(show) {
        document.getElementById("modalOverlay").style.display = show ? "flex" : "none";
        if(show) renderRecords();
    }

    function clearForm() {
        document.getElementById("studentName").value = "";
        ["g1","g2","g3","g4","g5"].forEach(id => document.getElementById(id).value = "");
        document.getElementById("avgDisplay").innerText = "0.00";
    }
</script>
</body>
</html>
