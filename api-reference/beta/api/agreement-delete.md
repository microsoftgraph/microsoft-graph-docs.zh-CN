---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: e954c23f6fb44b6258f468808370dc73a4af440c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962484"
---
# <a name="delete-agreement"></a><span data-ttu-id="430c1-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="430c1-103">Delete agreement</span></span>

<span data-ttu-id="430c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="430c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430c1-105">删除 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="430c1-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="430c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="430c1-106">Permissions</span></span>
<span data-ttu-id="430c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="430c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="430c1-109">Permission type</span></span>                        | <span data-ttu-id="430c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="430c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="430c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="430c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="430c1-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430c1-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="430c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="430c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="430c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="430c1-114">Not supported.</span></span> |
|<span data-ttu-id="430c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="430c1-115">Application</span></span>                            | <span data-ttu-id="430c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="430c1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="430c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="430c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="430c1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="430c1-118">Request headers</span></span>
| <span data-ttu-id="430c1-119">名称</span><span class="sxs-lookup"><span data-stu-id="430c1-119">Name</span></span>         | <span data-ttu-id="430c1-120">类型</span><span class="sxs-lookup"><span data-stu-id="430c1-120">Type</span></span>        | <span data-ttu-id="430c1-121">说明</span><span class="sxs-lookup"><span data-stu-id="430c1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="430c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="430c1-122">Authorization</span></span> | <span data-ttu-id="430c1-123">string</span><span class="sxs-lookup"><span data-stu-id="430c1-123">string</span></span> | <span data-ttu-id="430c1-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="430c1-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="430c1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="430c1-126">Request body</span></span>
<span data-ttu-id="430c1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="430c1-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="430c1-128">响应</span><span class="sxs-lookup"><span data-stu-id="430c1-128">Response</span></span>
<span data-ttu-id="430c1-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="430c1-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430c1-131">示例</span><span class="sxs-lookup"><span data-stu-id="430c1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="430c1-132">请求</span><span class="sxs-lookup"><span data-stu-id="430c1-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="430c1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="430c1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="430c1-134">C#</span><span class="sxs-lookup"><span data-stu-id="430c1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="430c1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="430c1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="430c1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="430c1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="430c1-137">Java</span><span class="sxs-lookup"><span data-stu-id="430c1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="430c1-138">响应</span><span class="sxs-lookup"><span data-stu-id="430c1-138">Response</span></span>
><span data-ttu-id="430c1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="430c1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


