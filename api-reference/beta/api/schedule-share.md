---
title: '日程安排: 共享'
description: 与 schedule 成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d28ecff0f83487e9040bfb7a0336648e27b20196
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457546"
---
# <a name="schedule-share"></a><span data-ttu-id="15adc-103">日程安排: 共享</span><span class="sxs-lookup"><span data-stu-id="15adc-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15adc-104">与 schedule 成员共享[计划](../resources/schedule.md)时间范围。</span><span class="sxs-lookup"><span data-stu-id="15adc-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="15adc-105">在指定的团队成员 (包括员工和经理) 可查看的[日程安排](../resources/schedule.md)的指定时间范围内, 创建[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)项目的集合。</span><span class="sxs-lookup"><span data-stu-id="15adc-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="15adc-106">[计划](../resources/schedule.md)中的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例都支持项目的草稿版本和共享版本。</span><span class="sxs-lookup"><span data-stu-id="15adc-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="15adc-107">草稿版本仅由经理查看, 并且共享版本可供员工和经理查看。</span><span class="sxs-lookup"><span data-stu-id="15adc-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="15adc-108">对于在指定时间范围内的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例, 共享操作将从草稿版本更新共享版本, 因此, 除了经理之外, 员工还可以查看有关该项目的最新信息。</span><span class="sxs-lookup"><span data-stu-id="15adc-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="15adc-109">**NotifyTeam**参数会进一步指定哪些员工可以查看该项目。</span><span class="sxs-lookup"><span data-stu-id="15adc-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="15adc-110">权限</span><span class="sxs-lookup"><span data-stu-id="15adc-110">Permissions</span></span>

<span data-ttu-id="15adc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15adc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15adc-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="15adc-113">Permission type</span></span>      | <span data-ttu-id="15adc-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15adc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15adc-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15adc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="15adc-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15adc-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="15adc-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15adc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15adc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="15adc-118">Not supported.</span></span>    |
|<span data-ttu-id="15adc-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="15adc-119">Application</span></span> | <span data-ttu-id="15adc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="15adc-120">Not supported.</span></span> |

> <span data-ttu-id="15adc-121">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="15adc-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="15adc-122">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="15adc-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="15adc-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15adc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="15adc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="15adc-124">Request headers</span></span>

| <span data-ttu-id="15adc-125">标头</span><span class="sxs-lookup"><span data-stu-id="15adc-125">Header</span></span>       | <span data-ttu-id="15adc-126">值</span><span class="sxs-lookup"><span data-stu-id="15adc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15adc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="15adc-127">Authorization</span></span>  | <span data-ttu-id="15adc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15adc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="15adc-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15adc-130">Content-Type</span></span>  | <span data-ttu-id="15adc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="15adc-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15adc-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="15adc-132">Request body</span></span>

<span data-ttu-id="15adc-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="15adc-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="15adc-134">参数</span><span class="sxs-lookup"><span data-stu-id="15adc-134">Parameter</span></span>                   |<span data-ttu-id="15adc-135">类型</span><span class="sxs-lookup"><span data-stu-id="15adc-135">Type</span></span>           |<span data-ttu-id="15adc-136">说明</span><span class="sxs-lookup"><span data-stu-id="15adc-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="15adc-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="15adc-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="15adc-138">指示整个团队是否应获取有关此操作的可见通知, 或仅获取已分配有班次的员工。</span><span class="sxs-lookup"><span data-stu-id="15adc-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="15adc-139">必需。</span><span class="sxs-lookup"><span data-stu-id="15adc-139">Required.</span></span>       |
| <span data-ttu-id="15adc-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="15adc-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="15adc-141">共享日程上的班次的开始时间。</span><span class="sxs-lookup"><span data-stu-id="15adc-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="15adc-142">必需。</span><span class="sxs-lookup"><span data-stu-id="15adc-142">Required.</span></span>   |
| <span data-ttu-id="15adc-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="15adc-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="15adc-144">在日程上共享班次的结束时间。</span><span class="sxs-lookup"><span data-stu-id="15adc-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="15adc-145">响应</span><span class="sxs-lookup"><span data-stu-id="15adc-145">Response</span></span>

<span data-ttu-id="15adc-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="15adc-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15adc-148">示例</span><span class="sxs-lookup"><span data-stu-id="15adc-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="15adc-149">请求</span><span class="sxs-lookup"><span data-stu-id="15adc-149">Request</span></span>

<span data-ttu-id="15adc-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15adc-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15adc-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="15adc-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="15adc-152">C#</span><span class="sxs-lookup"><span data-stu-id="15adc-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15adc-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="15adc-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15adc-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="15adc-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="15adc-155">响应</span><span class="sxs-lookup"><span data-stu-id="15adc-155">Response</span></span>

<span data-ttu-id="15adc-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15adc-156">The following is an example of the response.</span></span> 

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
