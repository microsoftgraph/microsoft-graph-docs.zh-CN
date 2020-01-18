---
title: 删除 tokenLifetimePolicy
description: 从应用程序或 servicePrincipal 中删除 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 055da6eb449c8600e39755f4725ce72af35af045
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234139"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="addc0-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="addc0-103">Remove tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="addc0-104">从[应用程序](../resources/application.md)或[ServicePrincipal](../resources/servicePrincipal.md)中删除[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="addc0-104">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="addc0-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="addc0-105">Permissions</span></span>

<span data-ttu-id="addc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="addc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="addc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="addc0-108">Permission type</span></span>                        | <span data-ttu-id="addc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="addc0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="addc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="addc0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="addc0-111">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="addc0-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="addc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="addc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="addc0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="addc0-113">Not supported.</span></span> |
| <span data-ttu-id="addc0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="addc0-114">Application</span></span>                            | <span data-ttu-id="addc0-115">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="addc0-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="addc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="addc0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="addc0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="addc0-117">Request headers</span></span>

| <span data-ttu-id="addc0-118">名称</span><span class="sxs-lookup"><span data-stu-id="addc0-118">Name</span></span>          | <span data-ttu-id="addc0-119">说明</span><span class="sxs-lookup"><span data-stu-id="addc0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="addc0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="addc0-120">Authorization</span></span> | <span data-ttu-id="addc0-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="addc0-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="addc0-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="addc0-122">Request body</span></span>

<span data-ttu-id="addc0-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="addc0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="addc0-124">响应</span><span class="sxs-lookup"><span data-stu-id="addc0-124">Response</span></span>

<span data-ttu-id="addc0-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="addc0-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="addc0-126">示例</span><span class="sxs-lookup"><span data-stu-id="addc0-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="addc0-127">请求</span><span class="sxs-lookup"><span data-stu-id="addc0-127">Request</span></span>

<span data-ttu-id="addc0-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="addc0-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="addc0-129">响应</span><span class="sxs-lookup"><span data-stu-id="addc0-129">Response</span></span>

<span data-ttu-id="addc0-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="addc0-130">The following is an example of the response.</span></span>

> <span data-ttu-id="addc0-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="addc0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->