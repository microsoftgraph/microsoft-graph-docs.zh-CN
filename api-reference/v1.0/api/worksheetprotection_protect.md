# <a name="worksheetprotection-protect"></a><span data-ttu-id="d1d4c-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="d1d4c-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="d1d4c-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1d4c-104">权限</span><span class="sxs-lookup"><span data-stu-id="d1d4c-104">Permissions</span></span>
<span data-ttu-id="d1d4c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d1d4c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1d4c-107">Permission type</span></span>      | <span data-ttu-id="d1d4c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1d4c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1d4c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1d4c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d1d4c-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1d4c-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1d4c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1d4c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1d4c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-112">Not supported.</span></span>    |
|<span data-ttu-id="d1d4c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1d4c-113">Application</span></span> | <span data-ttu-id="d1d4c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1d4c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1d4c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d1d4c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1d4c-116">Request headers</span></span>
| <span data-ttu-id="d1d4c-117">名称</span><span class="sxs-lookup"><span data-stu-id="d1d4c-117">Name</span></span>       | <span data-ttu-id="d1d4c-118">说明</span><span class="sxs-lookup"><span data-stu-id="d1d4c-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1d4c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1d4c-119">Authorization</span></span>  | <span data-ttu-id="d1d4c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1d4c-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1d4c-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1d4c-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1d4c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1d4c-125">Request body</span></span>
<span data-ttu-id="d1d4c-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1d4c-127">参数</span><span class="sxs-lookup"><span data-stu-id="d1d4c-127">Parameter</span></span>    | <span data-ttu-id="d1d4c-128">类型</span><span class="sxs-lookup"><span data-stu-id="d1d4c-128">Type</span></span>   |<span data-ttu-id="d1d4c-129">说明</span><span class="sxs-lookup"><span data-stu-id="d1d4c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1d4c-130">options</span><span class="sxs-lookup"><span data-stu-id="d1d4c-130">options</span></span>|<span data-ttu-id="d1d4c-131">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d1d4c-131">WorksheetProtectionOptions</span></span>|<span data-ttu-id="d1d4c-p105">可选。工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p105">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d1d4c-134">响应</span><span class="sxs-lookup"><span data-stu-id="d1d4c-134">Response</span></span>

<span data-ttu-id="d1d4c-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1d4c-137">示例</span><span class="sxs-lookup"><span data-stu-id="d1d4c-137">Example</span></span>
<span data-ttu-id="d1d4c-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1d4c-139">请求</span><span class="sxs-lookup"><span data-stu-id="d1d4c-139">Request</span></span>
<span data-ttu-id="d1d4c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="d1d4c-141">响应</span><span class="sxs-lookup"><span data-stu-id="d1d4c-141">Response</span></span>
<span data-ttu-id="d1d4c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d1d4c-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
