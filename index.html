import React, { useState } from 'react';
import { ChevronDown, ChevronRight, Plus, Trash2, Edit2, Save, X, Download, FileText } from 'lucide-react';

const initialData = [
  {
    id: 1,
    area: "Primary Goal",
    dsc: "Ensure the competitions operate smoothly, fairly, and to a high technical standard.",
    dscTasks: [],
    doo: "Ensure the Host Organization practically delivers the necessary resources, venue, and logistics.",
    dooTasks: []
  },
  {
    id: 2,
    area: "Expert & Official Management",
    dsc: "Critical Responsibility: Ensure every Official Skill has a nominated Chief Expert (CE) and Deputy Chief Expert (DCE) in place, as skills cannot operate without them. Approve final CE/DCE nominations after elections. Manage replacements and continuity if a CE or DCE steps down or withdraws. Oversee the recruitment and management of Jury Presidents and Team Leaders.",
    dscTasks: [],
    doo: "Logistical Support: Advise the Host on the accreditation and package requirements for these officials. Ensure the Host's accreditation system correctly categorizes Experts and Officials for access control. Advise on accommodation allocation to ensure Experts are housed appropriately (often separate from Competitors).",
    dooTasks: []
  },
  {
    id: 3,
    area: "Technical Standards & Quality",
    dsc: "Standard Setting: Oversee the Technical Descriptions and ensure they are updated and \"locked\" at the Skills Development Workshop (SDW). Manage the Test Project selection and validation process to ensure high-quality assessment tasks. Ensure accurate Results Processing and maintain the integrity of the marking system (CIS).",
    dscTasks: [],
    doo: "Resource Delivery: Guide the Host on the Infrastructure List (IL) acquisition process, ensuring the right equipment is sourced. Manage the \"WSE IL System\" tracking to ensure all requested items are physically accounted for. Validate that the \"Competitor Toolboxes\" logistics (shipping, customs, electrical testing) are managed correctly by the Host.",
    dooTasks: []
  },
  {
    id: 4,
    area: "Competition Committee (CC) & Governance",
    dsc: "Committee Liaison: Work directly with the Chair and Vice Chair of the CC on technical and operational matters. Lead Statutory Meetings (e.g., General Assembly updates) and Competition Committee meetings. Enforce Competition Rules and manage the \"Issue and Dispute Resolution\" process.",
    dscTasks: [],
    doo: "Host Liaison: Act as the primary operational link between WSE and the Host Organization (HO). Ensure the Host complies with the Hosting Agreement regarding logistical deliverables. Advise on the Accreditation Packages pricing and inclusions for Members.",
    dooTasks: []
  },
  {
    id: 5,
    area: "Event Preparation & Meetings",
    dsc: "Content & Agenda: Define the technical agenda for the Competition Preparation Meetings (CPM) to finalize Skills Management Plans. Run Team Leader briefings regarding competition rules and ceremonies.",
    dscTasks: [],
    doo: "Logistics & Venues: Ensure the Host provides suitable meeting rooms, plenary halls, and AV setups for CPMs and CC meetings. Manage the operational schedule for these meetings (room capacity, catering, access).",
    dooTasks: []
  },
  {
    id: 6,
    area: "Venue & Workshops",
    dsc: "Operational Environment: Approve the final workshop layouts to ensure they meet technical assessment needs (e.g., \"fairness\" of layout). Monitor Health, Safety & Environment (HSE) compliance within the skills environment.",
    dscTasks: [],
    doo: "Build & Facilities: Oversee the Build/Dismantle Plan, ensuring the Host gives access to workshops on time. Advise on venue utilities (power, compressed air, waste management) and general cleanliness. Manage the \"Warehousing Approach\" (onsite vs. offsite) and logistics flow.",
    dooTasks: []
  },
  {
    id: 7,
    area: "Delegate Services (Logistics)",
    dsc: "Participant Welfare: Ensure the competition schedule allows for proper breaks and competitor welfare. Oversee the \"Code of Ethics\" regarding competitor fairness.",
    dscTasks: [],
    doo: "Practical Delivery: Accommodation - Advise on hotel selection, grading, and capacity planning for all delegates. Transport - Validate the Host's transport master plan (airport arrivals, daily shuttle buses). Catering - Ensure adequate lunch systems (buffet vs. packed) and dietary requirement management (allergies, Halal, etc.).",
    dooTasks: []
  },
  {
    id: 8,
    area: "Medals & Ceremonies",
    dsc: "Official Protocol: Manage the official results data for the Closing Ceremony. Oversee the design and approval of Medals and Certificates. Ensure correct protocol for the \"Best of Nation\" and \"Jos de Goey\" awards.",
    dscTasks: [],
    doo: "Coordinate logistics for the \"Farewell Party\" and other social receptions.",
    dooTasks: []
  }
];

