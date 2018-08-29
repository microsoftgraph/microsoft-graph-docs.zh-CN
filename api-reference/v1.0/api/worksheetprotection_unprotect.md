# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="cb856-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="cb856-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="cb856-102">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="cb856-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="cb856-103">权限</span><span class="sxs-lookup"><span data-stu-id="cb856-103">Permissions</span></span>
<span data-ttu-id="cb856-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cb856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb856-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb856-106">Permission type</span></span>      | <span data-ttu-id="cb856-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb856-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb856-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb856-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cb856-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb856-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cb856-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb856-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb856-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb856-111">Not supported.</span></span>    |
|<span data-ttu-id="cb856-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb856-112">Application</span></span> | <span data-ttu-id="cb856-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb856-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb856-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb856-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="cb856-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb856-115">Request headers</span></span>
| <span data-ttu-id="cb856-116">名称</span><span class="sxs-lookup"><span data-stu-id="cb856-116">Name</span></span>       | <span data-ttu-id="cb856-117">说明</span><span class="sxs-lookup"><span data-stu-id="cb856-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb856-118">授权</span><span class="sxs-lookup"><span data-stu-id="cb856-118">Authorization</span></span>  | <span data-ttu-id="cb856-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb856-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb856-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cb856-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="cb856-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cb856-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb856-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb856-124">Request body</span></span>
<span data-ttu-id="cb856-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cb856-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb856-126">参数</span><span class="sxs-lookup"><span data-stu-id="cb856-126">Parameter</span></span>    | <span data-ttu-id="cb856-127">类型</span><span class="sxs-lookup"><span data-stu-id="cb856-127">Type</span></span>   |<span data-ttu-id="cb856-128">说明</span><span class="sxs-lookup"><span data-stu-id="cb856-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb856-129">password</span><span class="sxs-lookup"><span data-stu-id="cb856-129">password</span></span>|<span data-ttu-id="cb856-130">string</span><span class="sxs-lookup"><span data-stu-id="cb856-130">string</span></span>|<span data-ttu-id="cb856-p104">可选。工作表保护密码。</span><span class="sxs-lookup"><span data-stu-id="cb856-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="cb856-133">响应</span><span class="sxs-lookup"><span data-stu-id="cb856-133">Response</span></span>

<span data-ttu-id="cb856-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cb856-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb856-136">示例</span><span class="sxs-lookup"><span data-stu-id="cb856-136">Example</span></span>
<span data-ttu-id="cb856-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cb856-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb856-138">请求</span><span class="sxs-lookup"><span data-stu-id="cb856-138">Request</span></span>
<span data-ttu-id="cb856-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb856-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="cb856-140">响应</span><span class="sxs-lookup"><span data-stu-id="cb856-140">Response</span></span>
<span data-ttu-id="cb856-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cb856-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->