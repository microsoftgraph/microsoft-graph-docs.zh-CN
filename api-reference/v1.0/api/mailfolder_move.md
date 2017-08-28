# <a name="mailfolder-move"></a><span data-ttu-id="ac870-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="ac870-101">mailFolder: move</span></span>

<span data-ttu-id="ac870-102">将 Mailfolder 及其内容移动到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="ac870-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac870-103">权限</span><span class="sxs-lookup"><span data-stu-id="ac870-103">Permissions</span></span>
<span data-ttu-id="ac870-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ac870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac870-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac870-106">Permission type</span></span>      | <span data-ttu-id="ac870-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac870-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac870-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac870-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac870-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac870-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ac870-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac870-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac870-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac870-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ac870-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac870-112">Application</span></span> | <span data-ttu-id="ac870-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac870-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac870-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac870-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="ac870-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac870-115">Request headers</span></span>
| <span data-ttu-id="ac870-116">标头</span><span class="sxs-lookup"><span data-stu-id="ac870-116">Header</span></span>       | <span data-ttu-id="ac870-117">值</span><span class="sxs-lookup"><span data-stu-id="ac870-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac870-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac870-118">Authorization</span></span>  | <span data-ttu-id="ac870-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac870-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac870-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac870-121">Content-Type</span></span>  | <span data-ttu-id="ac870-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ac870-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac870-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac870-124">Request body</span></span>
<span data-ttu-id="ac870-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ac870-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac870-126">参数</span><span class="sxs-lookup"><span data-stu-id="ac870-126">Parameter</span></span>    | <span data-ttu-id="ac870-127">类型</span><span class="sxs-lookup"><span data-stu-id="ac870-127">Type</span></span>   |<span data-ttu-id="ac870-128">说明</span><span class="sxs-lookup"><span data-stu-id="ac870-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac870-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="ac870-129">destinationId</span></span>|<span data-ttu-id="ac870-130">String</span><span class="sxs-lookup"><span data-stu-id="ac870-130">String</span></span>|<span data-ttu-id="ac870-131">文件夹 ID，或*收件箱*、*草稿箱*、*已发送邮件*或*已删除邮件*的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="ac870-131">The folder ID, or the *Inbox*, *Drafts*, *SentItems*, or *DeletedItems* well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="ac870-132">响应</span><span class="sxs-lookup"><span data-stu-id="ac870-132">Response</span></span>

<span data-ttu-id="ac870-133">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac870-133">If successful, this method returns `200, OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac870-134">示例</span><span class="sxs-lookup"><span data-stu-id="ac870-134">Example</span></span>
<span data-ttu-id="ac870-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ac870-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac870-136">请求</span><span class="sxs-lookup"><span data-stu-id="ac870-136">Request</span></span>
<span data-ttu-id="ac870-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac870-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="ac870-138">响应</span><span class="sxs-lookup"><span data-stu-id="ac870-138">Response</span></span>
<span data-ttu-id="ac870-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac870-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
