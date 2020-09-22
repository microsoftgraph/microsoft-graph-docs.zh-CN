---
title: openShiftChangeRequest：拒绝
description: 拒绝 openShiftChangeRequest。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dcdc94950ace03452c3e1781b230b01ae0a4db5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059353"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="f0244-103">openShiftChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="f0244-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="f0244-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0244-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0244-105">拒绝 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0244-105">Decline an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0244-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0244-106">Permissions</span></span>

<span data-ttu-id="f0244-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0244-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0244-109">Permission type</span></span>                        | <span data-ttu-id="f0244-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0244-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0244-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0244-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0244-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="f0244-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f0244-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0244-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0244-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0244-114">Not supported.</span></span> |
| <span data-ttu-id="f0244-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0244-115">Application</span></span>                            | <span data-ttu-id="f0244-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0244-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f0244-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="f0244-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f0244-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="f0244-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f0244-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0244-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="f0244-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0244-120">Request headers</span></span>

| <span data-ttu-id="f0244-121">名称</span><span class="sxs-lookup"><span data-stu-id="f0244-121">Name</span></span>          | <span data-ttu-id="f0244-122">说明</span><span class="sxs-lookup"><span data-stu-id="f0244-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f0244-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0244-123">Authorization</span></span> | <span data-ttu-id="f0244-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0244-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0244-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f0244-126">Content-type</span></span> | <span data-ttu-id="f0244-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f0244-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0244-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0244-129">Request body</span></span>

<span data-ttu-id="f0244-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f0244-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0244-131">参数</span><span class="sxs-lookup"><span data-stu-id="f0244-131">Parameter</span></span>    | <span data-ttu-id="f0244-132">类型</span><span class="sxs-lookup"><span data-stu-id="f0244-132">Type</span></span>        | <span data-ttu-id="f0244-133">描述</span><span class="sxs-lookup"><span data-stu-id="f0244-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0244-134">message</span><span class="sxs-lookup"><span data-stu-id="f0244-134">message</span></span>|<span data-ttu-id="f0244-135">String</span><span class="sxs-lookup"><span data-stu-id="f0244-135">String</span></span>|<span data-ttu-id="f0244-136">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="f0244-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="f0244-137">响应</span><span class="sxs-lookup"><span data-stu-id="f0244-137">Response</span></span>

<span data-ttu-id="f0244-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f0244-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0244-140">示例</span><span class="sxs-lookup"><span data-stu-id="f0244-140">Examples</span></span>

<span data-ttu-id="f0244-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f0244-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f0244-142">请求</span><span class="sxs-lookup"><span data-stu-id="f0244-142">Request</span></span>

<span data-ttu-id="f0244-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0244-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="f0244-144">响应</span><span class="sxs-lookup"><span data-stu-id="f0244-144">Response</span></span>

<span data-ttu-id="f0244-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0244-145">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

