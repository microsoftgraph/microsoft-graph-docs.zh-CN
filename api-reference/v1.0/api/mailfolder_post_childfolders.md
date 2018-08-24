# <a name="create-mailfolder"></a><span data-ttu-id="67c7d-101">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="67c7d-101">Create MailFolder</span></span>

<span data-ttu-id="67c7d-102">使用此 API 新建子 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="67c7d-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="67c7d-103">权限</span><span class="sxs-lookup"><span data-stu-id="67c7d-103">Permissions</span></span>

<span data-ttu-id="67c7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="67c7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="67c7d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="67c7d-106">Permission type</span></span> | <span data-ttu-id="67c7d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67c7d-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="67c7d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67c7d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="67c7d-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67c7d-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="67c7d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67c7d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67c7d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67c7d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="67c7d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="67c7d-112">Application</span></span> | <span data-ttu-id="67c7d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67c7d-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="67c7d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67c7d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="67c7d-115">将查询 URL 中的父文件夹指定为文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="67c7d-115">Specify the parent folder in the query URL as a folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="67c7d-116">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="67c7d-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="67c7d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="67c7d-117">Request headers</span></span>

| <span data-ttu-id="67c7d-118">标头</span><span class="sxs-lookup"><span data-stu-id="67c7d-118">Header</span></span> | <span data-ttu-id="67c7d-119">值</span><span class="sxs-lookup"><span data-stu-id="67c7d-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="67c7d-120">授权</span><span class="sxs-lookup"><span data-stu-id="67c7d-120">Authorization</span></span> | <span data-ttu-id="67c7d-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="67c7d-121"></span></span> <span data-ttu-id="67c7d-122">必需。</span><span class="sxs-lookup"><span data-stu-id="67c7d-122">Required.</span></span> |
| <span data-ttu-id="67c7d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67c7d-123">Content-Type</span></span> | <span data-ttu-id="67c7d-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="67c7d-124"></span></span> <span data-ttu-id="67c7d-125">必需。</span><span class="sxs-lookup"><span data-stu-id="67c7d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67c7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67c7d-126">Request body</span></span>

<span data-ttu-id="67c7d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="67c7d-127">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="67c7d-128">**displayName** 是 [mailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="67c7d-128">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="67c7d-129">参数</span><span class="sxs-lookup"><span data-stu-id="67c7d-129">Parameter</span></span> | <span data-ttu-id="67c7d-130">类型</span><span class="sxs-lookup"><span data-stu-id="67c7d-130">Type</span></span> | <span data-ttu-id="67c7d-131">说明</span><span class="sxs-lookup"><span data-stu-id="67c7d-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="67c7d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="67c7d-132">displayName</span></span>|<span data-ttu-id="67c7d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="67c7d-133">String</span></span>|<span data-ttu-id="67c7d-134">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="67c7d-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="67c7d-135">响应</span><span class="sxs-lookup"><span data-stu-id="67c7d-135">Response</span></span>

<span data-ttu-id="67c7d-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mailFolder](../resources/mailfolder.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="67c7d-136">If successful, this method returns a `201 Created` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c7d-137">示例</span><span class="sxs-lookup"><span data-stu-id="67c7d-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="67c7d-138">请求</span><span class="sxs-lookup"><span data-stu-id="67c7d-138">Request</span></span>

<span data-ttu-id="67c7d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67c7d-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="67c7d-140">响应</span><span class="sxs-lookup"><span data-stu-id="67c7d-140">Response</span></span>
<span data-ttu-id="67c7d-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="67c7d-141">Here is an example of the response.</span></span>

> <span data-ttu-id="67c7d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67c7d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
