---
title: 调用： changeScreenSharingRole
description: 允许应用程序与组呼叫的参与者共享屏幕内容。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51fb5066100d4c8072d4df2dbcc62db03e3a1021
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871127"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="c9d6a-103">调用： changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="c9d6a-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="c9d6a-104">允许应用程序与组呼叫的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-104">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="c9d6a-105">**注意：** 只有使用应用程序托管媒体的组调用才支持这种情况。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-105">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9d6a-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9d6a-106">Permissions</span></span>
<span data-ttu-id="c9d6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9d6a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9d6a-109">Permission type</span></span>                        | <span data-ttu-id="c9d6a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9d6a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9d6a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9d6a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9d6a-112">不支持</span><span class="sxs-lookup"><span data-stu-id="c9d6a-112">Not Supported</span></span>                               |
| <span data-ttu-id="c9d6a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9d6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9d6a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="c9d6a-114">Not Supported</span></span>                               |
| <span data-ttu-id="c9d6a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9d6a-115">Application</span></span>                            | <span data-ttu-id="c9d6a-116">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="c9d6a-116">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="c9d6a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9d6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="c9d6a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9d6a-118">Request headers</span></span>
| <span data-ttu-id="c9d6a-119">名称</span><span class="sxs-lookup"><span data-stu-id="c9d6a-119">Name</span></span>          | <span data-ttu-id="c9d6a-120">说明</span><span class="sxs-lookup"><span data-stu-id="c9d6a-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c9d6a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9d6a-121">Authorization</span></span> | <span data-ttu-id="c9d6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9d6a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9d6a-124">Content-type</span></span>  | <span data-ttu-id="c9d6a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c9d6a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9d6a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9d6a-127">Request body</span></span>
<span data-ttu-id="c9d6a-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9d6a-129">参数</span><span class="sxs-lookup"><span data-stu-id="c9d6a-129">Parameter</span></span>      | <span data-ttu-id="c9d6a-130">类型</span><span class="sxs-lookup"><span data-stu-id="c9d6a-130">Type</span></span>    |<span data-ttu-id="c9d6a-131">说明</span><span class="sxs-lookup"><span data-stu-id="c9d6a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d6a-132">role</span><span class="sxs-lookup"><span data-stu-id="c9d6a-132">role</span></span>|<span data-ttu-id="c9d6a-133">String</span><span class="sxs-lookup"><span data-stu-id="c9d6a-133">String</span></span>|<span data-ttu-id="c9d6a-134">可能的值为： "查看器"、"共享资源"</span><span class="sxs-lookup"><span data-stu-id="c9d6a-134">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="c9d6a-135">响应</span><span class="sxs-lookup"><span data-stu-id="c9d6a-135">Response</span></span>
<span data-ttu-id="c9d6a-136">如果成功，此方法将返回`202 Accepted`响应代码，并且所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-136">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="c9d6a-137">示例</span><span class="sxs-lookup"><span data-stu-id="c9d6a-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9d6a-138">请求</span><span class="sxs-lookup"><span data-stu-id="c9d6a-138">Request</span></span>
<span data-ttu-id="c9d6a-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9d6a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d6a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9d6a-141">C#</span><span class="sxs-lookup"><span data-stu-id="c9d6a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9d6a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9d6a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9d6a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9d6a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9d6a-144">Java</span><span class="sxs-lookup"><span data-stu-id="c9d6a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c9d6a-145">响应</span><span class="sxs-lookup"><span data-stu-id="c9d6a-145">Response</span></span>
<span data-ttu-id="c9d6a-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-146">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="c9d6a-147">通知-名单随参与者发送屏幕共享视频而更新</span><span class="sxs-lookup"><span data-stu-id="c9d6a-147">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="c9d6a-148">记下`direction: sendOnly`媒体流上的属性。</span><span class="sxs-lookup"><span data-stu-id="c9d6a-148">Note the `direction: sendOnly` property on the media stream.</span></span>

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
