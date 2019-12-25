---
title: 日程安排：共享
description: 与 schedule 成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a650b4ac6cab35dcbb9d4dce488201418752f55
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866957"
---
# <a name="schedule-share"></a><span data-ttu-id="6314e-103">日程安排：共享</span><span class="sxs-lookup"><span data-stu-id="6314e-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6314e-104">与 schedule 成员共享[计划](../resources/schedule.md)时间范围。</span><span class="sxs-lookup"><span data-stu-id="6314e-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="6314e-105">在指定的团队成员（包括员工和经理）可查看的[日程安排](../resources/schedule.md)的指定时间范围内，创建[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)项目的集合。</span><span class="sxs-lookup"><span data-stu-id="6314e-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="6314e-106">[计划](../resources/schedule.md)中的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例都支持项目的草稿版本和共享版本。</span><span class="sxs-lookup"><span data-stu-id="6314e-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="6314e-107">草稿版本仅由经理查看，并且共享版本可供员工和经理查看。</span><span class="sxs-lookup"><span data-stu-id="6314e-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="6314e-108">对于在指定时间范围内的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例，共享操作将从草稿版本更新共享版本，因此，除了经理之外，员工还可以查看有关该项目的最新信息。</span><span class="sxs-lookup"><span data-stu-id="6314e-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="6314e-109">**NotifyTeam**参数会进一步指定哪些员工可以查看该项目。</span><span class="sxs-lookup"><span data-stu-id="6314e-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6314e-110">权限</span><span class="sxs-lookup"><span data-stu-id="6314e-110">Permissions</span></span>

<span data-ttu-id="6314e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6314e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6314e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6314e-113">Permission type</span></span>      | <span data-ttu-id="6314e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6314e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6314e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6314e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6314e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6314e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6314e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6314e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6314e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6314e-118">Not supported.</span></span>    |
|<span data-ttu-id="6314e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6314e-119">Application</span></span> | <span data-ttu-id="6314e-120">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="6314e-120">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="6314e-121">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="6314e-121">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="6314e-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6314e-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6314e-123">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="6314e-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6314e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6314e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="6314e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6314e-125">Request headers</span></span>

| <span data-ttu-id="6314e-126">标头</span><span class="sxs-lookup"><span data-stu-id="6314e-126">Header</span></span>       | <span data-ttu-id="6314e-127">值</span><span class="sxs-lookup"><span data-stu-id="6314e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6314e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6314e-128">Authorization</span></span>  | <span data-ttu-id="6314e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6314e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6314e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6314e-131">Content-Type</span></span>  | <span data-ttu-id="6314e-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6314e-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6314e-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="6314e-134">Request body</span></span>

<span data-ttu-id="6314e-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6314e-135">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="6314e-136">参数</span><span class="sxs-lookup"><span data-stu-id="6314e-136">Parameter</span></span>                   |<span data-ttu-id="6314e-137">类型</span><span class="sxs-lookup"><span data-stu-id="6314e-137">Type</span></span>           |<span data-ttu-id="6314e-138">说明</span><span class="sxs-lookup"><span data-stu-id="6314e-138">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="6314e-139">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="6314e-139">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="6314e-140">指示整个团队是否应获取有关此操作的可见通知，或仅获取已分配有班次的员工。</span><span class="sxs-lookup"><span data-stu-id="6314e-140">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="6314e-141">必需。</span><span class="sxs-lookup"><span data-stu-id="6314e-141">Required.</span></span>       |
| <span data-ttu-id="6314e-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6314e-142">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="6314e-143">共享日程上的班次的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6314e-143">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="6314e-144">必需。</span><span class="sxs-lookup"><span data-stu-id="6314e-144">Required.</span></span>   |
| <span data-ttu-id="6314e-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6314e-145">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="6314e-146">在日程上共享班次的结束时间。</span><span class="sxs-lookup"><span data-stu-id="6314e-146">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="6314e-147">响应</span><span class="sxs-lookup"><span data-stu-id="6314e-147">Response</span></span>

<span data-ttu-id="6314e-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6314e-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6314e-150">示例</span><span class="sxs-lookup"><span data-stu-id="6314e-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6314e-151">请求</span><span class="sxs-lookup"><span data-stu-id="6314e-151">Request</span></span>

<span data-ttu-id="6314e-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6314e-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6314e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6314e-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6314e-154">C#</span><span class="sxs-lookup"><span data-stu-id="6314e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6314e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6314e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6314e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6314e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6314e-157">响应</span><span class="sxs-lookup"><span data-stu-id="6314e-157">Response</span></span>

<span data-ttu-id="6314e-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6314e-158">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
