---
title: NamedItem：Range
description: 返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。
localization_priority: Normal
ms.openlocfilehash: 5d397820b216b1d067394082e8d7d8d1cf2f9406
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890273"
---
# <a name="nameditem-range"></a><span data-ttu-id="e8923-104">NamedItem：Range</span><span class="sxs-lookup"><span data-stu-id="e8923-104">NamedItem: Range</span></span>

<span data-ttu-id="e8923-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="e8923-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8923-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8923-107">Permissions</span></span>
<span data-ttu-id="e8923-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8923-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8923-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8923-110">Permission type</span></span>      | <span data-ttu-id="e8923-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8923-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8923-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8923-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8923-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8923-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8923-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8923-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8923-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8923-115">Not supported.</span></span>    |
|<span data-ttu-id="e8923-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8923-116">Application</span></span> | <span data-ttu-id="e8923-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8923-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8923-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8923-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="e8923-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8923-119">Request headers</span></span>
| <span data-ttu-id="e8923-120">名称</span><span class="sxs-lookup"><span data-stu-id="e8923-120">Name</span></span>       | <span data-ttu-id="e8923-121">说明</span><span class="sxs-lookup"><span data-stu-id="e8923-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8923-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8923-122">Authorization</span></span>  | <span data-ttu-id="e8923-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8923-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8923-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8923-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8923-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e8923-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8923-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8923-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e8923-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8923-129">Response</span></span>

<span data-ttu-id="e8923-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8923-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8923-131">示例</span><span class="sxs-lookup"><span data-stu-id="e8923-131">Example</span></span>
<span data-ttu-id="e8923-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e8923-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8923-133">请求</span><span class="sxs-lookup"><span data-stu-id="e8923-133">Request</span></span>
<span data-ttu-id="e8923-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8923-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8923-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e8923-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8923-136">C#</span><span class="sxs-lookup"><span data-stu-id="e8923-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8923-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8923-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8923-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8923-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8923-139">Java</span><span class="sxs-lookup"><span data-stu-id="e8923-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8923-140">响应</span><span class="sxs-lookup"><span data-stu-id="e8923-140">Response</span></span>
<span data-ttu-id="e8923-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8923-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
