# <a name="get-mailfolder"></a><span data-ttu-id="6a2db-101">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="6a2db-101">Get mailFolder</span></span>

<span data-ttu-id="6a2db-102">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a2db-102">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="6a2db-103">有两种方案相关应用程序可以在哪里找到另一个用户的邮件文件夹：</span><span class="sxs-lookup"><span data-stu-id="6a2db-103">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="6a2db-104">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="6a2db-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6a2db-105">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="6a2db-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6a2db-106">请参阅[详细信息和示例](../../../concepts/outlook-share-messages-folders.md)。</span><span class="sxs-lookup"><span data-stu-id="6a2db-106">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="6a2db-107">权限</span><span class="sxs-lookup"><span data-stu-id="6a2db-107">Permissions</span></span>
<span data-ttu-id="6a2db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6a2db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a2db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a2db-110">Permission type</span></span>      | <span data-ttu-id="6a2db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a2db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a2db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a2db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a2db-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a2db-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6a2db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a2db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a2db-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a2db-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6a2db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a2db-116">Application</span></span> | <span data-ttu-id="6a2db-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a2db-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a2db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a2db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a2db-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6a2db-119">Optional query parameters</span></span>
<span data-ttu-id="6a2db-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6a2db-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a2db-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a2db-121">Request headers</span></span>
| <span data-ttu-id="6a2db-122">名称</span><span class="sxs-lookup"><span data-stu-id="6a2db-122">Name</span></span>       | <span data-ttu-id="6a2db-123">类型</span><span class="sxs-lookup"><span data-stu-id="6a2db-123">Type</span></span> | <span data-ttu-id="6a2db-124">说明</span><span class="sxs-lookup"><span data-stu-id="6a2db-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a2db-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a2db-125">Authorization</span></span>  | <span data-ttu-id="6a2db-126">string</span><span class="sxs-lookup"><span data-stu-id="6a2db-126">string</span></span>  | <span data-ttu-id="6a2db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a2db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a2db-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a2db-129">Request body</span></span>
<span data-ttu-id="6a2db-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a2db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a2db-131">响应</span><span class="sxs-lookup"><span data-stu-id="6a2db-131">Response</span></span>

<span data-ttu-id="6a2db-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a2db-132">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a2db-133">示例</span><span class="sxs-lookup"><span data-stu-id="6a2db-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a2db-134">请求</span><span class="sxs-lookup"><span data-stu-id="6a2db-134">Request</span></span>
<span data-ttu-id="6a2db-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a2db-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="6a2db-136">响应</span><span class="sxs-lookup"><span data-stu-id="6a2db-136">Response</span></span>
<span data-ttu-id="6a2db-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a2db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
