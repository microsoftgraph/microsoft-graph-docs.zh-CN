# <a name="create-mailfolder"></a><span data-ttu-id="e15d1-101">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="e15d1-101">Create MailFolder</span></span>

<span data-ttu-id="e15d1-102">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="e15d1-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e15d1-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="e15d1-103">Prerequisites</span></span>
<span data-ttu-id="e15d1-104">要执行此 API，需要以下**范围**之一：*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="e15d1-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="e15d1-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e15d1-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="e15d1-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="e15d1-106">Request headers</span></span>
| <span data-ttu-id="e15d1-107">标头</span><span class="sxs-lookup"><span data-stu-id="e15d1-107">Header</span></span>       | <span data-ttu-id="e15d1-108">值</span><span class="sxs-lookup"><span data-stu-id="e15d1-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e15d1-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="e15d1-109">Authorization</span></span>  | <span data-ttu-id="e15d1-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e15d1-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e15d1-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e15d1-112">Content-Type</span></span>  | <span data-ttu-id="e15d1-113">application/json</span><span class="sxs-lookup"><span data-stu-id="e15d1-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e15d1-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="e15d1-114">Request body</span></span>
<span data-ttu-id="e15d1-p102">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="e15d1-p102">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="e15d1-117">参数</span><span class="sxs-lookup"><span data-stu-id="e15d1-117">Parameter</span></span>    | <span data-ttu-id="e15d1-118">类型</span><span class="sxs-lookup"><span data-stu-id="e15d1-118">Type</span></span>   |<span data-ttu-id="e15d1-119">说明</span><span class="sxs-lookup"><span data-stu-id="e15d1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e15d1-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e15d1-120">displayName</span></span>|<span data-ttu-id="e15d1-121">String</span><span class="sxs-lookup"><span data-stu-id="e15d1-121">String</span></span>|<span data-ttu-id="e15d1-122">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e15d1-122">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e15d1-123">响应</span><span class="sxs-lookup"><span data-stu-id="e15d1-123">Response</span></span>

<span data-ttu-id="e15d1-124">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e15d1-124">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e15d1-125">示例</span><span class="sxs-lookup"><span data-stu-id="e15d1-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e15d1-126">请求</span><span class="sxs-lookup"><span data-stu-id="e15d1-126">Request</span></span>
<span data-ttu-id="e15d1-127">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e15d1-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="e15d1-128">响应</span><span class="sxs-lookup"><span data-stu-id="e15d1-128">Response</span></span>
<span data-ttu-id="e15d1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e15d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
