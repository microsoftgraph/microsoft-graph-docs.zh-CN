# <a name="mailfolder-copy"></a><span data-ttu-id="8d074-101">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="8d074-101">mailFolder: copy</span></span>

<span data-ttu-id="8d074-102">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="8d074-102">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d074-103">权限</span><span class="sxs-lookup"><span data-stu-id="8d074-103">Permissions</span></span>

<span data-ttu-id="8d074-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8d074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8d074-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d074-106">Permission type</span></span> | <span data-ttu-id="8d074-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d074-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="8d074-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d074-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8d074-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d074-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8d074-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d074-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d074-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d074-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8d074-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d074-112">Application</span></span> | <span data-ttu-id="8d074-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d074-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d074-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d074-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="8d074-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d074-115">Request headers</span></span>
| <span data-ttu-id="8d074-116">标头</span><span class="sxs-lookup"><span data-stu-id="8d074-116">Header</span></span> | <span data-ttu-id="8d074-117">值</span><span class="sxs-lookup"><span data-stu-id="8d074-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="8d074-118">授权</span><span class="sxs-lookup"><span data-stu-id="8d074-118">Authorization</span></span> | <span data-ttu-id="8d074-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="8d074-119"></span></span> <span data-ttu-id="8d074-120">必需。</span><span class="sxs-lookup"><span data-stu-id="8d074-120">Required.</span></span> |
| <span data-ttu-id="8d074-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d074-121">Content-Type</span></span> | <span data-ttu-id="8d074-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="8d074-122"></span></span> <span data-ttu-id="8d074-123">必需。</span><span class="sxs-lookup"><span data-stu-id="8d074-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d074-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d074-124">Request body</span></span>

<span data-ttu-id="8d074-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8d074-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d074-126">参数</span><span class="sxs-lookup"><span data-stu-id="8d074-126">Parameter</span></span> | <span data-ttu-id="8d074-127">类型</span><span class="sxs-lookup"><span data-stu-id="8d074-127">Type</span></span> | <span data-ttu-id="8d074-128">说明</span><span class="sxs-lookup"><span data-stu-id="8d074-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="8d074-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="8d074-129">destinationId</span></span>|<span data-ttu-id="8d074-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8d074-130">String</span></span>|<span data-ttu-id="8d074-131">文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="8d074-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="8d074-132">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8d074-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8d074-133">响应</span><span class="sxs-lookup"><span data-stu-id="8d074-133">Response</span></span>

<span data-ttu-id="8d074-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8d074-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d074-135">示例</span><span class="sxs-lookup"><span data-stu-id="8d074-135">Example</span></span>

<span data-ttu-id="8d074-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8d074-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8d074-137">请求</span><span class="sxs-lookup"><span data-stu-id="8d074-137">Request</span></span>
<span data-ttu-id="8d074-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d074-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="8d074-139">响应</span><span class="sxs-lookup"><span data-stu-id="8d074-139">Response</span></span>

<span data-ttu-id="8d074-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d074-140">Here is an example of the response.</span></span>

> <span data-ttu-id="8d074-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d074-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
