<span data-ttu-id="74308-p123">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="74308-p123">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>|可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。          |

## <span data-ttu-id="74308-261">响应</span><span class="sxs-lookup"><span data-stu-id="74308-261">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="74308-262">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="74308-262">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="74308-263">示例</span><span class="sxs-lookup"><span data-stu-id="74308-263">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="74308-264">请求</span><span class="sxs-lookup"><span data-stu-id="74308-264">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="74308-265">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74308-265">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```
##### <span data-ttu-id="74308-266">响应</span><span class="sxs-lookup"><span data-stu-id="74308-266">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="74308-267">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74308-267">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
