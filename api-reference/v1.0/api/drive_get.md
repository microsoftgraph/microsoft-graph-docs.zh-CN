# <a name="get-drive"></a><span data-ttu-id="fd572-101">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="fd572-101">Get Drive</span></span>

<span data-ttu-id="fd572-p101">检索 [驱动器](../resources/drive.md) 资源的属性和关系。Drive 是文件系统的顶级容器。Graph API 允许访问用户 OneDrive/OneDrive for Business 或 SharePoint 文档库的 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="fd572-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd572-105">权限</span><span class="sxs-lookup"><span data-stu-id="fd572-105">Permissions</span></span>

<span data-ttu-id="fd572-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd572-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd572-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd572-108">Permission type</span></span>      | <span data-ttu-id="fd572-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd572-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd572-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd572-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd572-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd572-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd572-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd572-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd572-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd572-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd572-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd572-114">Application</span></span> | <span data-ttu-id="fd572-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd572-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-a-users-onedrive"></a><span data-ttu-id="fd572-116">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="fd572-116">Get a user's OneDrive</span></span>

<span data-ttu-id="fd572-117">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 [User](../resources/user.md) 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="fd572-117">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd572-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd572-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="fd572-119">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="fd572-119">Get the document library associated with a group</span></span>

<span data-ttu-id="fd572-120">若要访问[组](../resources/group.md)的默认文档库，你的应用程序应请求组中的**驱动器**关系。</span><span class="sxs-lookup"><span data-stu-id="fd572-120">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd572-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd572-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="fd572-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fd572-122">Optional query parameters</span></span>

<span data-ttu-id="fd572-123">此方法支持使用 `$expand` 和 `$select` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fd572-123">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="fd572-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd572-124">Request body</span></span>

<span data-ttu-id="fd572-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd572-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd572-126">响应</span><span class="sxs-lookup"><span data-stu-id="fd572-126">Response</span></span>

<span data-ttu-id="fd572-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [驱动器](../resources/drive.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="fd572-127">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd572-128">示例</span><span class="sxs-lookup"><span data-stu-id="fd572-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd572-129">请求</span><span class="sxs-lookup"><span data-stu-id="fd572-129">Request</span></span>

<span data-ttu-id="fd572-130">下面是一个请求获取已登录用户的 OneDrive 或 OneDrive for Business 的示例。</span><span class="sxs-lookup"><span data-stu-id="fd572-130">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="fd572-131">响应</span><span class="sxs-lookup"><span data-stu-id="fd572-131">Response</span></span>

<span data-ttu-id="fd572-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fd572-132">Here is an example of the response.</span></span>

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
