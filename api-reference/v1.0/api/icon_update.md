# <a name="update-icon"></a><span data-ttu-id="07eea-101">更新图标</span><span class="sxs-lookup"><span data-stu-id="07eea-101">Update icon</span></span>

<span data-ttu-id="07eea-102">更新 icon 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07eea-102">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07eea-103">权限</span><span class="sxs-lookup"><span data-stu-id="07eea-103">Permissions</span></span>
<span data-ttu-id="07eea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="07eea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="07eea-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="07eea-106">Permission type</span></span>      | <span data-ttu-id="07eea-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07eea-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="07eea-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07eea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="07eea-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07eea-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="07eea-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07eea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07eea-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="07eea-111">Not supported.</span></span>    | 
|<span data-ttu-id="07eea-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="07eea-112">Application</span></span> | <span data-ttu-id="07eea-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="07eea-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="07eea-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07eea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="07eea-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="07eea-115">Optional request headers</span></span>
| <span data-ttu-id="07eea-116">名称</span><span class="sxs-lookup"><span data-stu-id="07eea-116">Name</span></span>       | <span data-ttu-id="07eea-117">说明</span><span class="sxs-lookup"><span data-stu-id="07eea-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="07eea-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="07eea-118">Authorization</span></span>  | <span data-ttu-id="07eea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07eea-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="07eea-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="07eea-121">Request body</span></span>
<span data-ttu-id="07eea-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="07eea-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07eea-125">属性</span><span class="sxs-lookup"><span data-stu-id="07eea-125">Property</span></span>     | <span data-ttu-id="07eea-126">类型</span><span class="sxs-lookup"><span data-stu-id="07eea-126">Type</span></span>   |<span data-ttu-id="07eea-127">说明</span><span class="sxs-lookup"><span data-stu-id="07eea-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07eea-128">index</span><span class="sxs-lookup"><span data-stu-id="07eea-128">index</span></span>|<span data-ttu-id="07eea-129">int</span><span class="sxs-lookup"><span data-stu-id="07eea-129">int</span></span>|<span data-ttu-id="07eea-130">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="07eea-130">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="07eea-131">set</span><span class="sxs-lookup"><span data-stu-id="07eea-131">set</span></span>|<span data-ttu-id="07eea-132">string</span><span class="sxs-lookup"><span data-stu-id="07eea-132">string</span></span>|<span data-ttu-id="07eea-p104">表示图标所属的集合。可能的值是：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles``FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="07eea-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="07eea-135">响应</span><span class="sxs-lookup"><span data-stu-id="07eea-135">Response</span></span>

<span data-ttu-id="07eea-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07eea-136">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07eea-137">示例</span><span class="sxs-lookup"><span data-stu-id="07eea-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07eea-138">请求</span><span class="sxs-lookup"><span data-stu-id="07eea-138">Request</span></span>
<span data-ttu-id="07eea-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07eea-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="07eea-140">响应</span><span class="sxs-lookup"><span data-stu-id="07eea-140">Response</span></span>
<span data-ttu-id="07eea-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07eea-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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