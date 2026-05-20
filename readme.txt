<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Zaberman MVP Operational Hub</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>

<body class="bg-gray-100 text-gray-900 font-sans">
  <div class="min-h-screen flex">

    <!-- Sidebar -->
    <aside class="w-64 bg-white border-r border-gray-200 p-5 flex-shrink-0">
      <div class="mb-8">
        <div class="text-2xl font-bold">Zaberman IS</div>
        <div class="text-sm text-gray-500">Operational Hub</div>
      </div>

      <nav class="space-y-3 text-sm">
        <div class="bg-black text-white px-4 py-3 rounded-xl">Dashboard</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Orders</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Reports</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Analytics</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Routes</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Warehouse</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Integrations</div>
        <div class="bg-gray-50 border border-gray-200 px-4 py-3 rounded-xl">Admin</div>
      </nav>

      <div class="mt-8 text-xs text-gray-500">
        Operational Hub v0.1<br />
        Internal System Prototype
      </div>
    </aside>

    <!-- Main -->
    <main class="flex-1 min-w-0">

      <!-- Topbar -->
      <header class="bg-white border-b border-gray-200 px-6 py-4 flex items-center justify-between">
        <input
          type="text"
          placeholder="Search orders, customers, routes, contacts..."
          class="w-full max-w-xl border border-gray-300 rounded-xl px-4 py-3 outline-none text-sm"
        />

        <div class="flex items-center gap-4 ml-6">
          <div class="text-sm bg-yellow-50 text-yellow-700 border border-yellow-200 px-4 py-2 rounded-xl">
            🔔 12 Alerts
          </div>

          <select class="text-sm bg-gray-100 px-4 py-2 rounded-xl border border-gray-200">
            <option>BA Workspace</option>
            <option>Broker Workspace</option>
            <option>Dispatcher Workspace</option>
            <option>Warehouse Workspace</option>
            <option>Admin Workspace</option>
          </select>

          <div class="w-10 h-10 rounded-full bg-gray-300"></div>
        </div>
      </header>

      <!-- Content -->
      <div class="p-6 space-y-6">

        <!-- System Status -->
        <section class="bg-black text-white rounded-3xl p-5 shadow-sm">
          <div class="grid grid-cols-2 md:grid-cols-3 xl:grid-cols-6 gap-4 text-sm">
            <div>
              <div class="text-gray-400">Active Drivers</div>
              <div class="text-xl font-bold">42</div>
            </div>
            <div>
              <div class="text-gray-400">In Transit</div>
              <div class="text-xl font-bold">118</div>
            </div>
            <div>
              <div class="text-gray-400">SLA Risk</div>
              <div class="text-xl font-bold text-red-400">7</div>
            </div>
            <div>
              <div class="text-gray-400">Unassigned</div>
              <div class="text-xl font-bold text-yellow-300">14</div>
            </div>
            <div>
              <div class="text-gray-400">API Health</div>
              <div class="text-xl font-bold text-green-400">Online</div>
            </div>
            <div>
              <div class="text-gray-400">Last Sync</div>
              <div class="text-xl font-bold">2 min ago</div>
            </div>
          </div>
        </section>

        <!-- Quick Actions -->
        <section class="bg-white rounded-3xl shadow-sm border border-gray-200 p-6">
          <h2 class="text-xl font-semibold mb-5">Quick Actions</h2>

          <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-4">
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Export Active Orders</div>
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Open Kommo</div>
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Open Spoke</div>
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Generate Report</div>
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Upload XLS</div>
            <div class="border border-gray-300 bg-gray-50 rounded-2xl p-5 font-medium">Search Order</div>
          </div>
        </section>

        <!-- Filters -->
        <section class="bg-white rounded-3xl border border-gray-200 p-5 shadow-sm">
          <h2 class="text-lg font-semibold mb-4">Operational Filters</h2>

          <div class="grid grid-cols-2 md:grid-cols-3 xl:grid-cols-6 gap-4 text-sm">
            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Date Range</option>
              <option>Today</option>
              <option>This Week</option>
              <option>This Month</option>
            </select>

            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Region</option>
              <option>NY</option>
              <option>CA</option>
              <option>TX</option>
              <option>FL</option>
            </select>

            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Broker</option>
              <option>Broker A</option>
              <option>Broker B</option>
            </select>

            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Dispatcher</option>
              <option>Dispatcher A</option>
              <option>Dispatcher B</option>
            </select>

            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Source</option>
              <option>AptDeco</option>
              <option>UShip</option>
              <option>Manual</option>
            </select>

            <select class="border border-gray-300 rounded-xl px-4 py-3 bg-gray-50">
              <option>Status</option>
              <option>New</option>
              <option>Pickup</option>
              <option>In Transit</option>
              <option>Delivered</option>
            </select>
          </div>
        </section>

        <!-- KPI -->
        <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-6 gap-4">
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">Active Orders</div>
            <div class="text-3xl font-bold mt-3">245</div>
          </div>
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">Delivered Today</div>
            <div class="text-3xl font-bold mt-3 text-green-600">18</div>
          </div>
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">Revenue</div>
            <div class="text-3xl font-bold mt-3">$42k</div>
          </div>
          <div class="bg-white rounded-2xl border border-red-200 p-5 shadow-sm bg-red-50">
            <div class="text-sm text-red-500">Delayed Orders</div>
            <div class="text-3xl font-bold mt-3 text-red-600">7</div>
          </div>
          <div class="bg-white rounded-2xl border border-yellow-200 p-5 shadow-sm bg-yellow-50">
            <div class="text-sm text-yellow-700">Pending Tasks</div>
            <div class="text-3xl font-bold mt-3 text-yellow-700">31</div>
          </div>
          <div class="bg-white rounded-2xl border border-green-200 p-5 shadow-sm bg-green-50">
            <div class="text-sm text-green-700">Export Success</div>
            <div class="text-3xl font-bold mt-3 text-green-700">98%</div>
          </div>
        </section>

        <!-- SLA KPI -->
        <section class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-4 gap-4">
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">On-Time Delivery</div>
            <div class="text-3xl font-bold mt-3 text-green-600">94%</div>
          </div>
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">Avg Delivery Delay</div>
            <div class="text-3xl font-bold mt-3">2.1h</div>
          </div>
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">POD Completion</div>
            <div class="text-3xl font-bold mt-3 text-yellow-600">91%</div>
          </div>
          <div class="bg-white rounded-2xl border border-gray-200 p-5 shadow-sm">
            <div class="text-sm text-gray-500">No Export Errors</div>
            <div class="text-3xl font-bold mt-3 text-green-600">Clear</div>
          </div>
        </section>

        <!-- Charts -->
        <section class="grid grid-cols-1 xl:grid-cols-3 gap-6">

          <!-- Pie Chart -->
          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-lg font-semibold mb-5">Orders by Status</h2>

            <div class="h-64 border-2 border-dashed border-gray-300 rounded-2xl bg-gray-50 flex items-center justify-center">
              <svg width="230" height="230" viewBox="0 0 42 42">
                <circle cx="21" cy="21" r="15.915" fill="transparent" stroke="#e5e7eb" stroke-width="5"></circle>
                <circle cx="21" cy="21" r="15.915" fill="transparent" stroke="#10b981" stroke-width="5" stroke-dasharray="45 55" stroke-dashoffset="0"></circle>
                <circle cx="21" cy="21" r="15.915" fill="transparent" stroke="#3b82f6" stroke-width="5" stroke-dasharray="30 70" stroke-dashoffset="-45"></circle>
                <circle cx="21" cy="21" r="15.915" fill="transparent" stroke="#ef4444" stroke-width="5" stroke-dasharray="15 85" stroke-dashoffset="-75"></circle>
                <text x="21" y="21" text-anchor="middle" dy="1" font-size="3" fill="#111827" font-weight="bold">245</text>
                <text x="21" y="25" text-anchor="middle" font-size="2" fill="#6b7280">Orders</text>
              </svg>
            </div>
          </div>

          <!-- Line Chart -->
          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-lg font-semibold mb-5">Revenue Trend</h2>

            <div class="h-64 border-2 border-dashed border-gray-300 rounded-2xl bg-gray-50 p-4 flex items-center justify-center">
              <svg width="100%" height="100%" viewBox="0 0 500 220" preserveAspectRatio="xMidYMid meet">
                <line x1="40" y1="20" x2="40" y2="180" stroke="#d1d5db"></line>
                <line x1="40" y1="180" x2="470" y2="180" stroke="#d1d5db"></line>
                <line x1="40" y1="140" x2="470" y2="140" stroke="#e5e7eb"></line>
                <line x1="40" y1="100" x2="470" y2="100" stroke="#e5e7eb"></line>
                <line x1="40" y1="60" x2="470" y2="60" stroke="#e5e7eb"></line>
                <polyline fill="none" stroke="#3b82f6" stroke-width="4" points="40,150 100,130 160,135 220,90 280,110 340,70 400,85 460,40"></polyline>
                <circle cx="40" cy="150" r="5" fill="#3b82f6"></circle>
                <circle cx="100" cy="130" r="5" fill="#3b82f6"></circle>
                <circle cx="160" cy="135" r="5" fill="#3b82f6"></circle>
                <circle cx="220" cy="90" r="5" fill="#3b82f6"></circle>
                <circle cx="280" cy="110" r="5" fill="#3b82f6"></circle>
                <circle cx="340" cy="70" r="5" fill="#3b82f6"></circle>
                <circle cx="400" cy="85" r="5" fill="#3b82f6"></circle>
                <circle cx="460" cy="40" r="5" fill="#3b82f6"></circle>
                <text x="40" y="205" font-size="12" fill="#6b7280">Mon</text>
                <text x="100" y="205" font-size="12" fill="#6b7280">Tue</text>
                <text x="160" y="205" font-size="12" fill="#6b7280">Wed</text>
                <text x="220" y="205" font-size="12" fill="#6b7280">Thu</text>
                <text x="280" y="205" font-size="12" fill="#6b7280">Fri</text>
                <text x="340" y="205" font-size="12" fill="#6b7280">Sat</text>
                <text x="400" y="205" font-size="12" fill="#6b7280">Sun</text>
              </svg>
            </div>
          </div>

          <!-- Bar Chart -->
          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-lg font-semibold mb-5">Orders by Region</h2>

            <div class="h-64 border-2 border-dashed border-gray-300 rounded-2xl bg-gray-50 p-4 flex items-center justify-center">
              <svg width="100%" height="100%" viewBox="0 0 500 220" preserveAspectRatio="xMidYMid meet">
                <line x1="40" y1="20" x2="40" y2="180" stroke="#d1d5db"></line>
                <line x1="40" y1="180" x2="470" y2="180" stroke="#d1d5db"></line>
                <line x1="40" y1="140" x2="470" y2="140" stroke="#f3f4f6"></line>
                <line x1="40" y1="100" x2="470" y2="100" stroke="#f3f4f6"></line>
                <line x1="40" y1="60" x2="470" y2="60" stroke="#f3f4f6"></line>

                <rect x="70" y="90" width="50" height="90" fill="#3b82f6" rx="6"></rect>
                <rect x="150" y="50" width="50" height="130" fill="#10b981" rx="6"></rect>
                <rect x="230" y="110" width="50" height="70" fill="#f59e0b" rx="6"></rect>
                <rect x="310" y="70" width="50" height="110" fill="#ef4444" rx="6"></rect>
                <rect x="390" y="120" width="50" height="60" fill="#8b5cf6" rx="6"></rect>

                <text x="82" y="205" font-size="12" fill="#6b7280">NY</text>
                <text x="162" y="205" font-size="12" fill="#6b7280">CA</text>
                <text x="242" y="205" font-size="12" fill="#6b7280">TX</text>
                <text x="322" y="205" font-size="12" fill="#6b7280">FL</text>
                <text x="402" y="205" font-size="12" fill="#6b7280">IL</text>
              </svg>
            </div>
          </div>

        </section>

        <!-- Operational Widgets -->
        <section class="grid grid-cols-1 xl:grid-cols-3 gap-6">

          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Current Route Load</h2>

            <div class="space-y-4">
              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>NY → TX</span>
                  <span>78%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-blue-500 rounded-full w-[78%]"></div>
                </div>
              </div>

              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>CA → FL</span>
                  <span>54%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-green-500 rounded-full w-[54%]"></div>
                </div>
              </div>

              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>NY → CA</span>
                  <span>91%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-red-500 rounded-full w-[91%]"></div>
                </div>
              </div>
            </div>
          </div>

          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Warehouse Capacity</h2>

            <div class="space-y-4">
              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>NY Warehouse</span>
                  <span>81%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-yellow-500 rounded-full w-[81%]"></div>
                </div>
              </div>

              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>CA Warehouse</span>
                  <span>63%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-green-500 rounded-full w-[63%]"></div>
                </div>
              </div>

              <div>
                <div class="flex justify-between text-sm mb-2">
                  <span>Temporary Storage</span>
                  <span>44%</span>
                </div>
                <div class="h-3 bg-gray-100 rounded-full">
                  <div class="h-3 bg-blue-500 rounded-full w-[44%]"></div>
                </div>
              </div>
            </div>
          </div>

          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Interstate Trips</h2>

            <div class="grid grid-cols-2 gap-4">
              <div class="bg-gray-50 border rounded-2xl p-4">
                <div class="text-sm text-gray-500">Active Trips</div>
                <div class="text-3xl font-bold mt-2">2</div>
              </div>
              <div class="bg-gray-50 border rounded-2xl p-4">
                <div class="text-sm text-gray-500">Next Departure</div>
                <div class="text-xl font-bold mt-2">Fri</div>
              </div>
              <div class="bg-gray-50 border rounded-2xl p-4">
                <div class="text-sm text-gray-500">Avg Load</div>
                <div class="text-3xl font-bold mt-2">74%</div>
              </div>
              <div class="bg-gray-50 border rounded-2xl p-4">
                <div class="text-sm text-gray-500">SLA Risk</div>
                <div class="text-3xl font-bold mt-2 text-red-600">3</div>
              </div>
            </div>
          </div>

        </section>

        <!-- Map + Activity -->
        <section class="grid grid-cols-1 xl:grid-cols-3 gap-6">

          <div class="xl:col-span-2 bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Live Route Map</h2>

            <div class="h-80 bg-gray-50 border-2 border-dashed border-gray-300 rounded-2xl flex items-center justify-center">
              <svg width="90%" height="90%" viewBox="0 0 700 300" preserveAspectRatio="xMidYMid meet">
                <rect x="0" y="0" width="700" height="300" fill="#f9fafb"></rect>

                <path d="M90 130 C180 80, 260 90, 340 130 S520 190, 610 120" fill="none" stroke="#3b82f6" stroke-width="5" stroke-dasharray="10 8"></path>
                <path d="M110 190 C230 230, 330 210, 430 160 S560 110, 630 190" fill="none" stroke="#10b981" stroke-width="5" stroke-dasharray="10 8"></path>

                <circle cx="90" cy="130" r="10" fill="#111827"></circle>
                <text x="75" y="110" font-size="14" fill="#111827">NY</text>

                <circle cx="610" cy="120" r="10" fill="#111827"></circle>
                <text x="595" y="100" font-size="14" fill="#111827">CA</text>

                <circle cx="430" cy="160" r="10" fill="#ef4444"></circle>
                <text x="400" y="145" font-size="14" fill="#ef4444">SLA Risk</text>

                <circle cx="630" cy="190" r="10" fill="#111827"></circle>
                <text x="615" y="215" font-size="14" fill="#111827">FL</text>
              </svg>
            </div>
          </div>

          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Recent Activity</h2>

            <div class="space-y-3 text-sm">
              <div class="border border-gray-200 rounded-2xl p-4 bg-gray-50">Order #10425 exported</div>
              <div class="border border-gray-200 rounded-2xl p-4 bg-gray-50">POD uploaded for #10318</div>
              <div class="border border-gray-200 rounded-2xl p-4 bg-gray-50">Driver assigned to #10541</div>
              <div class="border border-gray-200 rounded-2xl p-4 bg-gray-50">Payment validated for #10287</div>
              <div class="border border-red-200 rounded-2xl p-4 bg-red-50 text-red-700">Delivery delay detected</div>
            </div>
          </div>

        </section>

        <!-- Orders + Alerts -->
        <section class="grid grid-cols-1 xl:grid-cols-3 gap-6">

          <div class="xl:col-span-2 bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <div class="flex items-center justify-between mb-5">
              <h2 class="text-xl font-semibold">Central Operational Table</h2>
              <button class="border border-gray-300 rounded-xl px-4 py-2 bg-gray-50 text-sm">Export</button>
            </div>

            <div class="overflow-hidden rounded-2xl border border-gray-200">
              <table class="w-full text-sm">
                <thead class="bg-gray-50">
                  <tr class="text-left">
                    <th class="p-4">Order ID</th>
                    <th class="p-4">Status</th>
                    <th class="p-4">Route</th>
                    <th class="p-4">SLA</th>
                    <th class="p-4">Source</th>
                    <th class="p-4">Owner</th>
                    <th class="p-4">Last Update</th>
                  </tr>
                </thead>
                <tbody>
                  <tr class="border-t border-gray-100">
                    <td class="p-4 font-medium">#10124</td>
                    <td class="p-4"><span class="bg-blue-50 text-blue-700 px-3 py-1 rounded-full">In Transit</span></td>
                    <td class="p-4">NY → TX</td>
                    <td class="p-4"><span class="bg-green-50 text-green-700 px-3 py-1 rounded-full">On Track</span></td>
                    <td class="p-4">AptDeco</td>
                    <td class="p-4">Dispatcher</td>
                    <td class="p-4">2 min ago</td>
                  </tr>

                  <tr class="border-t border-gray-100">
                    <td class="p-4 font-medium">#10224</td>
                    <td class="p-4"><span class="bg-yellow-50 text-yellow-700 px-3 py-1 rounded-full">Pickup</span></td>
                    <td class="p-4">CA → FL</td>
                    <td class="p-4"><span class="bg-yellow-50 text-yellow-700 px-3 py-1 rounded-full">Watch</span></td>
                    <td class="p-4">UShip</td>
                    <td class="p-4">Broker</td>
                    <td class="p-4">12 min ago</td>
                  </tr>

                  <tr class="border-t border-gray-100">
                    <td class="p-4 font-medium">#10324</td>
                    <td class="p-4"><span class="bg-red-50 text-red-700 px-3 py-1 rounded-full">Delayed</span></td>
                    <td class="p-4">NY → CA</td>
                    <td class="p-4"><span class="bg-red-50 text-red-700 px-3 py-1 rounded-full">Risk</span></td>
                    <td class="p-4">Manual</td>
                    <td class="p-4">Dispatcher</td>
                    <td class="p-4">31 min ago</td>
                  </tr>

                  <tr class="border-t border-gray-100">
                    <td class="p-4 font-medium">#10424</td>
                    <td class="p-4"><span class="bg-green-50 text-green-700 px-3 py-1 rounded-full">Delivered</span></td>
                    <td class="p-4">TX → FL</td>
                    <td class="p-4"><span class="bg-green-50 text-green-700 px-3 py-1 rounded-full">Done</span></td>
                    <td class="p-4">AptDeco</td>
                    <td class="p-4">Warehouse</td>
                    <td class="p-4">1h ago</td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>

          <div class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
            <h2 class="text-xl font-semibold mb-5">Alerts / Problems</h2>

            <div class="space-y-3">
              <div class="border border-red-200 bg-red-50 rounded-2xl p-4 text-sm">⚠ Orders without dispatcher</div>
              <div class="border border-red-200 bg-red-50 rounded-2xl p-4 text-sm">⚠ Delayed deliveries</div>
              <div class="border border-red-200 bg-red-50 rounded-2xl p-4 text-sm">⚠ Missing POD</div>
              <div class="border border-yellow-200 bg-yellow-50 rounded-2xl p-4 text-sm">⚠ Payment pending</div>
              <div class="border border-green-200 bg-green-50 rounded-2xl p-4 text-sm text-green-700">✓ No export errors</div>
            </div>
          </div>

        </section>

        <!-- Integrations -->
        <section class="bg-white rounded-3xl border border-gray-200 p-6 shadow-sm">
          <h2 class="text-xl font-semibold mb-5">Integrations Hub</h2>

          <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-4 gap-4">
            <div class="border border-gray-200 rounded-2xl p-5 bg-gray-50">
              <div class="font-semibold text-lg mb-2">Kommo CRM</div>
              <div class="text-sm text-green-600 mb-4">Status: Online</div>
              <button class="border border-gray-300 rounded-xl px-4 py-2 bg-white text-sm">Open Service</button>
            </div>

            <div class="border border-yellow-200 rounded-2xl p-5 bg-yellow-50">
              <div class="font-semibold text-lg mb-2">Spoke</div>
              <div class="text-sm text-yellow-700 mb-4">Status: Sync delayed</div>
              <button class="border border-gray-300 rounded-xl px-4 py-2 bg-white text-sm">Open Service</button>
            </div>

            <div class="border border-gray-200 rounded-2xl p-5 bg-gray-50">
              <div class="font-semibold text-lg mb-2">Google Drive</div>
              <div class="text-sm text-green-600 mb-4">Status: Online</div>
              <button class="border border-gray-300 rounded-xl px-4 py-2 bg-white text-sm">Open Service</button>
            </div>

            <div class="border border-gray-200 rounded-2xl p-5 bg-gray-50">
              <div class="font-semibold text-lg mb-2">BI Dashboard</div>
              <div class="text-sm text-green-600 mb-4">Status: Online</div>
              <button class="border border-gray-300 rounded-xl px-4 py-2 bg-white text-sm">Open Service</button>
            </div>
          </div>
        </section>

      </div>
    </main>
  </div>
</body>
</html>