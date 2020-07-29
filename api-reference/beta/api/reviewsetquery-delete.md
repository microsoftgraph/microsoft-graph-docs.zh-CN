---
title: 删除 reviewSetQuery
description: 删除 reviewSetQuery 对象。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8b400863cd9cbe6892f84f4c58d6b3ab738ddcb4
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510016"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="ed709-103">删除 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ed709-103">Delete reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed709-104">删除[reviewSetQuery](../resources/reviewsetquery.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed709-104">Delete a [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed709-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed709-105">Permissions</span></span>

<span data-ttu-id="ed709-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed709-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed709-108">Permission type</span></span>                        | <span data-ttu-id="ed709-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed709-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed709-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed709-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed709-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="ed709-111">User.Read</span></span> |
| <span data-ttu-id="ed709-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed709-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed709-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed709-113">Not supported.</span></span> |
| <span data-ttu-id="ed709-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed709-114">Application</span></span>                            | <span data-ttu-id="ed709-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed709-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed709-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed709-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed709-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed709-117">Request headers</span></span>

| <span data-ttu-id="ed709-118">名称</span><span class="sxs-lookup"><span data-stu-id="ed709-118">Name</span></span>          | <span data-ttu-id="ed709-119">说明</span><span class="sxs-lookup"><span data-stu-id="ed709-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed709-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed709-120">Authorization</span></span> | <span data-ttu-id="ed709-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed709-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed709-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed709-123">Request body</span></span>

<span data-ttu-id="ed709-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed709-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed709-125">响应</span><span class="sxs-lookup"><span data-stu-id="ed709-125">Response</span></span>

<span data-ttu-id="ed709-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ed709-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed709-128">示例</span><span class="sxs-lookup"><span data-stu-id="ed709-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed709-129">请求</span><span class="sxs-lookup"><span data-stu-id="ed709-129">Request</span></span>

<span data-ttu-id="ed709-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed709-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```

### <a name="response"></a><span data-ttu-id="ed709-131">响应</span><span class="sxs-lookup"><span data-stu-id="ed709-131">Response</span></span>

<span data-ttu-id="ed709-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed709-132">The following is an example of the response.</span></span>

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
  "description": "Delete reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
