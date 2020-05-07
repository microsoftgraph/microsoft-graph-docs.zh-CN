---
title: timeOffRequest：批准
description: 批准 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d61c0debe7420591d862727f0c8db46ecbeb54a9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154996"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="645a3-103">timeOffRequest：批准</span><span class="sxs-lookup"><span data-stu-id="645a3-103">timeOffRequest: approve</span></span>

<span data-ttu-id="645a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="645a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="645a3-105">批准[timeoffrequest](../resources/timeoffrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="645a3-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="645a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="645a3-106">Permissions</span></span>

<span data-ttu-id="645a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="645a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="645a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="645a3-109">Permission type</span></span>                        | <span data-ttu-id="645a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="645a3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="645a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="645a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="645a3-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="645a3-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="645a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="645a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="645a3-114">Not supported.</span></span>    |
|<span data-ttu-id="645a3-115">Application</span><span class="sxs-lookup"><span data-stu-id="645a3-115">Application</span></span> | <span data-ttu-id="645a3-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645a3-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="645a3-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="645a3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="645a3-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="645a3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="645a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="645a3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="645a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="645a3-120">Request headers</span></span>

| <span data-ttu-id="645a3-121">名称</span><span class="sxs-lookup"><span data-stu-id="645a3-121">Name</span></span>          | <span data-ttu-id="645a3-122">说明</span><span class="sxs-lookup"><span data-stu-id="645a3-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="645a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="645a3-123">Authorization</span></span> | <span data-ttu-id="645a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="645a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="645a3-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="645a3-126">Content-type</span></span> | <span data-ttu-id="645a3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="645a3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="645a3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="645a3-129">Request body</span></span>

<span data-ttu-id="645a3-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="645a3-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="645a3-131">参数</span><span class="sxs-lookup"><span data-stu-id="645a3-131">Parameter</span></span>    | <span data-ttu-id="645a3-132">类型</span><span class="sxs-lookup"><span data-stu-id="645a3-132">Type</span></span>        | <span data-ttu-id="645a3-133">描述</span><span class="sxs-lookup"><span data-stu-id="645a3-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="645a3-134">message</span><span class="sxs-lookup"><span data-stu-id="645a3-134">message</span></span>|<span data-ttu-id="645a3-135">String</span><span class="sxs-lookup"><span data-stu-id="645a3-135">String</span></span>|<span data-ttu-id="645a3-136">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="645a3-136">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="645a3-137">响应</span><span class="sxs-lookup"><span data-stu-id="645a3-137">Response</span></span>

<span data-ttu-id="645a3-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="645a3-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="645a3-140">示例</span><span class="sxs-lookup"><span data-stu-id="645a3-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="645a3-141">请求</span><span class="sxs-lookup"><span data-stu-id="645a3-141">Request</span></span>

<span data-ttu-id="645a3-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="645a3-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
---


### <a name="response"></a><span data-ttu-id="645a3-143">响应</span><span class="sxs-lookup"><span data-stu-id="645a3-143">Response</span></span>

<span data-ttu-id="645a3-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="645a3-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
