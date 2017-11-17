# <a name="list-childfolders"></a><span data-ttu-id="356bb-101">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="356bb-101">List childFolders</span></span>

<span data-ttu-id="356bb-p101">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="356bb-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="356bb-104">权限</span><span class="sxs-lookup"><span data-stu-id="356bb-104">Permissions</span></span>
<span data-ttu-id="356bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="356bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="356bb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="356bb-107">Permission type</span></span>      | <span data-ttu-id="356bb-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="356bb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356bb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="356bb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="356bb-110">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="356bb-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="356bb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="356bb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356bb-112">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="356bb-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="356bb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="356bb-113">Application</span></span> | <span data-ttu-id="356bb-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="356bb-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="356bb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="356bb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="356bb-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="356bb-116">Optional query parameters</span></span>
<span data-ttu-id="356bb-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="356bb-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="356bb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="356bb-118">Request headers</span></span>
| <span data-ttu-id="356bb-119">名称</span><span class="sxs-lookup"><span data-stu-id="356bb-119">Name</span></span>       | <span data-ttu-id="356bb-120">类型</span><span class="sxs-lookup"><span data-stu-id="356bb-120">Type</span></span> | <span data-ttu-id="356bb-121">说明</span><span class="sxs-lookup"><span data-stu-id="356bb-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="356bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="356bb-122">Authorization</span></span>  | <span data-ttu-id="356bb-123">string</span><span class="sxs-lookup"><span data-stu-id="356bb-123">string</span></span>  | <span data-ttu-id="356bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="356bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="356bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="356bb-126">Request body</span></span>
<span data-ttu-id="356bb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="356bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="356bb-128">响应</span><span class="sxs-lookup"><span data-stu-id="356bb-128">Response</span></span>

<span data-ttu-id="356bb-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="356bb-129">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="356bb-130">示例</span><span class="sxs-lookup"><span data-stu-id="356bb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="356bb-131">请求</span><span class="sxs-lookup"><span data-stu-id="356bb-131">Request</span></span>
<span data-ttu-id="356bb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="356bb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="356bb-133">响应</span><span class="sxs-lookup"><span data-stu-id="356bb-133">Response</span></span>
<span data-ttu-id="356bb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="356bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
