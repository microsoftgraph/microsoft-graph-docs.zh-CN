---
title: 删除 certificateBasedAuthConfiguration
description: 删除 certificateBasedAuthConfiguration。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8bab6d42550e009897db42a2556e687059330000
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539237"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="fa2c1-103">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa2c1-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="fa2c1-104">删除[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa2c1-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa2c1-105">Permissions</span></span>

<span data-ttu-id="fa2c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa2c1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa2c1-108">Permission type</span></span>                        | <span data-ttu-id="fa2c1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa2c1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa2c1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa2c1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa2c1-111">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="fa2c1-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="fa2c1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa2c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa2c1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-113">Not supported.</span></span> |
| <span data-ttu-id="fa2c1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa2c1-114">Application</span></span>    | <span data-ttu-id="fa2c1-115">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="fa2c1-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa2c1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa2c1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa2c1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa2c1-117">Request headers</span></span>

| <span data-ttu-id="fa2c1-118">名称</span><span class="sxs-lookup"><span data-stu-id="fa2c1-118">Name</span></span>          | <span data-ttu-id="fa2c1-119">说明</span><span class="sxs-lookup"><span data-stu-id="fa2c1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fa2c1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa2c1-120">Authorization</span></span> | <span data-ttu-id="fa2c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa2c1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa2c1-123">Request body</span></span>

<span data-ttu-id="fa2c1-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa2c1-125">响应</span><span class="sxs-lookup"><span data-stu-id="fa2c1-125">Response</span></span>

<span data-ttu-id="fa2c1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa2c1-128">示例</span><span class="sxs-lookup"><span data-stu-id="fa2c1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa2c1-129">请求</span><span class="sxs-lookup"><span data-stu-id="fa2c1-129">Request</span></span>

<span data-ttu-id="fa2c1-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa2c1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa2c1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
---


### <a name="response"></a><span data-ttu-id="fa2c1-132">响应</span><span class="sxs-lookup"><span data-stu-id="fa2c1-132">Response</span></span>

<span data-ttu-id="fa2c1-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa2c1-133">The following is an example of the response.</span></span>

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
