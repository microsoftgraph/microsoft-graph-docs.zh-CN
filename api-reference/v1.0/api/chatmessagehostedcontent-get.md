---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2a3fe469cd0a1cf10242c1f89370c8a6932ec866
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634289"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="502a2-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="502a2-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="502a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="502a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="502a2-105">检索 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="502a2-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="502a2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="502a2-106">Permissions</span></span>

<span data-ttu-id="502a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="502a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="502a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="502a2-109">Permission type</span></span>                        | <span data-ttu-id="502a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="502a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="502a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="502a2-111">Delegated (work or school account)</span></span>| <span data-ttu-id="502a2-112">对于 **通道** 资源：ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="502a2-112">For **channel** resource: ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="502a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="502a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="502a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="502a2-114">Not supported.</span></span>|
|<span data-ttu-id="502a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="502a2-115">Application</span></span>| <span data-ttu-id="502a2-116">对于 **通道** 资源：ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="502a2-116">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="502a2-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="502a2-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="502a2-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="502a2-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="502a2-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="502a2-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="502a2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="502a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="502a2-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="502a2-121">Optional query parameters</span></span>

<span data-ttu-id="502a2-122">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="502a2-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="502a2-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="502a2-123">Request headers</span></span>

| <span data-ttu-id="502a2-124">名称</span><span class="sxs-lookup"><span data-stu-id="502a2-124">Name</span></span>      |<span data-ttu-id="502a2-125">说明</span><span class="sxs-lookup"><span data-stu-id="502a2-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="502a2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="502a2-126">Authorization</span></span> | <span data-ttu-id="502a2-127">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="502a2-127">Bearer {code}.</span></span> <span data-ttu-id="502a2-128">必需。</span><span class="sxs-lookup"><span data-stu-id="502a2-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="502a2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="502a2-129">Request body</span></span>

<span data-ttu-id="502a2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="502a2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="502a2-131">响应</span><span class="sxs-lookup"><span data-stu-id="502a2-131">Response</span></span>

<span data-ttu-id="502a2-132">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="502a2-132">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="502a2-133">示例</span><span class="sxs-lookup"><span data-stu-id="502a2-133">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="502a2-134">示例 1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="502a2-134">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="502a2-135">请求</span><span class="sxs-lookup"><span data-stu-id="502a2-135">Request</span></span>

<span data-ttu-id="502a2-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="502a2-136">The following is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv
```

#### <a name="response"></a><span data-ttu-id="502a2-137">响应</span><span class="sxs-lookup"><span data-stu-id="502a2-137">Response</span></span>

<span data-ttu-id="502a2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="502a2-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="502a2-139">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="502a2-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="502a2-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="502a2-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes"></a><span data-ttu-id="502a2-141">示例 2：获取托管内容字节</span><span class="sxs-lookup"><span data-stu-id="502a2-141">Example 2: Get hosted content bytes</span></span>

#### <a name="request"></a><span data-ttu-id="502a2-142">请求</span><span class="sxs-lookup"><span data-stu-id="502a2-142">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv/$value
```

#### <a name="response"></a><span data-ttu-id="502a2-143">响应</span><span class="sxs-lookup"><span data-stu-id="502a2-143">Response</span></span>

> [!NOTE]
> <span data-ttu-id="502a2-144">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="502a2-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="502a2-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="502a2-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201

<ContentBytes>
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


