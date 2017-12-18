# openerplib.js

A simple json-rpc 2.0 lib to access odoo services

## Open Connection

```javascript
var con = openerplib.get_connection("localhost", 8069, "odoo", "admin", "admin");
```

### Access Model

```javascript
var account_obj = con.get_model("account.invoice");
account_obj.exec("search_read",[[],["name"]], None, function(err, res) {
  // handle result
});
```
