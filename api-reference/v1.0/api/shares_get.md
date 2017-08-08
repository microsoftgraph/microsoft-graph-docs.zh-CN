<span data-ttu-id="70e58-p101">虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。</span><span class="sxs-lookup"><span data-stu-id="70e58-p101">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。

## <a name="example-single-file"></a><span data-ttu-id="70e58-122">示例（单个文件）</span><span class="sxs-lookup"><span data-stu-id="70e58-122">Example (single file)</span></span>

##### <a name="request"></a><span data-ttu-id="70e58-123">请求</span><span class="sxs-lookup"><span data-stu-id="70e58-123">Request</span></span>

<span data-ttu-id="70e58-124">通过请求**根**关系，将返回共享的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="70e58-124">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a><span data-ttu-id="70e58-125">响应</span><span class="sxs-lookup"><span data-stu-id="70e58-125">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="70e58-126">示例（共享文件夹）</span><span class="sxs-lookup"><span data-stu-id="70e58-126">Example (shared folder)</span></span>

##### <a name="request"></a><span data-ttu-id="70e58-127">请求</span><span class="sxs-lookup"><span data-stu-id="70e58-127">Request</span></span>

<span data-ttu-id="70e58-128">通过请求**根**关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。</span><span class="sxs-lookup"><span data-stu-id="70e58-128">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a><span data-ttu-id="70e58-129">响应</span><span class="sxs-lookup"><span data-stu-id="70e58-129">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a><span data-ttu-id="70e58-130">转换共享 URL</span><span class="sxs-lookup"><span data-stu-id="70e58-130">Transform a sharing URL</span></span>

<span data-ttu-id="70e58-131">若要使用**共享** API 访问共享 URL，需要将 URL 转换为共享令牌。</span><span class="sxs-lookup"><span data-stu-id="70e58-131">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="70e58-132">要将 URL 转换为共享令牌：</span><span class="sxs-lookup"><span data-stu-id="70e58-132">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="70e58-133">Base64 编码共享 URL。</span><span class="sxs-lookup"><span data-stu-id="70e58-133">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="70e58-134">通过以下方法，将 base64 编码数据转换成[未填充的 base64url 格式](https://en.wikipedia.org/wiki/Base64)：</span><span class="sxs-lookup"><span data-stu-id="70e58-134">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="70e58-135">剪裁掉字符串最后的 `=` 字符</span><span class="sxs-lookup"><span data-stu-id="70e58-135">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="70e58-136">将不安全的 URL 字符替换成等效字符；将 `/` 替换成 `_`，将 `+` 替换成 `-`。</span><span class="sxs-lookup"><span data-stu-id="70e58-136">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="70e58-137">将 `u!` 追加到字符串的开头。</span><span class="sxs-lookup"><span data-stu-id="70e58-137">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="70e58-138">例如，以下 C# 方法将输入字符串转换为共享令牌：</span><span class="sxs-lookup"><span data-stu-id="70e58-138">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
