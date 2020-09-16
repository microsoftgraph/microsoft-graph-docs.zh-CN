---
title: 更新 onlineMeeting
description: 更新联机会议的属性。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6e971c8b608ad5e42c225cea2aa5da0ad06cedbc
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843259"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="a3278-103">更新 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a3278-103">Update onlineMeeting</span></span>

<span data-ttu-id="a3278-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3278-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3278-105">更新指定[onlineMeeting](../resources/onlinemeeting.md)的**startDateTime**、 **endDateTime**、**参与者**和**subject**属性。</span><span class="sxs-lookup"><span data-stu-id="a3278-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a3278-106">权限</span><span class="sxs-lookup"><span data-stu-id="a3278-106">Permissions</span></span>

| <span data-ttu-id="a3278-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3278-107">Permission type</span></span>                        | <span data-ttu-id="a3278-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3278-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a3278-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3278-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3278-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3278-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="a3278-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3278-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3278-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3278-112">Not Supported.</span></span>                              |
| <span data-ttu-id="a3278-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3278-113">Application</span></span>                            | <span data-ttu-id="a3278-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a3278-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="a3278-115">\* 管理员必须创建 [应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy.md) ，并向用户授予该策略中配置的应用程序，以便代表该用户更新联机会议 (用户 ID 在请求路径) 中指定。</span><span class="sxs-lookup"><span data-stu-id="a3278-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy.md) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="a3278-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3278-116">HTTP request</span></span>

<span data-ttu-id="a3278-117">使用委派令牌的请求：</span><span class="sxs-lookup"><span data-stu-id="a3278-117">Request using a delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="a3278-118">使用应用程序令牌请求：</span><span class="sxs-lookup"><span data-stu-id="a3278-118">Request using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="a3278-119">**注意：**</span><span class="sxs-lookup"><span data-stu-id="a3278-119">**Notes:**</span></span>
>
> - <span data-ttu-id="a3278-120">`userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="a3278-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="a3278-121">有关更多详细信息，请参阅 [应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy.md)。</span><span class="sxs-lookup"><span data-stu-id="a3278-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy.md).</span></span>
> - <span data-ttu-id="a3278-122">`meetingId`是[onlineMeeting 实体](../resources/onlinemeeting.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="a3278-122">`meetingId` is the **id** of an [onlineMeeting entity](../resources/onlinemeeting.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3278-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3278-123">Request headers</span></span>
| <span data-ttu-id="a3278-124">名称</span><span class="sxs-lookup"><span data-stu-id="a3278-124">Name</span></span>          | <span data-ttu-id="a3278-125">说明</span><span class="sxs-lookup"><span data-stu-id="a3278-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="a3278-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3278-126">Authorization</span></span> | <span data-ttu-id="a3278-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3278-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a3278-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="a3278-129">Content-type</span></span>  | <span data-ttu-id="a3278-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a3278-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3278-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3278-132">Request body</span></span>
<span data-ttu-id="a3278-133">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3278-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="a3278-134">只能修改 **startDateTime**、 **endDateTime**、 **参与者**和 **subject** 属性。</span><span class="sxs-lookup"><span data-stu-id="a3278-134">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="a3278-135">**StartDateTime**和**endDateTime**必须成对出现。</span><span class="sxs-lookup"><span data-stu-id="a3278-135">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="a3278-136">响应</span><span class="sxs-lookup"><span data-stu-id="a3278-136">Response</span></span>
<span data-ttu-id="a3278-137">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3278-137">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3278-138">示例</span><span class="sxs-lookup"><span data-stu-id="a3278-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3278-139">请求</span><span class="sxs-lookup"><span data-stu-id="a3278-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a3278-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3278-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_onlinemeeting_request"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="a3278-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3278-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-onlinemeeting-request-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3278-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3278-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-onlinemeeting-request-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3278-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3278-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-onlinemeeting-request-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3278-144">响应</span><span class="sxs-lookup"><span data-stu-id="a3278-144">Response</span></span>

><span data-ttu-id="a3278-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3278-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"{id}",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"number",
      "tollFreeNumber":null,
      "dialinUrl":"url"
   }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
