---
title: 获取日程安排
description: 检索**schedule**对象的属性和关系。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b953e911ba834b9707df33926e4a2a355653dcb3
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845881"
---
# <a name="get-schedule"></a><span data-ttu-id="0313e-103">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="0313e-103">Get schedule</span></span>

<span data-ttu-id="0313e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0313e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0313e-105">检索[schedule](../resources/schedule.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0313e-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="0313e-106">计划创建过程符合[基于资源的长时间运行的操作（RELO）的一个 API 指南](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。</span><span class="sxs-lookup"><span data-stu-id="0313e-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="0313e-107">当客户端使用[PUT 方法](team-put-schedule.md)时，如果设置了计划，该操作将更新计划;否则，该操作将在后台启动计划设置过程。</span><span class="sxs-lookup"><span data-stu-id="0313e-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="0313e-108">在计划设置过程中，客户端可以使用 GET 方法获取计划，并查看 `provisionStatus` 设置的当前状态的属性。</span><span class="sxs-lookup"><span data-stu-id="0313e-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="0313e-109">如果设置失败，客户端可以从属性获取其他信息 `provisionStatusCode` 。</span><span class="sxs-lookup"><span data-stu-id="0313e-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="0313e-110">客户端也可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="0313e-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="0313e-111">权限</span><span class="sxs-lookup"><span data-stu-id="0313e-111">Permissions</span></span>

<span data-ttu-id="0313e-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0313e-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0313e-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0313e-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0313e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0313e-114">Permission type</span></span>                        | <span data-ttu-id="0313e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0313e-115">Permissions (from least to most privileged)</span></span>                                    |
|:---------------------------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="0313e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0313e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0313e-117">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="0313e-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0313e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0313e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0313e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0313e-119">Not supported.</span></span>                                                                 |
| <span data-ttu-id="0313e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0313e-120">Application</span></span>                            | <span data-ttu-id="0313e-121">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="0313e-121">Schedule.Read.All, Schedule.ReadWrite.All</span></span>                                      |

> <span data-ttu-id="0313e-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0313e-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0313e-123">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="0313e-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0313e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0313e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0313e-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0313e-125">Optional query parameters</span></span>

<span data-ttu-id="0313e-126">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0313e-126">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0313e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0313e-127">Request headers</span></span>

| <span data-ttu-id="0313e-128">标头</span><span class="sxs-lookup"><span data-stu-id="0313e-128">Header</span></span>       | <span data-ttu-id="0313e-129">值</span><span class="sxs-lookup"><span data-stu-id="0313e-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0313e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0313e-130">Authorization</span></span>  | <span data-ttu-id="0313e-131">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0313e-131">Bearer {token}.</span></span> <span data-ttu-id="0313e-132">Required.</span><span class="sxs-lookup"><span data-stu-id="0313e-132">Required.</span></span>  |
| <span data-ttu-id="0313e-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0313e-133">Content-Type</span></span>  | <span data-ttu-id="0313e-134">application/json.</span><span class="sxs-lookup"><span data-stu-id="0313e-134">application/json.</span></span> <span data-ttu-id="0313e-135">Required.</span><span class="sxs-lookup"><span data-stu-id="0313e-135">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0313e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="0313e-136">Request body</span></span>
<span data-ttu-id="0313e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0313e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0313e-138">响应</span><span class="sxs-lookup"><span data-stu-id="0313e-138">Response</span></span>

<span data-ttu-id="0313e-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0313e-139">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0313e-140">示例</span><span class="sxs-lookup"><span data-stu-id="0313e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0313e-141">请求</span><span class="sxs-lookup"><span data-stu-id="0313e-141">Request</span></span>

<span data-ttu-id="0313e-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0313e-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0313e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0313e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="0313e-144">C#</span><span class="sxs-lookup"><span data-stu-id="0313e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0313e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0313e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0313e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0313e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0313e-147">Java</span><span class="sxs-lookup"><span data-stu-id="0313e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="0313e-148">响应</span><span class="sxs-lookup"><span data-stu-id="0313e-148">Response</span></span>

<span data-ttu-id="0313e-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0313e-149">The following is an example of the response.</span></span>

><span data-ttu-id="0313e-150">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0313e-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0313e-151">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0313e-151">All the properties will be returned from an actual call.</span></span>
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
