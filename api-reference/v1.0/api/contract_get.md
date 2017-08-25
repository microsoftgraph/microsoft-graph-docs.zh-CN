# <a name="get-contract"></a><span data-ttu-id="4c905-101">获取 Contract</span><span class="sxs-lookup"><span data-stu-id="4c905-101">Get Contract</span></span>

<span data-ttu-id="4c905-102">检索 [contract](../resources/contract.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c905-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c905-103">权限</span><span class="sxs-lookup"><span data-stu-id="4c905-103">Permissions</span></span>

<span data-ttu-id="4c905-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4c905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4c905-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c905-106">Permission type</span></span>      | <span data-ttu-id="4c905-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c905-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4c905-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c905-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4c905-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c905-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="4c905-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c905-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c905-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c905-111">Not supported.</span></span>    | 
|<span data-ttu-id="4c905-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c905-112">Application</span></span> | <span data-ttu-id="4c905-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c905-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c905-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c905-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c905-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4c905-115">Optional query parameters</span></span>

<span data-ttu-id="4c905-116">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4c905-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c905-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c905-117">Request headers</span></span>

| <span data-ttu-id="4c905-118">名称</span><span class="sxs-lookup"><span data-stu-id="4c905-118">Name</span></span>      |<span data-ttu-id="4c905-119">说明</span><span class="sxs-lookup"><span data-stu-id="4c905-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c905-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c905-120">Authorization</span></span>  | <span data-ttu-id="4c905-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c905-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c905-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c905-123">Request body</span></span>

<span data-ttu-id="4c905-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c905-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c905-125">响应</span><span class="sxs-lookup"><span data-stu-id="4c905-125">Response</span></span>

<span data-ttu-id="4c905-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contract](../resources/contract.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c905-126">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c905-127">示例</span><span class="sxs-lookup"><span data-stu-id="4c905-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c905-128">请求</span><span class="sxs-lookup"><span data-stu-id="4c905-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="4c905-129">响应</span><span class="sxs-lookup"><span data-stu-id="4c905-129">Response</span></span>
<span data-ttu-id="4c905-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c905-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->