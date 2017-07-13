<span data-ttu-id="3eff3-p101">检索 [驱动器](../resources/drive.md) 资源的属性和关系。Drive 是文件系统的顶级容器。Graph API 允许访问用户 OneDrive/OneDrive for Business 或 SharePoint 文档库的 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="3eff3-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

检索 [驱动器](../resources/drive.md) 资源的属性和关系。Drive 是文件系统的顶级容器。Graph API 允许访问用户 OneDrive/OneDrive for Business 或 SharePoint 文档库的 Drive 资源。

## <span data-ttu-id="3eff3-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="3eff3-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>

<span data-ttu-id="3eff3-106">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="3eff3-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="3eff3-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="3eff3-107">Files.Read</span></span>
* <span data-ttu-id="3eff3-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eff3-108">Files.ReadWrite</span></span>
* <span data-ttu-id="3eff3-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eff3-109">Files.Read.All</span></span>
* <span data-ttu-id="3eff3-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eff3-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="3eff3-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eff3-111">Sites.Read.All</span></span>
* <span data-ttu-id="3eff3-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eff3-112">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="3eff3-113">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="3eff3-113">Get a user's OneDrive</span></span>
<a id="get-a-users-onedrive" class="xliff"></a>

<span data-ttu-id="3eff3-114">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 [User](../resources/user.md) 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="3eff3-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

### <span data-ttu-id="3eff3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3eff3-115">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <span data-ttu-id="3eff3-116">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="3eff3-116">Get the document library associated with a group</span></span>
<a id="get-the-document-library-associated-with-a-group" class="xliff"></a>

<span data-ttu-id="3eff3-117">若要访问[组](../resources/group.md)的默认文档库，你的应用程序应请求组中的**驱动器**关系。</span><span class="sxs-lookup"><span data-stu-id="3eff3-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <span data-ttu-id="3eff3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3eff3-118">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <span data-ttu-id="3eff3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3eff3-119">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>

<span data-ttu-id="3eff3-120">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3eff3-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="3eff3-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="3eff3-121">Request body</span></span>
<a id="request-body" class="xliff"></a>

<span data-ttu-id="3eff3-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3eff3-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="3eff3-123">响应</span><span class="sxs-lookup"><span data-stu-id="3eff3-123">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="3eff3-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [驱动器](../resources/drive.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="3eff3-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <span data-ttu-id="3eff3-125">示例</span><span class="sxs-lookup"><span data-stu-id="3eff3-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="3eff3-126">请求</span><span class="sxs-lookup"><span data-stu-id="3eff3-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="3eff3-127">下面是一个请求获取已登录用户的 OneDrive 或 OneDrive for Business 的示例。</span><span class="sxs-lookup"><span data-stu-id="3eff3-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <span data-ttu-id="3eff3-128">响应</span><span class="sxs-lookup"><span data-stu-id="3eff3-128">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="3eff3-129">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3eff3-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
