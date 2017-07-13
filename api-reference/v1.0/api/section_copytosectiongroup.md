<span data-ttu-id="9d1ab-p105">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="9d1ab-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。

## <span data-ttu-id="9d1ab-138">示例</span><span class="sxs-lookup"><span data-stu-id="9d1ab-138">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="9d1ab-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9d1ab-139">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="9d1ab-140">请求</span><span class="sxs-lookup"><span data-stu-id="9d1ab-140">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="9d1ab-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d1ab-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="9d1ab-142">响应</span><span class="sxs-lookup"><span data-stu-id="9d1ab-142">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="9d1ab-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9d1ab-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->