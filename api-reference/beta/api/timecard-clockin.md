---
title: timeCard：clockIn
description: 时钟以启动一个时间卡。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7075b2323bcf2792dcb58b09c248dbcc095775d2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787883"
---
# <a name="timecard-clockin"></a><span data-ttu-id="e5e43-103">timeCard：clockIn</span><span class="sxs-lookup"><span data-stu-id="e5e43-103">timeCard: clockIn</span></span>

<span data-ttu-id="e5e43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5e43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5e43-105">Clock in to start a [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="e5e43-105">Clock in to start a [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5e43-106">权限</span><span class="sxs-lookup"><span data-stu-id="e5e43-106">Permissions</span></span>

<span data-ttu-id="e5e43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5e43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5e43-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5e43-109">Permission type</span></span>      | <span data-ttu-id="e5e43-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5e43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5e43-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5e43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5e43-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e43-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5e43-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5e43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5e43-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5e43-114">Not supported.</span></span>    |
|<span data-ttu-id="e5e43-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5e43-115">Application</span></span> | <span data-ttu-id="e5e43-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="e5e43-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="e5e43-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="e5e43-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5e43-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5e43-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/clockIn
```

## <a name="request-headers"></a><span data-ttu-id="e5e43-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5e43-119">Request headers</span></span>

| <span data-ttu-id="e5e43-120">标头</span><span class="sxs-lookup"><span data-stu-id="e5e43-120">Header</span></span>       | <span data-ttu-id="e5e43-121">值</span><span class="sxs-lookup"><span data-stu-id="e5e43-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5e43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5e43-122">Authorization</span></span>  | <span data-ttu-id="e5e43-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5e43-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5e43-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5e43-125">Content-type</span></span> | <span data-ttu-id="e5e43-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5e43-p103">application/json. Required.</span></span>|
| <span data-ttu-id="e5e43-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="e5e43-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="e5e43-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5e43-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="e5e43-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="e5e43-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5e43-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5e43-131">Request body</span></span>

<span data-ttu-id="e5e43-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e5e43-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5e43-133">参数</span><span class="sxs-lookup"><span data-stu-id="e5e43-133">Parameter</span></span>    | <span data-ttu-id="e5e43-134">类型</span><span class="sxs-lookup"><span data-stu-id="e5e43-134">Type</span></span>        | <span data-ttu-id="e5e43-135">说明</span><span class="sxs-lookup"><span data-stu-id="e5e43-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5e43-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="e5e43-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="e5e43-137">指示此操作是否发生在已批准的位置。</span><span class="sxs-lookup"><span data-stu-id="e5e43-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="e5e43-138">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="e5e43-138">onBehalfOfUserId</span></span>| <span data-ttu-id="e5e43-139">String</span><span class="sxs-lookup"><span data-stu-id="e5e43-139">String</span></span> | <span data-ttu-id="e5e43-140">管理员代表用户进行时钟的可选参数。</span><span class="sxs-lookup"><span data-stu-id="e5e43-140">Optional parameter used by the manager to clock in on behalf of a user.</span></span>|
|<span data-ttu-id="e5e43-141">notes</span><span class="sxs-lookup"><span data-stu-id="e5e43-141">notes</span></span>| [<span data-ttu-id="e5e43-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="e5e43-142">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="e5e43-143">时钟的备注。</span><span class="sxs-lookup"><span data-stu-id="e5e43-143">Notes for the clock in.</span></span> |

## <a name="response"></a><span data-ttu-id="e5e43-144">响应</span><span class="sxs-lookup"><span data-stu-id="e5e43-144">Response</span></span>

<span data-ttu-id="e5e43-145">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [timeCard](../resources/timeCard.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5e43-145">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5e43-146">示例</span><span class="sxs-lookup"><span data-stu-id="e5e43-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5e43-147">请求</span><span class="sxs-lookup"><span data-stu-id="e5e43-147">Request</span></span>
<span data-ttu-id="e5e43-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5e43-148">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="e5e43-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5e43-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-clockin"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/clockin
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock in notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="e5e43-150">响应</span><span class="sxs-lookup"><span data-stu-id="e5e43-150">Response</span></span>

<span data-ttu-id="e5e43-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5e43-151">The following is an example of the response.</span></span> 

><span data-ttu-id="e5e43-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5e43-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T22:58:41.327Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedIn",
    "confirmedBy": "none",
    "clockOutEvent": null,
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "breaks": [],
    "originalEntry": {
        "clockOutEvent": null,
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "breaks": []
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Clock In",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
