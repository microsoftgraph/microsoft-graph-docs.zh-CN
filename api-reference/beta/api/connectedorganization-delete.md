---
title: 删除 connectedOrganization
description: 删除 connectedOrganization。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a14207407d3810e53a1b6be871060e8e6f609c8c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437504"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="e5b71-103">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e5b71-103">Delete connectedOrganization</span></span>

<span data-ttu-id="e5b71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b71-105">删除 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5b71-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5b71-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e5b71-106">Permissions</span></span>

<span data-ttu-id="e5b71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5b71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b71-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5b71-109">Permission type</span></span>|<span data-ttu-id="e5b71-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5b71-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="e5b71-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5b71-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b71-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e5b71-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5b71-114">Not supported.</span></span> |
| <span data-ttu-id="e5b71-115">Application</span><span class="sxs-lookup"><span data-stu-id="e5b71-115">Application</span></span>                            | <span data-ttu-id="e5b71-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b71-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5b71-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5b71-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e5b71-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5b71-118">Request headers</span></span>
|<span data-ttu-id="e5b71-119">名称</span><span class="sxs-lookup"><span data-stu-id="e5b71-119">Name</span></span>|<span data-ttu-id="e5b71-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5b71-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5b71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b71-121">Authorization</span></span>|<span data-ttu-id="e5b71-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5b71-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b71-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5b71-124">Request body</span></span>
<span data-ttu-id="e5b71-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5b71-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b71-126">响应</span><span class="sxs-lookup"><span data-stu-id="e5b71-126">Response</span></span>

<span data-ttu-id="e5b71-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e5b71-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5b71-128">示例</span><span class="sxs-lookup"><span data-stu-id="e5b71-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5b71-129">请求</span><span class="sxs-lookup"><span data-stu-id="e5b71-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e5b71-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b71-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="e5b71-131">C#</span><span class="sxs-lookup"><span data-stu-id="e5b71-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5b71-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5b71-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5b71-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5b71-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5b71-134">Java</span><span class="sxs-lookup"><span data-stu-id="e5b71-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e5b71-135">响应</span><span class="sxs-lookup"><span data-stu-id="e5b71-135">Response</span></span>
<span data-ttu-id="e5b71-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5b71-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


