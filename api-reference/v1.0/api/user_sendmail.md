<span data-ttu-id="accb6-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="accb6-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="accb6-133">示例</span><span class="sxs-lookup"><span data-stu-id="accb6-133">Example</span></span>
<span data-ttu-id="accb6-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="accb6-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="accb6-135">请求</span><span class="sxs-lookup"><span data-stu-id="accb6-135">Request</span></span>
<span data-ttu-id="accb6-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="accb6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response"></a><span data-ttu-id="accb6-137">响应</span><span class="sxs-lookup"><span data-stu-id="accb6-137">Response</span></span>
<span data-ttu-id="accb6-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="accb6-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
