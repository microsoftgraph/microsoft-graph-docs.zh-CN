# <a name="table-converttorange"></a><span data-ttu-id="9f94d-101">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="9f94d-101">Table: convertToRange</span></span>

<span data-ttu-id="9f94d-p101">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="9f94d-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f94d-104">权限</span><span class="sxs-lookup"><span data-stu-id="9f94d-104">Permissions</span></span>
<span data-ttu-id="9f94d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9f94d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f94d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f94d-107">Permission type</span></span>      | <span data-ttu-id="9f94d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f94d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f94d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f94d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9f94d-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f94d-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f94d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f94d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f94d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f94d-112">Not supported.</span></span>    |
|<span data-ttu-id="9f94d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f94d-113">Application</span></span> | <span data-ttu-id="9f94d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f94d-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f94d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f94d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="9f94d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f94d-116">Request headers</span></span>
| <span data-ttu-id="9f94d-117">名称</span><span class="sxs-lookup"><span data-stu-id="9f94d-117">Name</span></span>       | <span data-ttu-id="9f94d-118">说明</span><span class="sxs-lookup"><span data-stu-id="9f94d-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f94d-119">授权</span><span class="sxs-lookup"><span data-stu-id="9f94d-119">Authorization</span></span>  | <span data-ttu-id="9f94d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f94d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f94d-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f94d-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f94d-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9f94d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f94d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f94d-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9f94d-126">响应</span><span class="sxs-lookup"><span data-stu-id="9f94d-126">Response</span></span>

<span data-ttu-id="9f94d-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f94d-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f94d-128">示例</span><span class="sxs-lookup"><span data-stu-id="9f94d-128">Example</span></span>
<span data-ttu-id="9f94d-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9f94d-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9f94d-130">请求</span><span class="sxs-lookup"><span data-stu-id="9f94d-130">Request</span></span>
<span data-ttu-id="9f94d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f94d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="9f94d-132">响应</span><span class="sxs-lookup"><span data-stu-id="9f94d-132">Response</span></span>
<span data-ttu-id="9f94d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f94d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->