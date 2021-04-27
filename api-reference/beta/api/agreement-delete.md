---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0e997d3b720ee56e756e067c2e181f909f7dd539
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048223"
---
# <a name="delete-agreement"></a><span data-ttu-id="7f839-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="7f839-103">Delete agreement</span></span>

<span data-ttu-id="7f839-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f839-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f839-105">删除 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f839-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f839-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f839-106">Permissions</span></span>
<span data-ttu-id="7f839-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f839-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f839-109">Permission type</span></span>                        | <span data-ttu-id="7f839-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f839-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f839-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f839-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f839-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f839-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="7f839-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f839-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f839-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f839-114">Not supported.</span></span> |
|<span data-ttu-id="7f839-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f839-115">Application</span></span>                            | <span data-ttu-id="7f839-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f839-116">Not supported.</span></span> |

<span data-ttu-id="7f839-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="7f839-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="7f839-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="7f839-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="7f839-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7f839-119">Global Administrator</span></span>
+ <span data-ttu-id="7f839-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="7f839-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="7f839-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="7f839-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7f839-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f839-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f839-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f839-123">Request headers</span></span>
| <span data-ttu-id="7f839-124">名称</span><span class="sxs-lookup"><span data-stu-id="7f839-124">Name</span></span>         | <span data-ttu-id="7f839-125">类型</span><span class="sxs-lookup"><span data-stu-id="7f839-125">Type</span></span>        | <span data-ttu-id="7f839-126">说明</span><span class="sxs-lookup"><span data-stu-id="7f839-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7f839-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f839-127">Authorization</span></span> | <span data-ttu-id="7f839-128">string</span><span class="sxs-lookup"><span data-stu-id="7f839-128">string</span></span> | <span data-ttu-id="7f839-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f839-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f839-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f839-131">Request body</span></span>
<span data-ttu-id="7f839-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f839-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7f839-133">响应</span><span class="sxs-lookup"><span data-stu-id="7f839-133">Response</span></span>
<span data-ttu-id="7f839-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7f839-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f839-136">示例</span><span class="sxs-lookup"><span data-stu-id="7f839-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f839-137">请求</span><span class="sxs-lookup"><span data-stu-id="7f839-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f839-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f839-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="7f839-139">C#</span><span class="sxs-lookup"><span data-stu-id="7f839-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f839-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f839-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f839-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f839-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f839-142">Java</span><span class="sxs-lookup"><span data-stu-id="7f839-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f839-143">响应</span><span class="sxs-lookup"><span data-stu-id="7f839-143">Response</span></span>
><span data-ttu-id="7f839-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7f839-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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


