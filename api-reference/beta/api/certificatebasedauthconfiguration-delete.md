---
title: 删除 certificateBasedAuthConfiguration
description: 删除 certificateBasedAuthConfiguration。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c9fc5a1bcc524551fd83efe54ab5dabf9bfc943
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667620"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="dcf0f-103">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcf0f-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf0f-104">删除[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf0f-105">权限</span><span class="sxs-lookup"><span data-stu-id="dcf0f-105">Permissions</span></span>

<span data-ttu-id="dcf0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcf0f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcf0f-108">Permission type</span></span>                        | <span data-ttu-id="dcf0f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcf0f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcf0f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf0f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcf0f-111">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="dcf0f-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="dcf0f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcf0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf0f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-113">Not supported.</span></span> |
| <span data-ttu-id="dcf0f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcf0f-114">Application</span></span>    | <span data-ttu-id="dcf0f-115">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="dcf0f-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf0f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcf0f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dcf0f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcf0f-117">Request headers</span></span>

| <span data-ttu-id="dcf0f-118">名称</span><span class="sxs-lookup"><span data-stu-id="dcf0f-118">Name</span></span>          | <span data-ttu-id="dcf0f-119">说明</span><span class="sxs-lookup"><span data-stu-id="dcf0f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dcf0f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf0f-120">Authorization</span></span> | <span data-ttu-id="dcf0f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dcf0f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf0f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcf0f-122">Request body</span></span>

<span data-ttu-id="dcf0f-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf0f-124">响应</span><span class="sxs-lookup"><span data-stu-id="dcf0f-124">Response</span></span>

<span data-ttu-id="dcf0f-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcf0f-127">示例</span><span class="sxs-lookup"><span data-stu-id="dcf0f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcf0f-128">请求</span><span class="sxs-lookup"><span data-stu-id="dcf0f-128">Request</span></span>

<span data-ttu-id="dcf0f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```

### <a name="response"></a><span data-ttu-id="dcf0f-130">响应</span><span class="sxs-lookup"><span data-stu-id="dcf0f-130">Response</span></span>

<span data-ttu-id="dcf0f-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dcf0f-131">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
