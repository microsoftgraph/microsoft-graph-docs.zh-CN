---
title: 创建或替换计划
description: 创建或替换**schedule**对象。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 84d34de6a0410e1372950688c610e6ed7c2e3554
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330521"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="a369b-103">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="a369b-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a369b-104">创建或替换[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a369b-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="a369b-105">计划创建过程符合[基于资源的长时间运行的操作 (RELO) 的一个 API 指南](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。</span><span class="sxs-lookup"><span data-stu-id="a369b-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="a369b-106">当客户端使用 PUT 方法时, 如果设置了计划, 则操作将替换计划;否则, 该操作将在后台启动计划设置过程。</span><span class="sxs-lookup"><span data-stu-id="a369b-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="a369b-107">在计划设置过程中, 客户端可以使用[get 方法](schedule-get.md)获取计划, 并查看设置`provisionStatus`的当前状态的属性。</span><span class="sxs-lookup"><span data-stu-id="a369b-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="a369b-108">如果设置失败, 客户端可以从`provisionStatusCode`属性获取其他信息。</span><span class="sxs-lookup"><span data-stu-id="a369b-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="a369b-109">客户端也可以检查计划的配置。</span><span class="sxs-lookup"><span data-stu-id="a369b-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="a369b-110">权限</span><span class="sxs-lookup"><span data-stu-id="a369b-110">Permissions</span></span>

<span data-ttu-id="a369b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a369b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a369b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a369b-113">Permission type</span></span>      | <span data-ttu-id="a369b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a369b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a369b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a369b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a369b-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a369b-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a369b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a369b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a369b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a369b-118">Not supported.</span></span>    |
|<span data-ttu-id="a369b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a369b-119">Application</span></span> | <span data-ttu-id="a369b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="a369b-120">Not supported.</span></span> |

> <span data-ttu-id="a369b-121">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a369b-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a369b-122">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a369b-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a369b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a369b-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="a369b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a369b-124">Request headers</span></span>

| <span data-ttu-id="a369b-125">标头</span><span class="sxs-lookup"><span data-stu-id="a369b-125">Header</span></span>       | <span data-ttu-id="a369b-126">值</span><span class="sxs-lookup"><span data-stu-id="a369b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a369b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a369b-127">Authorization</span></span>  | <span data-ttu-id="a369b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a369b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a369b-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a369b-130">Content-Type</span></span>  | <span data-ttu-id="a369b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a369b-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a369b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a369b-132">Request body</span></span>

<span data-ttu-id="a369b-133">在请求正文中, 提供[schedule](../resources/schedule.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a369b-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a369b-134">响应</span><span class="sxs-lookup"><span data-stu-id="a369b-134">Response</span></span>

<span data-ttu-id="a369b-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[schedule](../resources/schedule.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a369b-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a369b-136">示例</span><span class="sxs-lookup"><span data-stu-id="a369b-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a369b-137">请求</span><span class="sxs-lookup"><span data-stu-id="a369b-137">Request</span></span>

<span data-ttu-id="a369b-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a369b-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a369b-139">响应</span><span class="sxs-lookup"><span data-stu-id="a369b-139">Response</span></span>

<span data-ttu-id="a369b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a369b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="a369b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a369b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "provisionStatusCode": null
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
  "suppressions": []
}
-->
