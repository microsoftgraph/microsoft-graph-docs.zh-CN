---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f44523533b40212a7735dc8ecbe70a7ec12666b4
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154057"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="61c3e-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61c3e-103">Delete workforceIntegration</span></span>

<span data-ttu-id="61c3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61c3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61c3e-105">删除[workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="61c3e-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61c3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="61c3e-106">Permissions</span></span>

<span data-ttu-id="61c3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61c3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="61c3e-109">Permission type</span></span>                        | <span data-ttu-id="61c3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61c3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61c3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61c3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="61c3e-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61c3e-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="61c3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61c3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61c3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="61c3e-114">Not supported.</span></span> |
| <span data-ttu-id="61c3e-115">Application</span><span class="sxs-lookup"><span data-stu-id="61c3e-115">Application</span></span>                            | <span data-ttu-id="61c3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="61c3e-116">Not supported.</span></span> |

> <span data-ttu-id="61c3e-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="61c3e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="61c3e-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="61c3e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="61c3e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61c3e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="61c3e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="61c3e-120">Request headers</span></span>

| <span data-ttu-id="61c3e-121">名称</span><span class="sxs-lookup"><span data-stu-id="61c3e-121">Name</span></span>          | <span data-ttu-id="61c3e-122">说明</span><span class="sxs-lookup"><span data-stu-id="61c3e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="61c3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61c3e-123">Authorization</span></span> | <span data-ttu-id="61c3e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61c3e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61c3e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61c3e-126">Request body</span></span>

<span data-ttu-id="61c3e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61c3e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61c3e-128">响应</span><span class="sxs-lookup"><span data-stu-id="61c3e-128">Response</span></span>

<span data-ttu-id="61c3e-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="61c3e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61c3e-131">示例</span><span class="sxs-lookup"><span data-stu-id="61c3e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61c3e-132">请求</span><span class="sxs-lookup"><span data-stu-id="61c3e-132">Request</span></span>

<span data-ttu-id="61c3e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61c3e-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```

---


### <a name="response"></a><span data-ttu-id="61c3e-134">响应</span><span class="sxs-lookup"><span data-stu-id="61c3e-134">Response</span></span>

<span data-ttu-id="61c3e-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61c3e-135">The following is an example of the response.</span></span>

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
