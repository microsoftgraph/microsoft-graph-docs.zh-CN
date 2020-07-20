---
title: 更新 onlineMeeting
description: 更新联机会议的属性。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4fc506d37bc0166057fe7997e198d02a6771267d
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45184022"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="9e690-103">更新 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9e690-103">Update onlineMeeting</span></span>

<span data-ttu-id="9e690-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e690-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e690-105">更新指定[onlineMeeting](../resources/onlinemeeting.md)的**startDateTime**、 **endDateTime**、**参与者**和**subject**属性。</span><span class="sxs-lookup"><span data-stu-id="9e690-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e690-106">权限</span><span class="sxs-lookup"><span data-stu-id="9e690-106">Permissions</span></span>

| <span data-ttu-id="9e690-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e690-107">Permission type</span></span> | <span data-ttu-id="9e690-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e690-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="9e690-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e690-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e690-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e690-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="9e690-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e690-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e690-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e690-112">Not Supported.</span></span>                         |
| <span data-ttu-id="9e690-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e690-113">Application</span></span>                            | <span data-ttu-id="9e690-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e690-114">Not Supported.</span></span>                                  |


## <a name="http-request"></a><span data-ttu-id="9e690-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e690-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9e690-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e690-116">Request headers</span></span>
| <span data-ttu-id="9e690-117">名称</span><span class="sxs-lookup"><span data-stu-id="9e690-117">Name</span></span>          | <span data-ttu-id="9e690-118">说明</span><span class="sxs-lookup"><span data-stu-id="9e690-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9e690-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e690-119">Authorization</span></span> | <span data-ttu-id="9e690-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e690-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e690-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="9e690-122">Content-type</span></span>  | <span data-ttu-id="9e690-p102">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9e690-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e690-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e690-125">Request body</span></span>
<span data-ttu-id="9e690-126">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e690-126">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="9e690-127">只能修改**startDateTime**、 **endDateTime**、**参与者**和**subject**属性。</span><span class="sxs-lookup"><span data-stu-id="9e690-127">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="9e690-128">**StartDateTime**和**endDateTime**必须成对出现。</span><span class="sxs-lookup"><span data-stu-id="9e690-128">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="9e690-129">响应</span><span class="sxs-lookup"><span data-stu-id="9e690-129">Response</span></span>
<span data-ttu-id="9e690-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e690-130">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e690-131">示例</span><span class="sxs-lookup"><span data-stu-id="9e690-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e690-132">请求</span><span class="sxs-lookup"><span data-stu-id="9e690-132">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="9e690-133">响应</span><span class="sxs-lookup"><span data-stu-id="9e690-133">Response</span></span>

><span data-ttu-id="9e690-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9e690-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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
