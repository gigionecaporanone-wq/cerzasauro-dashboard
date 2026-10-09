<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Keep Home, replies and the restaurant archive as separate TanStack leaf routes within the shared mobile shell, so each tab is directly linkable.
- Share external database reads and one realtime subscription in a root provider; paginate archive reads to avoid the API row cap and preserve state between tabs.
- Keep PWA support manifest-only unless offline use is requested; this prevents stale app-shell caches in previews.
