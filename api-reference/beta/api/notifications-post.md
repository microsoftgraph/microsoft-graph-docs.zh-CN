---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 1828f72bfcedb701597ce4b0d55e274a25fcf834
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456682"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="26002-103">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="26002-103">Create and send a notification</span></span>

<span data-ttu-id="26002-104">命名空间： microsoft. graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="26002-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="26002-105">创建并发送针对用户通过 Microsoft Graph 的通知。</span><span class="sxs-lookup"><span data-stu-id="26002-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="26002-106">通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="26002-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="26002-107">权限</span><span class="sxs-lookup"><span data-stu-id="26002-107">Permissions</span></span>
<span data-ttu-id="26002-108">您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="26002-108">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="26002-109">如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="26002-109">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="26002-110">建议您不要选择此选项来创建通知。</span><span class="sxs-lookup"><span data-stu-id="26002-110">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="26002-111">如果想要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26002-111">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26002-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="26002-112">Permission type</span></span>      | <span data-ttu-id="26002-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26002-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26002-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26002-114">Delegated (work or school account)</span></span> | <span data-ttu-id="26002-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="26002-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="26002-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26002-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26002-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="26002-117">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="26002-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="26002-118">Application</span></span> | <span data-ttu-id="26002-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="26002-119">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="26002-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26002-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="26002-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="26002-121">Request headers</span></span>
|<span data-ttu-id="26002-122">名称</span><span class="sxs-lookup"><span data-stu-id="26002-122">Name</span></span> | <span data-ttu-id="26002-123">说明</span><span class="sxs-lookup"><span data-stu-id="26002-123">Description</span></span>|
|:----|:-----------|
|<span data-ttu-id="26002-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="26002-124">Authorization</span></span> | <span data-ttu-id="26002-125">授权标头用于传递呼叫方的凭据。</span><span class="sxs-lookup"><span data-stu-id="26002-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="26002-126">持有者 {令牌}。</span><span class="sxs-lookup"><span data-stu-id="26002-126">Bearer {token}.</span></span> <span data-ttu-id="26002-127">必填。</span><span class="sxs-lookup"><span data-stu-id="26002-127">Required.</span></span> |
|<span data-ttu-id="26002-128">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="26002-128">X-UNS-ID</span></span> | <span data-ttu-id="26002-129">Microsoft Graph 通知服务在创建订阅后返回的 UserNotificationSubscriptionId，并用于面向特定用户。</span><span class="sxs-lookup"><span data-stu-id="26002-129">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="26002-130">必需。</span><span class="sxs-lookup"><span data-stu-id="26002-130">Required.</span></span> |
|<span data-ttu-id="26002-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="26002-131">Content-type</span></span> | <span data-ttu-id="26002-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="26002-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26002-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="26002-134">Request body</span></span>
<span data-ttu-id="26002-135">在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26002-135">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26002-136">响应</span><span class="sxs-lookup"><span data-stu-id="26002-136">Response</span></span>
<span data-ttu-id="26002-137">如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。</span><span class="sxs-lookup"><span data-stu-id="26002-137">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="26002-138">随后，通知将通过有效订阅扇到所有指定的终结点。</span><span class="sxs-lookup"><span data-stu-id="26002-138">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

<span data-ttu-id="26002-139">下表列出了可能返回的错误和响应代码。</span><span class="sxs-lookup"><span data-stu-id="26002-139">The following table lists the possible error and response codes that can be returned.</span></span>

