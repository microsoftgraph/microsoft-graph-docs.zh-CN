---
title: call： changeScreenSharingRole
description: 允许应用程序与组呼叫的参与者共享屏幕内容。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5239d0c2929f43d457253268d190c1ae68e87870
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786571"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="443b9-103">call： changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="443b9-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="443b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="443b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="443b9-105">允许应用程序与组呼叫的参与者共享屏幕内容。</span><span class="sxs-lookup"><span data-stu-id="443b9-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="443b9-106">**注意：** 这仅适用于使用媒体的组App-Hosted支持。</span><span class="sxs-lookup"><span data-stu-id="443b9-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="443b9-107">权限</span><span class="sxs-lookup"><span data-stu-id="443b9-107">Permissions</span></span>
<span data-ttu-id="443b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="443b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="443b9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="443b9-110">Permission type</span></span>                        | <span data-ttu-id="443b9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="443b9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="443b9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="443b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="443b9-113">不支持</span><span class="sxs-lookup"><span data-stu-id="443b9-113">Not Supported</span></span>                               |
| <span data-ttu-id="443b9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="443b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="443b9-115">不支持</span><span class="sxs-lookup"><span data-stu-id="443b9-115">Not Supported</span></span>                               |
| <span data-ttu-id="443b9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="443b9-116">Application</span></span>                            | <span data-ttu-id="443b9-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="443b9-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="443b9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="443b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="443b9-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="443b9-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="443b9-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="443b9-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="443b9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="443b9-121">Request headers</span></span>
| <span data-ttu-id="443b9-122">名称</span><span class="sxs-lookup"><span data-stu-id="443b9-122">Name</span></span>          | <span data-ttu-id="443b9-123">说明</span><span class="sxs-lookup"><span data-stu-id="443b9-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="443b9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="443b9-124">Authorization</span></span> | <span data-ttu-id="443b9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="443b9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="443b9-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="443b9-127">Content-type</span></span>  | <span data-ttu-id="443b9-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="443b9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="443b9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="443b9-130">Request body</span></span>
<span data-ttu-id="443b9-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="443b9-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="443b9-132">参数</span><span class="sxs-lookup"><span data-stu-id="443b9-132">Parameter</span></span>      | <span data-ttu-id="443b9-133">类型</span><span class="sxs-lookup"><span data-stu-id="443b9-133">Type</span></span>    |<span data-ttu-id="443b9-134">说明</span><span class="sxs-lookup"><span data-stu-id="443b9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="443b9-135">role</span><span class="sxs-lookup"><span data-stu-id="443b9-135">role</span></span>|<span data-ttu-id="443b9-136">String</span><span class="sxs-lookup"><span data-stu-id="443b9-136">String</span></span>|<span data-ttu-id="443b9-137">可能的值包括："viewer"和"sharer"</span><span class="sxs-lookup"><span data-stu-id="443b9-137">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="443b9-138">响应</span><span class="sxs-lookup"><span data-stu-id="443b9-138">Response</span></span>
<span data-ttu-id="443b9-139">如果成功，此方法将返回 `202 Accepted` 响应代码，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="443b9-139">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="443b9-140">示例</span><span class="sxs-lookup"><span data-stu-id="443b9-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="443b9-141">请求</span><span class="sxs-lookup"><span data-stu-id="443b9-141">Request</span></span>
<span data-ttu-id="443b9-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="443b9-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="443b9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="443b9-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="443b9-144">C#</span><span class="sxs-lookup"><span data-stu-id="443b9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="443b9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="443b9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="443b9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="443b9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="443b9-147">Java</span><span class="sxs-lookup"><span data-stu-id="443b9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="443b9-148">响应</span><span class="sxs-lookup"><span data-stu-id="443b9-148">Response</span></span>
<span data-ttu-id="443b9-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="443b9-149">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="443b9-150">通知 - 使用参与者发送屏幕共享视频更新名单</span><span class="sxs-lookup"><span data-stu-id="443b9-150">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="443b9-151">记下 `direction: sendOnly` 媒体流上的 属性。</span><span class="sxs-lookup"><span data-stu-id="443b9-151">Note the `direction: sendOnly` property on the media stream.</span></span>

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


