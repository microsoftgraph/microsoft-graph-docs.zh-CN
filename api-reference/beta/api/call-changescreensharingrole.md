---
title: 调用： changeScreenSharingRole
description: 允许应用程序与组呼叫的参与者共享屏幕内容。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9c1195c0f2c7d76a163ad9f3194ea02e96c5982f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987447"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="3f7c1-103">调用： changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="3f7c1-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="3f7c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f7c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f7c1-105">允许应用程序与组呼叫的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="3f7c1-106">**注意：** 只有使用应用程序托管媒体的组调用才支持这种情况。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f7c1-107">权限</span><span class="sxs-lookup"><span data-stu-id="3f7c1-107">Permissions</span></span>
<span data-ttu-id="3f7c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f7c1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f7c1-110">Permission type</span></span>                        | <span data-ttu-id="3f7c1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f7c1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f7c1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7c1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f7c1-113">不支持</span><span class="sxs-lookup"><span data-stu-id="3f7c1-113">Not Supported</span></span>                               |
| <span data-ttu-id="3f7c1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f7c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f7c1-115">不支持</span><span class="sxs-lookup"><span data-stu-id="3f7c1-115">Not Supported</span></span>                               |
| <span data-ttu-id="3f7c1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f7c1-116">Application</span></span>                            | <span data-ttu-id="3f7c1-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="3f7c1-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="3f7c1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f7c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="3f7c1-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3f7c1-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f7c1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f7c1-121">Request headers</span></span>
| <span data-ttu-id="3f7c1-122">名称</span><span class="sxs-lookup"><span data-stu-id="3f7c1-122">Name</span></span>          | <span data-ttu-id="3f7c1-123">说明</span><span class="sxs-lookup"><span data-stu-id="3f7c1-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3f7c1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f7c1-124">Authorization</span></span> | <span data-ttu-id="3f7c1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f7c1-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="3f7c1-127">Content-type</span></span>  | <span data-ttu-id="3f7c1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3f7c1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f7c1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f7c1-130">Request body</span></span>
<span data-ttu-id="3f7c1-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f7c1-132">参数</span><span class="sxs-lookup"><span data-stu-id="3f7c1-132">Parameter</span></span>      | <span data-ttu-id="3f7c1-133">类型</span><span class="sxs-lookup"><span data-stu-id="3f7c1-133">Type</span></span>    |<span data-ttu-id="3f7c1-134">说明</span><span class="sxs-lookup"><span data-stu-id="3f7c1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f7c1-135">role</span><span class="sxs-lookup"><span data-stu-id="3f7c1-135">role</span></span>|<span data-ttu-id="3f7c1-136">String</span><span class="sxs-lookup"><span data-stu-id="3f7c1-136">String</span></span>|<span data-ttu-id="3f7c1-137">可能的值为： "查看器"、"共享资源"</span><span class="sxs-lookup"><span data-stu-id="3f7c1-137">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="3f7c1-138">响应</span><span class="sxs-lookup"><span data-stu-id="3f7c1-138">Response</span></span>
<span data-ttu-id="3f7c1-139">如果成功，此方法将返回 `202 Accepted` 响应代码，并且所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-139">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="3f7c1-140">示例</span><span class="sxs-lookup"><span data-stu-id="3f7c1-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3f7c1-141">请求</span><span class="sxs-lookup"><span data-stu-id="3f7c1-141">Request</span></span>
<span data-ttu-id="3f7c1-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f7c1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f7c1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="c"></a>[<span data-ttu-id="3f7c1-144">C#</span><span class="sxs-lookup"><span data-stu-id="3f7c1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f7c1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f7c1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f7c1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f7c1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f7c1-147">响应</span><span class="sxs-lookup"><span data-stu-id="3f7c1-147">Response</span></span>
<span data-ttu-id="3f7c1-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="3f7c1-149">通知-名单随参与者发送屏幕共享视频而更新</span><span class="sxs-lookup"><span data-stu-id="3f7c1-149">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="3f7c1-150">记下 `direction: sendOnly` 媒体流上的属性。</span><span class="sxs-lookup"><span data-stu-id="3f7c1-150">Note the `direction: sendOnly` property on the media stream.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "2765eb15-01f8-47c6-b12b-c32111a4a86f",
          "info": {
            "identity": {
              "user": {
                "displayName": "Bob",
                "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1",
              "direction": "sendOnly"
            }
          ],
          "isMuted": false,
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


