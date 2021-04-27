---
title: 获取日程安排
description: 检索 schedule 对象的属性 **和** 关系。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e0bcc91939ac53adbefe16a97986239fec955ab3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049035"
---
# <a name="get-schedule"></a><span data-ttu-id="cb7d9-103">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="cb7d9-103">Get schedule</span></span>

<span data-ttu-id="cb7d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb7d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb7d9-105">检索 schedule 对象的属性 [和](../resources/schedule.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="cb7d9-106">计划创建过程符合针对基于资源的长时间运行的操作的 One API 准则 ([RELO) 。 ](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)</span><span class="sxs-lookup"><span data-stu-id="cb7d9-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="cb7d9-107">当客户端使用 [PUT 方法时](team-put-schedule.md)，如果已设置计划，则操作将更新计划;否则，操作将在后台启动计划预配过程。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="cb7d9-108">在计划预配期间，客户端可以使用 GET 方法获取计划并查看 属性，了解 `provisionStatus` 预配的当前状态。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="cb7d9-109">如果设置失败，客户端可以从 属性获取其他 `provisionStatusCode` 信息。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="cb7d9-110">客户端还可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb7d9-111">权限</span><span class="sxs-lookup"><span data-stu-id="cb7d9-111">Permissions</span></span>

<span data-ttu-id="cb7d9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb7d9-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb7d9-114">Permission type</span></span>      | <span data-ttu-id="cb7d9-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb7d9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb7d9-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb7d9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cb7d9-117">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb7d9-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb7d9-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb7d9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb7d9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-119">Not supported.</span></span>    |
|<span data-ttu-id="cb7d9-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb7d9-120">Application</span></span> | <span data-ttu-id="cb7d9-121">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb7d9-121">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb7d9-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb7d9-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb7d9-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb7d9-123">Optional query parameters</span></span>

<span data-ttu-id="cb7d9-124">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-124">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb7d9-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb7d9-125">Request headers</span></span>

| <span data-ttu-id="cb7d9-126">标头</span><span class="sxs-lookup"><span data-stu-id="cb7d9-126">Header</span></span>       | <span data-ttu-id="cb7d9-127">值</span><span class="sxs-lookup"><span data-stu-id="cb7d9-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb7d9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb7d9-128">Authorization</span></span>  | <span data-ttu-id="cb7d9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb7d9-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb7d9-131">Content-Type</span></span>  | <span data-ttu-id="cb7d9-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb7d9-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb7d9-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb7d9-134">Request body</span></span>
<span data-ttu-id="cb7d9-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb7d9-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb7d9-136">Response</span></span>

<span data-ttu-id="cb7d9-137">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/schedule.md) 代码和 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb7d9-138">示例</span><span class="sxs-lookup"><span data-stu-id="cb7d9-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cb7d9-139">请求</span><span class="sxs-lookup"><span data-stu-id="cb7d9-139">Request</span></span>

<span data-ttu-id="cb7d9-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb7d9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb7d9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="cb7d9-142">C#</span><span class="sxs-lookup"><span data-stu-id="cb7d9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb7d9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb7d9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb7d9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb7d9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb7d9-145">Java</span><span class="sxs-lookup"><span data-stu-id="cb7d9-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb7d9-146">响应</span><span class="sxs-lookup"><span data-stu-id="cb7d9-146">Response</span></span>

<span data-ttu-id="cb7d9-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-147">The following is an example of the response.</span></span> 

><span data-ttu-id="cb7d9-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb7d9-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


