---
title: 创建和发送通知
description: '创建和发送通知目标用户通过 Microsoft Graph。 通知存储在 Microsoft Graph 通知源存储，并发送到的用户登录到所有设备终结点上的所有应用程序客户端。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 70c7992a6fd323b909d948976132304fa04393c4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528443"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="a16da-104">创建和发送通知</span><span class="sxs-lookup"><span data-stu-id="a16da-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a16da-105">创建和发送通知目标用户通过 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="a16da-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="a16da-106">通知存储在 Microsoft Graph 通知源存储，并发送到的用户登录到所有设备终结点上的所有应用程序客户端。</span><span class="sxs-lookup"><span data-stu-id="a16da-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="a16da-107">权限</span><span class="sxs-lookup"><span data-stu-id="a16da-107">Permissions</span></span>
<span data-ttu-id="a16da-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a16da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a16da-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a16da-110">Permission type</span></span>      | <span data-ttu-id="a16da-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a16da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a16da-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a16da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a16da-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a16da-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a16da-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a16da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a16da-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a16da-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="a16da-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a16da-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="a16da-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a16da-117">Request headers</span></span>
|<span data-ttu-id="a16da-118">名称</span><span class="sxs-lookup"><span data-stu-id="a16da-118">Name</span></span> | <span data-ttu-id="a16da-119">类型</span><span class="sxs-lookup"><span data-stu-id="a16da-119">Type</span></span> | <span data-ttu-id="a16da-120">说明</span><span class="sxs-lookup"><span data-stu-id="a16da-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a16da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a16da-121">Authorization</span></span> | <span data-ttu-id="a16da-122">string</span><span class="sxs-lookup"><span data-stu-id="a16da-122">string</span></span> |<span data-ttu-id="a16da-123">Authorization 标头用于传递的呼叫方凭据。</span><span class="sxs-lookup"><span data-stu-id="a16da-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="a16da-124">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="a16da-124">Bearer {token}.</span></span> <span data-ttu-id="a16da-125">必需。</span><span class="sxs-lookup"><span data-stu-id="a16da-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="a16da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a16da-126">Request body</span></span>
<span data-ttu-id="a16da-127">在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a16da-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a16da-128">响应</span><span class="sxs-lookup"><span data-stu-id="a16da-128">Response</span></span>
<span data-ttu-id="a16da-129">如果成功，此方法返回`201 Created`响应代码，指示已成功创建并存储通知。</span><span class="sxs-lookup"><span data-stu-id="a16da-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="a16da-130">示例</span><span class="sxs-lookup"><span data-stu-id="a16da-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a16da-131">请求</span><span class="sxs-lookup"><span data-stu-id="a16da-131">Request</span></span>
<span data-ttu-id="a16da-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a16da-132">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a16da-133">响应</span><span class="sxs-lookup"><span data-stu-id="a16da-133">Response</span></span>
<span data-ttu-id="a16da-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a16da-134">The following is an example of the response.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-notification-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
