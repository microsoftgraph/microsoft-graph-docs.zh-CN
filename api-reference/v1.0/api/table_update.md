# <a name="update-table"></a><span data-ttu-id="b9b9d-101">更新表</span><span class="sxs-lookup"><span data-stu-id="b9b9d-101">Update table</span></span>

<span data-ttu-id="b9b9d-102">更新 table 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9b9d-103">权限</span><span class="sxs-lookup"><span data-stu-id="b9b9d-103">Permissions</span></span>
<span data-ttu-id="b9b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9b9d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9b9d-106">Permission type</span></span>      | <span data-ttu-id="b9b9d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9b9d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9b9d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9b9d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9b9d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9b9d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9b9d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9b9d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9b9d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-111">Not supported.</span></span>    |
|<span data-ttu-id="b9b9d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9b9d-112">Application</span></span> | <span data-ttu-id="b9b9d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9b9d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9b9d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b9b9d-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b9b9d-115">Optional request headers</span></span>
| <span data-ttu-id="b9b9d-116">名称</span><span class="sxs-lookup"><span data-stu-id="b9b9d-116">Name</span></span>       | <span data-ttu-id="b9b9d-117">说明</span><span class="sxs-lookup"><span data-stu-id="b9b9d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b9b9d-118">授权</span><span class="sxs-lookup"><span data-stu-id="b9b9d-118">Authorization</span></span>  | <span data-ttu-id="b9b9d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9b9d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9b9d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9b9d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9b9d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9b9d-124">Request body</span></span>
<span data-ttu-id="b9b9d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9b9d-128">属性</span><span class="sxs-lookup"><span data-stu-id="b9b9d-128">Property</span></span>     | <span data-ttu-id="b9b9d-129">类型</span><span class="sxs-lookup"><span data-stu-id="b9b9d-129">Type</span></span>   |<span data-ttu-id="b9b9d-130">说明</span><span class="sxs-lookup"><span data-stu-id="b9b9d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9b9d-131">名称</span><span class="sxs-lookup"><span data-stu-id="b9b9d-131">name</span></span>|<span data-ttu-id="b9b9d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b9b9d-132">string</span></span>|<span data-ttu-id="b9b9d-133">表的名称。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-133">Name of the table.</span></span>|
|<span data-ttu-id="b9b9d-134">showHeaders</span><span class="sxs-lookup"><span data-stu-id="b9b9d-134">showHeaders</span></span>|<span data-ttu-id="b9b9d-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9b9d-135">boolean</span></span>|<span data-ttu-id="b9b9d-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="b9b9d-138">showTotals</span><span class="sxs-lookup"><span data-stu-id="b9b9d-138">showTotals</span></span>|<span data-ttu-id="b9b9d-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9b9d-139">boolean</span></span>|<span data-ttu-id="b9b9d-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="b9b9d-142">样式</span><span class="sxs-lookup"><span data-stu-id="b9b9d-142">style</span></span>|<span data-ttu-id="b9b9d-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b9b9d-143">string</span></span>|<span data-ttu-id="b9b9d-144">代表表格样式的常数值。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-144">Constant value that represents the Table style.</span></span> <span data-ttu-id="b9b9d-145">可能的值为：TableStyleLight1 到 TableStyleLight21，TableStyleMedium1 到 TableStyleMedium28，TableStyleStyleDark1 到 TableStyleStyleDark11。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-145">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="b9b9d-146">也可指定工作簿中存在的自定义的用户定义样式。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-146">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b9b9d-147">响应</span><span class="sxs-lookup"><span data-stu-id="b9b9d-147">Response</span></span>

<span data-ttu-id="b9b9d-148">如果成功，此方法在响应正文中返回`200 OK`响应代码和更新的 [WorkbookTable](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9b9d-149">示例</span><span class="sxs-lookup"><span data-stu-id="b9b9d-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9b9d-150">请求</span><span class="sxs-lookup"><span data-stu-id="b9b9d-150">Request</span></span>
<span data-ttu-id="b9b9d-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="b9b9d-152">响应</span><span class="sxs-lookup"><span data-stu-id="b9b9d-152">Response</span></span>
<span data-ttu-id="b9b9d-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9b9d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
