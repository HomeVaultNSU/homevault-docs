# WebDAV Protocol

## PROPFIND
The PROPFIND method in WebDAV is used to retrieve properties (like file metadata) of a resource or collection.

The `Depth` header in a `PROPFIND` request specifies how deep the server should return properties for:

- `Depth: 0` – Only the resource itself.
- `Depth: 1` – The resource and its immediate children.
- `Depth: infinity` – The resource and all descendants (recursive).

**Note:** Some servers may limit or disallow `Depth: infinity` due to performance concerns.
