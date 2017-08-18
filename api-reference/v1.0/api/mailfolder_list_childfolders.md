# <a name="list-childfolders"></a><span data-ttu-id="3c403-101">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="3c403-101">List childFolders</span></span>

<span data-ttu-id="3c403-p101">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="3c403-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c403-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c403-104">Prerequisites</span></span>
<span data-ttu-id="3c403-105">要执行此 API，需要以下**范围**之一：*Mail.Read；Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="3c403-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="3c403-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c403-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c403-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c403-107">Optional query parameters</span></span>
<span data-ttu-id="3c403-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c403-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c403-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c403-109">Request headers</span></span>
| <span data-ttu-id="3c403-110">名称</span><span class="sxs-lookup"><span data-stu-id="3c403-110">Name</span></span>       | <span data-ttu-id="3c403-111">类型</span><span class="sxs-lookup"><span data-stu-id="3c403-111">Type</span></span> | <span data-ttu-id="3c403-112">说明</span><span class="sxs-lookup"><span data-stu-id="3c403-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c403-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c403-113">Authorization</span></span>  | <span data-ttu-id="3c403-114">string</span><span class="sxs-lookup"><span data-stu-id="3c403-114">string</span></span>  | <span data-ttu-id="3c403-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c403-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c403-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c403-117">Request body</span></span>
<span data-ttu-id="3c403-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c403-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c403-119">响应</span><span class="sxs-lookup"><span data-stu-id="3c403-119">Response</span></span>

<span data-ttu-id="3c403-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c403-120">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c403-121">示例</span><span class="sxs-lookup"><span data-stu-id="3c403-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c403-122">请求</span><span class="sxs-lookup"><span data-stu-id="3c403-122">Request</span></span>
<span data-ttu-id="3c403-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c403-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="3c403-124">响应</span><span class="sxs-lookup"><span data-stu-id="3c403-124">Response</span></span>
<span data-ttu-id="3c403-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c403-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
