# <a name="get-subscribedsku"></a><span data-ttu-id="e2934-101">获取 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e2934-101">Get subscribedSku</span></span>
<span data-ttu-id="e2934-102">检索组织已获取的特定商业订阅。</span><span class="sxs-lookup"><span data-stu-id="e2934-102">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2934-103">权限</span><span class="sxs-lookup"><span data-stu-id="e2934-103">Permissions</span></span>
<span data-ttu-id="e2934-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e2934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e2934-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2934-106">Permission type</span></span>      | <span data-ttu-id="e2934-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2934-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e2934-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2934-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e2934-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2934-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="e2934-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2934-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2934-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2934-111">Not supported.</span></span>    | 
|<span data-ttu-id="e2934-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2934-112">Application</span></span> | <span data-ttu-id="e2934-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2934-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2934-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2934-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2934-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2934-115">Optional query parameters</span></span>
<span data-ttu-id="e2934-116">此方法**不**支持使用 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="e2934-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2934-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2934-117">Request headers</span></span>
| <span data-ttu-id="e2934-118">名称</span><span class="sxs-lookup"><span data-stu-id="e2934-118">Name</span></span>       | <span data-ttu-id="e2934-119">类型</span><span class="sxs-lookup"><span data-stu-id="e2934-119">Type</span></span> | <span data-ttu-id="e2934-120">说明</span><span class="sxs-lookup"><span data-stu-id="e2934-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e2934-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2934-121">Authorization</span></span>  | <span data-ttu-id="e2934-122">string</span><span class="sxs-lookup"><span data-stu-id="e2934-122">string</span></span>  | <span data-ttu-id="e2934-p102">持有者&lt;令牌&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="e2934-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2934-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2934-125">Request body</span></span>
<span data-ttu-id="e2934-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2934-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2934-127">响应</span><span class="sxs-lookup"><span data-stu-id="e2934-127">Response</span></span>

<span data-ttu-id="e2934-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscribedSku](../resources/subscribedsku.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2934-128">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2934-129">示例</span><span class="sxs-lookup"><span data-stu-id="e2934-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2934-130">请求</span><span class="sxs-lookup"><span data-stu-id="e2934-130">Request</span></span>
<span data-ttu-id="e2934-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2934-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="e2934-132">响应</span><span class="sxs-lookup"><span data-stu-id="e2934-132">Response</span></span>
<span data-ttu-id="e2934-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2934-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscribedSkus/$entity",
    "capabilityStatus": "Enabled",
    "consumedUnits": 14,
    "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
    "prepaidUnits": {
        "enabled": 25,
        "suspended": 0,
        "warning": 0
    },
    "servicePlans": [
        {
            "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
            "servicePlanName": "ADALLOM_S_O365",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
