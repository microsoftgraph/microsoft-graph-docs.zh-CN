---
title: 聊天： getAllMessages
description: 从用户参与的所有聊天中获取消息。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 12b645943297d34504bb4d4586ecbd8d3e79b7c6
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582653"
---
# <a name="chats-getallmessages"></a><span data-ttu-id="957a5-103">聊天： getAllMessages</span><span class="sxs-lookup"><span data-stu-id="957a5-103">chats: getAllMessages</span></span>

<span data-ttu-id="957a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="957a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="957a5-105">从用户参与的所有 [聊天](../resources/chatmessage.md) 中获取所有消息，包括一对一聊天、群聊天和会议聊天。</span><span class="sxs-lookup"><span data-stu-id="957a5-105">Get all messages from all [chats](../resources/chatmessage.md) that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span>

## <a name="permissions"></a><span data-ttu-id="957a5-106">权限</span><span class="sxs-lookup"><span data-stu-id="957a5-106">Permissions</span></span>

<span data-ttu-id="957a5-107">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="957a5-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="957a5-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="957a5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="957a5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="957a5-109">Permission type</span></span>      | <span data-ttu-id="957a5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="957a5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="957a5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="957a5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="957a5-112">不支持</span><span class="sxs-lookup"><span data-stu-id="957a5-112">Not supported</span></span> |
|<span data-ttu-id="957a5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="957a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="957a5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="957a5-114">Not supported</span></span> |
|<span data-ttu-id="957a5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="957a5-115">Application</span></span> | <span data-ttu-id="957a5-116">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957a5-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="957a5-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="957a5-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="957a5-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="957a5-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="957a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="957a5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="957a5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="957a5-120">Optional query parameters</span></span>

<span data-ttu-id="957a5-121">此操作支持 [日期范围参数](/graph/query-parameters) 来自定义响应，如下例所示。</span><span class="sxs-lookup"><span data-stu-id="957a5-121">This operation supports [date range parameters](/graph/query-parameters) to customize the response, as shown in the following example.</span></span>

```http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a><span data-ttu-id="957a5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="957a5-122">Request headers</span></span>
| <span data-ttu-id="957a5-123">标头</span><span class="sxs-lookup"><span data-stu-id="957a5-123">Header</span></span>       | <span data-ttu-id="957a5-124">值</span><span class="sxs-lookup"><span data-stu-id="957a5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="957a5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="957a5-125">Authorization</span></span>  | <span data-ttu-id="957a5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="957a5-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="957a5-128">响应</span><span class="sxs-lookup"><span data-stu-id="957a5-128">Response</span></span>

<span data-ttu-id="957a5-129">如果成功，此方法将在正文中返回 `200 OK` 响应代码和[chatMessages](../resources/chatmessage.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="957a5-129">If successful, this method returns a `200 OK` response code and a list of [chatMessages](../resources/chatmessage.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="957a5-130">示例</span><span class="sxs-lookup"><span data-stu-id="957a5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="957a5-131">请求</span><span class="sxs-lookup"><span data-stu-id="957a5-131">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages
```

### <a name="response"></a><span data-ttu-id="957a5-132">响应</span><span class="sxs-lookup"><span data-stu-id="957a5-132">Response</span></span>

><span data-ttu-id="957a5-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="957a5-133">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK 
Content-type: application/json 
Content-length: 347 

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.count":10,
   "@odata.nextLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages?$skip=10",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[
            
         ],
         "mentions":[
            
         ],
         "reactions":[
            
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
  "description": "chats: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
