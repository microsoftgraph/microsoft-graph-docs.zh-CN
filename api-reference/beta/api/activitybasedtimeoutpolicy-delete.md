---
title: 删除 activityBasedTimeoutPolicy
description: 删除 activityBasedTimeoutPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29b5e61e9401cd0ed0ee63c82f72042b668cafc1
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234142"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="dae35-103">删除 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="dae35-103">Delete activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dae35-104">删除[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dae35-104">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dae35-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="dae35-105">Permissions</span></span>

<span data-ttu-id="dae35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dae35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dae35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dae35-108">Permission type</span></span>                        | <span data-ttu-id="dae35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dae35-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dae35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dae35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dae35-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dae35-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="dae35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dae35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dae35-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dae35-113">Not supported.</span></span> |
| <span data-ttu-id="dae35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dae35-114">Application</span></span>                            | <span data-ttu-id="dae35-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="dae35-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dae35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dae35-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dae35-117">Request headers</span></span>

| <span data-ttu-id="dae35-118">名称</span><span class="sxs-lookup"><span data-stu-id="dae35-118">Name</span></span>          | <span data-ttu-id="dae35-119">说明</span><span class="sxs-lookup"><span data-stu-id="dae35-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dae35-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae35-120">Authorization</span></span> | <span data-ttu-id="dae35-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dae35-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dae35-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dae35-122">Request body</span></span>

<span data-ttu-id="dae35-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dae35-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dae35-124">响应</span><span class="sxs-lookup"><span data-stu-id="dae35-124">Response</span></span>

<span data-ttu-id="dae35-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dae35-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dae35-126">示例</span><span class="sxs-lookup"><span data-stu-id="dae35-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dae35-127">请求</span><span class="sxs-lookup"><span data-stu-id="dae35-127">Request</span></span>

<span data-ttu-id="dae35-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dae35-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="dae35-129">响应</span><span class="sxs-lookup"><span data-stu-id="dae35-129">Response</span></span>

<span data-ttu-id="dae35-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dae35-130">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->