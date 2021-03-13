---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: b9b441be1d3b8af2b79a4a71425059d90ba3cc37
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768912"
---
# <a name="delete-agreement"></a><span data-ttu-id="0337a-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="0337a-103">Delete agreement</span></span>

<span data-ttu-id="0337a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0337a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0337a-105">删除 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0337a-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0337a-106">权限</span><span class="sxs-lookup"><span data-stu-id="0337a-106">Permissions</span></span>
<span data-ttu-id="0337a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0337a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0337a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0337a-109">Permission type</span></span>                        | <span data-ttu-id="0337a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0337a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0337a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0337a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0337a-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0337a-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="0337a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0337a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0337a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0337a-114">Not supported.</span></span> |
|<span data-ttu-id="0337a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0337a-115">Application</span></span>                            | <span data-ttu-id="0337a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0337a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0337a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0337a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0337a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0337a-118">Request headers</span></span>
| <span data-ttu-id="0337a-119">名称</span><span class="sxs-lookup"><span data-stu-id="0337a-119">Name</span></span>         | <span data-ttu-id="0337a-120">类型</span><span class="sxs-lookup"><span data-stu-id="0337a-120">Type</span></span>        | <span data-ttu-id="0337a-121">说明</span><span class="sxs-lookup"><span data-stu-id="0337a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0337a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0337a-122">Authorization</span></span> | <span data-ttu-id="0337a-123">string</span><span class="sxs-lookup"><span data-stu-id="0337a-123">string</span></span> | <span data-ttu-id="0337a-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="0337a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0337a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0337a-126">Request body</span></span>
<span data-ttu-id="0337a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0337a-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0337a-128">响应</span><span class="sxs-lookup"><span data-stu-id="0337a-128">Response</span></span>
<span data-ttu-id="0337a-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0337a-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0337a-131">示例</span><span class="sxs-lookup"><span data-stu-id="0337a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0337a-132">请求</span><span class="sxs-lookup"><span data-stu-id="0337a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0337a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0337a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
```
# <a name="c"></a>[<span data-ttu-id="0337a-134">C#</span><span class="sxs-lookup"><span data-stu-id="0337a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0337a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0337a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0337a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0337a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0337a-137">Java</span><span class="sxs-lookup"><span data-stu-id="0337a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0337a-138">响应</span><span class="sxs-lookup"><span data-stu-id="0337a-138">Response</span></span>
><span data-ttu-id="0337a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0337a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


