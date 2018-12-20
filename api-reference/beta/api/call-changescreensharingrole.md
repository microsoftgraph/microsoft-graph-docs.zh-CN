---
title: 呼叫： changeScreenSharingRole
description: 启动和停止共享的调用中的屏幕。 此 API 用于允许应用程序共享屏幕内容与呼叫或会议的参与者。
author: VinodRavichandran
ms.openlocfilehash: a0f745fa6af1dbf97c19e95a70ca37350dacc408
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380458"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="5c658-104">呼叫： changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="5c658-104">call: changeScreenSharingRole</span></span>

> <span data-ttu-id="5c658-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c658-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c658-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c658-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c658-107">启动和停止共享的调用中的屏幕。</span><span class="sxs-lookup"><span data-stu-id="5c658-107">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="5c658-108">此 API 用于允许应用程序共享屏幕内容与呼叫或会议的参与者。</span><span class="sxs-lookup"><span data-stu-id="5c658-108">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c658-109">权限</span><span class="sxs-lookup"><span data-stu-id="5c658-109">Permissions</span></span>
<span data-ttu-id="5c658-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c658-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c658-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c658-112">Permission type</span></span>                        | <span data-ttu-id="5c658-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c658-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c658-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c658-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c658-115">不支持</span><span class="sxs-lookup"><span data-stu-id="5c658-115">Not Supported</span></span>                               |
| <span data-ttu-id="5c658-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c658-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c658-117">不支持</span><span class="sxs-lookup"><span data-stu-id="5c658-117">Not Supported</span></span>                               |
| <span data-ttu-id="5c658-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c658-118">Application</span></span>                            | <span data-ttu-id="5c658-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="5c658-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="5c658-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c658-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="5c658-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c658-121">Request headers</span></span>
| <span data-ttu-id="5c658-122">名称</span><span class="sxs-lookup"><span data-stu-id="5c658-122">Name</span></span>          | <span data-ttu-id="5c658-123">说明</span><span class="sxs-lookup"><span data-stu-id="5c658-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5c658-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c658-124">Authorization</span></span> | <span data-ttu-id="5c658-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c658-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c658-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c658-127">Request body</span></span>
<span data-ttu-id="5c658-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5c658-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c658-129">参数</span><span class="sxs-lookup"><span data-stu-id="5c658-129">Parameter</span></span>      | <span data-ttu-id="5c658-130">类型</span><span class="sxs-lookup"><span data-stu-id="5c658-130">Type</span></span>    |<span data-ttu-id="5c658-131">说明</span><span class="sxs-lookup"><span data-stu-id="5c658-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c658-132">role</span><span class="sxs-lookup"><span data-stu-id="5c658-132">role</span></span>|<span data-ttu-id="5c658-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5c658-133">String</span></span>|<span data-ttu-id="5c658-134">可能的值为: 查看、 共享</span><span class="sxs-lookup"><span data-stu-id="5c658-134">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="5c658-135">响应</span><span class="sxs-lookup"><span data-stu-id="5c658-135">Response</span></span>
<span data-ttu-id="5c658-136">返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="5c658-136">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c658-137">示例</span><span class="sxs-lookup"><span data-stu-id="5c658-137">Example</span></span>
<span data-ttu-id="5c658-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5c658-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5c658-139">请求</span><span class="sxs-lookup"><span data-stu-id="5c658-139">Request</span></span>
<span data-ttu-id="5c658-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c658-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="5c658-141">响应</span><span class="sxs-lookup"><span data-stu-id="5c658-141">Response</span></span>
<span data-ttu-id="5c658-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5c658-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
