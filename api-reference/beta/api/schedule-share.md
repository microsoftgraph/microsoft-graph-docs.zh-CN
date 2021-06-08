---
title: schedule： share
description: 与计划成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 47bd1e71b31a10b7dfb0ffc34c063d94f2e065fc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788015"
---
# <a name="schedule-share"></a><span data-ttu-id="6cdee-103">schedule： share</span><span class="sxs-lookup"><span data-stu-id="6cdee-103">schedule: share</span></span>

<span data-ttu-id="6cdee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cdee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cdee-105">与 [计划成员](../resources/schedule.md) 共享计划时间范围。</span><span class="sxs-lookup"><span data-stu-id="6cdee-105">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="6cdee-106">使指定的团队成员[（](../resources/shift.md)包括员工和经理）可以查看计划中指定时间范围内班次、openshift 和[timeOff](../resources/timeoff.md)项目的集合。 [](../resources/openshift.md) [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="6cdee-106">Make the collections of [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="6cdee-107">计划[中的](../resources/shift.md)[每个班次、openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md) [实例都支持](../resources/schedule.md)草稿版本和项目的共享版本。</span><span class="sxs-lookup"><span data-stu-id="6cdee-107">Each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="6cdee-108">草稿版本仅由经理查看，员工和经理可查看共享版本。</span><span class="sxs-lookup"><span data-stu-id="6cdee-108">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="6cdee-109">对于指定[](../resources/shift.md)时间范围内的每个班次[、openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例，共享操作从草稿版本更新共享版本，以便除经理外，员工还可以查看有关项目的最新信息。</span><span class="sxs-lookup"><span data-stu-id="6cdee-109">For each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="6cdee-110">**notifyTeam** 参数进一步指定哪些员工可以查看项目。</span><span class="sxs-lookup"><span data-stu-id="6cdee-110">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cdee-111">权限</span><span class="sxs-lookup"><span data-stu-id="6cdee-111">Permissions</span></span>

<span data-ttu-id="6cdee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cdee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cdee-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cdee-114">Permission type</span></span>      | <span data-ttu-id="6cdee-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cdee-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cdee-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cdee-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6cdee-117">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdee-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6cdee-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cdee-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cdee-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cdee-119">Not supported.</span></span>    |
|<span data-ttu-id="6cdee-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cdee-120">Application</span></span> | <span data-ttu-id="6cdee-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdee-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cdee-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cdee-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="6cdee-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cdee-123">Request headers</span></span>

| <span data-ttu-id="6cdee-124">标头</span><span class="sxs-lookup"><span data-stu-id="6cdee-124">Header</span></span>       | <span data-ttu-id="6cdee-125">值</span><span class="sxs-lookup"><span data-stu-id="6cdee-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cdee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cdee-126">Authorization</span></span>  | <span data-ttu-id="6cdee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cdee-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6cdee-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cdee-129">Content-Type</span></span>  | <span data-ttu-id="6cdee-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6cdee-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cdee-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cdee-132">Request body</span></span>

<span data-ttu-id="6cdee-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6cdee-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="6cdee-134">参数</span><span class="sxs-lookup"><span data-stu-id="6cdee-134">Parameter</span></span>                   |<span data-ttu-id="6cdee-135">类型</span><span class="sxs-lookup"><span data-stu-id="6cdee-135">Type</span></span>           |<span data-ttu-id="6cdee-136">说明</span><span class="sxs-lookup"><span data-stu-id="6cdee-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="6cdee-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="6cdee-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="6cdee-138">指示整个团队是应该收到此操作的可见通知，还是只收到分配有已共享班次的员工的通知。</span><span class="sxs-lookup"><span data-stu-id="6cdee-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="6cdee-139">必填。</span><span class="sxs-lookup"><span data-stu-id="6cdee-139">Required.</span></span>       |
| <span data-ttu-id="6cdee-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdee-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="6cdee-141">按计划共享班次的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6cdee-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="6cdee-142">必填。</span><span class="sxs-lookup"><span data-stu-id="6cdee-142">Required.</span></span>   |
| <span data-ttu-id="6cdee-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdee-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="6cdee-144">在计划前共享班次的结束时间。</span><span class="sxs-lookup"><span data-stu-id="6cdee-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="6cdee-145">响应</span><span class="sxs-lookup"><span data-stu-id="6cdee-145">Response</span></span>

<span data-ttu-id="6cdee-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6cdee-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cdee-148">示例</span><span class="sxs-lookup"><span data-stu-id="6cdee-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6cdee-149">请求</span><span class="sxs-lookup"><span data-stu-id="6cdee-149">Request</span></span>

<span data-ttu-id="6cdee-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cdee-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cdee-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cdee-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6cdee-152">C#</span><span class="sxs-lookup"><span data-stu-id="6cdee-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cdee-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cdee-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cdee-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cdee-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cdee-155">Java</span><span class="sxs-lookup"><span data-stu-id="6cdee-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cdee-156">响应</span><span class="sxs-lookup"><span data-stu-id="6cdee-156">Response</span></span>

<span data-ttu-id="6cdee-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cdee-157">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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


