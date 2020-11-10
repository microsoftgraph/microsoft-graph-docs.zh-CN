---
title: 获取频道
description: 检索频道的属性和关系。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 71fba99ad7cd3faa300c57264385e871cf386f2f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959227"
---
# <a name="get-channel"></a><span data-ttu-id="cc84b-103">获取频道</span><span class="sxs-lookup"><span data-stu-id="cc84b-103">Get channel</span></span>

<span data-ttu-id="cc84b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc84b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc84b-105">检索[频道](../resources/channel.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc84b-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc84b-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc84b-106">Permissions</span></span>

<span data-ttu-id="cc84b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc84b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc84b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc84b-109">Permission type</span></span>      | <span data-ttu-id="cc84b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc84b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc84b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc84b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc84b-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc84b-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cc84b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc84b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc84b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc84b-114">Not supported.</span></span>    |
|<span data-ttu-id="cc84b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc84b-115">Application</span></span> | <span data-ttu-id="cc84b-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc84b-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cc84b-117">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="cc84b-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="cc84b-118">**注意** ：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="cc84b-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="cc84b-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="cc84b-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc84b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc84b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc84b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc84b-121">Optional query parameters</span></span>

<span data-ttu-id="cc84b-122">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cc84b-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc84b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc84b-123">Request headers</span></span>

| <span data-ttu-id="cc84b-124">标头</span><span class="sxs-lookup"><span data-stu-id="cc84b-124">Header</span></span>       | <span data-ttu-id="cc84b-125">值</span><span class="sxs-lookup"><span data-stu-id="cc84b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc84b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc84b-126">Authorization</span></span>  | <span data-ttu-id="cc84b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc84b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc84b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc84b-129">Request body</span></span>

<span data-ttu-id="cc84b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc84b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc84b-131">响应</span><span class="sxs-lookup"><span data-stu-id="cc84b-131">Response</span></span>

<span data-ttu-id="cc84b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc84b-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc84b-133">示例</span><span class="sxs-lookup"><span data-stu-id="cc84b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc84b-134">请求</span><span class="sxs-lookup"><span data-stu-id="cc84b-134">Request</span></span>

<span data-ttu-id="cc84b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc84b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc84b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc84b-136">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

# <a name="c"></a>[<span data-ttu-id="cc84b-137">C#</span><span class="sxs-lookup"><span data-stu-id="cc84b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc84b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc84b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc84b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc84b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc84b-140">Java</span><span class="sxs-lookup"><span data-stu-id="cc84b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cc84b-141">响应</span><span class="sxs-lookup"><span data-stu-id="cc84b-141">Response</span></span>

<span data-ttu-id="cc84b-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc84b-142">Here is an example of the response.</span></span>

><span data-ttu-id="cc84b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cc84b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value",
    "membershipType": "membership-type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


