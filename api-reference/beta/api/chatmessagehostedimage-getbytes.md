---
title: 'chatMessageHostedImage: getBytes'
description: 获取频道或聊天消息中的托管图像的二进制表示形式。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4830e3f845d657e5b073c27e228976bfe9926630
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943566"
---
# <a name="chatmessagehostedimage-getbytes"></a><span data-ttu-id="dcbc0-103">chatMessageHostedImage: getBytes</span><span class="sxs-lookup"><span data-stu-id="dcbc0-103">chatMessageHostedImage: getBytes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcbc0-104">获取[邮件](../resources/chatmessage.md)中[托管图像](../resources/chatmessagehostedimage.md)的二进制表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-104">Get the binary representation of a [hosted image](../resources/chatmessagehostedimage.md) in a [message](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcbc0-105">权限</span><span class="sxs-lookup"><span data-stu-id="dcbc0-105">Permissions</span></span>

<span data-ttu-id="dcbc0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcbc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcbc0-108">Permission Type</span></span>|<span data-ttu-id="dcbc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcbc0-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="dcbc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbc0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="dcbc0-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcbc0-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="dcbc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbc0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcbc0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-113">Not supported.</span></span>|
|<span data-ttu-id="dcbc0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcbc0-114">Application</span></span>| <span data-ttu-id="dcbc0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcbc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcbc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}/$value
GET /chats/{id}/messages/{id}/hostedImages/{id}/$value
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcbc0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dcbc0-117">Optional query parameters</span></span>

<span data-ttu-id="dcbc0-118">此方法不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-118">This method does not support the [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcbc0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcbc0-119">Request headers</span></span>

| <span data-ttu-id="dcbc0-120">标头</span><span class="sxs-lookup"><span data-stu-id="dcbc0-120">Header</span></span>       | <span data-ttu-id="dcbc0-121">值</span><span class="sxs-lookup"><span data-stu-id="dcbc0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dcbc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcbc0-122">Authorization</span></span>  | <span data-ttu-id="dcbc0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dcbc0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcbc0-125">Request body</span></span>

<span data-ttu-id="dcbc0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcbc0-127">响应</span><span class="sxs-lookup"><span data-stu-id="dcbc0-127">Response</span></span>

<span data-ttu-id="dcbc0-128">如果成功, 此方法将`200 OK`返回请求的图像的响应代码和二进制数据。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-128">If successful, this method returns a `200 OK` response code and binary data of the requested image.</span></span>

## <a name="example"></a><span data-ttu-id="dcbc0-129">示例</span><span class="sxs-lookup"><span data-stu-id="dcbc0-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dcbc0-130">请求</span><span class="sxs-lookup"><span data-stu-id="dcbc0-130">Request</span></span>

<span data-ttu-id="dcbc0-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->

```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
```

##### <a name="response"></a><span data-ttu-id="dcbc0-132">响应</span><span class="sxs-lookup"><span data-stu-id="dcbc0-132">Response</span></span>

<span data-ttu-id="dcbc0-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-133">Here is an example of the response.</span></span>

><span data-ttu-id="dcbc0-134">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="dcbc0-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dcbc0-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bytes of a hosted image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-getbytes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
