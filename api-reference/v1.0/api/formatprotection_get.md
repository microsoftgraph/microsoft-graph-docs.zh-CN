# <a name="get-formatprotection"></a><span data-ttu-id="006dd-101">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="006dd-101">Get FormatProtection</span></span>

<span data-ttu-id="006dd-102">检索 formatprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="006dd-102">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="006dd-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="006dd-103">Prerequisites</span></span>
<span data-ttu-id="006dd-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="006dd-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="006dd-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="006dd-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="006dd-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="006dd-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="006dd-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="006dd-107">Optional query parameters</span></span>
<span data-ttu-id="006dd-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="006dd-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="006dd-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="006dd-109">Request headers</span></span>
| <span data-ttu-id="006dd-110">名称</span><span class="sxs-lookup"><span data-stu-id="006dd-110">Name</span></span>      |<span data-ttu-id="006dd-111">说明</span><span class="sxs-lookup"><span data-stu-id="006dd-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="006dd-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="006dd-112">Authorization</span></span>  | <span data-ttu-id="006dd-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="006dd-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="006dd-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="006dd-115">Request body</span></span>
<span data-ttu-id="006dd-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="006dd-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="006dd-117">响应</span><span class="sxs-lookup"><span data-stu-id="006dd-117">Response</span></span>

<span data-ttu-id="006dd-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="006dd-118">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="006dd-119">示例</span><span class="sxs-lookup"><span data-stu-id="006dd-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="006dd-120">请求</span><span class="sxs-lookup"><span data-stu-id="006dd-120">Request</span></span>
<span data-ttu-id="006dd-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="006dd-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="006dd-122">响应</span><span class="sxs-lookup"><span data-stu-id="006dd-122">Response</span></span>
<span data-ttu-id="006dd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="006dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->