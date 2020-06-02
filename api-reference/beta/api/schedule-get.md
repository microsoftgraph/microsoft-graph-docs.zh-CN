---
title: 获取日程安排
description: 检索**schedule**对象的属性和关系。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 705c42339dc64ff66f89ce72715d51a6753357d0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154246"
---
# <a name="get-schedule"></a><span data-ttu-id="a1088-103">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="a1088-103">Get schedule</span></span>

<span data-ttu-id="a1088-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1088-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1088-105">检索[schedule](../resources/schedule.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1088-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="a1088-106">计划创建过程符合[基于资源的长时间运行的操作（RELO）的一个 API 指南](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。</span><span class="sxs-lookup"><span data-stu-id="a1088-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="a1088-107">当客户端使用[PUT 方法](team-put-schedule.md)时，如果设置了计划，该操作将更新计划;否则，该操作将在后台启动计划设置过程。</span><span class="sxs-lookup"><span data-stu-id="a1088-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="a1088-108">在计划设置过程中，客户端可以使用 GET 方法获取计划，并查看 `provisionStatus` 设置的当前状态的属性。</span><span class="sxs-lookup"><span data-stu-id="a1088-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="a1088-109">如果设置失败，客户端可以从属性获取其他信息 `provisionStatusCode` 。</span><span class="sxs-lookup"><span data-stu-id="a1088-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="a1088-110">客户端也可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="a1088-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1088-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="a1088-111">Permissions</span></span>

<span data-ttu-id="a1088-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1088-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1088-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1088-114">Permission type</span></span>      | <span data-ttu-id="a1088-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1088-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1088-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1088-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a1088-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1088-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1088-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1088-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1088-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1088-119">Not supported.</span></span>    |
|<span data-ttu-id="a1088-120">Application</span><span class="sxs-lookup"><span data-stu-id="a1088-120">Application</span></span> | <span data-ttu-id="a1088-121">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="a1088-121">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="a1088-122">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="a1088-122">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="a1088-123">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a1088-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a1088-124">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a1088-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a1088-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1088-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1088-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1088-126">Optional query parameters</span></span>

<span data-ttu-id="a1088-127">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1088-127">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1088-128">请求头</span><span class="sxs-lookup"><span data-stu-id="a1088-128">Request headers</span></span>

| <span data-ttu-id="a1088-129">标头</span><span class="sxs-lookup"><span data-stu-id="a1088-129">Header</span></span>       | <span data-ttu-id="a1088-130">值</span><span class="sxs-lookup"><span data-stu-id="a1088-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1088-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1088-131">Authorization</span></span>  | <span data-ttu-id="a1088-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1088-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1088-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1088-134">Content-Type</span></span>  | <span data-ttu-id="a1088-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a1088-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1088-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1088-137">Request body</span></span>
<span data-ttu-id="a1088-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1088-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1088-139">响应</span><span class="sxs-lookup"><span data-stu-id="a1088-139">Response</span></span>

<span data-ttu-id="a1088-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1088-140">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1088-141">示例</span><span class="sxs-lookup"><span data-stu-id="a1088-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a1088-142">请求</span><span class="sxs-lookup"><span data-stu-id="a1088-142">Request</span></span>

<span data-ttu-id="a1088-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1088-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1088-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1088-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="a1088-145">C#</span><span class="sxs-lookup"><span data-stu-id="a1088-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1088-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1088-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1088-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1088-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a1088-148">响应</span><span class="sxs-lookup"><span data-stu-id="a1088-148">Response</span></span>

<span data-ttu-id="a1088-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1088-149">The following is an example of the response.</span></span> 

><span data-ttu-id="a1088-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a1088-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
