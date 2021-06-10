---
title: timeCard：endBreak
description: 结束特定时间卡中的打开中断。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 61c80ea006ad0def4d9c8f58e36e44ae4caac851
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870575"
---
# <a name="timecard-endbreak"></a><span data-ttu-id="50ad1-103">timeCard：endBreak</span><span class="sxs-lookup"><span data-stu-id="50ad1-103">timeCard: endBreak</span></span>

<span data-ttu-id="50ad1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50ad1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50ad1-105">结束特定 timeCard 中的 [打开中断](../resources/timeCard.md)。</span><span class="sxs-lookup"><span data-stu-id="50ad1-105">End the open break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="50ad1-106">权限</span><span class="sxs-lookup"><span data-stu-id="50ad1-106">Permissions</span></span>

<span data-ttu-id="50ad1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ad1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50ad1-109">Permission type</span></span>      | <span data-ttu-id="50ad1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50ad1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ad1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50ad1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50ad1-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ad1-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="50ad1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50ad1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50ad1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50ad1-114">Not supported.</span></span>    |
|<span data-ttu-id="50ad1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50ad1-115">Application</span></span> | <span data-ttu-id="50ad1-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="50ad1-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="50ad1-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="50ad1-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="50ad1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50ad1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/endBreak
```

## <a name="request-headers"></a><span data-ttu-id="50ad1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50ad1-119">Request headers</span></span>

| <span data-ttu-id="50ad1-120">标头</span><span class="sxs-lookup"><span data-stu-id="50ad1-120">Header</span></span>       | <span data-ttu-id="50ad1-121">值</span><span class="sxs-lookup"><span data-stu-id="50ad1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50ad1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ad1-122">Authorization</span></span>  | <span data-ttu-id="50ad1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50ad1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50ad1-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="50ad1-125">Content-type</span></span> | <span data-ttu-id="50ad1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50ad1-p103">application/json. Required.</span></span>|
| <span data-ttu-id="50ad1-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="50ad1-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="50ad1-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="50ad1-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="50ad1-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="50ad1-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50ad1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="50ad1-131">Request body</span></span>

<span data-ttu-id="50ad1-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="50ad1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50ad1-133">参数</span><span class="sxs-lookup"><span data-stu-id="50ad1-133">Parameter</span></span>    | <span data-ttu-id="50ad1-134">类型</span><span class="sxs-lookup"><span data-stu-id="50ad1-134">Type</span></span>        | <span data-ttu-id="50ad1-135">说明</span><span class="sxs-lookup"><span data-stu-id="50ad1-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50ad1-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="50ad1-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="50ad1-137">指示此操作是否发生在已批准的位置。</span><span class="sxs-lookup"><span data-stu-id="50ad1-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="50ad1-138">notes</span><span class="sxs-lookup"><span data-stu-id="50ad1-138">notes</span></span>| [<span data-ttu-id="50ad1-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="50ad1-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="50ad1-140">中断结束的注释。</span><span class="sxs-lookup"><span data-stu-id="50ad1-140">Notes during end of break.</span></span>|

## <a name="response"></a><span data-ttu-id="50ad1-141">响应</span><span class="sxs-lookup"><span data-stu-id="50ad1-141">Response</span></span>

<span data-ttu-id="50ad1-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="50ad1-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50ad1-143">示例</span><span class="sxs-lookup"><span data-stu-id="50ad1-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ad1-144">请求</span><span class="sxs-lookup"><span data-stu-id="50ad1-144">Request</span></span>
<span data-ttu-id="50ad1-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="50ad1-145">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="50ad1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="50ad1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-endbreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/endbreak

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "end break smaple notes"
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="50ad1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50ad1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-endbreak-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50ad1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50ad1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-endbreak-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50ad1-149">响应</span><span class="sxs-lookup"><span data-stu-id="50ad1-149">Response</span></span>

<span data-ttu-id="50ad1-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="50ad1-150">The following is an example of the response.</span></span> 

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
  "description": "End Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
