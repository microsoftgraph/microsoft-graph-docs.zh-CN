<span data-ttu-id="412b0-p120">返回错误，其中包括 HTTP 错误代码和错误对象。错误 `code` 和 `message` 解释了导致错误的原因。</span><span class="sxs-lookup"><span data-stu-id="412b0-p120">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span> 

返回错误，其中包括 HTTP 错误代码和错误对象。错误 `code` 和 `message` 解释了导致错误的原因。
 
<span data-ttu-id="412b0-277">以下是一个示例。</span><span class="sxs-lookup"><span data-stu-id="412b0-277">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

