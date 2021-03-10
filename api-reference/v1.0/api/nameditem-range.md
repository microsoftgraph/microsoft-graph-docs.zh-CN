---
title: NamedItem：Range
description: 返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d2515f3ff07bc81bf782a5197ceda87df9feb85b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577301"
---
# <a name="nameditem-range"></a><span data-ttu-id="18fe8-104">NamedItem：Range</span><span class="sxs-lookup"><span data-stu-id="18fe8-104">NamedItem: Range</span></span>

<span data-ttu-id="18fe8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18fe8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18fe8-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="18fe8-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="18fe8-108">权限</span><span class="sxs-lookup"><span data-stu-id="18fe8-108">Permissions</span></span>
<span data-ttu-id="18fe8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18fe8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18fe8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18fe8-111">Permission type</span></span>      | <span data-ttu-id="18fe8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18fe8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18fe8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18fe8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18fe8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18fe8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18fe8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18fe8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18fe8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fe8-116">Not supported.</span></span>    |
|<span data-ttu-id="18fe8-117">Application</span><span class="sxs-lookup"><span data-stu-id="18fe8-117">Application</span></span> | <span data-ttu-id="18fe8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="18fe8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18fe8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18fe8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="18fe8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18fe8-120">Request headers</span></span>
| <span data-ttu-id="18fe8-121">名称</span><span class="sxs-lookup"><span data-stu-id="18fe8-121">Name</span></span>       | <span data-ttu-id="18fe8-122">说明</span><span class="sxs-lookup"><span data-stu-id="18fe8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18fe8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18fe8-123">Authorization</span></span>  | <span data-ttu-id="18fe8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18fe8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18fe8-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="18fe8-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="18fe8-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="18fe8-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18fe8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="18fe8-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="18fe8-130">响应</span><span class="sxs-lookup"><span data-stu-id="18fe8-130">Response</span></span>

<span data-ttu-id="18fe8-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18fe8-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18fe8-132">示例</span><span class="sxs-lookup"><span data-stu-id="18fe8-132">Example</span></span>
<span data-ttu-id="18fe8-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="18fe8-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18fe8-134">请求</span><span class="sxs-lookup"><span data-stu-id="18fe8-134">Request</span></span>
<span data-ttu-id="18fe8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18fe8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18fe8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="18fe8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="18fe8-137">C#</span><span class="sxs-lookup"><span data-stu-id="18fe8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18fe8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18fe8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18fe8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18fe8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18fe8-140">Java</span><span class="sxs-lookup"><span data-stu-id="18fe8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18fe8-141">响应</span><span class="sxs-lookup"><span data-stu-id="18fe8-141">Response</span></span>
<span data-ttu-id="18fe8-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18fe8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

