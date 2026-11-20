# pairtime-witness

Once a day, pairtime's server ([pairtimed](https://github.com/some-du6e/pairtime)) commits a signed root of every device's ledger batches here. Each commit is a public, timestamped promise of what the server held that day. Anyone can check that it never re-dated or rewrote a batch afterwards: compare a batch a device revealed with the root committed on its day ([DESIGN 7.4](https://github.com/some-du6e/pairtime/blob/main/docs/DESIGN.md)).

Only the server writes here, through a deploy key. Nothing in this repo identifies a person: the roots are hashes.
