---
title: 删除 tokenLifetimePolicy
description: 从应用程序或 servicePrincipal 中删除 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d914f4878e0db8113e4e1a85e780f9feb42243e
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562617"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="306e2-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="306e2-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="306e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="306e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="306e2-105">从[应用程序](../resources/application.md)或[ServicePrincipal](../resources/servicePrincipal.md)中删除[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="306e2-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="306e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="306e2-106">Permissions</span></span>

<span data-ttu-id="306e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="306e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="306e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="306e2-109">Permission type</span></span>                        | <span data-ttu-id="306e2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="306e2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="306e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="306e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="306e2-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="306e2-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="306e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="306e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="306e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="306e2-114">Not supported.</span></span> |
| <span data-ttu-id="306e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="306e2-115">Application</span></span>                            | <span data-ttu-id="306e2-116">Application.readwrite.ownedby 和 ApplicationConfiguration 和 Application.readwrite.ownedby、、ApplicationConfiguration 和中的所有应用程序的、、、、和中的应用程序的读写。</span><span class="sxs-lookup"><span data-stu-id="306e2-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="306e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="306e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="306e2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="306e2-118">Request headers</span></span>

| <span data-ttu-id="306e2-119">名称</span><span class="sxs-lookup"><span data-stu-id="306e2-119">Name</span></span>          | <span data-ttu-id="306e2-120">说明</span><span class="sxs-lookup"><span data-stu-id="306e2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="306e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="306e2-121">Authorization</span></span> | <span data-ttu-id="306e2-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="306e2-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="306e2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="306e2-123">Request body</span></span>

<span data-ttu-id="306e2-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="306e2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="306e2-125">响应</span><span class="sxs-lookup"><span data-stu-id="306e2-125">Response</span></span>

<span data-ttu-id="306e2-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="306e2-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="306e2-127">示例</span><span class="sxs-lookup"><span data-stu-id="306e2-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="306e2-128">请求</span><span class="sxs-lookup"><span data-stu-id="306e2-128">Request</span></span>

<span data-ttu-id="306e2-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="306e2-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="306e2-130">响应</span><span class="sxs-lookup"><span data-stu-id="306e2-130">Response</span></span>

<span data-ttu-id="306e2-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="306e2-131">The following is an example of the response.</span></span>

> <span data-ttu-id="306e2-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="306e2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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