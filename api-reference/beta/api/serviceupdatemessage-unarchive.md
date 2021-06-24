---
title: serviceUpdateMessage：unarchive
description: 取消存档已登录用户的服务更新消息的列表。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 79c5b5045200a366e9ce4df24eb21f554ae92c1a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107781"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="26cce-103">serviceUpdateMessage：unarchive</span><span class="sxs-lookup"><span data-stu-id="26cce-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="26cce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26cce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26cce-105">取消存档已登录用户的 [serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="26cce-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="26cce-106">权限</span><span class="sxs-lookup"><span data-stu-id="26cce-106">Permissions</span></span>
<span data-ttu-id="26cce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26cce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26cce-109">Permission type</span></span>|<span data-ttu-id="26cce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26cce-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26cce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26cce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26cce-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="26cce-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="26cce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26cce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26cce-114">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="26cce-114">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="26cce-115">应用</span><span class="sxs-lookup"><span data-stu-id="26cce-115">Application</span></span>|<span data-ttu-id="26cce-116">不支持</span><span class="sxs-lookup"><span data-stu-id="26cce-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="26cce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26cce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="26cce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26cce-118">Request headers</span></span>
|<span data-ttu-id="26cce-119">名称</span><span class="sxs-lookup"><span data-stu-id="26cce-119">Name</span></span>|<span data-ttu-id="26cce-120">说明</span><span class="sxs-lookup"><span data-stu-id="26cce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26cce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26cce-121">Authorization</span></span>|<span data-ttu-id="26cce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26cce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26cce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26cce-124">Content-Type</span></span>|<span data-ttu-id="26cce-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="26cce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26cce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="26cce-127">Request body</span></span>
<span data-ttu-id="26cce-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26cce-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="26cce-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="26cce-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26cce-130">参数</span><span class="sxs-lookup"><span data-stu-id="26cce-130">Parameter</span></span>|<span data-ttu-id="26cce-131">类型</span><span class="sxs-lookup"><span data-stu-id="26cce-131">Type</span></span>|<span data-ttu-id="26cce-132">说明</span><span class="sxs-lookup"><span data-stu-id="26cce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26cce-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="26cce-133">messageIds</span></span>|<span data-ttu-id="26cce-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="26cce-134">String collection</span></span>|<span data-ttu-id="26cce-135">要取消存档的邮件 ID 的列表。</span><span class="sxs-lookup"><span data-stu-id="26cce-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="26cce-136">响应</span><span class="sxs-lookup"><span data-stu-id="26cce-136">Response</span></span>

<span data-ttu-id="26cce-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` `true` 布尔值。</span><span class="sxs-lookup"><span data-stu-id="26cce-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="26cce-138">否则，将在 `false` 响应正文中返回 。</span><span class="sxs-lookup"><span data-stu-id="26cce-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26cce-139">示例</span><span class="sxs-lookup"><span data-stu-id="26cce-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="26cce-140">请求</span><span class="sxs-lookup"><span data-stu-id="26cce-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_unarchive"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/unarchive
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```


### <a name="response"></a><span data-ttu-id="26cce-141">响应</span><span class="sxs-lookup"><span data-stu-id="26cce-141">Response</span></span>
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