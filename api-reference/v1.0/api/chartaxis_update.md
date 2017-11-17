# <a name="update-chartaxis"></a><span data-ttu-id="1da57-101">更新 chartaxis</span><span class="sxs-lookup"><span data-stu-id="1da57-101">Update chartaxis</span></span>

<span data-ttu-id="1da57-102">更新 chartaxis 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1da57-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1da57-103">权限</span><span class="sxs-lookup"><span data-stu-id="1da57-103">Permissions</span></span>
<span data-ttu-id="1da57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1da57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1da57-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="1da57-106">Permission type</span></span>      | <span data-ttu-id="1da57-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1da57-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1da57-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1da57-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1da57-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da57-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1da57-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1da57-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1da57-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1da57-111">Not supported.</span></span>    |
|<span data-ttu-id="1da57-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="1da57-112">Application</span></span> | <span data-ttu-id="1da57-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1da57-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1da57-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1da57-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="1da57-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="1da57-115">Optional request headers</span></span>
| <span data-ttu-id="1da57-116">名称</span><span class="sxs-lookup"><span data-stu-id="1da57-116">Name</span></span>       | <span data-ttu-id="1da57-117">说明</span><span class="sxs-lookup"><span data-stu-id="1da57-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1da57-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="1da57-118">Authorization</span></span>  | <span data-ttu-id="1da57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1da57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1da57-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="1da57-121">Request body</span></span>
<span data-ttu-id="1da57-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1da57-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1da57-125">属性</span><span class="sxs-lookup"><span data-stu-id="1da57-125">Property</span></span>     | <span data-ttu-id="1da57-126">类型</span><span class="sxs-lookup"><span data-stu-id="1da57-126">Type</span></span>   |<span data-ttu-id="1da57-127">说明</span><span class="sxs-lookup"><span data-stu-id="1da57-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1da57-128">majorUnit</span><span class="sxs-lookup"><span data-stu-id="1da57-128">majorUnit</span></span>|<span data-ttu-id="1da57-129">对象</span><span class="sxs-lookup"><span data-stu-id="1da57-129">object</span></span>|<span data-ttu-id="1da57-p104">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="1da57-p104">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="1da57-133">maximum</span><span class="sxs-lookup"><span data-stu-id="1da57-133">maximum</span></span>|<span data-ttu-id="1da57-134">object</span><span class="sxs-lookup"><span data-stu-id="1da57-134">object</span></span>|<span data-ttu-id="1da57-p105">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="1da57-p105">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="1da57-138">minimum</span><span class="sxs-lookup"><span data-stu-id="1da57-138">minimum</span></span>|<span data-ttu-id="1da57-139">object</span><span class="sxs-lookup"><span data-stu-id="1da57-139">object</span></span>|<span data-ttu-id="1da57-p106">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="1da57-p106">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="1da57-143">minorUnit</span><span class="sxs-lookup"><span data-stu-id="1da57-143">minorUnit</span></span>|<span data-ttu-id="1da57-144">对象</span><span class="sxs-lookup"><span data-stu-id="1da57-144">object</span></span>|<span data-ttu-id="1da57-p107">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="1da57-p107">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="1da57-148">响应</span><span class="sxs-lookup"><span data-stu-id="1da57-148">Response</span></span>

<span data-ttu-id="1da57-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartAxis](../resources/chartaxis.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1da57-149">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1da57-150">示例</span><span class="sxs-lookup"><span data-stu-id="1da57-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1da57-151">请求</span><span class="sxs-lookup"><span data-stu-id="1da57-151">Request</span></span>
<span data-ttu-id="1da57-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1da57-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="1da57-153">响应</span><span class="sxs-lookup"><span data-stu-id="1da57-153">Response</span></span>
<span data-ttu-id="1da57-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1da57-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->