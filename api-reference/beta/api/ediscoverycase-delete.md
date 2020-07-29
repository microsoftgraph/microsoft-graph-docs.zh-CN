---
title: 删除 ediscoveryCase
description: 删除 ediscoveryCase 对象。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c1ef35c31bb349c2e4ea8622d2f18f90ed6e0b83
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509990"
---
# <a name="delete-ediscoverycase"></a><span data-ttu-id="eb379-103">删除 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="eb379-103">Delete ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb379-104">删除[ediscoveryCase](../resources/ediscoverycase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb379-104">Delete an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb379-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb379-105">Permissions</span></span>

<span data-ttu-id="eb379-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb379-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb379-108">Permission type</span></span>                        | <span data-ttu-id="eb379-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb379-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb379-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb379-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb379-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="eb379-111">User.Read</span></span>      |
| <span data-ttu-id="eb379-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb379-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb379-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb379-113">Not supported.</span></span> |
| <span data-ttu-id="eb379-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb379-114">Application</span></span>                            | <span data-ttu-id="eb379-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb379-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb379-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb379-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb379-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb379-117">Request headers</span></span>

| <span data-ttu-id="eb379-118">名称</span><span class="sxs-lookup"><span data-stu-id="eb379-118">Name</span></span>          | <span data-ttu-id="eb379-119">说明</span><span class="sxs-lookup"><span data-stu-id="eb379-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eb379-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb379-120">Authorization</span></span> | <span data-ttu-id="eb379-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb379-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb379-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb379-123">Request body</span></span>

<span data-ttu-id="eb379-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb379-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb379-125">响应</span><span class="sxs-lookup"><span data-stu-id="eb379-125">Response</span></span>

<span data-ttu-id="eb379-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb379-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb379-128">示例</span><span class="sxs-lookup"><span data-stu-id="eb379-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb379-129">请求</span><span class="sxs-lookup"><span data-stu-id="eb379-129">Request</span></span>

<span data-ttu-id="eb379-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb379-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_ediscoverycase"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="eb379-131">响应</span><span class="sxs-lookup"><span data-stu-id="eb379-131">Response</span></span>

<span data-ttu-id="eb379-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb379-132">The following is an example of the response.</span></span>

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
  "description": "Delete ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
