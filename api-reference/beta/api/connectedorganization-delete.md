---
title: 删除 connectedOrganization
description: 删除 connectedOrganization。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ce2aed28aaa4d1b97767e7ebb46e9b206d32d75
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872714"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="f149a-103">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="f149a-103">Delete connectedOrganization</span></span>

<span data-ttu-id="f149a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f149a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f149a-105">删除 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f149a-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f149a-106">权限</span><span class="sxs-lookup"><span data-stu-id="f149a-106">Permissions</span></span>

<span data-ttu-id="f149a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f149a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f149a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f149a-109">Permission type</span></span>|<span data-ttu-id="f149a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f149a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="f149a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f149a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f149a-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f149a-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f149a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f149a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f149a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f149a-114">Not supported.</span></span> |
| <span data-ttu-id="f149a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f149a-115">Application</span></span>                            | <span data-ttu-id="f149a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f149a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f149a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f149a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f149a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f149a-118">Request headers</span></span>
|<span data-ttu-id="f149a-119">名称</span><span class="sxs-lookup"><span data-stu-id="f149a-119">Name</span></span>|<span data-ttu-id="f149a-120">说明</span><span class="sxs-lookup"><span data-stu-id="f149a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f149a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f149a-121">Authorization</span></span>|<span data-ttu-id="f149a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f149a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f149a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f149a-124">Request body</span></span>
<span data-ttu-id="f149a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f149a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f149a-126">响应</span><span class="sxs-lookup"><span data-stu-id="f149a-126">Response</span></span>

<span data-ttu-id="f149a-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f149a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f149a-128">示例</span><span class="sxs-lookup"><span data-stu-id="f149a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f149a-129">请求</span><span class="sxs-lookup"><span data-stu-id="f149a-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f149a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f149a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="f149a-131">C#</span><span class="sxs-lookup"><span data-stu-id="f149a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f149a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f149a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f149a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f149a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f149a-134">Java</span><span class="sxs-lookup"><span data-stu-id="f149a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f149a-135">响应</span><span class="sxs-lookup"><span data-stu-id="f149a-135">Response</span></span>
<span data-ttu-id="f149a-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f149a-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


