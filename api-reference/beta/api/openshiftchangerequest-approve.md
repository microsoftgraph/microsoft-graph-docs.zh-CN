---
title: openShiftChangeRequest：批准
description: 批准 openshift 请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0a088e12c41d349806ad142013dd01c40c00f080
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456395"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="5562d-103">openShiftChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="5562d-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="5562d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5562d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5562d-105">批准[openshiftchangerequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5562d-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5562d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5562d-106">Permissions</span></span>

<span data-ttu-id="5562d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5562d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5562d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5562d-109">Permission type</span></span>                        | <span data-ttu-id="5562d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5562d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5562d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5562d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5562d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5562d-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5562d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5562d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5562d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5562d-114">Not supported.</span></span> |
| <span data-ttu-id="5562d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5562d-115">Application</span></span>                            | <span data-ttu-id="5562d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5562d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5562d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5562d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="5562d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5562d-118">Request headers</span></span>

| <span data-ttu-id="5562d-119">名称</span><span class="sxs-lookup"><span data-stu-id="5562d-119">Name</span></span>          | <span data-ttu-id="5562d-120">说明</span><span class="sxs-lookup"><span data-stu-id="5562d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5562d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5562d-121">Authorization</span></span> | <span data-ttu-id="5562d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5562d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5562d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5562d-124">Content-type</span></span> | <span data-ttu-id="5562d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5562d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5562d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5562d-127">Request body</span></span>

<span data-ttu-id="5562d-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5562d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5562d-129">参数</span><span class="sxs-lookup"><span data-stu-id="5562d-129">Parameter</span></span>    | <span data-ttu-id="5562d-130">类型</span><span class="sxs-lookup"><span data-stu-id="5562d-130">Type</span></span>        | <span data-ttu-id="5562d-131">描述</span><span class="sxs-lookup"><span data-stu-id="5562d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5562d-132">message</span><span class="sxs-lookup"><span data-stu-id="5562d-132">message</span></span>|<span data-ttu-id="5562d-133">String</span><span class="sxs-lookup"><span data-stu-id="5562d-133">String</span></span>|<span data-ttu-id="5562d-134">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="5562d-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="5562d-135">响应</span><span class="sxs-lookup"><span data-stu-id="5562d-135">Response</span></span>

<span data-ttu-id="5562d-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5562d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5562d-138">示例</span><span class="sxs-lookup"><span data-stu-id="5562d-138">Examples</span></span>

<span data-ttu-id="5562d-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5562d-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5562d-140">请求</span><span class="sxs-lookup"><span data-stu-id="5562d-140">Request</span></span>

<span data-ttu-id="5562d-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5562d-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="5562d-142">响应</span><span class="sxs-lookup"><span data-stu-id="5562d-142">Response</span></span>

<span data-ttu-id="5562d-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5562d-143">The following is an example of the response.</span></span>
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
