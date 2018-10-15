# <a name="add-named-item"></a><span data-ttu-id="db75d-101">添加已命名项</span><span class="sxs-lookup"><span data-stu-id="db75d-101">Add Named Item</span></span>

<span data-ttu-id="db75d-102">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="db75d-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="db75d-103">权限</span><span class="sxs-lookup"><span data-stu-id="db75d-103">Permissions</span></span>
<span data-ttu-id="db75d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db75d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db75d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="db75d-106">Permission type</span></span>      | <span data-ttu-id="db75d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db75d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db75d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db75d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="db75d-109">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="db75d-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="db75d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db75d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db75d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="db75d-111">Not supported.</span></span>    |
|<span data-ttu-id="db75d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="db75d-112">Application</span></span> | <span data-ttu-id="db75d-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="db75d-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db75d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db75d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="db75d-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="db75d-115">Request headers</span></span>
| <span data-ttu-id="db75d-116">名称</span><span class="sxs-lookup"><span data-stu-id="db75d-116">Name</span></span>       | <span data-ttu-id="db75d-117">说明</span><span class="sxs-lookup"><span data-stu-id="db75d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db75d-118">授权</span><span class="sxs-lookup"><span data-stu-id="db75d-118">Authorization</span></span>  | <span data-ttu-id="db75d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db75d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db75d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db75d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="db75d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="db75d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db75d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="db75d-124">Request body</span></span>
<span data-ttu-id="db75d-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="db75d-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db75d-126">参数</span><span class="sxs-lookup"><span data-stu-id="db75d-126">Parameter</span></span>    | <span data-ttu-id="db75d-127">类型</span><span class="sxs-lookup"><span data-stu-id="db75d-127">Type</span></span>   |<span data-ttu-id="db75d-128">说明</span><span class="sxs-lookup"><span data-stu-id="db75d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db75d-129">name</span><span class="sxs-lookup"><span data-stu-id="db75d-129">name</span></span>|<span data-ttu-id="db75d-130">string</span><span class="sxs-lookup"><span data-stu-id="db75d-130">string</span></span>|<span data-ttu-id="db75d-131">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="db75d-131">The name of the named item.</span></span>|
|<span data-ttu-id="db75d-132">reference</span><span class="sxs-lookup"><span data-stu-id="db75d-132">reference</span></span>|<span data-ttu-id="db75d-133">Json</span><span class="sxs-lookup"><span data-stu-id="db75d-133">Json</span></span>|<span data-ttu-id="db75d-134">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="db75d-134">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="db75d-135">comment</span><span class="sxs-lookup"><span data-stu-id="db75d-135">comment</span></span>|<span data-ttu-id="db75d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="db75d-136">string</span></span>|<span data-ttu-id="db75d-137">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="db75d-137">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="db75d-138">响应</span><span class="sxs-lookup"><span data-stu-id="db75d-138">Response</span></span>

<span data-ttu-id="db75d-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [WorkbookNamedItem](../resources/NamedItem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db75d-139">If successful, this method returns `200 OK` response code and [groupSetting](../resources/NamedItem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="db75d-140">示例</span><span class="sxs-lookup"><span data-stu-id="db75d-140">Example</span></span>
<span data-ttu-id="db75d-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db75d-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="db75d-142">请求</span><span class="sxs-lookup"><span data-stu-id="db75d-142">Request</span></span>
<span data-ttu-id="db75d-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db75d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="db75d-144">响应</span><span class="sxs-lookup"><span data-stu-id="db75d-144">Response</span></span>
<span data-ttu-id="db75d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db75d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->
