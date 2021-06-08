---
title: timeCard：startBreak
description: 使用特定时间卡开始中断。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 95c220d9b6bcead0f0c734959bb99788e8b5e2fd
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787846"
---
# <a name="timecard-startbreak"></a><span data-ttu-id="4b4df-103">timeCard：startBreak</span><span class="sxs-lookup"><span data-stu-id="4b4df-103">timeCard: startBreak</span></span>

<span data-ttu-id="4b4df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b4df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b4df-105">启动特定 [timeCard](../resources/timeCard.md)中的中断。</span><span class="sxs-lookup"><span data-stu-id="4b4df-105">Start a break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b4df-106">权限</span><span class="sxs-lookup"><span data-stu-id="4b4df-106">Permissions</span></span>

<span data-ttu-id="4b4df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b4df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b4df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b4df-109">Permission type</span></span>      | <span data-ttu-id="4b4df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b4df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b4df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b4df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b4df-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b4df-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b4df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b4df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b4df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b4df-114">Not supported.</span></span>    |
|<span data-ttu-id="4b4df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b4df-115">Application</span></span> | <span data-ttu-id="4b4df-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="4b4df-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="4b4df-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="4b4df-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b4df-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b4df-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/startBreak
```

## <a name="request-headers"></a><span data-ttu-id="4b4df-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b4df-119">Request headers</span></span>

| <span data-ttu-id="4b4df-120">标头</span><span class="sxs-lookup"><span data-stu-id="4b4df-120">Header</span></span>       | <span data-ttu-id="4b4df-121">值</span><span class="sxs-lookup"><span data-stu-id="4b4df-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b4df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b4df-122">Authorization</span></span>  | <span data-ttu-id="4b4df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b4df-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b4df-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4b4df-125">Content-type</span></span> | <span data-ttu-id="4b4df-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4b4df-p103">application/json. Required.</span></span>|
| <span data-ttu-id="4b4df-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="4b4df-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="4b4df-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="4b4df-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="4b4df-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="4b4df-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b4df-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b4df-131">Request body</span></span>

<span data-ttu-id="4b4df-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4b4df-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b4df-133">参数</span><span class="sxs-lookup"><span data-stu-id="4b4df-133">Parameter</span></span>    | <span data-ttu-id="4b4df-134">类型</span><span class="sxs-lookup"><span data-stu-id="4b4df-134">Type</span></span>        | <span data-ttu-id="4b4df-135">说明</span><span class="sxs-lookup"><span data-stu-id="4b4df-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b4df-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="4b4df-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="4b4df-137">指示此操作是否发生在已批准的位置。</span><span class="sxs-lookup"><span data-stu-id="4b4df-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="4b4df-138">notes</span><span class="sxs-lookup"><span data-stu-id="4b4df-138">notes</span></span>| [<span data-ttu-id="4b4df-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="4b4df-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="4b4df-140">中断开始时的注释。</span><span class="sxs-lookup"><span data-stu-id="4b4df-140">Notes during start of break.</span></span>|

## <a name="response"></a><span data-ttu-id="4b4df-141">响应</span><span class="sxs-lookup"><span data-stu-id="4b4df-141">Response</span></span>

<span data-ttu-id="4b4df-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4b4df-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b4df-143">示例</span><span class="sxs-lookup"><span data-stu-id="4b4df-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b4df-144">请求</span><span class="sxs-lookup"><span data-stu-id="4b4df-144">Request</span></span>
<span data-ttu-id="4b4df-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b4df-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-startBreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/startbreak
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "start break smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="4b4df-146">响应</span><span class="sxs-lookup"><span data-stu-id="4b4df-146">Response</span></span>

<span data-ttu-id="4b4df-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b4df-147">The following is an example of the response.</span></span> 

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
  "description": "Start Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
