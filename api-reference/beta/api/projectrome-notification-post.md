---
title: 创建和发送通知
description: '创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中, 并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 86e67d040dcae3a013d8848c638ffadca41e4f5f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331940"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="d216e-104">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="d216e-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d216e-105">创建并发送针对用户通过 Microsoft Graph 的通知。</span><span class="sxs-lookup"><span data-stu-id="d216e-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="d216e-106">通知存储在 Microsoft Graph 通知源存储中, 并发送到用户登录到的所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="d216e-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="d216e-107">权限</span><span class="sxs-lookup"><span data-stu-id="d216e-107">Permissions</span></span>
<span data-ttu-id="d216e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d216e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d216e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d216e-110">Permission type</span></span>      | <span data-ttu-id="d216e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d216e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d216e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d216e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d216e-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d216e-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d216e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d216e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d216e-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d216e-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d216e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d216e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="d216e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d216e-117">Request headers</span></span>
|<span data-ttu-id="d216e-118">名称</span><span class="sxs-lookup"><span data-stu-id="d216e-118">Name</span></span> | <span data-ttu-id="d216e-119">类型</span><span class="sxs-lookup"><span data-stu-id="d216e-119">Type</span></span> | <span data-ttu-id="d216e-120">说明</span><span class="sxs-lookup"><span data-stu-id="d216e-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d216e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d216e-121">Authorization</span></span> | <span data-ttu-id="d216e-122">string</span><span class="sxs-lookup"><span data-stu-id="d216e-122">string</span></span> |<span data-ttu-id="d216e-123">授权标头用于传递呼叫方的凭据。</span><span class="sxs-lookup"><span data-stu-id="d216e-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="d216e-124">持有者 {令牌}。</span><span class="sxs-lookup"><span data-stu-id="d216e-124">Bearer {token}.</span></span> <span data-ttu-id="d216e-125">必需。</span><span class="sxs-lookup"><span data-stu-id="d216e-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d216e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d216e-126">Request body</span></span>
<span data-ttu-id="d216e-127">在请求正文中, 提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d216e-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d216e-128">响应</span><span class="sxs-lookup"><span data-stu-id="d216e-128">Response</span></span>
<span data-ttu-id="d216e-129">如果成功, 此方法将`201 Created`返回指示已成功创建和存储通知的响应代码。</span><span class="sxs-lookup"><span data-stu-id="d216e-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="d216e-130">示例</span><span class="sxs-lookup"><span data-stu-id="d216e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d216e-131">请求</span><span class="sxs-lookup"><span data-stu-id="d216e-131">Request</span></span>
<span data-ttu-id="d216e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d216e-132">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d216e-133">响应</span><span class="sxs-lookup"><span data-stu-id="d216e-133">Response</span></span>
<span data-ttu-id="d216e-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d216e-134">The following is an example of the response.</span></span>

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


