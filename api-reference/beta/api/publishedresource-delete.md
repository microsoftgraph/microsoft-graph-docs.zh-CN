---
title: 删除 publishedResource
description: 删除[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ad533b0b3a6f25702dd93d63be1597ac95c262f
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840987"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="2d60e-103">删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2d60e-103">Delete publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d60e-104">删除[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d60e-104">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d60e-105">权限</span><span class="sxs-lookup"><span data-stu-id="2d60e-105">Permissions</span></span>

<span data-ttu-id="2d60e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d60e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d60e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d60e-108">Permission type</span></span>                        | <span data-ttu-id="2d60e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d60e-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2d60e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d60e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d60e-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="2d60e-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2d60e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d60e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d60e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d60e-113">Not supported.</span></span> |
| <span data-ttu-id="2d60e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d60e-114">Application</span></span>                            | <span data-ttu-id="2d60e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d60e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d60e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d60e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2d60e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d60e-117">Request headers</span></span>

| <span data-ttu-id="2d60e-118">名称</span><span class="sxs-lookup"><span data-stu-id="2d60e-118">Name</span></span>          | <span data-ttu-id="2d60e-119">说明</span><span class="sxs-lookup"><span data-stu-id="2d60e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2d60e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d60e-120">Authorization</span></span> | <span data-ttu-id="2d60e-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2d60e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d60e-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d60e-122">Request body</span></span>

<span data-ttu-id="2d60e-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d60e-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d60e-124">响应</span><span class="sxs-lookup"><span data-stu-id="2d60e-124">Response</span></span>

<span data-ttu-id="2d60e-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d60e-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d60e-127">示例</span><span class="sxs-lookup"><span data-stu-id="2d60e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d60e-128">请求</span><span class="sxs-lookup"><span data-stu-id="2d60e-128">Request</span></span>

<span data-ttu-id="2d60e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d60e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```

### <a name="response"></a><span data-ttu-id="2d60e-130">响应</span><span class="sxs-lookup"><span data-stu-id="2d60e-130">Response</span></span>

<span data-ttu-id="2d60e-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d60e-131">The following is an example of the response.</span></span>

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
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
