# <a name="update-chartlineformat"></a><span data-ttu-id="6dd71-101">更新 chartlineformat</span><span class="sxs-lookup"><span data-stu-id="6dd71-101">Update chartlineformat</span></span>

<span data-ttu-id="6dd71-102">更新 chartlineformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6dd71-102">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6dd71-103">权限</span><span class="sxs-lookup"><span data-stu-id="6dd71-103">Permissions</span></span>
<span data-ttu-id="6dd71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6dd71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6dd71-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dd71-106">Permission type</span></span>      | <span data-ttu-id="6dd71-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6dd71-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dd71-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dd71-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6dd71-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dd71-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6dd71-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dd71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dd71-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dd71-111">Not supported.</span></span>    |
|<span data-ttu-id="6dd71-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dd71-112">Application</span></span> | <span data-ttu-id="6dd71-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dd71-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dd71-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dd71-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="6dd71-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="6dd71-115">Optional request headers</span></span>
| <span data-ttu-id="6dd71-116">名称</span><span class="sxs-lookup"><span data-stu-id="6dd71-116">Name</span></span>       | <span data-ttu-id="6dd71-117">说明</span><span class="sxs-lookup"><span data-stu-id="6dd71-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6dd71-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dd71-118">Authorization</span></span>  | <span data-ttu-id="6dd71-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6dd71-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dd71-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dd71-121">Request body</span></span>
<span data-ttu-id="6dd71-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6dd71-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6dd71-125">属性</span><span class="sxs-lookup"><span data-stu-id="6dd71-125">Property</span></span>     | <span data-ttu-id="6dd71-126">类型</span><span class="sxs-lookup"><span data-stu-id="6dd71-126">Type</span></span>   |<span data-ttu-id="6dd71-127">说明</span><span class="sxs-lookup"><span data-stu-id="6dd71-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dd71-128">color</span><span class="sxs-lookup"><span data-stu-id="6dd71-128">color</span></span>|<span data-ttu-id="6dd71-129">string</span><span class="sxs-lookup"><span data-stu-id="6dd71-129">string</span></span>|<span data-ttu-id="6dd71-130">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="6dd71-130">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="6dd71-131">响应</span><span class="sxs-lookup"><span data-stu-id="6dd71-131">Response</span></span>

<span data-ttu-id="6dd71-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartLineFormat](../resources/chartlineformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6dd71-132">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dd71-133">示例</span><span class="sxs-lookup"><span data-stu-id="6dd71-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dd71-134">请求</span><span class="sxs-lookup"><span data-stu-id="6dd71-134">Request</span></span>
<span data-ttu-id="6dd71-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dd71-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="6dd71-136">响应</span><span class="sxs-lookup"><span data-stu-id="6dd71-136">Response</span></span>
<span data-ttu-id="6dd71-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dd71-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->