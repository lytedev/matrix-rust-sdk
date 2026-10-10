Add `Room::tags`, `Room::set_tag` and `Room::remove_tag`, which use raw tag
names so that tags outside of the `m.*` and `u.*` namespaces (such as Element
Web's `element.io.section.*` custom room list sections) can be read and
written; `Client::observe_room_tags` to follow tag changes of every room with a
single subscription; `Client::observe_raw_account_data` to follow global account
data types the SDK does not model; and the `NonIdentifiers` room list filter.
