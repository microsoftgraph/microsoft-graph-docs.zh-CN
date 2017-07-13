<span data-ttu-id="0cf74-p102">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="0cf74-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>                                          | 共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。 |
| <span data-ttu-id="0cf74-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="0cf74-122">requireSignIn</span></span>    | <span data-ttu-id="0cf74-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cf74-123">Boolean</span></span>                                         | <span data-ttu-id="0cf74-124">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="0cf74-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="0cf74-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="0cf74-125">sendInvitation</span></span>   | <span data-ttu-id="0cf74-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cf74-126">Boolean</span></span>                                         | <span data-ttu-id="0cf74-127">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="0cf74-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="0cf74-128">roles</span><span class="sxs-lookup"><span data-stu-id="0cf74-128">roles</span></span>            | <span data-ttu-id="0cf74-129">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="0cf74-129">Collection(String)</span></span>                              | <span data-ttu-id="0cf74-130">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="0cf74-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <span data-ttu-id="0cf74-131">响应</span><span class="sxs-lookup"><span data-stu-id="0cf74-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0cf74-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="0cf74-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <span data-ttu-id="0cf74-133">示例</span><span class="sxs-lookup"><span data-stu-id="0cf74-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="0cf74-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0cf74-134">Here is an example of how to call this API.</span></span>

##### <span data-ttu-id="0cf74-135">请求</span><span class="sxs-lookup"><span data-stu-id="0cf74-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="0cf74-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cf74-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <span data-ttu-id="0cf74-137">响应</span><span class="sxs-lookup"><span data-stu-id="0cf74-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0cf74-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0cf74-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <span data-ttu-id="0cf74-139">注解</span><span class="sxs-lookup"><span data-stu-id="0cf74-139">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="0cf74-140">具有 `personal` **driveType**（OneDrive 个人版）的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="0cf74-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="0cf74-141">如需可用角色的列表，请参阅 [角色枚举](../resources/permission.md#roles-enumeration)。</span><span class="sxs-lookup"><span data-stu-id="0cf74-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
