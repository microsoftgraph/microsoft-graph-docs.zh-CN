---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: dkershaw10
ms.openlocfilehash: 41c679a9fa2a55a0137d1197f08515e64750d4dc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361962"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="3c00a-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3c00a-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="3c00a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c00a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c00a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c00a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c00a-106">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="3c00a-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c00a-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c00a-107">Permissions</span></span>

<span data-ttu-id="3c00a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c00a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c00a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c00a-110">Permission type</span></span>      | <span data-ttu-id="3c00a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c00a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c00a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c00a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c00a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c00a-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c00a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c00a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c00a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="3c00a-115">Not supported</span></span> |
|<span data-ttu-id="3c00a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c00a-116">Application</span></span> | <span data-ttu-id="3c00a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c00a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c00a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c00a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="3c00a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c00a-119">Request headers</span></span>

| <span data-ttu-id="3c00a-120">Name</span><span class="sxs-lookup"><span data-stu-id="3c00a-120">Name</span></span> | <span data-ttu-id="3c00a-121">说明</span><span class="sxs-lookup"><span data-stu-id="3c00a-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3c00a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c00a-122">Authorization</span></span> | <span data-ttu-id="3c00a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c00a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c00a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c00a-125">Content-Type</span></span>  | <span data-ttu-id="3c00a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c00a-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c00a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c00a-127">Request body</span></span>
<span data-ttu-id="3c00a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c00a-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3c00a-129">响应</span><span class="sxs-lookup"><span data-stu-id="3c00a-129">Response</span></span>

<span data-ttu-id="3c00a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c00a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c00a-132">示例</span><span class="sxs-lookup"><span data-stu-id="3c00a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c00a-133">请求</span><span class="sxs-lookup"><span data-stu-id="3c00a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="3c00a-134">响应</span><span class="sxs-lookup"><span data-stu-id="3c00a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->