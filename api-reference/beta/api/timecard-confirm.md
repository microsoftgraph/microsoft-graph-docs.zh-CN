---
title: timeCard： confirm
description: 确认特定时间卡。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 42ee0d8c1259b31ebf96716ca1c49656af4075f8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787855"
---
# <a name="timecard-confirm"></a><span data-ttu-id="a0eb0-103">timeCard： confirm</span><span class="sxs-lookup"><span data-stu-id="a0eb0-103">timeCard: confirm</span></span>

<span data-ttu-id="a0eb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0eb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0eb0-105">确认特定 [timeCard](../resources/timeCard.md)。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-105">Confirm a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0eb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0eb0-106">Permissions</span></span>

<span data-ttu-id="a0eb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0eb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0eb0-109">Permission type</span></span>      | <span data-ttu-id="a0eb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0eb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0eb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0eb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0eb0-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0eb0-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0eb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0eb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0eb0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-114">Not supported.</span></span>    |
|<span data-ttu-id="a0eb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0eb0-115">Application</span></span> | <span data-ttu-id="a0eb0-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a0eb0-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a0eb0-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0eb0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0eb0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/confirm
```

## <a name="request-headers"></a><span data-ttu-id="a0eb0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0eb0-119">Request headers</span></span>

| <span data-ttu-id="a0eb0-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0eb0-120">Header</span></span>       | <span data-ttu-id="a0eb0-121">值</span><span class="sxs-lookup"><span data-stu-id="a0eb0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0eb0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0eb0-122">Authorization</span></span>  | <span data-ttu-id="a0eb0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0eb0-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="a0eb0-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="a0eb0-126">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="a0eb0-127">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0eb0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0eb0-128">Request body</span></span>
<span data-ttu-id="a0eb0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0eb0-130">响应</span><span class="sxs-lookup"><span data-stu-id="a0eb0-130">Response</span></span>

<span data-ttu-id="a0eb0-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a0eb0-132">示例</span><span class="sxs-lookup"><span data-stu-id="a0eb0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0eb0-133">请求</span><span class="sxs-lookup"><span data-stu-id="a0eb0-133">Request</span></span>
<span data-ttu-id="a0eb0-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-confirm"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/confirm
```

### <a name="response"></a><span data-ttu-id="a0eb0-135">响应</span><span class="sxs-lookup"><span data-stu-id="a0eb0-135">Response</span></span>

<span data-ttu-id="a0eb0-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0eb0-136">The following is an example of the response.</span></span> 

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
  "description": "Confirm timecard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