|<span data-ttu-id="26002-140">错误代码</span><span class="sxs-lookup"><span data-stu-id="26002-140">Error code</span></span>             | <span data-ttu-id="26002-141">Descrition</span><span class="sxs-lookup"><span data-stu-id="26002-141">Descrition</span></span>                             |
|:-----------------------------------|:----------------------------------------------------------|
|<span data-ttu-id="26002-142">HttpStatusCode。 BadRequest</span><span class="sxs-lookup"><span data-stu-id="26002-142">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="26002-143">Body 为数组（不支持多个通知）。</span><span class="sxs-lookup"><span data-stu-id="26002-143">Body is an array (multiple notifications is not supported).</span></span>|
|<span data-ttu-id="26002-144">HttpStatusCode。 BadRequest</span><span class="sxs-lookup"><span data-stu-id="26002-144">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="26002-145">正文与 API 的协定不匹配。</span><span class="sxs-lookup"><span data-stu-id="26002-145">Body doesn't match the contract for the API.</span></span>               |
|<span data-ttu-id="26002-146">HttpStatusCode</span><span class="sxs-lookup"><span data-stu-id="26002-146">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="26002-147">呼叫者位于阻止列表中。</span><span class="sxs-lookup"><span data-stu-id="26002-147">Caller is on the blocked list.</span></span>                          |
|<span data-ttu-id="26002-148">HttpStatusCode。 MethodNotAllowed</span><span class="sxs-lookup"><span data-stu-id="26002-148">HttpStatusCode.MethodNotAllowed</span></span>     | <span data-ttu-id="26002-149">不支持使用的 HTTP 方法。</span><span class="sxs-lookup"><span data-stu-id="26002-149">The HTTP method used is not supported.</span></span>                     |
|<span data-ttu-id="26002-150">HttpStatusCode。 BadRequest</span><span class="sxs-lookup"><span data-stu-id="26002-150">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="26002-151">请求中存在不受支持的标头。</span><span class="sxs-lookup"><span data-stu-id="26002-151">Unsupported headers are present in the request.</span></span> <span data-ttu-id="26002-152">不支持两个标头：</span><span class="sxs-lookup"><span data-stu-id="26002-152">Two headers are not supported:</span></span><br/><br/><span data-ttu-id="26002-153">修改时间-自</span><span class="sxs-lookup"><span data-stu-id="26002-153">If-Modified-Since</span></span><br/><span data-ttu-id="26002-154">If-Range</span><span class="sxs-lookup"><span data-stu-id="26002-154">If-Range</span></span> |                    
|<span data-ttu-id="26002-155">HttpStatusCode。 UnsupportedMediaType</span><span class="sxs-lookup"><span data-stu-id="26002-155">HttpStatusCode.UnsupportedMediaType</span></span> | <span data-ttu-id="26002-156">标头内容编码存在，并且具有除`Deflate`或`Gzip`之外的压缩算法值。</span><span class="sxs-lookup"><span data-stu-id="26002-156">The header Content-Encoding is present and has compression algorithm values other than `Deflate` or `Gzip`.</span></span>  |
|<span data-ttu-id="26002-157">HttpStatusCode。 BadRequest</span><span class="sxs-lookup"><span data-stu-id="26002-157">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="26002-158">有效负载无效。</span><span class="sxs-lookup"><span data-stu-id="26002-158">Invalid payload.</span></span>                                           |
|<span data-ttu-id="26002-159">HttpStatusCode</span><span class="sxs-lookup"><span data-stu-id="26002-159">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="26002-160">呼叫者无权代表用户执行操作或向用户发送通知。</span><span class="sxs-lookup"><span data-stu-id="26002-160">Caller is not authorized to act on behalf of the user or send notification to the user.</span></span>                         |
|<span data-ttu-id="26002-161">HttpStatusCode 未经授权</span><span class="sxs-lookup"><span data-stu-id="26002-161">HttpStatusCode.Unauthorized</span></span>         |  <span data-ttu-id="26002-162">请求正文包含无效的活动数据类型。</span><span class="sxs-lookup"><span data-stu-id="26002-162">Request body contains invalid activity data types.</span></span>        |
|<span data-ttu-id="26002-163">HttpStatusCode</span><span class="sxs-lookup"><span data-stu-id="26002-163">HttpStatusCode.OK</span></span>                   |  <span data-ttu-id="26002-164">已成功创建活动。</span><span class="sxs-lookup"><span data-stu-id="26002-164">Activity successfully created.</span></span>                            |
|<span data-ttu-id="26002-165">HttpStatusCode。 NotAcceptable</span><span class="sxs-lookup"><span data-stu-id="26002-165">HttpStatusCode.NotAcceptable</span></span>        |  <span data-ttu-id="26002-166">请求已被阻止或服务器正忙。</span><span class="sxs-lookup"><span data-stu-id="26002-166">Request has been throttled or the server is busy.</span></span>    |


## <a name="example"></a><span data-ttu-id="26002-167">示例</span><span class="sxs-lookup"><span data-stu-id="26002-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="26002-168">请求</span><span class="sxs-lookup"><span data-stu-id="26002-168">Request</span></span>
<span data-ttu-id="26002-169">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="26002-169">The following is an example of a request.</span></span>

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

### <a name="response"></a><span data-ttu-id="26002-170">响应</span><span class="sxs-lookup"><span data-stu-id="26002-170">Response</span></span>
<span data-ttu-id="26002-171">下面是对应响应的一个示例。</span><span class="sxs-lookup"><span data-stu-id="26002-171">The following is an example of the corresponding response.</span></span>

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

