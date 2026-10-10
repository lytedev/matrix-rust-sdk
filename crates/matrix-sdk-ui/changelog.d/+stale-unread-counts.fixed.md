`Timeline::mark_as_read` now clears the client-side unread counts when the
user's receipt already covers the latest event, instead of leaving stale counts
that nothing else would recompute.
