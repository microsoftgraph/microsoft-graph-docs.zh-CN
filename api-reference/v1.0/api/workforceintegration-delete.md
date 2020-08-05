---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3c3b0c33c617ba03b56a53e1ebb4be9c51bcaa2
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/04/2020
ms.locfileid: "44217283"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="6558a-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="6558a-103">Delete workforceIntegration</span></span>

<span data-ttu-id="6558a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6558a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6558a-105">删除[workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="6558a-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6558a-106">权限</span><span class="sxs-lookup"><span data-stu-id="6558a-106">Permissions</span></span>

<span data-ttu-id="6558a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6558a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6558a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6558a-109">Permission type</span></span>                        | <span data-ttu-id="6558a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6558a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6558a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6558a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6558a-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="6558a-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="6558a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6558a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6558a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6558a-114">Not supported.</span></span> |
| <span data-ttu-id="6558a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6558a-115">Application</span></span>                            | <span data-ttu-id="6558a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6558a-116">Not supported.</span></span> |

> <span data-ttu-id="6558a-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6558a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6558a-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="6558a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6558a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6558a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="6558a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6558a-120">Request headers</span></span>

| <span data-ttu-id="6558a-121">名称</span><span class="sxs-lookup"><span data-stu-id="6558a-121">Name</span></span>          | <span data-ttu-id="6558a-122">说明</span><span class="sxs-lookup"><span data-stu-id="6558a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6558a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6558a-123">Authorization</span></span> | <span data-ttu-id="6558a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6558a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6558a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6558a-126">Request body</span></span>

<span data-ttu-id="6558a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6558a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6558a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6558a-128">Response</span></span>

<span data-ttu-id="6558a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6558a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6558a-131">示例</span><span class="sxs-lookup"><span data-stu-id="6558a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6558a-132">请求</span><span class="sxs-lookup"><span data-stu-id="6558a-132">Request</span></span>

<span data-ttu-id="6558a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6558a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6558a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6558a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="6558a-135">C#</span><span class="sxs-lookup"><span data-stu-id="6558a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6558a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6558a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6558a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6558a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6558a-138">Java</span><span class="sxs-lookup"><span data-stu-id="6558a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="6558a-139">响应</span><span class="sxs-lookup"><span data-stu-id="6558a-139">Response</span></span>

<span data-ttu-id="6558a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6558a-140">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
