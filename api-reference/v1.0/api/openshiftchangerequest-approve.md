---
title: openShiftChangeRequest： approve
description: 批准 openShiftChangeRequest 请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b6adfeb7cd69ba90b79aea5c1ec3108c3fd6085
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292397"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="0883e-103">openShiftChangeRequest： approve</span><span class="sxs-lookup"><span data-stu-id="0883e-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="0883e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0883e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0883e-105">批准 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0883e-105">Approve an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0883e-106">权限</span><span class="sxs-lookup"><span data-stu-id="0883e-106">Permissions</span></span>

<span data-ttu-id="0883e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0883e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0883e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0883e-109">Permission type</span></span>                        | <span data-ttu-id="0883e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0883e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0883e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0883e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0883e-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0883e-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0883e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0883e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0883e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0883e-114">Not supported.</span></span> |
| <span data-ttu-id="0883e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0883e-115">Application</span></span>                            | <span data-ttu-id="0883e-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0883e-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="0883e-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0883e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0883e-118">全局管理员可以访问不是其成员组的组。</span><span class="sxs-lookup"><span data-stu-id="0883e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0883e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0883e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="0883e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0883e-120">Request headers</span></span>

| <span data-ttu-id="0883e-121">名称</span><span class="sxs-lookup"><span data-stu-id="0883e-121">Name</span></span>          | <span data-ttu-id="0883e-122">说明</span><span class="sxs-lookup"><span data-stu-id="0883e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0883e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0883e-123">Authorization</span></span> | <span data-ttu-id="0883e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0883e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0883e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="0883e-126">Content-type</span></span> | <span data-ttu-id="0883e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0883e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0883e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0883e-129">Request body</span></span>

<span data-ttu-id="0883e-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0883e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0883e-131">参数</span><span class="sxs-lookup"><span data-stu-id="0883e-131">Parameter</span></span>    | <span data-ttu-id="0883e-132">类型</span><span class="sxs-lookup"><span data-stu-id="0883e-132">Type</span></span>        | <span data-ttu-id="0883e-133">描述</span><span class="sxs-lookup"><span data-stu-id="0883e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0883e-134">message</span><span class="sxs-lookup"><span data-stu-id="0883e-134">message</span></span>|<span data-ttu-id="0883e-135">String</span><span class="sxs-lookup"><span data-stu-id="0883e-135">String</span></span>|<span data-ttu-id="0883e-136">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="0883e-136">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="0883e-137">响应</span><span class="sxs-lookup"><span data-stu-id="0883e-137">Response</span></span>

<span data-ttu-id="0883e-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0883e-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0883e-140">示例</span><span class="sxs-lookup"><span data-stu-id="0883e-140">Examples</span></span>

<span data-ttu-id="0883e-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0883e-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0883e-142">请求</span><span class="sxs-lookup"><span data-stu-id="0883e-142">Request</span></span>

<span data-ttu-id="0883e-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0883e-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="0883e-144">响应</span><span class="sxs-lookup"><span data-stu-id="0883e-144">Response</span></span>

<span data-ttu-id="0883e-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0883e-145">The following is an example of the response.</span></span>
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

