---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ff4776b35544b62c7388bc760a54893c35dba36
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720873"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="ed5b5-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="ed5b5-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed5b5-104">检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed5b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed5b5-105">Permissions</span></span>

<span data-ttu-id="ed5b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed5b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed5b5-108">Permission type</span></span>                        | <span data-ttu-id="ed5b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed5b5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed5b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed5b5-111">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="ed5b5-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="ed5b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed5b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-113">Not supported.</span></span> |
| <span data-ttu-id="ed5b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed5b5-114">Application</span></span>                            | <span data-ttu-id="ed5b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed5b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed5b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed5b5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed5b5-117">Optional query parameters</span></span>

<span data-ttu-id="ed5b5-118">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed5b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed5b5-119">Request headers</span></span>

| <span data-ttu-id="ed5b5-120">名称</span><span class="sxs-lookup"><span data-stu-id="ed5b5-120">Name</span></span>      |<span data-ttu-id="ed5b5-121">说明</span><span class="sxs-lookup"><span data-stu-id="ed5b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed5b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed5b5-122">Authorization</span></span> | <span data-ttu-id="ed5b5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ed5b5-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed5b5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed5b5-124">Request body</span></span>

<span data-ttu-id="ed5b5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5b5-126">响应</span><span class="sxs-lookup"><span data-stu-id="ed5b5-126">Response</span></span>

<span data-ttu-id="ed5b5-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed5b5-128">示例</span><span class="sxs-lookup"><span data-stu-id="ed5b5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed5b5-129">请求</span><span class="sxs-lookup"><span data-stu-id="ed5b5-129">Request</span></span>

<span data-ttu-id="ed5b5-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```

### <a name="response"></a><span data-ttu-id="ed5b5-131">响应</span><span class="sxs-lookup"><span data-stu-id="ed5b5-131">Response</span></span>

<span data-ttu-id="ed5b5-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ed5b5-133">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ed5b5-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed5b5-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->