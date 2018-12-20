---
title: 参与者： muteAll
description: 将呼叫中的所有参与者设为都静音。
author: VinodRavichandran
ms.openlocfilehash: fb395fd5a49a0a13616d32de9645f3899e4641d2
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380497"
---
# <a name="participant-muteall"></a><span data-ttu-id="8e691-103">参与者： muteAll</span><span class="sxs-lookup"><span data-stu-id="8e691-103">participant: muteAll</span></span>

> <span data-ttu-id="8e691-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e691-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e691-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e691-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e691-106">将呼叫中的所有参与者设为都静音。</span><span class="sxs-lookup"><span data-stu-id="8e691-106">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e691-107">权限</span><span class="sxs-lookup"><span data-stu-id="8e691-107">Permissions</span></span>
<span data-ttu-id="8e691-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e691-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e691-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e691-110">Permission type</span></span>                        | <span data-ttu-id="8e691-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e691-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e691-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e691-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e691-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8e691-113">Not Supported</span></span>                               |
| <span data-ttu-id="8e691-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e691-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e691-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8e691-115">Not Supported</span></span>                               |
| <span data-ttu-id="8e691-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e691-116">Application</span></span>                            | <span data-ttu-id="8e691-117">无</span><span class="sxs-lookup"><span data-stu-id="8e691-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8e691-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e691-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="8e691-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e691-119">Request headers</span></span>
| <span data-ttu-id="8e691-120">名称</span><span class="sxs-lookup"><span data-stu-id="8e691-120">Name</span></span>          | <span data-ttu-id="8e691-121">说明</span><span class="sxs-lookup"><span data-stu-id="8e691-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8e691-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e691-122">Authorization</span></span> | <span data-ttu-id="8e691-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e691-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e691-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e691-125">Request body</span></span>
<span data-ttu-id="8e691-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8e691-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e691-127">参数</span><span class="sxs-lookup"><span data-stu-id="8e691-127">Parameter</span></span>      | <span data-ttu-id="8e691-128">类型</span><span class="sxs-lookup"><span data-stu-id="8e691-128">Type</span></span>    |<span data-ttu-id="8e691-129">说明</span><span class="sxs-lookup"><span data-stu-id="8e691-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e691-130">participants</span><span class="sxs-lookup"><span data-stu-id="8e691-130">participants</span></span>|<span data-ttu-id="8e691-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e691-131">String collection</span></span>|<span data-ttu-id="8e691-132">若要将设为静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="8e691-132">The participants to be muted.</span></span>|
|<span data-ttu-id="8e691-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="8e691-133">clientContext</span></span>|<span data-ttu-id="8e691-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8e691-134">String</span></span>|<span data-ttu-id="8e691-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="8e691-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8e691-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e691-136">Response</span></span>
<span data-ttu-id="8e691-137">如果成功，此方法返回`200 OK`响应正文中的响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e691-137">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e691-138">示例</span><span class="sxs-lookup"><span data-stu-id="8e691-138">Example</span></span>
<span data-ttu-id="8e691-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8e691-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8e691-140">请求</span><span class="sxs-lookup"><span data-stu-id="8e691-140">Request</span></span>
<span data-ttu-id="8e691-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e691-141">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="8e691-142">响应</span><span class="sxs-lookup"><span data-stu-id="8e691-142">Response</span></span>

> <span data-ttu-id="8e691-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e691-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