export default function WSEResponsibilities() {
  const [data, setData] = useState(initialData);
  const [expandedRows, setExpandedRows] = useState(new Set());
  const [editingArea, setEditingArea] = useState(null);
  const [editingDsc, setEditingDsc] = useState(null);
  const [editingDoo, setEditingDoo] = useState(null);
  const [newTaskDsc, setNewTaskDsc] = useState({});
  const [newTaskDoo, setNewTaskDoo] = useState({});
  const [editValues, setEditValues] = useState({});
  const [showAddRow, setShowAddRow] = useState(false);
  const [newRow, setNewRow] = useState({ area: '', dsc: '', doo: '' });

  const toggleRow = (id) => {
    const newExpanded = new Set(expandedRows);
    if (newExpanded.has(id)) {
      newExpanded.delete(id);
    } else {
      newExpanded.add(id);
    }
    setExpandedRows(newExpanded);
  };

  const startEditing = (type, id, value) => {
    setEditValues({ ...editValues, [`${type}-${id}`]: value });
    if (type === 'area') setEditingArea(id);
    else if (type === 'dsc') setEditingDsc(id);
    else if (type === 'doo') setEditingDoo(id);
  };

  const saveEdit = (type, id) => {
    const value = editValues[`${type}-${id}`];
    setData(data.map(row => {
      if (row.id === id) {
        return { ...row, [type]: value };
      }
      return row;
    }));
    if (type === 'area') setEditingArea(null);
    else if (type === 'dsc') setEditingDsc(null);
    else if (type === 'doo') setEditingDoo(null);
  };

  const cancelEdit = (type) => {
    if (type === 'area') setEditingArea(null);
    else if (type === 'dsc') setEditingDsc(null);
    else if (type === 'doo') setEditingDoo(null);
  };

  const addTask = (rowId, role) => {
    const taskText = role === 'dsc' ? newTaskDsc[rowId] : newTaskDoo[rowId];
    if (!taskText?.trim()) return;
    
    setData(data.map(row => {
      if (row.id === rowId) {
        const tasks = role === 'dsc' ? [...row.dscTasks, taskText] : [...row.dooTasks, taskText];
        return { ...row, [role === 'dsc' ? 'dscTasks' : 'dooTasks']: tasks };
      }
      return row;
    }));
    
    if (role === 'dsc') {
      setNewTaskDsc({ ...newTaskDsc, [rowId]: '' });
    } else {
      setNewTaskDoo({ ...newTaskDoo, [rowId]: '' });
    }
  };

  const removeTask = (rowId, role, taskIndex) => {
    setData(data.map(row => {
      if (row.id === rowId) {
        const taskKey = role === 'dsc' ? 'dscTasks' : 'dooTasks';
        const tasks = row[taskKey].filter((_, i) => i !== taskIndex);
        return { ...row, [taskKey]: tasks };
      }
      return row;
    }));
  };

  const addNewRow = () => {
    if (!newRow.area.trim()) return;
    const newId = Math.max(...data.map(d => d.id)) + 1;
    setData([...data, { 
      id: newId, 
      area: newRow.area, 
      dsc: newRow.dsc, 
      doo: newRow.doo,
      dscTasks: [],
      dooTasks: []
    }]);
    setNewRow({ area: '', dsc: '', doo: '' });
    setShowAddRow(false);
  };

  const deleteRow = (id) => {
    if (window.confirm('Delete this responsibility area?')) {
      setData(data.filter(row => row.id !== id));
    }
  };

  const exportToPDF = () => {
    const printContent = `
      <!DOCTYPE html>
      <html>
      <head>
        <title>WSE Director Responsibilities</title>
        <style>
          @page { size: landscape; margin: 15mm; }
          body { font-family: Arial, sans-serif; font-size: 10px; line-height: 1.4; }
          h1 { font-size: 16px; color: #1e3a5f; margin-bottom: 5px; }
          h2 { font-size: 11px; color: #666; margin-bottom: 15px; font-weight: normal; }
          table { width: 100%; border-collapse: collapse; }
          th { background: #1e3a5f; color: white; padding: 8px 6px; text-align: left; font-size: 9px; }
          td { border: 1px solid #ddd; padding: 6px; vertical-align: top; }
          .area { font-weight: bold; background: #f8f9fa; width: 15%; }
          .role-col { width: 42.5%; }
          .responsibility { margin-bottom: 6px; }
          .tasks { margin-top: 8px; padding-top: 6px; border-top: 1px dashed #ccc; }
          .task-title { font-weight: bold; font-size: 9px; color: #666; margin-bottom: 4px; }
          .task-item { margin: 3px 0; padding-left: 10px; position: relative; }
          .task-item:before { content: "•"; position: absolute; left: 0; color: #1e3a5f; }
          .footer { margin-top: 20px; font-size: 8px; color: #999; text-align: center; }
        </style>
      </head>
      <body>
        <h1>WorldSkills Europe - Director Responsibilities Matrix</h1>
        <h2>Division of responsibilities between Director of Skills Competitions and Director of Operations</h2>
        <table>
          <thead>
            <tr>
              <th style="width:15%">Key Area</th>
              <th class="role-col">Director of Skills Competitions<br/><span style="font-weight:normal;font-size:8px">(Quality, Governance & Experts)</span></th>
              <th class="role-col">Director of Operations<br/><span style="font-weight:normal;font-size:8px">(Host Advisory, Infrastructure & Logistics)</span></th>
            </tr>
          </thead>
          <tbody>
            ${data.map(row => `
              <tr>
                <td class="area">${row.area}</td>
                <td>
                  <div class="responsibility">${row.dsc}</div>
                  ${row.dscTasks.length > 0 ? `
                    <div class="tasks">
                      <div class="task-title">Specific Tasks:</div>
                      ${row.dscTasks.map(task => `<div class="task-item">${task}</div>`).join('')}
                    </div>
                  ` : ''}
                </td>
                <td>
                  <div class="responsibility">${row.doo}</div>
                  ${row.dooTasks.length > 0 ? `
                    <div class="tasks">
                      <div class="task-title">Specific Tasks:</div>
                      ${row.dooTasks.map(task => `<div class="task-item">${task}</div>`).join('')}
                    </div>
                  ` : ''}
                </td>
              </tr>
            `).join('')}
          </tbody>
        </table>
        <div class="footer">Generated on ${new Date().toLocaleDateString('en-GB', { day: 'numeric', month: 'long', year: 'numeric' })}</div>
      </body>
      </html>
    `;
    
    const printWindow = window.open('', '_blank');
    printWindow.document.write(printContent);
    printWindow.document.close();
    printWindow.onload = () => {
      printWindow.print();
    };
  };

  return (
    <div className="min-h-screen bg-gray-50 p-4">
      <div className="max-w-7xl mx-auto">
        {/* Header */}
        <div className="bg-white rounded-lg shadow-sm p-6 mb-4">
          <div className="flex justify-between items-start">
            <div>
              <h1 className="text-2xl font-bold text-slate-800">WSE Director Responsibilities</h1>
              <p className="text-slate-500 mt-1">Manage responsibilities and tasks for WorldSkills Europe Director roles</p>
            </div>
            <div className="flex gap-2">
              <button
                onClick={() => setShowAddRow(true)}
                className="flex items-center gap-2 px-4 py-2 bg-slate-700 text-white rounded-lg hover:bg-slate-800 transition-colors"
              >
                <Plus size={18} /> Add Area
              </button>
              <button
                onClick={exportToPDF}
                className="flex items-center gap-2 px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700 transition-colors"
              >
                <Download size={18} /> Export PDF
              </button>
            </div>
          </div>
        </div>

        {/* Add New Row Modal */}
        {showAddRow && (
          <div className="fixed inset-0 bg-black/50 flex items-center justify-center z-50">
            <div className="bg-white rounded-lg shadow-xl p-6 w-full max-w-2xl mx-4">
              <h3 className="text-lg font-semibold mb-4">Add New Responsibility Area</h3>
              <div className="space-y-4">
                <div>
                  <label className="block text-sm font-medium text-gray-700 mb-1">Key Area Name</label>
                  <input
                    type="text"
                    value={newRow.area}
                    onChange={(e) => setNewRow({...newRow, area: e.target.value})}
                    className="w-full border rounded-lg px-3 py-2 focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
                    placeholder="e.g., Sponsor Relations"
                  />
                </div>
                <div>
                  <label className="block text-sm font-medium text-gray-700 mb-1">Director of Skills Competitions</label>
                  <textarea
                    value={newRow.dsc}
                    onChange={(e) => setNewRow({...newRow, dsc: e.target.value})}
                    className="w-full border rounded-lg px-3 py-2 h-24 focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
                    placeholder="High-level responsibility..."
                  />
                </div>
                <div>
                  <label className="block text-sm font-medium text-gray-700 mb-1">Director of Operations</label>
                  <textarea
                    value={newRow.doo}
                    onChange={(e) => setNewRow({...newRow, doo: e.target.value})}
                    className="w-full border rounded-lg px-3 py-2 h-24 focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
                    placeholder="High-level responsibility..."
                  />
                </div>
              </div>
              <div className="flex justify-end gap-2 mt-6">
                <button
                  onClick={() => { setShowAddRow(false); setNewRow({ area: '', dsc: '', doo: '' }); }}
                  className="px-4 py-2 border rounded-lg hover:bg-gray-50"
                >
                  Cancel
                </button>
                <button
                  onClick={addNewRow}
                  className="px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700"
                >
                  Add Area
                </button>
              </div>
            </div>
          </div>
        )}

        {/* Legend */}
        <div className="grid grid-cols-3 gap-4 mb-4">
          <div className="bg-slate-100 rounded-lg p-3 text-center">
            <span className="text-xs text-slate-500 uppercase tracking-wide">Key Areas</span>
          </div>
          <div className="bg-blue-50 border-l-4 border-blue-600 rounded-lg p-3 text-center">
            <span className="text-sm font-medium text-blue-800">Director of Skills Competitions</span>
            <span className="block text-xs text-blue-600">Quality, Governance & Experts</span>
          </div>
          <div className="bg-emerald-50 border-l-4 border-emerald-600 rounded-lg p-3 text-center">
            <span className="text-sm font-medium text-emerald-800">Director of Operations</span>
            <span className="block text-xs text-emerald-600">Host Advisory, Infrastructure & Logistics</span>
          </div>
        </div>

        {/* Table */}
        <div className="bg-white rounded-lg shadow-sm overflow-hidden">
          {data.map((row) => (
            <div key={row.id} className="border-b last:border-b-0">
              {/* Main Row */}
              <div className="grid grid-cols-12 min-h-[80px]">
                {/* Area Column */}
                <div className="col-span-2 bg-slate-50 p-3 flex items-start gap-2 border-r">
                  <button
                    onClick={() => toggleRow(row.id)}
                    className="mt-1 text-slate-400 hover:text-slate-600 flex-shrink-0"
                  >
                    {expandedRows.has(row.id) ? <ChevronDown size={16} /> : <ChevronRight size={16} />}
                  </button>
                  <div className="flex-1">
                    {editingArea === row.id ? (
                      <div className="flex items-center gap-1">
                        <input
                          type="text"
                          value={editValues[`area-${row.id}`] || ''}
                          onChange={(e) => setEditValues({...editValues, [`area-${row.id}`]: e.target.value})}
                          className="flex-1 border rounded px-2 py-1 text-sm"
                          autoFocus
                        />
                        <button onClick={() => saveEdit('area', row.id)} className="text-green-600 hover:text-green-700">
                          <Save size={14} />
                        </button>
                        <button onClick={() => cancelEdit('area')} className="text-red-500 hover:text-red-600">
                          <X size={14} />
                        </button>
                      </div>
                    ) : (
                      <div className="group flex items-start justify-between">
                        <span className="font-semibold text-slate-800 text-sm">{row.area}</span>
                        <div className="opacity-0 group-hover:opacity-100 flex gap-1 ml-1">
                          <button
                            onClick={() => startEditing('area', row.id, row.area)}
                            className="text-slate-400 hover:text-blue-600"
                          >
                            <Edit2 size={12} />
                          </button>
                          <button
                            onClick={() => deleteRow(row.id)}
                            className="text-slate-400 hover:text-red-600"
                          >
                            <Trash2 size={12} />
                          </button>
                        </div>
                      </div>
                    )}
                  </div>
                </div>

                {/* DSC Column */}
                <div className="col-span-5 p-3 border-r bg-blue-50/30">
                  {editingDsc === row.id ? (
                    <div className="space-y-2">
                      <textarea
                        value={editValues[`dsc-${row.id}`] || ''}
                        onChange={(e) => setEditValues({...editValues, [`dsc-${row.id}`]: e.target.value})}
                        className="w-full border rounded px-2 py-1 text-sm h-24"
                        autoFocus
                      />
                      <div className="flex gap-1">
                        <button onClick={() => saveEdit('dsc', row.id)} className="text-green-600 hover:text-green-700 text-xs flex items-center gap-1">
                          <Save size={12} /> Save
                        </button>
                        <button onClick={() => cancelEdit('dsc')} className="text-red-500 hover:text-red-600 text-xs flex items-center gap-1">
                          <X size={12} /> Cancel
                        </button>
                      </div>
                    </div>
                  ) : (
                    <div className="group">
                      <p className="text-sm text-slate-700 leading-relaxed">{row.dsc}</p>
                      <button
                        onClick={() => startEditing('dsc', row.id, row.dsc)}
                        className="opacity-0 group-hover:opacity-100 text-blue-600 text-xs mt-2 flex items-center gap-1"
                      >
                        <Edit2 size={10} /> Edit
                      </button>
                    </div>
                  )}
                </div>

                {/* DOO Column */}
                <div className="col-span-5 p-3 bg-emerald-50/30">
                  {editingDoo === row.id ? (
                    <div className="space-y-2">
                      <textarea
                        value={editValues[`doo-${row.id}`] || ''}
                        onChange={(e) => setEditValues({...editValues, [`doo-${row.id}`]: e.target.value})}
                        className="w-full border rounded px-2 py-1 text-sm h-24"
                        autoFocus
                      />
                      <div className="flex gap-1">
                        <button onClick={() => saveEdit('doo', row.id)} className="text-green-600 hover:text-green-700 text-xs flex items-center gap-1">
                          <Save size={12} /> Save
                        </button>
                        <button onClick={() => cancelEdit('doo')} className="text-red-500 hover:text-red-600 text-xs flex items-center gap-1">
                          <X size={12} /> Cancel
                        </button>
                      </div>
                    </div>
                  ) : (
                    <div className="group">
                      <p className="text-sm text-slate-700 leading-relaxed">{row.doo}</p>
                      <button
                        onClick={() => startEditing('doo', row.id, row.doo)}
                        className="opacity-0 group-hover:opacity-100 text-emerald-600 text-xs mt-2 flex items-center gap-1"
                      >
                        <Edit2 size={10} /> Edit
                      </button>
                    </div>
                  )}
                </div>
              </div>

              {/* Expanded Tasks Section */}
              {expandedRows.has(row.id) && (
                <div className="grid grid-cols-12 bg-slate-50/50 border-t">
                  <div className="col-span-2 p-3 border-r">
                    <span className="text-xs font-medium text-slate-500 uppercase tracking-wide">Specific Tasks</span>
                  </div>
                  
                  {/* DSC Tasks */}
                  <div className="col-span-5 p-3 border-r">
                    <div className="space-y-2">
                      {row.dscTasks.map((task, idx) => (
                        <div key={idx} className="flex items-start gap-2 bg-white rounded px-2 py-1.5 group">
                          <span className="text-blue-600 mt-0.5">•</span>
                          <span className="flex-1 text-sm text-slate-600">{task}</span>
                          <button
                            onClick={() => removeTask(row.id, 'dsc', idx)}
                            className="opacity-0 group-hover:opacity-100 text-red-400 hover:text-red-600"
                          >
                            <Trash2 size={12} />
                          </button>
                        </div>
                      ))}
                      <div className="flex gap-2 mt-2">
                        <input
                          type="text"
                          value={newTaskDsc[row.id] || ''}
                          onChange={(e) => setNewTaskDsc({...newTaskDsc, [row.id]: e.target.value})}
                          onKeyDown={(e) => e.key === 'Enter' && addTask(row.id, 'dsc')}
                          placeholder="Add specific task..."
                          className="flex-1 text-sm border rounded px-2 py-1.5 focus:ring-1 focus:ring-blue-500"
                        />
                        <button
                          onClick={() => addTask(row.id, 'dsc')}
                          className="px-2 py-1 bg-blue-100 text-blue-700 rounded hover:bg-blue-200 text-sm"
                        >
                          <Plus size={14} />
                        </button>
                      </div>
                    </div>
                  </div>

                  {/* DOO Tasks */}
                  <div className="col-span-5 p-3">
                    <div className="space-y-2">
                      {row.dooTasks.map((task, idx) => (
                        <div key={idx} className="flex items-start gap-2 bg-white rounded px-2 py-1.5 group">
                          <span className="text-emerald-600 mt-0.5">•</span>
                          <span className="flex-1 text-sm text-slate-600">{task}</span>
                          <button
                            onClick={() => removeTask(row.id, 'doo', idx)}
                            className="opacity-0 group-hover:opacity-100 text-red-400 hover:text-red-600"
                          >
                            <Trash2 size={12} />
                          </button>
                        </div>
                      ))}
                      <div className="flex gap-2 mt-2">
                        <input
                          type="text"
                          value={newTaskDoo[row.id] || ''}
                          onChange={(e) => setNewTaskDoo({...newTaskDoo, [row.id]: e.target.value})}
                          onKeyDown={(e) => e.key === 'Enter' && addTask(row.id, 'doo')}
                          placeholder="Add specific task..."
                          className="flex-1 text-sm border rounded px-2 py-1.5 focus:ring-1 focus:ring-emerald-500"
                        />
                        <button
                          onClick={() => addTask(row.id, 'doo')}
                          className="px-2 py-1 bg-emerald-100 text-emerald-700 rounded hover:bg-emerald-200 text-sm"
                        >
                          <Plus size={14} />
                        </button>
                      </div>
                    </div>
                  </div>
                </div>
              )}
            </div>
          ))}
        </div>

        {/* Footer */}
        <div className="mt-4 text-center text-sm text-slate-400">
          Click the arrow next to any area to expand and add specific tasks • Hover over text to edit
        </div>
      </div>
    </div>
  );
}
