# <a name="list-available-drives"></a><span data-ttu-id="f4d8c-101">列出可用的驱动器</span><span class="sxs-lookup"><span data-stu-id="f4d8c-101">List available drives</span></span>

<span data-ttu-id="f4d8c-p101">检索可用于目标 [用户](../resources/user.md) 或 [组](../resources/group.md) 的 [驱动器](../resources/drive.md) 资源的列表。你的应用程序也可以请求 SharePoint 根网站上的文档库集。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-p101">Retrieve the list of [Drive](../resources/drive.md) resources available for a target [User](../resources/user.md) or [Group](../resources/group.md). Your app can also request the set of document libraries on the SharePoint root site.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4d8c-104">权限</span><span class="sxs-lookup"><span data-stu-id="f4d8c-104">Permissions</span></span>

<span data-ttu-id="f4d8c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4d8c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4d8c-107">Permission type</span></span>      | <span data-ttu-id="f4d8c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4d8c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4d8c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d8c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f4d8c-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d8c-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4d8c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d8c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4d8c-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d8c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4d8c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4d8c-113">Application</span></span> | <span data-ttu-id="f4d8c-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d8c-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4d8c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4d8c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives
GET /me/drives
GET /sites/{site-id}/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4d8c-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4d8c-116">Optional query parameters</span></span>
<span data-ttu-id="f4d8c-117">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-117">This method supports the `$expand` and `$orderby` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="f4d8c-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4d8c-118">Request body</span></span>

<span data-ttu-id="f4d8c-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4d8c-120">响应</span><span class="sxs-lookup"><span data-stu-id="f4d8c-120">Response</span></span>

<span data-ttu-id="f4d8c-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Drive](../resources/drive.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-121">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4d8c-122">示例</span><span class="sxs-lookup"><span data-stu-id="f4d8c-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4d8c-123">请求</span><span class="sxs-lookup"><span data-stu-id="f4d8c-123">Request</span></span>

<span data-ttu-id="f4d8c-124">下面是一个请求用户驱动器的示例。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-124">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a><span data-ttu-id="f4d8c-125">响应</span><span class="sxs-lookup"><span data-stu-id="f4d8c-125">Response</span></span>

<span data-ttu-id="f4d8c-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
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
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="f4d8c-127">注解</span><span class="sxs-lookup"><span data-stu-id="f4d8c-127">Remarks</span></span>

<span data-ttu-id="f4d8c-p103">大多数用户将只有一个驱动器资源。组和部分用户可能有多个驱动器可用。</span><span class="sxs-lookup"><span data-stu-id="f4d8c-p103">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
