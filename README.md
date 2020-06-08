# Repo for reproducing a Cursive deps.edn issue

## Repro steps

1. Clone the project
2. Open as Project selecting `deps.edn`
3. Observe deps working normally
4. Open `deps.edn` and Setup SDK (any JDK)
5. Uncomment a duplicate key :prod in `deps.edn`
6. Confirm "Import changes" in the popup dialog
7. Restart IDEA using `File/Invalidate Caches / Restart / Just Restart`
8. The Clojure Deps tab is gone and it won't come back even if you fix your `deps.edn`

Note: in this case it is still possible to manually add "+ Add as Clojure Deps project" but depending on the project stat it might not be.
