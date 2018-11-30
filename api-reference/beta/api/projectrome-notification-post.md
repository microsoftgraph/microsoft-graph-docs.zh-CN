---
title: 创建和发送通知
description: '创建和发送通知目标用户通过 Microsoft Graph。 通知存储在 Microsoft Graph 通知源存储，并发送到的用户登录到所有设备终结点上的所有应用程序客户端。  '
ms.openlocfilehash: 7855d8b369a2efc6dada33c66c12ae76384a2760
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046832"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="f81b6-104">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="f81b6-104">Create and send a notification</span></span>
> <span data-ttu-id="f81b6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f81b6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f81b6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f81b6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f81b6-107">创建和发送通知目标用户通过 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="f81b6-107">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="f81b6-108">通知存储在 Microsoft Graph 通知源存储，并发送到的用户登录到所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="f81b6-108">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="f81b6-109">权限</span><span class="sxs-lookup"><span data-stu-id="f81b6-109">Permissions</span></span>
<span data-ttu-id="f81b6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f81b6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f81b6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f81b6-112">Permission type</span></span>      | <span data-ttu-id="f81b6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f81b6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f81b6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f81b6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f81b6-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f81b6-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f81b6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f81b6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81b6-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f81b6-117">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="f81b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f81b6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="f81b6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f81b6-119">Request headers</span></span>
|<span data-ttu-id="f81b6-120">名称</span><span class="sxs-lookup"><span data-stu-id="f81b6-120">Name</span></span> | <span data-ttu-id="f81b6-121">类型</span><span class="sxs-lookup"><span data-stu-id="f81b6-121">Type</span></span> | <span data-ttu-id="f81b6-122">说明</span><span class="sxs-lookup"><span data-stu-id="f81b6-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f81b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f81b6-123">Authorization</span></span> | <span data-ttu-id="f81b6-124">string</span><span class="sxs-lookup"><span data-stu-id="f81b6-124">string</span></span> |<span data-ttu-id="f81b6-125">Authorization 标头用于传递的呼叫方凭据。</span><span class="sxs-lookup"><span data-stu-id="f81b6-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="f81b6-126">持有者 {令牌}。</span><span class="sxs-lookup"><span data-stu-id="f81b6-126">Bearer {token}.</span></span> <span data-ttu-id="f81b6-127">必需。</span><span class="sxs-lookup"><span data-stu-id="f81b6-127">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="f81b6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f81b6-128">Request body</span></span>
<span data-ttu-id="f81b6-129">在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f81b6-129">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f81b6-130">响应</span><span class="sxs-lookup"><span data-stu-id="f81b6-130">Response</span></span>
<span data-ttu-id="f81b6-131">如果成功，此方法返回`201 Created`响应代码，指示已成功创建并存储通知。</span><span class="sxs-lookup"><span data-stu-id="f81b6-131">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="f81b6-132">示例</span><span class="sxs-lookup"><span data-stu-id="f81b6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f81b6-133">请求</span><span class="sxs-lookup"><span data-stu-id="f81b6-133">Request</span></span>
<span data-ttu-id="f81b6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f81b6-134">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a><span data-ttu-id="f81b6-135">响应</span><span class="sxs-lookup"><span data-stu-id="f81b6-135">Response</span></span>
<span data-ttu-id="f81b6-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f81b6-136">The following is an example of the response.</span></span>

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


