# CTunnix Builder

Public multi-platform build and release automation for the private
`fireunix-app/shadow-ctunnix` repository.

CTunnix also consumes a manifest dependency from private
`fireunix-app/shadow-stunnix`; each repository has a separate read-only PAT.
Private source and project build output are excluded from repository content,
workflow artifacts, and caches. Release archives contain compiled binaries and
explicitly published runtime templates only.

GitHub Releases are written back to the private CTunnix repository through a
separate single-repository write token. This public repository never hosts
Releases; R2 receives only the reviewed binary archives and checksums.
