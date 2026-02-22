 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 92c6f2f05998c13329dd41fe4f8894da2a86d211..19b22214b456ad6e440bd5d9e950b4ea15f1e1a1 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,17 @@
 # reserve-dashboard
-Time Dashboard for UP Reserve Deputies
+
+Live, professional dashboard for Union Parish Reserve Deputy hour tracking.
+
+## Data source
+This dashboard reads directly from Google Sheets using the gviz JSON endpoint:
+
+- Sheet ID: `1XKQne56PC_iC317LUWkEyq4xnQ4AineeUko5EGvqkEM`
+- GID: `787165735`
+
+## Local preview
+```bash
+python3 -m http.server 4173
+```
+Then open `http://localhost:4173`.
+
+> Important: The sheet must be shared as **Anyone with the link can view** for live data to load.
 
EOF
)
