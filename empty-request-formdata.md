# Problem

- HTTP RFC does not allow 'multipart/form-data' in PUT requests
- Laravel cannot parse FormData in PUT requests, so the request is empty

# Solutions

- Avoid formdata in put requests => use json
- Use POST request with "_method: PUT" for formData