# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="4ae33-101">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="4ae33-101">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="4ae33-102">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="4ae33-102">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ae33-103">权限</span><span class="sxs-lookup"><span data-stu-id="4ae33-103">Permissions</span></span>
<span data-ttu-id="4ae33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ae33-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ae33-106">Permission type</span></span>      | <span data-ttu-id="4ae33-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ae33-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ae33-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae33-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4ae33-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ae33-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ae33-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae33-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ae33-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae33-111">Not supported.</span></span>    |
|<span data-ttu-id="4ae33-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ae33-112">Application</span></span> | <span data-ttu-id="4ae33-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae33-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ae33-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ae33-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="4ae33-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ae33-115">Request headers</span></span>
| <span data-ttu-id="4ae33-116">名称</span><span class="sxs-lookup"><span data-stu-id="4ae33-116">Name</span></span>       | <span data-ttu-id="4ae33-117">说明</span><span class="sxs-lookup"><span data-stu-id="4ae33-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ae33-118">授权</span><span class="sxs-lookup"><span data-stu-id="4ae33-118">Authorization</span></span>  | <span data-ttu-id="4ae33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ae33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ae33-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ae33-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ae33-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4ae33-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae33-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ae33-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4ae33-125">响应</span><span class="sxs-lookup"><span data-stu-id="4ae33-125">Response</span></span>

<span data-ttu-id="4ae33-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ae33-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae33-127">示例</span><span class="sxs-lookup"><span data-stu-id="4ae33-127">Example</span></span>
<span data-ttu-id="4ae33-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4ae33-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ae33-129">请求</span><span class="sxs-lookup"><span data-stu-id="4ae33-129">Request</span></span>
<span data-ttu-id="4ae33-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ae33-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="4ae33-131">响应</span><span class="sxs-lookup"><span data-stu-id="4ae33-131">Response</span></span>
<span data-ttu-id="4ae33-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ae33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->