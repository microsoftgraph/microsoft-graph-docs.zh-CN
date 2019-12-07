---
title: openShiftChangeRequest：拒绝
description: 拒绝 openshift 请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9fa98977d06d2eb3e1f2993779f2390bc364780c
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895600"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="8c3d1-103">openShiftChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="8c3d1-103">openShiftChangeRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c3d1-104">拒绝[openshiftchangerequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-104">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c3d1-105">权限</span><span class="sxs-lookup"><span data-stu-id="8c3d1-105">Permissions</span></span>

<span data-ttu-id="8c3d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c3d1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c3d1-108">Permission type</span></span>                        | <span data-ttu-id="8c3d1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c3d1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c3d1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c3d1-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3d1-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8c3d1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c3d1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-113">Not supported.</span></span> |
| <span data-ttu-id="8c3d1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c3d1-114">Application</span></span>                            | <span data-ttu-id="8c3d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c3d1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c3d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="8c3d1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c3d1-117">Request headers</span></span>

| <span data-ttu-id="8c3d1-118">名称</span><span class="sxs-lookup"><span data-stu-id="8c3d1-118">Name</span></span>          | <span data-ttu-id="8c3d1-119">说明</span><span class="sxs-lookup"><span data-stu-id="8c3d1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8c3d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c3d1-120">Authorization</span></span> | <span data-ttu-id="8c3d1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c3d1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c3d1-123">Request body</span></span>

<span data-ttu-id="8c3d1-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c3d1-125">参数</span><span class="sxs-lookup"><span data-stu-id="8c3d1-125">Parameter</span></span>    | <span data-ttu-id="8c3d1-126">类型</span><span class="sxs-lookup"><span data-stu-id="8c3d1-126">Type</span></span>        | <span data-ttu-id="8c3d1-127">描述</span><span class="sxs-lookup"><span data-stu-id="8c3d1-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c3d1-128">message</span><span class="sxs-lookup"><span data-stu-id="8c3d1-128">message</span></span>|<span data-ttu-id="8c3d1-129">String</span><span class="sxs-lookup"><span data-stu-id="8c3d1-129">String</span></span>|<span data-ttu-id="8c3d1-130">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-130">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8c3d1-131">响应</span><span class="sxs-lookup"><span data-stu-id="8c3d1-131">Response</span></span>

<span data-ttu-id="8c3d1-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c3d1-134">示例</span><span class="sxs-lookup"><span data-stu-id="8c3d1-134">Examples</span></span>

<span data-ttu-id="8c3d1-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8c3d1-136">请求</span><span class="sxs-lookup"><span data-stu-id="8c3d1-136">Request</span></span>

<span data-ttu-id="8c3d1-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="8c3d1-138">响应</span><span class="sxs-lookup"><span data-stu-id="8c3d1-138">Response</span></span>

<span data-ttu-id="8c3d1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c3d1-139">The following is an example of the response.</span></span>
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
