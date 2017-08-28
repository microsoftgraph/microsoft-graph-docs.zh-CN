# <a name="get-icon"></a><span data-ttu-id="7bc81-101">获取图标</span><span class="sxs-lookup"><span data-stu-id="7bc81-101">Get Icon</span></span>

<span data-ttu-id="7bc81-102">检索 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7bc81-102">Retrieve the properties and relationships of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bc81-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bc81-103">Prerequisites</span></span>
<span data-ttu-id="7bc81-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="7bc81-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="7bc81-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bc81-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="7bc81-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bc81-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bc81-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7bc81-107">Optional query parameters</span></span>
<span data-ttu-id="7bc81-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7bc81-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bc81-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bc81-109">Request headers</span></span>
| <span data-ttu-id="7bc81-110">名称</span><span class="sxs-lookup"><span data-stu-id="7bc81-110">Name</span></span>      |<span data-ttu-id="7bc81-111">说明</span><span class="sxs-lookup"><span data-stu-id="7bc81-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bc81-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bc81-112">Authorization</span></span>  | <span data-ttu-id="7bc81-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bc81-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bc81-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bc81-115">Request body</span></span>
<span data-ttu-id="7bc81-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7bc81-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bc81-117">响应</span><span class="sxs-lookup"><span data-stu-id="7bc81-117">Response</span></span>

<span data-ttu-id="7bc81-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bc81-118">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bc81-119">示例</span><span class="sxs-lookup"><span data-stu-id="7bc81-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bc81-120">请求</span><span class="sxs-lookup"><span data-stu-id="7bc81-120">Request</span></span>
<span data-ttu-id="7bc81-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bc81-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="7bc81-122">响应</span><span class="sxs-lookup"><span data-stu-id="7bc81-122">Response</span></span>
<span data-ttu-id="7bc81-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bc81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->