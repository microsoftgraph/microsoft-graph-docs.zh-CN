# <a name="message-copy"></a><span data-ttu-id="4be17-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="4be17-101">message: copy</span></span>

<span data-ttu-id="4be17-102">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="4be17-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be17-103">权限</span><span class="sxs-lookup"><span data-stu-id="4be17-103">Permissions</span></span>

<span data-ttu-id="4be17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4be17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="4be17-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4be17-106">Permission type</span></span> | <span data-ttu-id="4be17-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4be17-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4be17-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4be17-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4be17-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be17-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4be17-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4be17-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be17-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be17-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4be17-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4be17-112">Application</span></span> | <span data-ttu-id="4be17-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be17-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be17-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4be17-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="4be17-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="4be17-115">Request headers</span></span>

| <span data-ttu-id="4be17-116">标头</span><span class="sxs-lookup"><span data-stu-id="4be17-116">Header</span></span> | <span data-ttu-id="4be17-117">值</span><span class="sxs-lookup"><span data-stu-id="4be17-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4be17-118">授权</span><span class="sxs-lookup"><span data-stu-id="4be17-118">Authorization</span></span> | <span data-ttu-id="4be17-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="4be17-119"></span></span> <span data-ttu-id="4be17-120">必需。</span><span class="sxs-lookup"><span data-stu-id="4be17-120">Required.</span></span> |
| <span data-ttu-id="4be17-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4be17-121">Content-Type</span></span> | <span data-ttu-id="4be17-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="4be17-122"></span></span> <span data-ttu-id="4be17-123">必需。</span><span class="sxs-lookup"><span data-stu-id="4be17-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be17-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4be17-124">Request body</span></span>

<span data-ttu-id="4be17-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4be17-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4be17-126">参数</span><span class="sxs-lookup"><span data-stu-id="4be17-126">Parameter</span></span> | <span data-ttu-id="4be17-127">类型</span><span class="sxs-lookup"><span data-stu-id="4be17-127">Type</span></span> | <span data-ttu-id="4be17-128">说明</span><span class="sxs-lookup"><span data-stu-id="4be17-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="4be17-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="4be17-129">destinationId</span></span>|<span data-ttu-id="4be17-130">字符串</span><span class="sxs-lookup"><span data-stu-id="4be17-130">String</span></span>|<span data-ttu-id="4be17-131">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="4be17-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="4be17-132">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="4be17-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4be17-133">响应</span><span class="sxs-lookup"><span data-stu-id="4be17-133">Response</span></span>

<span data-ttu-id="4be17-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [消息](../resources/message.md)资源。</span><span class="sxs-lookup"><span data-stu-id="4be17-134">If successful, this method returns a `201 Created` response code and a [sharedDriveItem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be17-135">示例</span><span class="sxs-lookup"><span data-stu-id="4be17-135">Example</span></span>

<span data-ttu-id="4be17-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4be17-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4be17-137">请求</span><span class="sxs-lookup"><span data-stu-id="4be17-137">Request</span></span>
<span data-ttu-id="4be17-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4be17-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="4be17-139">响应</span><span class="sxs-lookup"><span data-stu-id="4be17-139">Response</span></span>

<span data-ttu-id="4be17-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4be17-140">Here is an example of the response.</span></span>

> <span data-ttu-id="4be17-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4be17-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
