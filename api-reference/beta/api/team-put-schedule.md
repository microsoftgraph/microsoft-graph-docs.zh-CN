---
title: 创建或替换计划
description: 创建或替换 **schedule** 对象。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa7deb3a8b3ddd4da5ba99d97c270d6ef3b04556
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971073"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="bcaaf-103">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="bcaaf-103">Create or replace schedule</span></span>

<span data-ttu-id="bcaaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcaaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcaaf-105">创建或替换 [schedule](../resources/schedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="bcaaf-106">计划创建过程符合 [基于资源的长时间运行操作 (RELO) 的 API 指南 ](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="bcaaf-107">当客户端使用 PUT 方法时，如果设置了计划，则操作将替换计划;否则，该操作将在后台启动计划设置过程。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="bcaaf-108">在计划设置过程中，客户端可以使用 [get 方法](schedule-get.md) 获取计划，并查看 `provisionStatus` 设置的当前状态的属性。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="bcaaf-109">如果设置失败，客户端可以从属性获取其他信息 `provisionStatusCode` 。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="bcaaf-110">客户端也可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="bcaaf-111">权限</span><span class="sxs-lookup"><span data-stu-id="bcaaf-111">Permissions</span></span>

<span data-ttu-id="bcaaf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcaaf-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcaaf-114">Permission type</span></span>      | <span data-ttu-id="bcaaf-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcaaf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcaaf-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcaaf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bcaaf-117">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="bcaaf-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcaaf-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcaaf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcaaf-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-119">Not supported.</span></span>    |
|<span data-ttu-id="bcaaf-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcaaf-120">Application</span></span> | <span data-ttu-id="bcaaf-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcaaf-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcaaf-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcaaf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="bcaaf-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcaaf-123">Request headers</span></span>

| <span data-ttu-id="bcaaf-124">标头</span><span class="sxs-lookup"><span data-stu-id="bcaaf-124">Header</span></span>       | <span data-ttu-id="bcaaf-125">值</span><span class="sxs-lookup"><span data-stu-id="bcaaf-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcaaf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcaaf-126">Authorization</span></span>  | <span data-ttu-id="bcaaf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bcaaf-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcaaf-129">Content-Type</span></span>  | <span data-ttu-id="bcaaf-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bcaaf-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcaaf-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcaaf-132">Request body</span></span>

<span data-ttu-id="bcaaf-133">在请求正文中，提供 [schedule](../resources/schedule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcaaf-134">响应</span><span class="sxs-lookup"><span data-stu-id="bcaaf-134">Response</span></span>

<span data-ttu-id="bcaaf-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [schedule](../resources/schedule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcaaf-136">示例</span><span class="sxs-lookup"><span data-stu-id="bcaaf-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bcaaf-137">请求</span><span class="sxs-lookup"><span data-stu-id="bcaaf-137">Request</span></span>

<span data-ttu-id="bcaaf-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcaaf-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcaaf-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bcaaf-140">C#</span><span class="sxs-lookup"><span data-stu-id="bcaaf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcaaf-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcaaf-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcaaf-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcaaf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcaaf-143">Java</span><span class="sxs-lookup"><span data-stu-id="bcaaf-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-put-schedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bcaaf-144">响应</span><span class="sxs-lookup"><span data-stu-id="bcaaf-144">Response</span></span>

<span data-ttu-id="bcaaf-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-145">The following is an example of the response.</span></span> 

><span data-ttu-id="bcaaf-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bcaaf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


