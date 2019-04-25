---
title: '日程安排: 共享'
description: 与 schedule 成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eaa2eae082c2b50f39b4a3ac2547ca5b0135381f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537818"
---
# <a name="schedule-share"></a><span data-ttu-id="4e380-103">日程安排: 共享</span><span class="sxs-lookup"><span data-stu-id="4e380-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e380-104">与 schedule 成员共享[计划](../resources/schedule.md)时间范围。</span><span class="sxs-lookup"><span data-stu-id="4e380-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="4e380-105">在指定的团队成员 (包括员工和经理) 可查看的[日程安排](../resources/schedule.md)的指定时间范围内, 创建[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)项目的集合。</span><span class="sxs-lookup"><span data-stu-id="4e380-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="4e380-106">[计划](../resources/schedule.md)中的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例都支持项目的草稿版本和共享版本。</span><span class="sxs-lookup"><span data-stu-id="4e380-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="4e380-107">草稿版本仅由经理查看, 并且共享版本可供员工和经理查看。</span><span class="sxs-lookup"><span data-stu-id="4e380-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="4e380-108">对于在指定时间范围内的每个[shift](../resources/shift.md)和[timeOff](../resources/timeoff.md)实例, 共享操作将从草稿版本更新共享版本, 因此, 除了经理之外, 员工还可以查看有关该项目的最新信息。</span><span class="sxs-lookup"><span data-stu-id="4e380-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="4e380-109">**notifyTeam**参数会进一步指定哪些员工可以查看该项目。</span><span class="sxs-lookup"><span data-stu-id="4e380-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e380-110">权限</span><span class="sxs-lookup"><span data-stu-id="4e380-110">Permissions</span></span>

<span data-ttu-id="4e380-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e380-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e380-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e380-113">Permission type</span></span>      | <span data-ttu-id="4e380-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e380-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e380-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e380-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4e380-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e380-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e380-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e380-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e380-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e380-118">Not supported.</span></span>    |
|<span data-ttu-id="4e380-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e380-119">Application</span></span> | <span data-ttu-id="4e380-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e380-120">Not supported.</span></span> |

> <span data-ttu-id="4e380-121">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="4e380-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4e380-122">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="4e380-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e380-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e380-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="4e380-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e380-124">Request headers</span></span>

| <span data-ttu-id="4e380-125">标头</span><span class="sxs-lookup"><span data-stu-id="4e380-125">Header</span></span>       | <span data-ttu-id="4e380-126">值</span><span class="sxs-lookup"><span data-stu-id="4e380-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e380-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e380-127">Authorization</span></span>  | <span data-ttu-id="4e380-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e380-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e380-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e380-130">Content-Type</span></span>  | <span data-ttu-id="4e380-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4e380-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e380-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e380-132">Request body</span></span>

<span data-ttu-id="4e380-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4e380-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="4e380-134">参数</span><span class="sxs-lookup"><span data-stu-id="4e380-134">Parameter</span></span>                   |<span data-ttu-id="4e380-135">类型</span><span class="sxs-lookup"><span data-stu-id="4e380-135">Type</span></span>           |<span data-ttu-id="4e380-136">说明</span><span class="sxs-lookup"><span data-stu-id="4e380-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="4e380-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="4e380-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="4e380-138">指示整个团队是否应获取有关此操作的可见通知, 或仅获取已分配有班次的员工。</span><span class="sxs-lookup"><span data-stu-id="4e380-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="4e380-139">必需。</span><span class="sxs-lookup"><span data-stu-id="4e380-139">Required.</span></span>       |
| <span data-ttu-id="4e380-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e380-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="4e380-141">共享日程上的班次的开始时间。</span><span class="sxs-lookup"><span data-stu-id="4e380-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="4e380-142">必需。</span><span class="sxs-lookup"><span data-stu-id="4e380-142">Required.</span></span>   |
| <span data-ttu-id="4e380-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e380-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="4e380-144">在日程上共享班次的结束时间。</span><span class="sxs-lookup"><span data-stu-id="4e380-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="4e380-145">响应</span><span class="sxs-lookup"><span data-stu-id="4e380-145">Response</span></span>

<span data-ttu-id="4e380-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e380-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e380-148">示例</span><span class="sxs-lookup"><span data-stu-id="4e380-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4e380-149">请求</span><span class="sxs-lookup"><span data-stu-id="4e380-149">Request</span></span>

<span data-ttu-id="4e380-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e380-150">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="4e380-151">响应</span><span class="sxs-lookup"><span data-stu-id="4e380-151">Response</span></span>

<span data-ttu-id="4e380-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e380-152">The following is an example of the response.</span></span> 

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
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
