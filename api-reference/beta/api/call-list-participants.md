---
title: 列出参与者
description: 在呼叫中检索参与者对象的列表。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cf4b44f9e02037597a2c502272f55263568cd869
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440799"
---
# <a name="list-participants"></a><span data-ttu-id="911a3-103">列出参与者</span><span class="sxs-lookup"><span data-stu-id="911a3-103">List participants</span></span>

<span data-ttu-id="911a3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="911a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="911a3-105">在呼叫中检索参与者对象的列表。</span><span class="sxs-lookup"><span data-stu-id="911a3-105">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="911a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="911a3-106">Permissions</span></span>

| <span data-ttu-id="911a3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="911a3-107">Permission type</span></span> | <span data-ttu-id="911a3-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="911a3-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="911a3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="911a3-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="911a3-110">不支持</span><span class="sxs-lookup"><span data-stu-id="911a3-110">Not Supported</span></span>        |
| <span data-ttu-id="911a3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="911a3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="911a3-112">不支持</span><span class="sxs-lookup"><span data-stu-id="911a3-112">Not Supported</span></span>        |
| <span data-ttu-id="911a3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="911a3-113">Application</span></span>     | <span data-ttu-id="911a3-114">无</span><span class="sxs-lookup"><span data-stu-id="911a3-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="911a3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="911a3-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /communications/calls/{id}/participants
```
> <span data-ttu-id="911a3-116">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="911a3-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="911a3-117">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="911a3-117">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="911a3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="911a3-118">Optional query parameters</span></span>

<span data-ttu-id="911a3-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="911a3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="911a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="911a3-120">Request headers</span></span>

| <span data-ttu-id="911a3-121">名称</span><span class="sxs-lookup"><span data-stu-id="911a3-121">Name</span></span>          | <span data-ttu-id="911a3-122">说明</span><span class="sxs-lookup"><span data-stu-id="911a3-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="911a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="911a3-123">Authorization</span></span> | <span data-ttu-id="911a3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="911a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="911a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="911a3-126">Request body</span></span>

<span data-ttu-id="911a3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="911a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="911a3-128">响应</span><span class="sxs-lookup"><span data-stu-id="911a3-128">Response</span></span>

<span data-ttu-id="911a3-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[参与者](../resources/participant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="911a3-129">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="911a3-130">示例</span><span class="sxs-lookup"><span data-stu-id="911a3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="911a3-131">请求</span><span class="sxs-lookup"><span data-stu-id="911a3-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="911a3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="911a3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="c"></a>[<span data-ttu-id="911a3-133">C#</span><span class="sxs-lookup"><span data-stu-id="911a3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="911a3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="911a3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="911a3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="911a3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="911a3-136">响应</span><span class="sxs-lookup"><span data-stu-id="911a3-136">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "id":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
                  "displayName":null
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"3",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"a7ebfb2d-871e-419c-87af-27290b22e8db",
         "metadata":null,
         "recordingInfo":null
      },
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "displayName":"Test Participant",
                  "id":"ef43e42b-4c05-4594-9756-1edb3ccbc989",
                  "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"278405a3-f568-4b3e-b684-009193463064"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"1",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
         "metadata":null,
         "recordingInfo":null
      }
   ],
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
