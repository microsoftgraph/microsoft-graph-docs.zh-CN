---
title: openShiftChangeRequest：批准
description: 批准 openshift 请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1301a975dcf858ff1d6f65beb1665d3ca5933de6
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219683"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="cc7bf-103">openShiftChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="cc7bf-103">openShiftChangeRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc7bf-104">批准[openshiftchangerequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-104">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc7bf-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="cc7bf-105">Permissions</span></span>

<span data-ttu-id="cc7bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc7bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc7bf-108">Permission type</span></span>                        | <span data-ttu-id="cc7bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc7bf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc7bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc7bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc7bf-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7bf-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cc7bf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc7bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc7bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-113">Not supported.</span></span> |
| <span data-ttu-id="cc7bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc7bf-114">Application</span></span>                            | <span data-ttu-id="cc7bf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc7bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc7bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="cc7bf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc7bf-117">Request headers</span></span>

| <span data-ttu-id="cc7bf-118">名称</span><span class="sxs-lookup"><span data-stu-id="cc7bf-118">Name</span></span>          | <span data-ttu-id="cc7bf-119">说明</span><span class="sxs-lookup"><span data-stu-id="cc7bf-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cc7bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc7bf-120">Authorization</span></span> | <span data-ttu-id="cc7bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc7bf-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc7bf-123">Content-type</span></span> | <span data-ttu-id="cc7bf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc7bf-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc7bf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc7bf-126">Request body</span></span>

<span data-ttu-id="cc7bf-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc7bf-128">参数</span><span class="sxs-lookup"><span data-stu-id="cc7bf-128">Parameter</span></span>    | <span data-ttu-id="cc7bf-129">类型</span><span class="sxs-lookup"><span data-stu-id="cc7bf-129">Type</span></span>        | <span data-ttu-id="cc7bf-130">描述</span><span class="sxs-lookup"><span data-stu-id="cc7bf-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc7bf-131">message</span><span class="sxs-lookup"><span data-stu-id="cc7bf-131">message</span></span>|<span data-ttu-id="cc7bf-132">String</span><span class="sxs-lookup"><span data-stu-id="cc7bf-132">String</span></span>|<span data-ttu-id="cc7bf-133">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-133">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="cc7bf-134">响应</span><span class="sxs-lookup"><span data-stu-id="cc7bf-134">Response</span></span>

<span data-ttu-id="cc7bf-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc7bf-137">示例</span><span class="sxs-lookup"><span data-stu-id="cc7bf-137">Examples</span></span>

<span data-ttu-id="cc7bf-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cc7bf-139">请求</span><span class="sxs-lookup"><span data-stu-id="cc7bf-139">Request</span></span>

<span data-ttu-id="cc7bf-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-140">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc7bf-141">响应</span><span class="sxs-lookup"><span data-stu-id="cc7bf-141">Response</span></span>

<span data-ttu-id="cc7bf-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc7bf-142">The following is an example of the response.</span></span>
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
