---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 722e7986a32670a764f1dd11b2875194a1c5a257
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324966"
---
# <a name="delete-educationclass"></a><span data-ttu-id="19de7-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="19de7-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19de7-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="19de7-105">Delete a class.</span></span> <span data-ttu-id="19de7-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="19de7-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="19de7-107">权限</span><span class="sxs-lookup"><span data-stu-id="19de7-107">Permissions</span></span>
<span data-ttu-id="19de7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19de7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19de7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19de7-110">Permission type</span></span>      | <span data-ttu-id="19de7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19de7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19de7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19de7-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="19de7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19de7-113">Not supported.</span></span>  |
|<span data-ttu-id="19de7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19de7-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="19de7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19de7-115">Not supported.</span></span>  |
|<span data-ttu-id="19de7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19de7-116">Application</span></span> | <span data-ttu-id="19de7-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19de7-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19de7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19de7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="19de7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19de7-119">Request headers</span></span>
| <span data-ttu-id="19de7-120">标头</span><span class="sxs-lookup"><span data-stu-id="19de7-120">Header</span></span>       | <span data-ttu-id="19de7-121">值</span><span class="sxs-lookup"><span data-stu-id="19de7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19de7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19de7-122">Authorization</span></span>  | <span data-ttu-id="19de7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19de7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19de7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="19de7-125">Request body</span></span>
<span data-ttu-id="19de7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19de7-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="19de7-127">响应</span><span class="sxs-lookup"><span data-stu-id="19de7-127">Response</span></span>
<span data-ttu-id="19de7-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="19de7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19de7-130">示例</span><span class="sxs-lookup"><span data-stu-id="19de7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19de7-131">请求</span><span class="sxs-lookup"><span data-stu-id="19de7-131">Request</span></span>
<span data-ttu-id="19de7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19de7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="19de7-133">响应</span><span class="sxs-lookup"><span data-stu-id="19de7-133">Response</span></span>
<span data-ttu-id="19de7-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19de7-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
