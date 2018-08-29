# <a name="rangebordercollection-itemat"></a><span data-ttu-id="553da-101">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="553da-101">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="553da-102">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="553da-102">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="553da-103">权限</span><span class="sxs-lookup"><span data-stu-id="553da-103">Permissions</span></span>
<span data-ttu-id="553da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="553da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="553da-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="553da-106">Permission type</span></span>      | <span data-ttu-id="553da-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="553da-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553da-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="553da-108">Delegated (work or school account)</span></span> | <span data-ttu-id="553da-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553da-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="553da-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="553da-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="553da-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="553da-111">Not supported.</span></span>    |
|<span data-ttu-id="553da-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="553da-112">Application</span></span> | <span data-ttu-id="553da-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="553da-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="553da-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="553da-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="553da-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="553da-115">Request headers</span></span>
| <span data-ttu-id="553da-116">名称</span><span class="sxs-lookup"><span data-stu-id="553da-116">Name</span></span>       | <span data-ttu-id="553da-117">说明</span><span class="sxs-lookup"><span data-stu-id="553da-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="553da-118">授权</span><span class="sxs-lookup"><span data-stu-id="553da-118">Authorization</span></span>  | <span data-ttu-id="553da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="553da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="553da-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="553da-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="553da-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="553da-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="553da-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="553da-124">Request body</span></span>
<span data-ttu-id="553da-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="553da-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="553da-126">参数</span><span class="sxs-lookup"><span data-stu-id="553da-126">Parameter</span></span>    | <span data-ttu-id="553da-127">类型</span><span class="sxs-lookup"><span data-stu-id="553da-127">Type</span></span>   |<span data-ttu-id="553da-128">说明</span><span class="sxs-lookup"><span data-stu-id="553da-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="553da-129">index</span><span class="sxs-lookup"><span data-stu-id="553da-129">index</span></span>|<span data-ttu-id="553da-130">Int32</span><span class="sxs-lookup"><span data-stu-id="553da-130">Int32</span></span>|<span data-ttu-id="553da-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="553da-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="553da-133">响应</span><span class="sxs-lookup"><span data-stu-id="553da-133">Response</span></span>

<span data-ttu-id="553da-134">如果成功，此方法在响应正文中返回`200 OK`响应代码和 [WorkbookRangeBorder](../resources/rangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="553da-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="553da-135">示例</span><span class="sxs-lookup"><span data-stu-id="553da-135">Example</span></span>
<span data-ttu-id="553da-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="553da-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="553da-137">请求</span><span class="sxs-lookup"><span data-stu-id="553da-137">Request</span></span>
<span data-ttu-id="553da-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="553da-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="553da-139">响应</span><span class="sxs-lookup"><span data-stu-id="553da-139">Response</span></span>
<span data-ttu-id="553da-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="553da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->