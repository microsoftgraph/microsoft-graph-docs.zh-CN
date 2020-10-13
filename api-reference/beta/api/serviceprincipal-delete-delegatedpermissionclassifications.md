---
title: 删除 delegatedPermissionClassification
description: 从 API 的服务主体中删除委派的权限分类。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8a246fbed9b226e36429d82cfb99eee704ca754c
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433519"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="8a4b2-103">删除 delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="8a4b2-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="8a4b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a4b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a4b2-105">删除以前为委派权限设置的 [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a4b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a4b2-106">Permissions</span></span>

<span data-ttu-id="8a4b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a4b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a4b2-109">Permission type</span></span>      | <span data-ttu-id="8a4b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a4b2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a4b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a4b2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4b2-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="8a4b2-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="8a4b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a4b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4b2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-114">Not supported.</span></span>    |
|<span data-ttu-id="8a4b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a4b2-115">Application</span></span> | <span data-ttu-id="8a4b2-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="8a4b2-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a4b2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a4b2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a4b2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a4b2-118">Request headers</span></span>

| <span data-ttu-id="8a4b2-119">名称</span><span class="sxs-lookup"><span data-stu-id="8a4b2-119">Name</span></span>       | <span data-ttu-id="8a4b2-120">类型</span><span class="sxs-lookup"><span data-stu-id="8a4b2-120">Type</span></span> | <span data-ttu-id="8a4b2-121">说明</span><span class="sxs-lookup"><span data-stu-id="8a4b2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a4b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a4b2-122">Authorization</span></span>  | <span data-ttu-id="8a4b2-123">string</span><span class="sxs-lookup"><span data-stu-id="8a4b2-123">string</span></span>  | <span data-ttu-id="8a4b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a4b2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a4b2-126">Request body</span></span>

<span data-ttu-id="8a4b2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a4b2-128">响应</span><span class="sxs-lookup"><span data-stu-id="8a4b2-128">Response</span></span>

<span data-ttu-id="8a4b2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a4b2-131">示例</span><span class="sxs-lookup"><span data-stu-id="8a4b2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a4b2-132">请求</span><span class="sxs-lookup"><span data-stu-id="8a4b2-132">Request</span></span>

<span data-ttu-id="8a4b2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

### <a name="response"></a><span data-ttu-id="8a4b2-134">响应</span><span class="sxs-lookup"><span data-stu-id="8a4b2-134">Response</span></span>

<span data-ttu-id="8a4b2-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a4b2-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
