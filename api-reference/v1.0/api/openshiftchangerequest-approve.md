---
title: openShiftChangeRequest：批准
description: 批准 openShiftChangeRequest 请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 148b4c52a6f288d961c949cc0d599cb468c8b322
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155066"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="4bc5f-103">openShiftChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="4bc5f-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="4bc5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bc5f-105">批准[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-105">Approve an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bc5f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4bc5f-106">Permissions</span></span>

<span data-ttu-id="4bc5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bc5f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bc5f-109">Permission type</span></span>                        | <span data-ttu-id="4bc5f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bc5f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bc5f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc5f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bc5f-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="4bc5f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4bc5f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc5f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-114">Not supported.</span></span> |
| <span data-ttu-id="4bc5f-115">Application</span><span class="sxs-lookup"><span data-stu-id="4bc5f-115">Application</span></span>                            | <span data-ttu-id="4bc5f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc5f-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="4bc5f-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4bc5f-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4bc5f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bc5f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="4bc5f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bc5f-120">Request headers</span></span>

| <span data-ttu-id="4bc5f-121">名称</span><span class="sxs-lookup"><span data-stu-id="4bc5f-121">Name</span></span>          | <span data-ttu-id="4bc5f-122">说明</span><span class="sxs-lookup"><span data-stu-id="4bc5f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4bc5f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc5f-123">Authorization</span></span> | <span data-ttu-id="4bc5f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bc5f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4bc5f-126">Content-type</span></span> | <span data-ttu-id="4bc5f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4bc5f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bc5f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bc5f-129">Request body</span></span>

<span data-ttu-id="4bc5f-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bc5f-131">参数</span><span class="sxs-lookup"><span data-stu-id="4bc5f-131">Parameter</span></span>    | <span data-ttu-id="4bc5f-132">类型</span><span class="sxs-lookup"><span data-stu-id="4bc5f-132">Type</span></span>        | <span data-ttu-id="4bc5f-133">描述</span><span class="sxs-lookup"><span data-stu-id="4bc5f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4bc5f-134">message</span><span class="sxs-lookup"><span data-stu-id="4bc5f-134">message</span></span>|<span data-ttu-id="4bc5f-135">String</span><span class="sxs-lookup"><span data-stu-id="4bc5f-135">String</span></span>|<span data-ttu-id="4bc5f-136">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-136">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="4bc5f-137">响应</span><span class="sxs-lookup"><span data-stu-id="4bc5f-137">Response</span></span>

<span data-ttu-id="4bc5f-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bc5f-140">示例</span><span class="sxs-lookup"><span data-stu-id="4bc5f-140">Examples</span></span>

<span data-ttu-id="4bc5f-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4bc5f-142">请求</span><span class="sxs-lookup"><span data-stu-id="4bc5f-142">Request</span></span>

<span data-ttu-id="4bc5f-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="4bc5f-144">响应</span><span class="sxs-lookup"><span data-stu-id="4bc5f-144">Response</span></span>

<span data-ttu-id="4bc5f-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bc5f-145">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
