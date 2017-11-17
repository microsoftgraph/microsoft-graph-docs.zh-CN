# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="6a0b7-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="6a0b7-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="6a0b7-102">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="6a0b7-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="6a0b7-103">权限</span><span class="sxs-lookup"><span data-stu-id="6a0b7-103">Permissions</span></span>
<span data-ttu-id="6a0b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a0b7-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a0b7-106">Permission type</span></span>      | <span data-ttu-id="6a0b7-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a0b7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a0b7-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a0b7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6a0b7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a0b7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a0b7-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a0b7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a0b7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-111">Not supported.</span></span>    |
|<span data-ttu-id="6a0b7-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a0b7-112">Application</span></span> | <span data-ttu-id="6a0b7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a0b7-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a0b7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="6a0b7-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a0b7-115">Request headers</span></span>
| <span data-ttu-id="6a0b7-116">名称</span><span class="sxs-lookup"><span data-stu-id="6a0b7-116">Name</span></span>       | <span data-ttu-id="6a0b7-117">说明</span><span class="sxs-lookup"><span data-stu-id="6a0b7-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a0b7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a0b7-118">Authorization</span></span>  | <span data-ttu-id="6a0b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a0b7-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a0b7-121">Request body</span></span>
<span data-ttu-id="6a0b7-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a0b7-123">参数</span><span class="sxs-lookup"><span data-stu-id="6a0b7-123">Parameter</span></span>    | <span data-ttu-id="6a0b7-124">类型</span><span class="sxs-lookup"><span data-stu-id="6a0b7-124">Type</span></span>   |<span data-ttu-id="6a0b7-125">说明</span><span class="sxs-lookup"><span data-stu-id="6a0b7-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a0b7-126">password</span><span class="sxs-lookup"><span data-stu-id="6a0b7-126">password</span></span>|<span data-ttu-id="6a0b7-127">string</span><span class="sxs-lookup"><span data-stu-id="6a0b7-127">string</span></span>|<span data-ttu-id="6a0b7-p103">可选。工作表保护密码。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-p103">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="6a0b7-130">响应</span><span class="sxs-lookup"><span data-stu-id="6a0b7-130">Response</span></span>

<span data-ttu-id="6a0b7-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a0b7-133">示例</span><span class="sxs-lookup"><span data-stu-id="6a0b7-133">Example</span></span>
<span data-ttu-id="6a0b7-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6a0b7-135">请求</span><span class="sxs-lookup"><span data-stu-id="6a0b7-135">Request</span></span>
<span data-ttu-id="6a0b7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6a0b7-137">响应</span><span class="sxs-lookup"><span data-stu-id="6a0b7-137">Response</span></span>
<span data-ttu-id="6a0b7-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a0b7-138">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->