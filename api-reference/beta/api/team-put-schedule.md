---
title: 创建或替换计划
description: 创建或替换**schedule**对象。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb45a560356b6f0ba536bd44ed869f0797677f35
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864955"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="7e92f-103">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="7e92f-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e92f-104">创建或替换[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7e92f-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="7e92f-105">计划创建过程符合[基于资源的长时间运行的操作（RELO）的一个 API 指南](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。</span><span class="sxs-lookup"><span data-stu-id="7e92f-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="7e92f-106">当客户端使用 PUT 方法时，如果设置了计划，则操作将替换计划;否则，该操作将在后台启动计划设置过程。</span><span class="sxs-lookup"><span data-stu-id="7e92f-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="7e92f-107">在计划设置过程中，客户端可以使用[get 方法](schedule-get.md)获取计划，并查看设置`provisionStatus`的当前状态的属性。</span><span class="sxs-lookup"><span data-stu-id="7e92f-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="7e92f-108">如果设置失败，客户端可以从`provisionStatusCode`属性获取其他信息。</span><span class="sxs-lookup"><span data-stu-id="7e92f-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="7e92f-109">客户端也可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="7e92f-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="7e92f-110">权限</span><span class="sxs-lookup"><span data-stu-id="7e92f-110">Permissions</span></span>

<span data-ttu-id="7e92f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e92f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e92f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e92f-113">Permission type</span></span>      | <span data-ttu-id="7e92f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e92f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e92f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e92f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7e92f-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e92f-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e92f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e92f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e92f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e92f-118">Not supported.</span></span>    |
|<span data-ttu-id="7e92f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e92f-119">Application</span></span> | <span data-ttu-id="7e92f-120">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="7e92f-120">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="7e92f-121">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="7e92f-121">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="7e92f-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="7e92f-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7e92f-123">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="7e92f-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e92f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e92f-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="7e92f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e92f-125">Request headers</span></span>

| <span data-ttu-id="7e92f-126">标头</span><span class="sxs-lookup"><span data-stu-id="7e92f-126">Header</span></span>       | <span data-ttu-id="7e92f-127">值</span><span class="sxs-lookup"><span data-stu-id="7e92f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e92f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e92f-128">Authorization</span></span>  | <span data-ttu-id="7e92f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e92f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e92f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e92f-131">Content-Type</span></span>  | <span data-ttu-id="7e92f-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7e92f-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e92f-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e92f-134">Request body</span></span>

<span data-ttu-id="7e92f-135">在请求正文中，提供[schedule](../resources/schedule.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e92f-135">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e92f-136">响应</span><span class="sxs-lookup"><span data-stu-id="7e92f-136">Response</span></span>

<span data-ttu-id="7e92f-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7e92f-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e92f-138">示例</span><span class="sxs-lookup"><span data-stu-id="7e92f-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e92f-139">请求</span><span class="sxs-lookup"><span data-stu-id="7e92f-139">Request</span></span>

<span data-ttu-id="7e92f-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e92f-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e92f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e92f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e92f-142">C#</span><span class="sxs-lookup"><span data-stu-id="7e92f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e92f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e92f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e92f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e92f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e92f-145">响应</span><span class="sxs-lookup"><span data-stu-id="7e92f-145">Response</span></span>

<span data-ttu-id="7e92f-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e92f-146">The following is an example of the response.</span></span> 

><span data-ttu-id="7e92f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e92f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
