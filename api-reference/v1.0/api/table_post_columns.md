# <a name="create-tablecolumn"></a><span data-ttu-id="4f91b-101">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="4f91b-101">Create TableColumn</span></span>

<span data-ttu-id="4f91b-102">使用此 API 创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="4f91b-102">Use this API to create a new TableColumn.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f91b-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f91b-103">Prerequisites</span></span>
<span data-ttu-id="4f91b-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="4f91b-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="4f91b-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f91b-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="4f91b-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f91b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="4f91b-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f91b-107">Request headers</span></span>
| <span data-ttu-id="4f91b-108">名称</span><span class="sxs-lookup"><span data-stu-id="4f91b-108">Name</span></span>       | <span data-ttu-id="4f91b-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f91b-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f91b-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f91b-110">Authorization</span></span>  | <span data-ttu-id="4f91b-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f91b-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4f91b-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f91b-113">Request body</span></span>
<span data-ttu-id="4f91b-114">在请求正文中，提供 [TableColumn](../resources/tablecolumn.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f91b-114">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4f91b-115">响应</span><span class="sxs-lookup"><span data-stu-id="4f91b-115">Response</span></span>

<span data-ttu-id="4f91b-116">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f91b-116">If successful, this method returns `201, Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f91b-117">示例</span><span class="sxs-lookup"><span data-stu-id="4f91b-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f91b-118">请求</span><span class="sxs-lookup"><span data-stu-id="4f91b-118">Request</span></span>
<span data-ttu-id="4f91b-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f91b-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="4f91b-120">在请求正文中，提供 [TableColumn](../resources/tablecolumn.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f91b-120">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4f91b-121">响应</span><span class="sxs-lookup"><span data-stu-id="4f91b-121">Response</span></span>
<span data-ttu-id="4f91b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f91b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->