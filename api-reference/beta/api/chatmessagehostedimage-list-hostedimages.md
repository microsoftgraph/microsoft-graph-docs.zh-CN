---
title: 在 chatmessage 中列出 chatMessageHostedImages
description: 在 chatMessage 中列出所有托管图像。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 351e473e0d97ec23c1a4b859d637c40a3e49b7ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943552"
---
# <a name="list-chatmessagehostedimages-in-a-chatmessage"></a><span data-ttu-id="ba9c8-103">在 chatMessage 中列出 chatMessageHostedImages</span><span class="sxs-lookup"><span data-stu-id="ba9c8-103">List chatMessageHostedImages in a chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba9c8-104">在 [chatMessage](../resources/chatmessage.md) 中列出所有[托管图像](../resources/chatmessagehostedimage.md)。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-104">List all [hosted images](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba9c8-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba9c8-105">Permissions</span></span>

<span data-ttu-id="ba9c8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba9c8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba9c8-108">Permission Type</span></span>|<span data-ttu-id="ba9c8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba9c8-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ba9c8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba9c8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ba9c8-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba9c8-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="ba9c8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba9c8-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba9c8-113">不支持</span><span class="sxs-lookup"><span data-stu-id="ba9c8-113">Not supported</span></span>|
|<span data-ttu-id="ba9c8-114">Application</span><span class="sxs-lookup"><span data-stu-id="ba9c8-114">Application</span></span>| <span data-ttu-id="ba9c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba9c8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba9c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages
GET /chats/{id}/messages/{id}/hostedImages
GET /users/{id}/chats/{id}/messages/{id}/hostedImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba9c8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba9c8-117">Optional query parameters</span></span>

<span data-ttu-id="ba9c8-118">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba9c8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba9c8-119">Request headers</span></span>

| <span data-ttu-id="ba9c8-120">标头</span><span class="sxs-lookup"><span data-stu-id="ba9c8-120">Header</span></span>       | <span data-ttu-id="ba9c8-121">值</span><span class="sxs-lookup"><span data-stu-id="ba9c8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba9c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba9c8-122">Authorization</span></span>  | <span data-ttu-id="ba9c8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba9c8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba9c8-125">Request body</span></span>

<span data-ttu-id="ba9c8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba9c8-127">响应</span><span class="sxs-lookup"><span data-stu-id="ba9c8-127">Response</span></span>

<span data-ttu-id="ba9c8-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [hostedImage](../resources/chatmessagehostedimage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/chatmessagehostedimage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba9c8-129">示例</span><span class="sxs-lookup"><span data-stu-id="ba9c8-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba9c8-130">请求</span><span class="sxs-lookup"><span data-stu-id="ba9c8-130">Request</span></span>

<span data-ttu-id="ba9c8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/hostedImages
```

##### <a name="response"></a><span data-ttu-id="ba9c8-132">响应</span><span class="sxs-lookup"><span data-stu-id="ba9c8-132">Response</span></span>

<span data-ttu-id="ba9c8-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-133">Here is an example of the response.</span></span> 

><span data-ttu-id="ba9c8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "url": "url-value"
    },
    {
        "id": "id-value",
        "url": "url-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List hosted images in a chatmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
