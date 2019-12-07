---
title: timeOffRequest：拒绝
description: 拒绝 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0c73a983094ffae12980eeda9a12681ec9e90cb
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895577"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="8f9e7-103">timeOffRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="8f9e7-103">timeOffRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f9e7-104">拒绝[timeoffrequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-104">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f9e7-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f9e7-105">Permissions</span></span>

<span data-ttu-id="8f9e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f9e7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f9e7-108">Permission type</span></span>                        | <span data-ttu-id="8f9e7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f9e7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f9e7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f9e7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f9e7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f9e7-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8f9e7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f9e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f9e7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-113">Not supported.</span></span> |
| <span data-ttu-id="8f9e7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f9e7-114">Application</span></span>                            | <span data-ttu-id="8f9e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f9e7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f9e7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="8f9e7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f9e7-117">Request headers</span></span>

| <span data-ttu-id="8f9e7-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f9e7-118">Name</span></span>          | <span data-ttu-id="8f9e7-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f9e7-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f9e7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f9e7-120">Authorization</span></span> | <span data-ttu-id="8f9e7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f9e7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8f9e7-123">Content-type</span></span> | <span data-ttu-id="8f9e7-124">application-json。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-124">application-json.</span></span> <span data-ttu-id="8f9e7-125">必需。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f9e7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f9e7-126">Request body</span></span>

<span data-ttu-id="8f9e7-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f9e7-128">参数</span><span class="sxs-lookup"><span data-stu-id="8f9e7-128">Parameter</span></span>    | <span data-ttu-id="8f9e7-129">类型</span><span class="sxs-lookup"><span data-stu-id="8f9e7-129">Type</span></span>        | <span data-ttu-id="8f9e7-130">描述</span><span class="sxs-lookup"><span data-stu-id="8f9e7-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f9e7-131">message</span><span class="sxs-lookup"><span data-stu-id="8f9e7-131">message</span></span>|<span data-ttu-id="8f9e7-132">String</span><span class="sxs-lookup"><span data-stu-id="8f9e7-132">String</span></span>|<span data-ttu-id="8f9e7-133">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-133">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8f9e7-134">响应</span><span class="sxs-lookup"><span data-stu-id="8f9e7-134">Response</span></span>

<span data-ttu-id="8f9e7-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f9e7-137">示例</span><span class="sxs-lookup"><span data-stu-id="8f9e7-137">Examples</span></span>

<span data-ttu-id="8f9e7-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-138">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8f9e7-139">请求</span><span class="sxs-lookup"><span data-stu-id="8f9e7-139">Request</span></span>

<span data-ttu-id="8f9e7-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="8f9e7-141">响应</span><span class="sxs-lookup"><span data-stu-id="8f9e7-141">Response</span></span>

<span data-ttu-id="8f9e7-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f9e7-142">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
