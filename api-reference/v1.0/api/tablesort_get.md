# <a name="get-tablesort"></a><span data-ttu-id="cefbb-101">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="cefbb-101">Get TableSort</span></span>

<span data-ttu-id="cefbb-102">检索 tablesort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cefbb-102">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cefbb-103">权限</span><span class="sxs-lookup"><span data-stu-id="cefbb-103">Permissions</span></span>
<span data-ttu-id="cefbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cefbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cefbb-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cefbb-106">Permission type</span></span>      | <span data-ttu-id="cefbb-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cefbb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cefbb-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cefbb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cefbb-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cefbb-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cefbb-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cefbb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cefbb-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="cefbb-111">Not supported.</span></span>    |
|<span data-ttu-id="cefbb-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cefbb-112">Application</span></span> | <span data-ttu-id="cefbb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cefbb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cefbb-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cefbb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cefbb-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cefbb-115">Optional query parameters</span></span>
<span data-ttu-id="cefbb-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cefbb-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cefbb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cefbb-117">Request headers</span></span>
| <span data-ttu-id="cefbb-118">名称</span><span class="sxs-lookup"><span data-stu-id="cefbb-118">Name</span></span>      |<span data-ttu-id="cefbb-119">说明</span><span class="sxs-lookup"><span data-stu-id="cefbb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cefbb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cefbb-120">Authorization</span></span>  | <span data-ttu-id="cefbb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cefbb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cefbb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cefbb-123">Request body</span></span>
<span data-ttu-id="cefbb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cefbb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cefbb-125">响应</span><span class="sxs-lookup"><span data-stu-id="cefbb-125">Response</span></span>

<span data-ttu-id="cefbb-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableSort](../resources/tablesort.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cefbb-126">If successful, this method returns a `200 OK` response code and [TableSort](../resources/tablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cefbb-127">示例</span><span class="sxs-lookup"><span data-stu-id="cefbb-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cefbb-128">请求</span><span class="sxs-lookup"><span data-stu-id="cefbb-128">Request</span></span>
<span data-ttu-id="cefbb-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cefbb-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
##### <a name="response"></a><span data-ttu-id="cefbb-130">响应</span><span class="sxs-lookup"><span data-stu-id="cefbb-130">Response</span></span>
<span data-ttu-id="cefbb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cefbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->