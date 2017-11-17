# <a name="update-worksheet"></a><span data-ttu-id="c7069-101">更新工作表</span><span class="sxs-lookup"><span data-stu-id="c7069-101">Update worksheet</span></span>

<span data-ttu-id="c7069-102">更新 worksheet 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c7069-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7069-103">权限</span><span class="sxs-lookup"><span data-stu-id="c7069-103">Permissions</span></span>
<span data-ttu-id="c7069-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c7069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7069-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7069-106">Permission type</span></span>      | <span data-ttu-id="c7069-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7069-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7069-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7069-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c7069-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7069-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7069-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7069-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7069-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7069-111">Not supported.</span></span>    |
|<span data-ttu-id="c7069-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7069-112">Application</span></span> | <span data-ttu-id="c7069-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7069-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7069-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7069-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c7069-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c7069-115">Optional request headers</span></span>
| <span data-ttu-id="c7069-116">名称</span><span class="sxs-lookup"><span data-stu-id="c7069-116">Name</span></span>       | <span data-ttu-id="c7069-117">说明</span><span class="sxs-lookup"><span data-stu-id="c7069-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c7069-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7069-118">Authorization</span></span>  | <span data-ttu-id="c7069-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7069-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7069-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7069-121">Request body</span></span>
<span data-ttu-id="c7069-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c7069-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7069-125">属性</span><span class="sxs-lookup"><span data-stu-id="c7069-125">Property</span></span>     | <span data-ttu-id="c7069-126">类型</span><span class="sxs-lookup"><span data-stu-id="c7069-126">Type</span></span>   |<span data-ttu-id="c7069-127">说明</span><span class="sxs-lookup"><span data-stu-id="c7069-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7069-128">name</span><span class="sxs-lookup"><span data-stu-id="c7069-128">name</span></span>|<span data-ttu-id="c7069-129">string</span><span class="sxs-lookup"><span data-stu-id="c7069-129">string</span></span>|<span data-ttu-id="c7069-130">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c7069-130">The display name of the worksheet.</span></span>|
|<span data-ttu-id="c7069-131">position</span><span class="sxs-lookup"><span data-stu-id="c7069-131">position</span></span>|<span data-ttu-id="c7069-132">int</span><span class="sxs-lookup"><span data-stu-id="c7069-132">int</span></span>|<span data-ttu-id="c7069-133">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="c7069-133">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="c7069-134">visibility</span><span class="sxs-lookup"><span data-stu-id="c7069-134">visibility</span></span>|<span data-ttu-id="c7069-135">string</span><span class="sxs-lookup"><span data-stu-id="c7069-135">string</span></span>|<span data-ttu-id="c7069-p104">工作表的可见性。可能的值是：`Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="c7069-p104">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="c7069-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7069-138">Response</span></span>

<span data-ttu-id="c7069-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Worksheet](../resources/worksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7069-139">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7069-140">示例</span><span class="sxs-lookup"><span data-stu-id="c7069-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7069-141">请求</span><span class="sxs-lookup"><span data-stu-id="c7069-141">Request</span></span>
<span data-ttu-id="c7069-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7069-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="c7069-143">响应</span><span class="sxs-lookup"><span data-stu-id="c7069-143">Response</span></span>
<span data-ttu-id="c7069-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7069-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->