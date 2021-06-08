---
title: 删除 timeCard
description: 删除计划中的 timeCard 实例。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f87fe8145d65793b33dc539ed1db235a7e09aebf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787853"
---
# <a name="delete-timecard"></a><span data-ttu-id="68602-103">删除 timeCard</span><span class="sxs-lookup"><span data-stu-id="68602-103">Delete timeCard</span></span>

<span data-ttu-id="68602-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68602-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68602-105">删除 [计划 中的 timeCard](../resources/timeCard.md) [实例](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="68602-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68602-106">权限</span><span class="sxs-lookup"><span data-stu-id="68602-106">Permissions</span></span>

<span data-ttu-id="68602-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68602-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="68602-109">Permission type</span></span>      | <span data-ttu-id="68602-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68602-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68602-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68602-111">Delegated (work or school account)</span></span> | <span data-ttu-id="68602-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68602-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="68602-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68602-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68602-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="68602-114">Not supported.</span></span>    |
|<span data-ttu-id="68602-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="68602-115">Application</span></span> | <span data-ttu-id="68602-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="68602-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="68602-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="68602-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="68602-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68602-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="68602-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68602-119">Request headers</span></span>

| <span data-ttu-id="68602-120">标头</span><span class="sxs-lookup"><span data-stu-id="68602-120">Header</span></span>       | <span data-ttu-id="68602-121">值</span><span class="sxs-lookup"><span data-stu-id="68602-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68602-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68602-122">Authorization</span></span>  | <span data-ttu-id="68602-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68602-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68602-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="68602-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="68602-126">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="68602-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="68602-127">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="68602-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68602-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="68602-128">Request body</span></span>
<span data-ttu-id="68602-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68602-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68602-130">响应</span><span class="sxs-lookup"><span data-stu-id="68602-130">Response</span></span>

<span data-ttu-id="68602-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="68602-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68602-132">示例</span><span class="sxs-lookup"><span data-stu-id="68602-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="68602-133">请求</span><span class="sxs-lookup"><span data-stu-id="68602-133">Request</span></span>
<span data-ttu-id="68602-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="68602-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```

### <a name="response"></a><span data-ttu-id="68602-135">响应</span><span class="sxs-lookup"><span data-stu-id="68602-135">Response</span></span>

<span data-ttu-id="68602-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68602-136">The following is an example of the response.</span></span> 

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
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
