{
  "verdict": "fail",
  "framework_detected": "static-html",
  "total_files_scanned": 36,
  "issues": [
    {
      "severity": "critical",
      "category": "framework_violation",
      "file": "index.html",
      "line": null,
      "description": "index.html contains a <style> block with over 35,000 characters of inlined CSS",
      "suggestion": "Extract styles into an external CSS file and link via <link> to comply with static-html best practices and improve maintainability"
    },
    {
      "severity": "critical",
      "category": "framework_violation",
      "file": "index.html",
      "line": null,
      "description": "index.html uses inline <style> tags instead of linking an external stylesheet",
      "suggestion": "Move all CSS to styles.css and reference it with <link rel='stylesheet' href='/styles.css'>"
    },
    {
      "severity": "warning",
      "category": "missing_dep",
      "file": "package.json",
      "line": null,
      "description": "package.json is missing from the codebase",
      "suggestion": "Add package.json to define project metadata and dependencies, even for static sites"
    },
    {
      "severity": "warning",
      "category": "corrupted_pkg",
      "file": "package.json",
      "line": null,
      "description": "package.json is absent, implying missing or corrupted project configuration",
      "suggestion": "Generate a minimal package.json with name, version, and scripts for consistency"
    }
  ]
}