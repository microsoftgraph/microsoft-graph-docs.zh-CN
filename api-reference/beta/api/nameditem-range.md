---
title: NamedItem：Range
description: 返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 362fc951603ffbd3dc6f6ec2283ec92fef4b1443
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052115"
---
# <a name="nameditem-range"></a><span data-ttu-id="9dced-104">NamedItem：Range</span><span class="sxs-lookup"><span data-stu-id="9dced-104">NamedItem: Range</span></span>

<span data-ttu-id="9dced-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dced-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dced-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="9dced-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="9dced-108">权限</span><span class="sxs-lookup"><span data-stu-id="9dced-108">Permissions</span></span>
<span data-ttu-id="9dced-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dced-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dced-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dced-111">Permission type</span></span>      | <span data-ttu-id="9dced-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dced-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dced-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dced-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9dced-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dced-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dced-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dced-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dced-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dced-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dced-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dced-117">Application</span></span> | <span data-ttu-id="9dced-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dced-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dced-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dced-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/Range
GET /me/drive/root:/{item-path}:/workbook/names/{name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="9dced-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dced-120">Request headers</span></span>
| <span data-ttu-id="9dced-121">名称</span><span class="sxs-lookup"><span data-stu-id="9dced-121">Name</span></span>       | <span data-ttu-id="9dced-122">说明</span><span class="sxs-lookup"><span data-stu-id="9dced-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dced-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dced-123">Authorization</span></span>  | <span data-ttu-id="9dced-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9dced-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9dced-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9dced-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="9dced-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9dced-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dced-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dced-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9dced-130">响应</span><span class="sxs-lookup"><span data-stu-id="9dced-130">Response</span></span>

<span data-ttu-id="9dced-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9dced-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dced-132">示例</span><span class="sxs-lookup"><span data-stu-id="9dced-132">Example</span></span>
<span data-ttu-id="9dced-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9dced-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9dced-134">请求</span><span class="sxs-lookup"><span data-stu-id="9dced-134">Request</span></span>
<span data-ttu-id="9dced-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dced-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9dced-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dced-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/Range
```
# <a name="c"></a>[<span data-ttu-id="9dced-137">C#</span><span class="sxs-lookup"><span data-stu-id="9dced-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dced-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dced-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dced-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dced-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dced-140">Java</span><span class="sxs-lookup"><span data-stu-id="9dced-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditem-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9dced-141">响应</span><span class="sxs-lookup"><span data-stu-id="9dced-141">Response</span></span>
<span data-ttu-id="9dced-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9dced-142">Here is an example of the response.</span></span> <span data-ttu-id="9dced-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9dced-143">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


