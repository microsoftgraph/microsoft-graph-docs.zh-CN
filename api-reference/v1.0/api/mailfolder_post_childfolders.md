# <a name="create-mailfolder"></a><span data-ttu-id="bf64f-101">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="bf64f-101">Create MailFolder</span></span>

<span data-ttu-id="bf64f-102">使用此 API 新建子 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="bf64f-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf64f-103">权限</span><span class="sxs-lookup"><span data-stu-id="bf64f-103">Permissions</span></span>
<span data-ttu-id="bf64f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bf64f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf64f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf64f-106">Permission type</span></span>      | <span data-ttu-id="bf64f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf64f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf64f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf64f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bf64f-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf64f-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bf64f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf64f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf64f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf64f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bf64f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf64f-112">Application</span></span> | <span data-ttu-id="bf64f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf64f-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf64f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf64f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="bf64f-115">将查询 URL 中的父文件夹指定为文件夹 ID，或*收件箱*、*草稿箱*、*已发送邮件*或*已删除邮件*等已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="bf64f-115">Specify the parent folder in the query URL as a folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="bf64f-116">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="bf64f-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf64f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf64f-117">Request headers</span></span>
| <span data-ttu-id="bf64f-118">标头</span><span class="sxs-lookup"><span data-stu-id="bf64f-118">Header</span></span>       | <span data-ttu-id="bf64f-119">值</span><span class="sxs-lookup"><span data-stu-id="bf64f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf64f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf64f-120">Authorization</span></span>  | <span data-ttu-id="bf64f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf64f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf64f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf64f-123">Content-Type</span></span>  | <span data-ttu-id="bf64f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf64f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf64f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf64f-126">Request body</span></span>
<span data-ttu-id="bf64f-p105">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="bf64f-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="bf64f-129">参数</span><span class="sxs-lookup"><span data-stu-id="bf64f-129">Parameter</span></span>    | <span data-ttu-id="bf64f-130">类型</span><span class="sxs-lookup"><span data-stu-id="bf64f-130">Type</span></span>   |<span data-ttu-id="bf64f-131">说明</span><span class="sxs-lookup"><span data-stu-id="bf64f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf64f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bf64f-132">displayName</span></span>|<span data-ttu-id="bf64f-133">String</span><span class="sxs-lookup"><span data-stu-id="bf64f-133">String</span></span>|<span data-ttu-id="bf64f-134">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bf64f-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="bf64f-135">响应</span><span class="sxs-lookup"><span data-stu-id="bf64f-135">Response</span></span>

<span data-ttu-id="bf64f-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf64f-136">If successful, this method returns `201 Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf64f-137">示例</span><span class="sxs-lookup"><span data-stu-id="bf64f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf64f-138">请求</span><span class="sxs-lookup"><span data-stu-id="bf64f-138">Request</span></span>
<span data-ttu-id="bf64f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf64f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="bf64f-140">响应</span><span class="sxs-lookup"><span data-stu-id="bf64f-140">Response</span></span>
<span data-ttu-id="bf64f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf64f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
