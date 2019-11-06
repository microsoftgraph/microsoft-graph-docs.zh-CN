---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996262"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="45143-103">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="45143-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45143-104">创建并发送针对用户通过 Microsoft Graph 的通知。</span><span class="sxs-lookup"><span data-stu-id="45143-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="45143-105">通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="45143-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="45143-106">权限</span><span class="sxs-lookup"><span data-stu-id="45143-106">Permissions</span></span>
<span data-ttu-id="45143-107">您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="45143-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="45143-108">如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="45143-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="45143-109">建议不要在发布通知时选择此选项，但如果您想了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45143-109">We don't recommend this option for posting notifications but if you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45143-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45143-110">Permission type</span></span>      | <span data-ttu-id="45143-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45143-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45143-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45143-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45143-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="45143-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="45143-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45143-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45143-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="45143-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
| <span data-ttu-id="45143-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="45143-116">Application</span></span>                           | <span data-ttu-id="45143-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="45143-117">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="45143-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45143-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="45143-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="45143-119">Request headers</span></span>
|<span data-ttu-id="45143-120">名称</span><span class="sxs-lookup"><span data-stu-id="45143-120">Name</span></span> | <span data-ttu-id="45143-121">类型</span><span class="sxs-lookup"><span data-stu-id="45143-121">Type</span></span> | <span data-ttu-id="45143-122">说明</span><span class="sxs-lookup"><span data-stu-id="45143-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="45143-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45143-123">Authorization</span></span> | <span data-ttu-id="45143-124">string</span><span class="sxs-lookup"><span data-stu-id="45143-124">string</span></span> |<span data-ttu-id="45143-125">授权标头用于传递呼叫方的凭据。</span><span class="sxs-lookup"><span data-stu-id="45143-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="45143-126">持有者 {令牌}。</span><span class="sxs-lookup"><span data-stu-id="45143-126">Bearer {token}.</span></span> <span data-ttu-id="45143-127">必填。</span><span class="sxs-lookup"><span data-stu-id="45143-127">Required.</span></span> |
|<span data-ttu-id="45143-128">X-UNS-ID</span><span class="sxs-lookup"><span data-stu-id="45143-128">X-UNS-ID</span></span> | <span data-ttu-id="45143-129">string</span><span class="sxs-lookup"><span data-stu-id="45143-129">string</span></span> |<span data-ttu-id="45143-130">Microsoft Graph 通知服务在客户端上创建订阅后返回的 UserNotificationSubscriptionId，用于面向特定用户。</span><span class="sxs-lookup"><span data-stu-id="45143-130">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription on the client-side, and is used to target the specific user.</span></span> <span data-ttu-id="45143-131">必需。</span><span class="sxs-lookup"><span data-stu-id="45143-131">Required.</span></span> |
|<span data-ttu-id="45143-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="45143-132">Content-type</span></span>| <span data-ttu-id="45143-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="45143-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45143-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="45143-135">Request body</span></span>
<span data-ttu-id="45143-136">在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45143-136">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45143-137">响应</span><span class="sxs-lookup"><span data-stu-id="45143-137">Response</span></span>
<span data-ttu-id="45143-138">如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。</span><span class="sxs-lookup"><span data-stu-id="45143-138">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="45143-139">随后，通知将通过有效订阅扇到所有指定的终结点。</span><span class="sxs-lookup"><span data-stu-id="45143-139">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="45143-140">示例</span><span class="sxs-lookup"><span data-stu-id="45143-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="45143-141">请求</span><span class="sxs-lookup"><span data-stu-id="45143-141">Request</span></span>
<span data-ttu-id="45143-142">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="45143-142">The following is an example of a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45143-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="45143-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45143-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45143-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45143-145">响应</span><span class="sxs-lookup"><span data-stu-id="45143-145">Response</span></span>
<span data-ttu-id="45143-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45143-146">The following is an example of the response.</span></span>

> <span data-ttu-id="45143-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="45143-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
