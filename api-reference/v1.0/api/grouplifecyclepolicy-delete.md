---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9d58eca82c72008cb30095fe4fbfacf5a382111a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567436"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="98edb-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="98edb-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="98edb-104">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="98edb-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98edb-105">权限</span><span class="sxs-lookup"><span data-stu-id="98edb-105">Permissions</span></span>

<span data-ttu-id="98edb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98edb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98edb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="98edb-108">Permission type</span></span>      | <span data-ttu-id="98edb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98edb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98edb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98edb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98edb-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98edb-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="98edb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98edb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98edb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="98edb-113">Not supported.</span></span>    |
|<span data-ttu-id="98edb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="98edb-114">Application</span></span> | <span data-ttu-id="98edb-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98edb-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98edb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98edb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="98edb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="98edb-117">Request headers</span></span>

| <span data-ttu-id="98edb-118">名称</span><span class="sxs-lookup"><span data-stu-id="98edb-118">Name</span></span> | <span data-ttu-id="98edb-119">说明</span><span class="sxs-lookup"><span data-stu-id="98edb-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="98edb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98edb-120">Authorization</span></span> | <span data-ttu-id="98edb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98edb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98edb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98edb-123">Content-Type</span></span>  | <span data-ttu-id="98edb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="98edb-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="98edb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="98edb-125">Request body</span></span>
<span data-ttu-id="98edb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98edb-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="98edb-127">响应</span><span class="sxs-lookup"><span data-stu-id="98edb-127">Response</span></span>

<span data-ttu-id="98edb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="98edb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98edb-130">示例</span><span class="sxs-lookup"><span data-stu-id="98edb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98edb-131">请求</span><span class="sxs-lookup"><span data-stu-id="98edb-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="98edb-132">响应</span><span class="sxs-lookup"><span data-stu-id="98edb-132">Response</span></span>

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
