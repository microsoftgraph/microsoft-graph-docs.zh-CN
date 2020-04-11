---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9d6b917ac9e819371ab5d91f379c7d69621665b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229110"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="62c0d-103">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="62c0d-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="62c0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c0d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="62c0d-105">将[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)分配给[应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="62c0d-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62c0d-106">权限</span><span class="sxs-lookup"><span data-stu-id="62c0d-106">Permissions</span></span>

<span data-ttu-id="62c0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62c0d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62c0d-109">Permission type</span></span>                        | <span data-ttu-id="62c0d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62c0d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62c0d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62c0d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62c0d-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="62c0d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="62c0d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62c0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c0d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62c0d-114">Not supported.</span></span> |
| <span data-ttu-id="62c0d-115">Application</span><span class="sxs-lookup"><span data-stu-id="62c0d-115">Application</span></span>                            | <span data-ttu-id="62c0d-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="62c0d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62c0d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62c0d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="62c0d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62c0d-118">Request headers</span></span>

| <span data-ttu-id="62c0d-119">名称</span><span class="sxs-lookup"><span data-stu-id="62c0d-119">Name</span></span>          | <span data-ttu-id="62c0d-120">说明</span><span class="sxs-lookup"><span data-stu-id="62c0d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="62c0d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62c0d-121">Authorization</span></span> | <span data-ttu-id="62c0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62c0d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62c0d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62c0d-124">Content-Type</span></span> | <span data-ttu-id="62c0d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62c0d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62c0d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62c0d-127">Request body</span></span>

<span data-ttu-id="62c0d-128">在请求正文中，提供应分配给应用[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)程序或服务主体的`@odata.id` tokenLifetimePolicy 对象的标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="62c0d-128">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="62c0d-129">响应</span><span class="sxs-lookup"><span data-stu-id="62c0d-129">Response</span></span>

<span data-ttu-id="62c0d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="62c0d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62c0d-132">示例</span><span class="sxs-lookup"><span data-stu-id="62c0d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62c0d-133">请求</span><span class="sxs-lookup"><span data-stu-id="62c0d-133">Request</span></span>

<span data-ttu-id="62c0d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62c0d-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="62c0d-135">响应</span><span class="sxs-lookup"><span data-stu-id="62c0d-135">Response</span></span>

<span data-ttu-id="62c0d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62c0d-136">The following is an example of the response.</span></span>

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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
