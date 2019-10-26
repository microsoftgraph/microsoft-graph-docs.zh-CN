---
title: 删除 userFlow
description: 删除 userFlow。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 174cc8324b58c3a4deb627cd6f40bcbbab31f6a3
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734545"
---
# <a name="delete-userflow"></a><span data-ttu-id="b7e28-103">删除 userFlow</span><span class="sxs-lookup"><span data-stu-id="b7e28-103">Delete userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7e28-104">删除现有的[userFlow](../resources/identityuserflow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7e28-104">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7e28-105">权限</span><span class="sxs-lookup"><span data-stu-id="b7e28-105">Permissions</span></span>

<span data-ttu-id="b7e28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7e28-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7e28-108">Permission type</span></span>                        | <span data-ttu-id="b7e28-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7e28-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7e28-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e28-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7e28-111">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="b7e28-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="b7e28-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e28-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7e28-113">Not supported.</span></span> |
| <span data-ttu-id="b7e28-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7e28-114">Application</span></span>                            | <span data-ttu-id="b7e28-115">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="b7e28-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e28-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7e28-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b7e28-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7e28-117">Request headers</span></span>

| <span data-ttu-id="b7e28-118">名称</span><span class="sxs-lookup"><span data-stu-id="b7e28-118">Name</span></span>          | <span data-ttu-id="b7e28-119">说明</span><span class="sxs-lookup"><span data-stu-id="b7e28-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b7e28-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7e28-120">Authorization</span></span> | <span data-ttu-id="b7e28-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7e28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7e28-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7e28-123">Request body</span></span>

<span data-ttu-id="b7e28-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7e28-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7e28-125">响应</span><span class="sxs-lookup"><span data-stu-id="b7e28-125">Response</span></span>

<span data-ttu-id="b7e28-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b7e28-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7e28-128">示例</span><span class="sxs-lookup"><span data-stu-id="b7e28-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7e28-129">请求</span><span class="sxs-lookup"><span data-stu-id="b7e28-129">Request</span></span>

<span data-ttu-id="b7e28-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7e28-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```

### <a name="response"></a><span data-ttu-id="b7e28-131">响应</span><span class="sxs-lookup"><span data-stu-id="b7e28-131">Response</span></span>

<span data-ttu-id="b7e28-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7e28-132">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->