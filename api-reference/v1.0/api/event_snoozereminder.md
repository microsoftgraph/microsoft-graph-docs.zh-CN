<span data-ttu-id="34ac4-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="34ac4-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="34ac4-129">示例</span><span class="sxs-lookup"><span data-stu-id="34ac4-129">Example</span></span>
<span data-ttu-id="34ac4-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="34ac4-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34ac4-131">请求</span><span class="sxs-lookup"><span data-stu-id="34ac4-131">Request</span></span>
<span data-ttu-id="34ac4-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34ac4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="34ac4-133">响应</span><span class="sxs-lookup"><span data-stu-id="34ac4-133">Response</span></span>
<span data-ttu-id="34ac4-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="34ac4-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
