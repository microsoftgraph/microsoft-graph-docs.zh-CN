---
title: 删除 accessPackage
description: 删除 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b48b132bc12bd35b248be0efe33b038fcd884a35
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176400"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="bc5a2-103">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="bc5a2-103">Delete accessPackage</span></span>

<span data-ttu-id="bc5a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc5a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5a2-105">删除 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="bc5a2-106">Permissions</span></span>

<span data-ttu-id="bc5a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc5a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc5a2-109">Permission type</span></span>                        | <span data-ttu-id="bc5a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc5a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bc5a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc5a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc5a2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc5a2-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="bc5a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc5a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-114">Not supported.</span></span> |
| <span data-ttu-id="bc5a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc5a2-115">Application</span></span>                            | <span data-ttu-id="bc5a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc5a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc5a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc5a2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc5a2-118">Request headers</span></span>

| <span data-ttu-id="bc5a2-119">名称</span><span class="sxs-lookup"><span data-stu-id="bc5a2-119">Name</span></span>          | <span data-ttu-id="bc5a2-120">说明</span><span class="sxs-lookup"><span data-stu-id="bc5a2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bc5a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc5a2-121">Authorization</span></span> | <span data-ttu-id="bc5a2-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-122">Bearer \{token\}.</span></span> <span data-ttu-id="bc5a2-123">必需。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc5a2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc5a2-124">Request body</span></span>

<span data-ttu-id="bc5a2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc5a2-126">响应</span><span class="sxs-lookup"><span data-stu-id="bc5a2-126">Response</span></span>

<span data-ttu-id="bc5a2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc5a2-129">示例</span><span class="sxs-lookup"><span data-stu-id="bc5a2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc5a2-130">请求</span><span class="sxs-lookup"><span data-stu-id="bc5a2-130">Request</span></span>

<span data-ttu-id="bc5a2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc5a2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5a2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="bc5a2-133">C#</span><span class="sxs-lookup"><span data-stu-id="bc5a2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc5a2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc5a2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc5a2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc5a2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc5a2-136">Java</span><span class="sxs-lookup"><span data-stu-id="bc5a2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc5a2-137">响应</span><span class="sxs-lookup"><span data-stu-id="bc5a2-137">Response</span></span>

<span data-ttu-id="bc5a2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc5a2-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


