# <a name="update-icon"></a><span data-ttu-id="60906-101">更新图标</span><span class="sxs-lookup"><span data-stu-id="60906-101">Update icon</span></span>

<span data-ttu-id="60906-102">更新 icon 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60906-102">Update the properties of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60906-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="60906-103">Prerequisites</span></span>
<span data-ttu-id="60906-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="60906-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="60906-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60906-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="60906-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60906-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="60906-107">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="60906-107">Optional request headers</span></span>
| <span data-ttu-id="60906-108">名称</span><span class="sxs-lookup"><span data-stu-id="60906-108">Name</span></span>       | <span data-ttu-id="60906-109">说明</span><span class="sxs-lookup"><span data-stu-id="60906-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60906-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="60906-110">Authorization</span></span>  | <span data-ttu-id="60906-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60906-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60906-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="60906-113">Request body</span></span>
<span data-ttu-id="60906-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="60906-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60906-117">属性</span><span class="sxs-lookup"><span data-stu-id="60906-117">Property</span></span>     | <span data-ttu-id="60906-118">类型</span><span class="sxs-lookup"><span data-stu-id="60906-118">Type</span></span>   |<span data-ttu-id="60906-119">说明</span><span class="sxs-lookup"><span data-stu-id="60906-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60906-120">index</span><span class="sxs-lookup"><span data-stu-id="60906-120">index</span></span>|<span data-ttu-id="60906-121">int</span><span class="sxs-lookup"><span data-stu-id="60906-121">int</span></span>|<span data-ttu-id="60906-122">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="60906-122">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="60906-123">set</span><span class="sxs-lookup"><span data-stu-id="60906-123">set</span></span>|<span data-ttu-id="60906-124">string</span><span class="sxs-lookup"><span data-stu-id="60906-124">string</span></span>|<span data-ttu-id="60906-p103">表示图标所属的集合。可能的值是：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles``FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="60906-p103">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="60906-127">响应</span><span class="sxs-lookup"><span data-stu-id="60906-127">Response</span></span>

<span data-ttu-id="60906-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60906-128">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60906-129">示例</span><span class="sxs-lookup"><span data-stu-id="60906-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60906-130">请求</span><span class="sxs-lookup"><span data-stu-id="60906-130">Request</span></span>
<span data-ttu-id="60906-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60906-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="60906-132">响应</span><span class="sxs-lookup"><span data-stu-id="60906-132">Response</span></span>
<span data-ttu-id="60906-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60906-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->