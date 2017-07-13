<span data-ttu-id="d958a-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d958a-p105">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="d958a-156">示例</span><span class="sxs-lookup"><span data-stu-id="d958a-156">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="d958a-157">请求</span><span class="sxs-lookup"><span data-stu-id="d958a-157">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="d958a-158">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="d958a-158">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="d958a-159">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="d958a-159">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <span data-ttu-id="d958a-160">响应</span><span class="sxs-lookup"><span data-stu-id="d958a-160">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="d958a-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d958a-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->