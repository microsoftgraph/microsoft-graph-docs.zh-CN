# <a name="update-chart"></a><span data-ttu-id="fd5ce-101">更新图表</span><span class="sxs-lookup"><span data-stu-id="fd5ce-101">Update chart</span></span>

<span data-ttu-id="fd5ce-102">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd5ce-103">权限</span><span class="sxs-lookup"><span data-stu-id="fd5ce-103">Permissions</span></span>
<span data-ttu-id="fd5ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd5ce-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd5ce-106">Permission type</span></span>      | <span data-ttu-id="fd5ce-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd5ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd5ce-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd5ce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fd5ce-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd5ce-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd5ce-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd5ce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd5ce-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-111">Not supported.</span></span>    |
|<span data-ttu-id="fd5ce-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd5ce-112">Application</span></span> | <span data-ttu-id="fd5ce-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd5ce-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd5ce-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="fd5ce-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fd5ce-115">Optional request headers</span></span>
| <span data-ttu-id="fd5ce-116">名称</span><span class="sxs-lookup"><span data-stu-id="fd5ce-116">Name</span></span>       | <span data-ttu-id="fd5ce-117">说明</span><span class="sxs-lookup"><span data-stu-id="fd5ce-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fd5ce-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd5ce-118">Authorization</span></span>  | <span data-ttu-id="fd5ce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd5ce-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd5ce-121">Request body</span></span>
<span data-ttu-id="fd5ce-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd5ce-125">属性</span><span class="sxs-lookup"><span data-stu-id="fd5ce-125">Property</span></span>     | <span data-ttu-id="fd5ce-126">类型</span><span class="sxs-lookup"><span data-stu-id="fd5ce-126">Type</span></span>   |<span data-ttu-id="fd5ce-127">说明</span><span class="sxs-lookup"><span data-stu-id="fd5ce-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd5ce-128">height</span><span class="sxs-lookup"><span data-stu-id="fd5ce-128">height</span></span>|<span data-ttu-id="fd5ce-129">double</span><span class="sxs-lookup"><span data-stu-id="fd5ce-129">double</span></span>|<span data-ttu-id="fd5ce-130">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-130">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="fd5ce-131">left</span><span class="sxs-lookup"><span data-stu-id="fd5ce-131">left</span></span>|<span data-ttu-id="fd5ce-132">double</span><span class="sxs-lookup"><span data-stu-id="fd5ce-132">double</span></span>|<span data-ttu-id="fd5ce-133">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-133">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="fd5ce-134">name</span><span class="sxs-lookup"><span data-stu-id="fd5ce-134">name</span></span>|<span data-ttu-id="fd5ce-135">string</span><span class="sxs-lookup"><span data-stu-id="fd5ce-135">string</span></span>|<span data-ttu-id="fd5ce-136">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-136">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="fd5ce-137">top</span><span class="sxs-lookup"><span data-stu-id="fd5ce-137">top</span></span>|<span data-ttu-id="fd5ce-138">double</span><span class="sxs-lookup"><span data-stu-id="fd5ce-138">double</span></span>|<span data-ttu-id="fd5ce-139">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-139">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="fd5ce-140">width</span><span class="sxs-lookup"><span data-stu-id="fd5ce-140">width</span></span>|<span data-ttu-id="fd5ce-141">double</span><span class="sxs-lookup"><span data-stu-id="fd5ce-141">double</span></span>|<span data-ttu-id="fd5ce-142">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-142">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="fd5ce-143">响应</span><span class="sxs-lookup"><span data-stu-id="fd5ce-143">Response</span></span>

<span data-ttu-id="fd5ce-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-144">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd5ce-145">示例</span><span class="sxs-lookup"><span data-stu-id="fd5ce-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd5ce-146">请求</span><span class="sxs-lookup"><span data-stu-id="fd5ce-146">Request</span></span>
<span data-ttu-id="fd5ce-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="fd5ce-148">响应</span><span class="sxs-lookup"><span data-stu-id="fd5ce-148">Response</span></span>
<span data-ttu-id="fd5ce-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd5ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->