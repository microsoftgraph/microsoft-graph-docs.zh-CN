---
title: offerShiftRequest：拒绝
description: 拒绝促销活动请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 94daed01b2b7d4131a09504773c5377889b7e587
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154940"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="20fd5-103">offerShiftRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="20fd5-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="20fd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20fd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20fd5-105">拒绝[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20fd5-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20fd5-106">权限</span><span class="sxs-lookup"><span data-stu-id="20fd5-106">Permissions</span></span>

<span data-ttu-id="20fd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20fd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20fd5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20fd5-109">Permission type</span></span>                        | <span data-ttu-id="20fd5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20fd5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20fd5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20fd5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20fd5-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="20fd5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="20fd5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20fd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20fd5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20fd5-114">Not supported.</span></span> |
| <span data-ttu-id="20fd5-115">Application</span><span class="sxs-lookup"><span data-stu-id="20fd5-115">Application</span></span>                            | <span data-ttu-id="20fd5-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20fd5-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="20fd5-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="20fd5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="20fd5-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="20fd5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="20fd5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20fd5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="20fd5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20fd5-120">Request headers</span></span>

| <span data-ttu-id="20fd5-121">名称</span><span class="sxs-lookup"><span data-stu-id="20fd5-121">Name</span></span>          | <span data-ttu-id="20fd5-122">说明</span><span class="sxs-lookup"><span data-stu-id="20fd5-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20fd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20fd5-123">Authorization</span></span> | <span data-ttu-id="20fd5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20fd5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20fd5-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="20fd5-126">Content-type</span></span> | <span data-ttu-id="20fd5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="20fd5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20fd5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="20fd5-129">Request body</span></span>

<span data-ttu-id="20fd5-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="20fd5-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20fd5-131">参数</span><span class="sxs-lookup"><span data-stu-id="20fd5-131">Parameter</span></span>    | <span data-ttu-id="20fd5-132">类型</span><span class="sxs-lookup"><span data-stu-id="20fd5-132">Type</span></span>        | <span data-ttu-id="20fd5-133">描述</span><span class="sxs-lookup"><span data-stu-id="20fd5-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20fd5-134">message</span><span class="sxs-lookup"><span data-stu-id="20fd5-134">message</span></span>|<span data-ttu-id="20fd5-135">String</span><span class="sxs-lookup"><span data-stu-id="20fd5-135">String</span></span>|<span data-ttu-id="20fd5-136">在拒绝时发送自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="20fd5-136">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="20fd5-137">响应</span><span class="sxs-lookup"><span data-stu-id="20fd5-137">Response</span></span>

<span data-ttu-id="20fd5-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="20fd5-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20fd5-140">示例</span><span class="sxs-lookup"><span data-stu-id="20fd5-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20fd5-141">请求</span><span class="sxs-lookup"><span data-stu-id="20fd5-141">Request</span></span>

<span data-ttu-id="20fd5-142">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="20fd5-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```

---


### <a name="response"></a><span data-ttu-id="20fd5-143">响应</span><span class="sxs-lookup"><span data-stu-id="20fd5-143">Response</span></span>

<span data-ttu-id="20fd5-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="20fd5-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
