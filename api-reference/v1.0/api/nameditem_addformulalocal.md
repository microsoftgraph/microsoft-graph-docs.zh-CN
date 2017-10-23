# <a name="add-named-item-formulalocal"></a><span data-ttu-id="8e9ea-101">添加已命名项 FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="8e9ea-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="8e9ea-102">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e9ea-103">权限</span><span class="sxs-lookup"><span data-stu-id="8e9ea-103">Permissions</span></span>
<span data-ttu-id="8e9ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e9ea-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e9ea-106">Permission type</span></span>      | <span data-ttu-id="8e9ea-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e9ea-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e9ea-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e9ea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8e9ea-109">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e9ea-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="8e9ea-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e9ea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e9ea-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-111">Not supported.</span></span>    |
|<span data-ttu-id="8e9ea-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e9ea-112">Application</span></span> | <span data-ttu-id="8e9ea-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e9ea-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e9ea-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e9ea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="8e9ea-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e9ea-115">Request headers</span></span>
| <span data-ttu-id="8e9ea-116">名称</span><span class="sxs-lookup"><span data-stu-id="8e9ea-116">Name</span></span>       | <span data-ttu-id="8e9ea-117">说明</span><span class="sxs-lookup"><span data-stu-id="8e9ea-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e9ea-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9ea-118">Authorization</span></span>  | <span data-ttu-id="8e9ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e9ea-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e9ea-121">Request body</span></span>
<span data-ttu-id="8e9ea-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e9ea-123">参数</span><span class="sxs-lookup"><span data-stu-id="8e9ea-123">Parameter</span></span>    | <span data-ttu-id="8e9ea-124">类型</span><span class="sxs-lookup"><span data-stu-id="8e9ea-124">Type</span></span>   |<span data-ttu-id="8e9ea-125">说明</span><span class="sxs-lookup"><span data-stu-id="8e9ea-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e9ea-126">name</span><span class="sxs-lookup"><span data-stu-id="8e9ea-126">name</span></span>|<span data-ttu-id="8e9ea-127">string</span><span class="sxs-lookup"><span data-stu-id="8e9ea-127">string</span></span>|<span data-ttu-id="8e9ea-128">已命名项的名称。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-128">The name of the named item.</span></span>|
|<span data-ttu-id="8e9ea-129">公式</span><span class="sxs-lookup"><span data-stu-id="8e9ea-129">formula</span></span>|<span data-ttu-id="8e9ea-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8e9ea-130">string</span></span>|<span data-ttu-id="8e9ea-131">名称将引用的公式或区域。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="8e9ea-132">comment</span><span class="sxs-lookup"><span data-stu-id="8e9ea-132">comment</span></span>|<span data-ttu-id="8e9ea-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8e9ea-133">string</span></span>|<span data-ttu-id="8e9ea-134">与此已命名项相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="8e9ea-135">响应</span><span class="sxs-lookup"><span data-stu-id="8e9ea-135">Response</span></span>

<span data-ttu-id="8e9ea-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [NamedItem](../resources/NamedItem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-136">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9ea-137">示例</span><span class="sxs-lookup"><span data-stu-id="8e9ea-137">Example</span></span>
<span data-ttu-id="8e9ea-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8e9ea-139">请求</span><span class="sxs-lookup"><span data-stu-id="8e9ea-139">Request</span></span>
<span data-ttu-id="8e9ea-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="8e9ea-141">响应</span><span class="sxs-lookup"><span data-stu-id="8e9ea-141">Response</span></span>
<span data-ttu-id="8e9ea-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e9ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
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
  "tocPath": ""
}-->
