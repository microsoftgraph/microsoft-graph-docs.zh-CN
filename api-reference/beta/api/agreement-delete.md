---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 252a7a798e689d74e6cccacb3e2c66fd4b4cf1ef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318928"
---
# <a name="delete-agreement"></a><span data-ttu-id="86ae3-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="86ae3-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86ae3-104">删除[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86ae3-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86ae3-105">权限</span><span class="sxs-lookup"><span data-stu-id="86ae3-105">Permissions</span></span>
<span data-ttu-id="86ae3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86ae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ae3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="86ae3-108">Permission type</span></span>                        | <span data-ttu-id="86ae3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86ae3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ae3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86ae3-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ae3-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="86ae3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ae3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="86ae3-113">Not supported.</span></span> |
|<span data-ttu-id="86ae3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="86ae3-114">Application</span></span>                            | <span data-ttu-id="86ae3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86ae3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86ae3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86ae3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="86ae3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="86ae3-117">Request headers</span></span>
| <span data-ttu-id="86ae3-118">名称</span><span class="sxs-lookup"><span data-stu-id="86ae3-118">Name</span></span>         | <span data-ttu-id="86ae3-119">类型</span><span class="sxs-lookup"><span data-stu-id="86ae3-119">Type</span></span>        | <span data-ttu-id="86ae3-120">说明</span><span class="sxs-lookup"><span data-stu-id="86ae3-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="86ae3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ae3-121">Authorization</span></span> | <span data-ttu-id="86ae3-122">string</span><span class="sxs-lookup"><span data-stu-id="86ae3-122">string</span></span> | <span data-ttu-id="86ae3-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="86ae3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86ae3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="86ae3-125">Request body</span></span>
<span data-ttu-id="86ae3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86ae3-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="86ae3-127">响应</span><span class="sxs-lookup"><span data-stu-id="86ae3-127">Response</span></span>
<span data-ttu-id="86ae3-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="86ae3-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ae3-130">示例</span><span class="sxs-lookup"><span data-stu-id="86ae3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86ae3-131">请求</span><span class="sxs-lookup"><span data-stu-id="86ae3-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86ae3-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="86ae3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86ae3-133">C#</span><span class="sxs-lookup"><span data-stu-id="86ae3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86ae3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86ae3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86ae3-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="86ae3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86ae3-136">Java</span><span class="sxs-lookup"><span data-stu-id="86ae3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86ae3-137">响应</span><span class="sxs-lookup"><span data-stu-id="86ae3-137">Response</span></span>
><span data-ttu-id="86ae3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86ae3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
