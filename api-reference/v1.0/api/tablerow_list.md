# <a name="list-tablerowcollection"></a><span data-ttu-id="36afd-101">列出 TableRowCollection</span><span class="sxs-lookup"><span data-stu-id="36afd-101">List TableRowCollection</span></span>

<span data-ttu-id="36afd-102">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="36afd-102">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="36afd-103">权限</span><span class="sxs-lookup"><span data-stu-id="36afd-103">Permissions</span></span>
<span data-ttu-id="36afd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="36afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36afd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="36afd-106">Permission type</span></span>      | <span data-ttu-id="36afd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36afd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36afd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36afd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="36afd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36afd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36afd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36afd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36afd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="36afd-111">Not supported.</span></span>    |
|<span data-ttu-id="36afd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="36afd-112">Application</span></span> | <span data-ttu-id="36afd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="36afd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36afd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36afd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36afd-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36afd-115">Optional query parameters</span></span>
<span data-ttu-id="36afd-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36afd-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36afd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="36afd-117">Request headers</span></span>
| <span data-ttu-id="36afd-118">名称</span><span class="sxs-lookup"><span data-stu-id="36afd-118">Name</span></span>      |<span data-ttu-id="36afd-119">说明</span><span class="sxs-lookup"><span data-stu-id="36afd-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36afd-120">授权</span><span class="sxs-lookup"><span data-stu-id="36afd-120">Authorization</span></span>  | <span data-ttu-id="36afd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36afd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36afd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36afd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="36afd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="36afd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36afd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36afd-126">Request body</span></span>
<span data-ttu-id="36afd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36afd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36afd-128">响应</span><span class="sxs-lookup"><span data-stu-id="36afd-128">Response</span></span>

<span data-ttu-id="36afd-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[ WorkbookTableRow](../resources/tablerow.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="36afd-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36afd-130">示例</span><span class="sxs-lookup"><span data-stu-id="36afd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36afd-131">请求</span><span class="sxs-lookup"><span data-stu-id="36afd-131">Request</span></span>
<span data-ttu-id="36afd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36afd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerowcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
```
##### <a name="response"></a><span data-ttu-id="36afd-133">响应</span><span class="sxs-lookup"><span data-stu-id="36afd-133">Response</span></span>
<span data-ttu-id="36afd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36afd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableRowCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->