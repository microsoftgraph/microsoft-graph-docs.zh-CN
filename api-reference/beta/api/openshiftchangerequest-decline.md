---
title: openShiftChangeRequest： decline
description: 拒绝开放临时请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 766faedd7fb46fb3cd6cf8434c2987e26a0ba96b
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292439"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="1ab39-103">openShiftChangeRequest： decline</span><span class="sxs-lookup"><span data-stu-id="1ab39-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="1ab39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ab39-105">拒绝 [openshiftchangerequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ab39-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ab39-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ab39-106">Permissions</span></span>

<span data-ttu-id="1ab39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ab39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ab39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ab39-109">Permission type</span></span>                        | <span data-ttu-id="1ab39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ab39-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ab39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ab39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ab39-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab39-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1ab39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ab39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ab39-114">Not supported.</span></span> |
| <span data-ttu-id="1ab39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ab39-115">Application</span></span>                            | <span data-ttu-id="1ab39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ab39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ab39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ab39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="1ab39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ab39-118">Request headers</span></span>

| <span data-ttu-id="1ab39-119">名称</span><span class="sxs-lookup"><span data-stu-id="1ab39-119">Name</span></span>          | <span data-ttu-id="1ab39-120">说明</span><span class="sxs-lookup"><span data-stu-id="1ab39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1ab39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ab39-121">Authorization</span></span> | <span data-ttu-id="1ab39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ab39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ab39-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ab39-124">Request body</span></span>

<span data-ttu-id="1ab39-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1ab39-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1ab39-126">参数</span><span class="sxs-lookup"><span data-stu-id="1ab39-126">Parameter</span></span>    | <span data-ttu-id="1ab39-127">类型</span><span class="sxs-lookup"><span data-stu-id="1ab39-127">Type</span></span>        | <span data-ttu-id="1ab39-128">描述</span><span class="sxs-lookup"><span data-stu-id="1ab39-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ab39-129">message</span><span class="sxs-lookup"><span data-stu-id="1ab39-129">message</span></span>|<span data-ttu-id="1ab39-130">String</span><span class="sxs-lookup"><span data-stu-id="1ab39-130">String</span></span>|<span data-ttu-id="1ab39-131">自定义拒绝消息。</span><span class="sxs-lookup"><span data-stu-id="1ab39-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="1ab39-132">响应</span><span class="sxs-lookup"><span data-stu-id="1ab39-132">Response</span></span>

<span data-ttu-id="1ab39-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1ab39-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ab39-135">示例</span><span class="sxs-lookup"><span data-stu-id="1ab39-135">Examples</span></span>

<span data-ttu-id="1ab39-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1ab39-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1ab39-137">请求</span><span class="sxs-lookup"><span data-stu-id="1ab39-137">Request</span></span>

<span data-ttu-id="1ab39-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ab39-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="1ab39-139">响应</span><span class="sxs-lookup"><span data-stu-id="1ab39-139">Response</span></span>

<span data-ttu-id="1ab39-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ab39-140">The following is an example of the response.</span></span>
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


