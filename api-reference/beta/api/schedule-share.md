---
title: 日程安排：共享
description: 与 schedule 成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fce02b8f18a2745b06d1782ecadb7bc7bd3adc0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154239"
---
# <a name="schedule-share"></a><span data-ttu-id="67339-103">日程安排：共享</span><span class="sxs-lookup"><span data-stu-id="67339-103">schedule: share</span></span>

<span data-ttu-id="67339-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67339-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67339-105">与 schedule 成员共享[计划](../resources/schedule.md)时间范围。</span><span class="sxs-lookup"><span data-stu-id="67339-105">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="67339-106">在指定的团队成员（包括员工和经理）可查看的[日程安排](../resources/schedule.md)的指定时间范围内，创建[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)项目的集合。</span><span class="sxs-lookup"><span data-stu-id="67339-106">Make the collections of [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="67339-107">[计划](../resources/schedule.md)中的每个[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例都支持项目的草稿版本和共享版本。</span><span class="sxs-lookup"><span data-stu-id="67339-107">Each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="67339-108">草稿版本仅由经理查看，并且共享版本可供员工和经理查看。</span><span class="sxs-lookup"><span data-stu-id="67339-108">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="67339-109">对于每个[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例在指定的时间范围内，共享操作将从草稿版本更新共享版本，因此，除了经理之外，员工还可以查看有关该项目的最新信息。</span><span class="sxs-lookup"><span data-stu-id="67339-109">For each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="67339-110">**NotifyTeam**参数会进一步指定哪些员工可以查看该项目。</span><span class="sxs-lookup"><span data-stu-id="67339-110">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="67339-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="67339-111">Permissions</span></span>

<span data-ttu-id="67339-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67339-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67339-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="67339-114">Permission type</span></span>      | <span data-ttu-id="67339-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67339-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67339-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67339-116">Delegated (work or school account)</span></span> | <span data-ttu-id="67339-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67339-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="67339-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67339-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67339-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="67339-119">Not supported.</span></span>    |
|<span data-ttu-id="67339-120">Application</span><span class="sxs-lookup"><span data-stu-id="67339-120">Application</span></span> | <span data-ttu-id="67339-121">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="67339-121">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="67339-122">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="67339-122">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="67339-123">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="67339-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="67339-124">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="67339-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="67339-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67339-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="67339-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="67339-126">Request headers</span></span>

| <span data-ttu-id="67339-127">标头</span><span class="sxs-lookup"><span data-stu-id="67339-127">Header</span></span>       | <span data-ttu-id="67339-128">值</span><span class="sxs-lookup"><span data-stu-id="67339-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67339-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="67339-129">Authorization</span></span>  | <span data-ttu-id="67339-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67339-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="67339-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67339-132">Content-Type</span></span>  | <span data-ttu-id="67339-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="67339-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67339-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="67339-135">Request body</span></span>

<span data-ttu-id="67339-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="67339-136">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="67339-137">参数</span><span class="sxs-lookup"><span data-stu-id="67339-137">Parameter</span></span>                   |<span data-ttu-id="67339-138">类型</span><span class="sxs-lookup"><span data-stu-id="67339-138">Type</span></span>           |<span data-ttu-id="67339-139">Description</span><span class="sxs-lookup"><span data-stu-id="67339-139">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="67339-140">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="67339-140">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="67339-141">指示整个团队是否应获取有关此操作的可见通知，或仅获取已分配有班次的员工。</span><span class="sxs-lookup"><span data-stu-id="67339-141">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="67339-142">必填。</span><span class="sxs-lookup"><span data-stu-id="67339-142">Required.</span></span>       |
| <span data-ttu-id="67339-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="67339-143">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="67339-144">共享日程上的班次的开始时间。</span><span class="sxs-lookup"><span data-stu-id="67339-144">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="67339-145">必填。</span><span class="sxs-lookup"><span data-stu-id="67339-145">Required.</span></span>   |
| <span data-ttu-id="67339-146">endDateTime</span><span class="sxs-lookup"><span data-stu-id="67339-146">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="67339-147">在日程上共享班次的结束时间。</span><span class="sxs-lookup"><span data-stu-id="67339-147">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="67339-148">响应</span><span class="sxs-lookup"><span data-stu-id="67339-148">Response</span></span>

<span data-ttu-id="67339-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67339-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67339-151">示例</span><span class="sxs-lookup"><span data-stu-id="67339-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="67339-152">请求</span><span class="sxs-lookup"><span data-stu-id="67339-152">Request</span></span>

<span data-ttu-id="67339-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67339-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67339-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="67339-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67339-155">C#</span><span class="sxs-lookup"><span data-stu-id="67339-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67339-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67339-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67339-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67339-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67339-158">响应</span><span class="sxs-lookup"><span data-stu-id="67339-158">Response</span></span>

<span data-ttu-id="67339-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67339-159">The following is an example of the response.</span></span> 

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
