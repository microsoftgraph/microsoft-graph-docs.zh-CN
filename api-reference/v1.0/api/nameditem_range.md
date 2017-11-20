# <a name="nameditem-range"></a><span data-ttu-id="8798b-101">NamedItem：Range</span><span class="sxs-lookup"><span data-stu-id="8798b-101">NamedItem: Range</span></span>

<span data-ttu-id="8798b-p101">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="8798b-p101">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="8798b-104">权限</span><span class="sxs-lookup"><span data-stu-id="8798b-104">Permissions</span></span>
<span data-ttu-id="8798b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8798b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8798b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8798b-107">Permission type</span></span>      | <span data-ttu-id="8798b-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8798b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8798b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8798b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8798b-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8798b-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8798b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8798b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8798b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8798b-112">Not supported.</span></span>    |
|<span data-ttu-id="8798b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8798b-113">Application</span></span> | <span data-ttu-id="8798b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8798b-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8798b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8798b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/Range

```
## <a name="request-headers"></a><span data-ttu-id="8798b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8798b-116">Request headers</span></span>
| <span data-ttu-id="8798b-117">名称</span><span class="sxs-lookup"><span data-stu-id="8798b-117">Name</span></span>       | <span data-ttu-id="8798b-118">说明</span><span class="sxs-lookup"><span data-stu-id="8798b-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8798b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8798b-119">Authorization</span></span>  | <span data-ttu-id="8798b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8798b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8798b-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8798b-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="8798b-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8798b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8798b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8798b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8798b-126">响应</span><span class="sxs-lookup"><span data-stu-id="8798b-126">Response</span></span>

<span data-ttu-id="8798b-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8798b-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8798b-128">示例</span><span class="sxs-lookup"><span data-stu-id="8798b-128">Example</span></span>
<span data-ttu-id="8798b-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8798b-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8798b-130">请求</span><span class="sxs-lookup"><span data-stu-id="8798b-130">Request</span></span>
<span data-ttu-id="8798b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8798b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/Range
```

##### <a name="response"></a><span data-ttu-id="8798b-132">响应</span><span class="sxs-lookup"><span data-stu-id="8798b-132">Response</span></span>
<span data-ttu-id="8798b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8798b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->