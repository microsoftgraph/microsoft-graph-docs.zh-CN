---
title: serviceUpdateMessage： archive
description: 存档已登录用户的服务更新消息列表。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: afe038f6bb41f69c6f0c58bb6b68adc739f3f52f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109079"
---
# <a name="serviceupdatemessage-archive"></a><span data-ttu-id="1565d-103">serviceUpdateMessage： archive</span><span class="sxs-lookup"><span data-stu-id="1565d-103">serviceUpdateMessage: archive</span></span>
<span data-ttu-id="1565d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1565d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1565d-105">存档已登录 [用户的 serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="1565d-105">Archive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1565d-106">权限</span><span class="sxs-lookup"><span data-stu-id="1565d-106">Permissions</span></span>
<span data-ttu-id="1565d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1565d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1565d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1565d-109">Permission type</span></span>|<span data-ttu-id="1565d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1565d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1565d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1565d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1565d-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="1565d-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="1565d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1565d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1565d-114">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="1565d-114">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="1565d-115">应用</span><span class="sxs-lookup"><span data-stu-id="1565d-115">Application</span></span>|<span data-ttu-id="1565d-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1565d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1565d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1565d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/archive
```

## <a name="request-headers"></a><span data-ttu-id="1565d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1565d-118">Request headers</span></span>
|<span data-ttu-id="1565d-119">名称</span><span class="sxs-lookup"><span data-stu-id="1565d-119">Name</span></span>|<span data-ttu-id="1565d-120">说明</span><span class="sxs-lookup"><span data-stu-id="1565d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1565d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1565d-121">Authorization</span></span>|<span data-ttu-id="1565d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1565d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1565d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1565d-124">Content-Type</span></span>|<span data-ttu-id="1565d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1565d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1565d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1565d-127">Request body</span></span>
<span data-ttu-id="1565d-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1565d-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="1565d-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1565d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1565d-130">参数</span><span class="sxs-lookup"><span data-stu-id="1565d-130">Parameter</span></span>|<span data-ttu-id="1565d-131">类型</span><span class="sxs-lookup"><span data-stu-id="1565d-131">Type</span></span>|<span data-ttu-id="1565d-132">说明</span><span class="sxs-lookup"><span data-stu-id="1565d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1565d-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="1565d-133">messageIds</span></span>|<span data-ttu-id="1565d-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="1565d-134">String collection</span></span>|<span data-ttu-id="1565d-135">要存档的邮件 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1565d-135">List of message IDs to archive.</span></span>|

## <a name="response"></a><span data-ttu-id="1565d-136">响应</span><span class="sxs-lookup"><span data-stu-id="1565d-136">Response</span></span>

<span data-ttu-id="1565d-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` `true` 布尔值。</span><span class="sxs-lookup"><span data-stu-id="1565d-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="1565d-138">否则，将在 `false` 响应正文中返回 。</span><span class="sxs-lookup"><span data-stu-id="1565d-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1565d-139">示例</span><span class="sxs-lookup"><span data-stu-id="1565d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1565d-140">请求</span><span class="sxs-lookup"><span data-stu-id="1565d-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_archive"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/archive
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a><span data-ttu-id="1565d-141">响应</span><span class="sxs-lookup"><span data-stu-id="1565d-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```