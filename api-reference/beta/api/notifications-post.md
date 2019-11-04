---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 6062153c1eaff68a19cd5b27ac10efa9bacafb93
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937922"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="82d61-103">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="82d61-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d61-104">创建并发送针对用户通过 Microsoft Graph 的通知。</span><span class="sxs-lookup"><span data-stu-id="82d61-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="82d61-105">通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="82d61-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="82d61-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="82d61-106">Permissions</span></span>
<span data-ttu-id="82d61-107">您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="82d61-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="82d61-108">如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="82d61-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="82d61-109">建议您不要选择此选项来创建通知。</span><span class="sxs-lookup"><span data-stu-id="82d61-109">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="82d61-110">如果想要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82d61-110">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="82d61-111">Permission type</span></span>      | <span data-ttu-id="82d61-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82d61-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82d61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82d61-113">Delegated (work or school account)</span></span> | <span data-ttu-id="82d61-114">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="82d61-114">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="82d61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82d61-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d61-116">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="82d61-116">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="82d61-117">Application</span><span class="sxs-lookup"><span data-stu-id="82d61-117">Application</span></span> | <span data-ttu-id="82d61-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="82d61-118">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="82d61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82d61-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="82d61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="82d61-120">Request headers</span></span>
|<span data-ttu-id="82d61-121">名称</span><span class="sxs-lookup"><span data-stu-id="82d61-121">Name</span></span> | <span data-ttu-id="82d61-122">类型</span><span class="sxs-lookup"><span data-stu-id="82d61-122">Type</span></span> | <span data-ttu-id="82d61-123">说明</span><span class="sxs-lookup"><span data-stu-id="82d61-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="82d61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d61-124">Authorization</span></span> | <span data-ttu-id="82d61-125">string</span><span class="sxs-lookup"><span data-stu-id="82d61-125">string</span></span> |<span data-ttu-id="82d61-126">授权标头用于传递呼叫方的凭据。</span><span class="sxs-lookup"><span data-stu-id="82d61-126">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="82d61-127">持有者 {令牌}。</span><span class="sxs-lookup"><span data-stu-id="82d61-127">Bearer {token}.</span></span> <span data-ttu-id="82d61-128">必填。</span><span class="sxs-lookup"><span data-stu-id="82d61-128">Required.</span></span> |
|<span data-ttu-id="82d61-129">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="82d61-129">X-UNS-ID</span></span> | <span data-ttu-id="82d61-130">string</span><span class="sxs-lookup"><span data-stu-id="82d61-130">string</span></span> |<span data-ttu-id="82d61-131">Microsoft Graph 通知服务在创建订阅后返回的 UserNotificationSubscriptionId，并用于面向特定用户。</span><span class="sxs-lookup"><span data-stu-id="82d61-131">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="82d61-132">必需。</span><span class="sxs-lookup"><span data-stu-id="82d61-132">Required.</span></span> |
|<span data-ttu-id="82d61-133">Content-type</span><span class="sxs-lookup"><span data-stu-id="82d61-133">Content-type</span></span> | <span data-ttu-id="82d61-134">appliation/json。</span><span class="sxs-lookup"><span data-stu-id="82d61-134">appliation/json.</span></span> <span data-ttu-id="82d61-135">必填。</span><span class="sxs-lookup"><span data-stu-id="82d61-135">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d61-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="82d61-136">Request body</span></span>
<span data-ttu-id="82d61-137">在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82d61-137">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="82d61-138">响应</span><span class="sxs-lookup"><span data-stu-id="82d61-138">Response</span></span>
<span data-ttu-id="82d61-139">如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。</span><span class="sxs-lookup"><span data-stu-id="82d61-139">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="82d61-140">随后，通知将通过有效订阅扇到所有指定的终结点。</span><span class="sxs-lookup"><span data-stu-id="82d61-140">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="82d61-141">示例</span><span class="sxs-lookup"><span data-stu-id="82d61-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="82d61-142">请求</span><span class="sxs-lookup"><span data-stu-id="82d61-142">Request</span></span>
<span data-ttu-id="82d61-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="82d61-143">The following is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a><span data-ttu-id="82d61-144">响应</span><span class="sxs-lookup"><span data-stu-id="82d61-144">Response</span></span>
<span data-ttu-id="82d61-145">下面是对应响应的一个示例。</span><span class="sxs-lookup"><span data-stu-id="82d61-145">The following is an example of the corresponding response.</span></span>

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```
