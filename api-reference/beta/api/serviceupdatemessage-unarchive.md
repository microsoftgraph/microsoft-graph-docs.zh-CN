---
title: serviceUpdateMessage：unarchive
description: 取消存档已登录用户的服务更新消息的列表。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 38144a2f3e6512631f47a22ebecdf7a41e70a417
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209120"
---
# <a name="serviceupdatemessage-unarchive"></a><span data-ttu-id="04e3c-103">serviceUpdateMessage：unarchive</span><span class="sxs-lookup"><span data-stu-id="04e3c-103">serviceUpdateMessage: unarchive</span></span>
<span data-ttu-id="04e3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04e3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04e3c-105">取消存档已登录用户的 [serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="04e3c-105">Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="04e3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="04e3c-106">Permissions</span></span>
<span data-ttu-id="04e3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04e3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04e3c-109">Permission type</span></span>|<span data-ttu-id="04e3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04e3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04e3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04e3c-112">ServiceMessageViewpoint.Write</span><span class="sxs-lookup"><span data-stu-id="04e3c-112">ServiceMessageViewpoint.Write</span></span>|
|<span data-ttu-id="04e3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04e3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e3c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04e3c-114">Not supported.</span></span>|
|<span data-ttu-id="04e3c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04e3c-115">Application</span></span>|<span data-ttu-id="04e3c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="04e3c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e3c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04e3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="04e3c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04e3c-118">Request headers</span></span>
|<span data-ttu-id="04e3c-119">名称</span><span class="sxs-lookup"><span data-stu-id="04e3c-119">Name</span></span>|<span data-ttu-id="04e3c-120">说明</span><span class="sxs-lookup"><span data-stu-id="04e3c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04e3c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e3c-121">Authorization</span></span>|<span data-ttu-id="04e3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04e3c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04e3c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04e3c-124">Content-Type</span></span>|<span data-ttu-id="04e3c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="04e3c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04e3c-127">Request body</span></span>
<span data-ttu-id="04e3c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04e3c-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="04e3c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="04e3c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04e3c-130">参数</span><span class="sxs-lookup"><span data-stu-id="04e3c-130">Parameter</span></span>|<span data-ttu-id="04e3c-131">类型</span><span class="sxs-lookup"><span data-stu-id="04e3c-131">Type</span></span>|<span data-ttu-id="04e3c-132">说明</span><span class="sxs-lookup"><span data-stu-id="04e3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e3c-133">messageIds</span><span class="sxs-lookup"><span data-stu-id="04e3c-133">messageIds</span></span>|<span data-ttu-id="04e3c-134">String collection</span><span class="sxs-lookup"><span data-stu-id="04e3c-134">String collection</span></span>|<span data-ttu-id="04e3c-135">要取消存档的邮件 ID 的列表。</span><span class="sxs-lookup"><span data-stu-id="04e3c-135">List of message IDs to unarchive.</span></span>|

## <a name="response"></a><span data-ttu-id="04e3c-136">响应</span><span class="sxs-lookup"><span data-stu-id="04e3c-136">Response</span></span>

<span data-ttu-id="04e3c-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` `true` 布尔值。</span><span class="sxs-lookup"><span data-stu-id="04e3c-137">If successful, this action returns a `200 OK` response code and a Boolean value `true` in the response body.</span></span> <span data-ttu-id="04e3c-138">否则，将在 `false` 响应正文中返回 。</span><span class="sxs-lookup"><span data-stu-id="04e3c-138">Otherwise, will return `false` in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e3c-139">示例</span><span class="sxs-lookup"><span data-stu-id="04e3c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="04e3c-140">请求</span><span class="sxs-lookup"><span data-stu-id="04e3c-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="04e3c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="04e3c-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="04e3c-142">C#</span><span class="sxs-lookup"><span data-stu-id="04e3c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceupdatemessage-unarchive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04e3c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04e3c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceupdatemessage-unarchive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04e3c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04e3c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceupdatemessage-unarchive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04e3c-145">Java</span><span class="sxs-lookup"><span data-stu-id="04e3c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceupdatemessage-unarchive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="04e3c-146">响应</span><span class="sxs-lookup"><span data-stu-id="04e3c-146">Response</span></span>
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
