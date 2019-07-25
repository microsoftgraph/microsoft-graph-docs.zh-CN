---
title: 获取 chatMessageHostedImage
description: 在了 chatmessage 中检索承载的图像。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 017ea361fd0626212d8227b0c8197aabab8dd5f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863414"
---
# <a name="get-chatmessagehostedimage"></a><span data-ttu-id="73505-103">获取 chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="73505-103">Get chatMessageHostedImage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73505-104">在[了 chatmessage](../resources/chatmessage.md)中检索[承载的图像](../resources/chatmessagehostedimage.md)。</span><span class="sxs-lookup"><span data-stu-id="73505-104">Retrieve a [hosted image](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73505-105">权限</span><span class="sxs-lookup"><span data-stu-id="73505-105">Permissions</span></span>

<span data-ttu-id="73505-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73505-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73505-108">Permission Type</span></span>|<span data-ttu-id="73505-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73505-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="73505-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73505-110">Delegated (work or school account)</span></span>|<span data-ttu-id="73505-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73505-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="73505-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73505-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73505-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="73505-113">Not supported.</span></span>|
|<span data-ttu-id="73505-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73505-114">Application</span></span>| <span data-ttu-id="73505-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73505-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73505-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73505-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}
GET /chats/{id}/messages/{id}/hostedImages/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73505-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73505-117">Optional query parameters</span></span>

<span data-ttu-id="73505-118">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73505-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73505-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73505-119">Request headers</span></span>

| <span data-ttu-id="73505-120">标头</span><span class="sxs-lookup"><span data-stu-id="73505-120">Header</span></span>       | <span data-ttu-id="73505-121">值</span><span class="sxs-lookup"><span data-stu-id="73505-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73505-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73505-122">Authorization</span></span>  | <span data-ttu-id="73505-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73505-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73505-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="73505-125">Request body</span></span>

<span data-ttu-id="73505-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73505-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73505-127">响应</span><span class="sxs-lookup"><span data-stu-id="73505-127">Response</span></span>

<span data-ttu-id="73505-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[托管的 image](../resources/chatmessagehostedimage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73505-128">If successful, this method returns a `200 OK` response code and a [hosted image](../resources/chatmessagehostedimage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73505-129">示例</span><span class="sxs-lookup"><span data-stu-id="73505-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73505-130">请求</span><span class="sxs-lookup"><span data-stu-id="73505-130">Request</span></span>

<span data-ttu-id="73505-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73505-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73505-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="73505-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73505-133">C#</span><span class="sxs-lookup"><span data-stu-id="73505-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73505-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="73505-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73505-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="73505-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73505-136">Java</span><span class="sxs-lookup"><span data-stu-id="73505-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73505-137">响应</span><span class="sxs-lookup"><span data-stu-id="73505-137">Response</span></span>

<span data-ttu-id="73505-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73505-138">Here is an example of the response.</span></span> 

><span data-ttu-id="73505-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73505-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "url": "url-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat message image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
