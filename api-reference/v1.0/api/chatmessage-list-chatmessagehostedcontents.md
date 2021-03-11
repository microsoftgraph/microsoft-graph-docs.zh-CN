---
title: 列出 chatMessageHostedContents
description: 从邮件中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16dc59427eeab168d816780c9fcdc5c6603a1955
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634290"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="337b9-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="337b9-103">List hostedContents</span></span>

<span data-ttu-id="337b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="337b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="337b9-105">从邮件中 [检索 chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="337b9-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="337b9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="337b9-106">Permissions</span></span>

<span data-ttu-id="337b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="337b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="337b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="337b9-109">Permission type</span></span>                        | <span data-ttu-id="337b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="337b9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="337b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="337b9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="337b9-112">对于 **通道** 资源：ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="337b9-112">For **channel** resource: ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="337b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="337b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="337b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="337b9-114">Not supported.</span></span>|
|<span data-ttu-id="337b9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="337b9-115">Application</span></span>| <span data-ttu-id="337b9-116">对于 **通道** 资源：ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="337b9-116">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="337b9-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="337b9-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="337b9-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="337b9-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="337b9-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="337b9-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="337b9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="337b9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="337b9-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="337b9-121">Optional query parameters</span></span>

<span data-ttu-id="337b9-122">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="337b9-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="337b9-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="337b9-123">Request headers</span></span>

| <span data-ttu-id="337b9-124">名称</span><span class="sxs-lookup"><span data-stu-id="337b9-124">Name</span></span>      |<span data-ttu-id="337b9-125">说明</span><span class="sxs-lookup"><span data-stu-id="337b9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="337b9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="337b9-126">Authorization</span></span> | <span data-ttu-id="337b9-127">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="337b9-127">Bearer {code}.</span></span> <span data-ttu-id="337b9-128">必需。</span><span class="sxs-lookup"><span data-stu-id="337b9-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="337b9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="337b9-129">Request body</span></span>

<span data-ttu-id="337b9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="337b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="337b9-131">响应</span><span class="sxs-lookup"><span data-stu-id="337b9-131">Response</span></span>

<span data-ttu-id="337b9-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="337b9-132">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="337b9-133">示例</span><span class="sxs-lookup"><span data-stu-id="337b9-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="337b9-134">请求</span><span class="sxs-lookup"><span data-stu-id="337b9-134">Request</span></span>

<span data-ttu-id="337b9-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="337b9-135">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents
```

### <a name="response"></a><span data-ttu-id="337b9-136">响应</span><span class="sxs-lookup"><span data-stu-id="337b9-136">Response</span></span>

<span data-ttu-id="337b9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="337b9-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="337b9-138">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="337b9-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="337b9-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="337b9-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


