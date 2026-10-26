# Graph Report - robloxstud  (2026-10-26)

## Corpus Check
- 24 files · ~113,547 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 7 file(s) not represented in the graph (top: (none) 4, .command 1, .bat 1)

## Summary
- 369 nodes · 642 edges · 29 communities (17 shown, 12 thin omitted)
- Extraction: 93% EXTRACTED · 7% INFERRED · 0% AMBIGUOUS · INFERRED: 46 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `8064f29f`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- bridge.py
- test-parser.js
- ZeroScript - Free AI Agent for Roblox Studio
- main.js
- manifest.json
- MCPManager
- background.js
- launch_studio_mcp.py
- agentLoop
- MCPClient
- build
- diag
- buildMenu
- withSysResend
- chatgpt-cm.js
- ZeroScript Free - AI Roblox Studio Agent (ChatGPT, DeepSeek, Gemini, Kimi, GLM, Qwen, Arena, Meta AI)
- syncSessionState
- popup.js
- gemini.js
- kimi.js
- qwen.js
- qwen-net.js
- config.js
- parser.js
- arena.js
- chatgpt.js
- deepseek.js
- glm.js
- meta.js

## God Nodes (most connected - your core abstractions)
1. `log()` - 27 edges
2. `diag()` - 18 edges
3. `MCPClient` - 15 edges
4. `agentLoop()` - 15 edges
5. `studio_watch()` - 14 edges
6. `main()` - 14 edges
7. `_boot_and_diagnose()` - 12 edges
8. `handler()` - 11 edges
9. `classify()` - 11 edges
10. `buildMenu()` - 11 edges

## Surprising Connections (you probably didn't know these)
- `_current_studio_exe()` --calls--> `find_studio_mcp()`  [EXTRACTED]
  bridge.py → launch_studio_mcp.py

## Import Cycles
- None detected.

## Communities (29 total, 12 thin omitted)

### Community 0 - "bridge.py"
Cohesion: 0.07
Nodes (35): action_banner(), broadcast_status(), check_studio_port(), _clear_spinner_line(), config_add_server(), config_remove_server(), _current_studio_exe(), _descendant_pids() (+27 more)

### Community 1 - "test-parser.js"
Cohesion: 0.06
Nodes (28): blanks, cmBlock(), collapsed, el(), node, emptyTap, fs, P (+20 more)

### Community 2 - "ZeroScript - Free AI Agent for Roblox Studio"
Cohesion: 0.06
Nodes (31): [1.5.1] - 2026-08-13, [1.5.2] - 2026-08-14, [1.5.3] - 2026-08-22, [1.5.4] - 2026-09-06, [1.5.5] - 2026-09-10, Added, Added, Changed (+23 more)

### Community 3 - "main.js"
Cohesion: 0.10
Nodes (18): blendOver(), bridgeAlert(), buildSetup(), hideSetup(), inputCover(), markStopping(), opaqueBg(), parseColor() (+10 more)

### Community 4 - "manifest.json"
Cohesion: 0.10
Nodes (20): action, default_icon, default_popup, default_title, background, service_worker, content_scripts, 128 (+12 more)

### Community 5 - "MCPManager"
Cohesion: 0.14
Nodes (3): MCPManager, _run(), _Spinner

### Community 6 - "background.js"
Cohesion: 0.23
Nodes (17): broadcastStatus(), connect(), failAllPending(), handleBridgeMessage(), log(), pending, PROVIDER_URLS, refreshStudioStatus() (+9 more)

### Community 7 - "launch_studio_mcp.py"
Cohesion: 0.21
Nodes (8): _candidate_roots(), find_studio_mcp(), _find_studio_mcp_mac(), _find_studio_mcp_windows(), _mac_app_candidates(), main(), _newest_path(), _resolve_override_path()

### Community 8 - "agentLoop"
Cohesion: 0.17
Nodes (17): agentLoop(), argSummary(), callBody(), captureSendToken(), ensureTools(), jitterBeforeSend(), jsonSummary(), knownTool() (+9 more)

### Community 10 - "build"
Cohesion: 0.14
Nodes (15): applyTheme(), build(), clearAnchorPad(), computeBarMount(), effectiveBg(), markStoppedTurn(), nudgeStart(), onActionClick() (+7 more)

### Community 11 - "diag"
Cohesion: 0.21
Nodes (14): chip(), classify(), diag(), ensureOwnedChip(), forgetHalted(), iconFor(), isRememberedExecuted(), isRememberedHalted() (+6 more)

### Community 12 - "buildMenu"
Cohesion: 0.32
Nodes (7): bg(), buildMenu(), mcpSlug(), mergedMcpServers(), saveCustomMcpServers(), splitCommand(), waitForBridgeBack()

### Community 13 - "withSysResend"
Cohesion: 0.29
Nodes (8): bumpSys(), resetSysCount(), saveSysCount(), sinceLastSys(), sinceLastSysInDom(), sysResendDue(), systemPrompt(), withSysResend()

### Community 14 - "chatgpt-cm.js"
Cohesion: 0.70
Nodes (4): docOf(), syncAll(), syncOne(), viewOf()

### Community 15 - "ZeroScript Free - AI Roblox Studio Agent (ChatGPT, DeepSeek, Gemini, Kimi, GLM, Qwen, Arena, Meta AI)"
Cohesion: 0.40
Nodes (4): Architecture (for contributors), Setup, Support, ZeroScript Free - AI Roblox Studio Agent (ChatGPT, DeepSeek, Gemini, Kimi, GLM, Qwen, Arena, Meta AI)

### Community 16 - "syncSessionState"
Cohesion: 0.50
Nodes (4): domHasZsSignal(), rememberSession(), scheduleSweep(), syncSessionState()

### Community 17 - "popup.js"
Cohesion: 0.67
Nodes (3): refresh(), render(), SUPPORTED_HOSTS

## Knowledge Gaps
- **12 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `log()` connect `bridge.py` to `MCPClient`, `MCPManager`?**
  _High betweenness centrality (0.017) - this node is a cross-community bridge._
- **Are the 5 inferred relationships involving `studio_watch()` (e.g. with `_current_studio_exe()` and `_kill_port_squatter()`) actually correct?**
  _`studio_watch()` has 5 INFERRED edges - model-reasoned connections that need verification._
- **Should `bridge.py` be split into smaller, more focused modules?**
  _Cohesion score 0.06729264475743349 - nodes in this community are weakly interconnected._
- **Why does `MCPClient` connect `MCPClient` to `bridge.py`, `MCPManager`?**
  _High betweenness centrality (0.013) - this node is a cross-community bridge._
- **Should `test-parser.js` be split into smaller, more focused modules?**
  _Cohesion score 0.057057057057057055 - nodes in this community are weakly interconnected._
- **Why does `MCPManager` connect `MCPManager` to `bridge.py`?**
  _High betweenness centrality (0.011) - this node is a cross-community bridge._
- **Should `ZeroScript - Free AI Agent for Roblox Studio` be split into smaller, more focused modules?**
  _Cohesion score 0.06060606060606061 - nodes in this community are weakly interconnected._