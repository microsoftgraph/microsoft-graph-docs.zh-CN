# <a name="list-licensedetails"></a><span data-ttu-id="bd113-101">列出 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="bd113-101">List licenseDetails</span></span>

<span data-ttu-id="bd113-102">检索 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="bd113-102">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd113-103">权限</span><span class="sxs-lookup"><span data-stu-id="bd113-103">Permissions</span></span>
<span data-ttu-id="bd113-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bd113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd113-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd113-106">Permission type</span></span>      | <span data-ttu-id="bd113-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd113-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd113-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd113-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bd113-109">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd113-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd113-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd113-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd113-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="bd113-111">User.Read</span></span>    |
|<span data-ttu-id="bd113-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd113-112">Application</span></span> | <span data-ttu-id="bd113-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd113-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd113-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd113-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd113-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd113-115">Optional query parameters</span></span>
<span data-ttu-id="bd113-116">该方法**不**支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="bd113-116">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd113-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd113-117">Request headers</span></span>
| <span data-ttu-id="bd113-118">名称</span><span class="sxs-lookup"><span data-stu-id="bd113-118">Name</span></span>      |<span data-ttu-id="bd113-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd113-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd113-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd113-120">Authorization</span></span>  | <span data-ttu-id="bd113-121">持有者&lt;代码&gt;</span><span class="sxs-lookup"><span data-stu-id="bd113-121">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd113-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd113-122">Request body</span></span>
<span data-ttu-id="bd113-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd113-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd113-124">响应</span><span class="sxs-lookup"><span data-stu-id="bd113-124">Response</span></span>

<span data-ttu-id="bd113-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd113-125">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd113-126">示例</span><span class="sxs-lookup"><span data-stu-id="bd113-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd113-127">请求</span><span class="sxs-lookup"><span data-stu-id="bd113-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="bd113-128">响应</span><span class="sxs-lookup"><span data-stu-id="bd113-128">Response</span></span>
<span data-ttu-id="bd113-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd113-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->