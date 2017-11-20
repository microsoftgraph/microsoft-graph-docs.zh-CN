# <a name="tablecollection-add"></a><span data-ttu-id="04477-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="04477-101">TableCollection: add</span></span>

<span data-ttu-id="04477-p101">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="04477-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="04477-105">权限</span><span class="sxs-lookup"><span data-stu-id="04477-105">Permissions</span></span>
<span data-ttu-id="04477-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04477-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04477-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="04477-108">Permission type</span></span>      | <span data-ttu-id="04477-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04477-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04477-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04477-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04477-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04477-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04477-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04477-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04477-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="04477-113">Not supported.</span></span>    |
|<span data-ttu-id="04477-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="04477-114">Application</span></span> | <span data-ttu-id="04477-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04477-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04477-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04477-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="04477-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="04477-117">Request headers</span></span>
| <span data-ttu-id="04477-118">名称</span><span class="sxs-lookup"><span data-stu-id="04477-118">Name</span></span>       | <span data-ttu-id="04477-119">说明</span><span class="sxs-lookup"><span data-stu-id="04477-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04477-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04477-120">Authorization</span></span>  | <span data-ttu-id="04477-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04477-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04477-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="04477-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="04477-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="04477-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04477-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04477-126">Request body</span></span>
<span data-ttu-id="04477-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="04477-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04477-128">参数</span><span class="sxs-lookup"><span data-stu-id="04477-128">Parameter</span></span>    | <span data-ttu-id="04477-129">类型</span><span class="sxs-lookup"><span data-stu-id="04477-129">Type</span></span>   |<span data-ttu-id="04477-130">说明</span><span class="sxs-lookup"><span data-stu-id="04477-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04477-131">地址</span><span class="sxs-lookup"><span data-stu-id="04477-131">address</span></span>|<span data-ttu-id="04477-132">string</span><span class="sxs-lookup"><span data-stu-id="04477-132">string</span></span>|<span data-ttu-id="04477-p105">表示数据源的 range 对象的地址或名称。如果该地址不包含工作表名称，则使用当前活动的工作表。</span><span class="sxs-lookup"><span data-stu-id="04477-p105">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="04477-135">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="04477-135">hasHeaders</span></span>|<span data-ttu-id="04477-136">布尔</span><span class="sxs-lookup"><span data-stu-id="04477-136">boolean</span></span>|<span data-ttu-id="04477-p106">指示导入的数据是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="04477-p106">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="04477-140">响应</span><span class="sxs-lookup"><span data-stu-id="04477-140">Response</span></span>

<span data-ttu-id="04477-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04477-141">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04477-142">示例</span><span class="sxs-lookup"><span data-stu-id="04477-142">Example</span></span>
<span data-ttu-id="04477-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="04477-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="04477-144">请求</span><span class="sxs-lookup"><span data-stu-id="04477-144">Request</span></span>
<span data-ttu-id="04477-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04477-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="04477-146">响应</span><span class="sxs-lookup"><span data-stu-id="04477-146">Response</span></span>
<span data-ttu-id="04477-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04477-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
