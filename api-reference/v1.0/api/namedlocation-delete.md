---
title: 删除 namedLocation
description: 删除 namedLocation 对象。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a98506992157868b1d80059697a3e4c2ae76d606
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384610"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="4fc69-103">删除 namedLocation</span><span class="sxs-lookup"><span data-stu-id="4fc69-103">Delete namedLocation</span></span>

<span data-ttu-id="4fc69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fc69-105">删除[namedLocation](../resources/namedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fc69-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fc69-106">权限</span><span class="sxs-lookup"><span data-stu-id="4fc69-106">Permissions</span></span>

<span data-ttu-id="4fc69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fc69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fc69-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fc69-109">Permission type</span></span>                        | <span data-ttu-id="4fc69-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fc69-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fc69-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fc69-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fc69-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="4fc69-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="4fc69-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fc69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fc69-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fc69-114">Not supported.</span></span> |
| <span data-ttu-id="4fc69-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fc69-115">Application</span></span>                            | <span data-ttu-id="4fc69-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="4fc69-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fc69-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fc69-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fc69-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fc69-118">Request headers</span></span>

| <span data-ttu-id="4fc69-119">名称</span><span class="sxs-lookup"><span data-stu-id="4fc69-119">Name</span></span>          | <span data-ttu-id="4fc69-120">说明</span><span class="sxs-lookup"><span data-stu-id="4fc69-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4fc69-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc69-121">Authorization</span></span> | <span data-ttu-id="4fc69-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fc69-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fc69-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fc69-124">Request body</span></span>

<span data-ttu-id="4fc69-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fc69-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fc69-126">响应</span><span class="sxs-lookup"><span data-stu-id="4fc69-126">Response</span></span>

<span data-ttu-id="4fc69-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4fc69-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fc69-129">示例</span><span class="sxs-lookup"><span data-stu-id="4fc69-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fc69-130">请求</span><span class="sxs-lookup"><span data-stu-id="4fc69-130">Request</span></span>

<span data-ttu-id="4fc69-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fc69-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="4fc69-132">响应</span><span class="sxs-lookup"><span data-stu-id="4fc69-132">Response</span></span>

<span data-ttu-id="4fc69-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4fc69-133">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
