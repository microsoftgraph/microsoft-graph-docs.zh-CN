# <a name="update-nameditem"></a><span data-ttu-id="25cc5-101">更新 nameditem</span><span class="sxs-lookup"><span data-stu-id="25cc5-101">Update nameditem</span></span>

<span data-ttu-id="25cc5-102">更新 nameditem 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="25cc5-102">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="25cc5-103">权限</span><span class="sxs-lookup"><span data-stu-id="25cc5-103">Permissions</span></span>
<span data-ttu-id="25cc5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="25cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25cc5-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="25cc5-106">Permission type</span></span>      | <span data-ttu-id="25cc5-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25cc5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25cc5-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25cc5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="25cc5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25cc5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="25cc5-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25cc5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25cc5-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="25cc5-111">Not supported.</span></span>    |
|<span data-ttu-id="25cc5-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="25cc5-112">Application</span></span> | <span data-ttu-id="25cc5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="25cc5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25cc5-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25cc5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="25cc5-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="25cc5-115">Optional request headers</span></span>
| <span data-ttu-id="25cc5-116">名称</span><span class="sxs-lookup"><span data-stu-id="25cc5-116">Name</span></span>       | <span data-ttu-id="25cc5-117">说明</span><span class="sxs-lookup"><span data-stu-id="25cc5-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="25cc5-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="25cc5-118">Authorization</span></span>  | <span data-ttu-id="25cc5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25cc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25cc5-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="25cc5-121">Request body</span></span>
<span data-ttu-id="25cc5-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="25cc5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="25cc5-125">属性</span><span class="sxs-lookup"><span data-stu-id="25cc5-125">Property</span></span>     | <span data-ttu-id="25cc5-126">类型</span><span class="sxs-lookup"><span data-stu-id="25cc5-126">Type</span></span>   |<span data-ttu-id="25cc5-127">说明</span><span class="sxs-lookup"><span data-stu-id="25cc5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25cc5-128">visible</span><span class="sxs-lookup"><span data-stu-id="25cc5-128">visible</span></span>|<span data-ttu-id="25cc5-129">boolean</span><span class="sxs-lookup"><span data-stu-id="25cc5-129">boolean</span></span>|<span data-ttu-id="25cc5-130">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="25cc5-130">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="25cc5-131">comment</span><span class="sxs-lookup"><span data-stu-id="25cc5-131">comment</span></span>|   <span data-ttu-id="25cc5-132">string</span><span class="sxs-lookup"><span data-stu-id="25cc5-132">string</span></span>  |<span data-ttu-id="25cc5-133">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="25cc5-133">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="25cc5-134">响应</span><span class="sxs-lookup"><span data-stu-id="25cc5-134">Response</span></span>

<span data-ttu-id="25cc5-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [NamedItem](../resources/nameditem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25cc5-135">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25cc5-136">示例</span><span class="sxs-lookup"><span data-stu-id="25cc5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25cc5-137">请求</span><span class="sxs-lookup"><span data-stu-id="25cc5-137">Request</span></span>
<span data-ttu-id="25cc5-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25cc5-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="25cc5-139">响应</span><span class="sxs-lookup"><span data-stu-id="25cc5-139">Response</span></span>
<span data-ttu-id="25cc5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25cc5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
