---
title: 获取频道
description: 检索频道的属性和关系。
author: nkramer
doc_type: apiPageType
ms.prod: microsoft-teams
localization_priority: Normal
ms.openlocfilehash: 13309e8a52be84516d8bf8c7fd5e82a51eb9330b
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507044"
---
# <a name="get-channel"></a><span data-ttu-id="cd8bc-103">获取频道</span><span class="sxs-lookup"><span data-stu-id="cd8bc-103">Get channel</span></span>

<span data-ttu-id="cd8bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd8bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd8bc-105">检索[频道](../resources/channel.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd8bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="cd8bc-106">Permissions</span></span>

<span data-ttu-id="cd8bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd8bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd8bc-109">Permission type</span></span>      | <span data-ttu-id="cd8bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd8bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd8bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd8bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd8bc-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd8bc-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cd8bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd8bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd8bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-114">Not supported.</span></span>    |
|<span data-ttu-id="cd8bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd8bc-115">Application</span></span> | <span data-ttu-id="cd8bc-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd8bc-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cd8bc-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="cd8bc-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cd8bc-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cd8bc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd8bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd8bc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cd8bc-121">Optional query parameters</span></span>

<span data-ttu-id="cd8bc-122">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd8bc-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd8bc-123">Request headers</span></span>

| <span data-ttu-id="cd8bc-124">标头</span><span class="sxs-lookup"><span data-stu-id="cd8bc-124">Header</span></span>       | <span data-ttu-id="cd8bc-125">值</span><span class="sxs-lookup"><span data-stu-id="cd8bc-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd8bc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd8bc-126">Authorization</span></span>  | <span data-ttu-id="cd8bc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd8bc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd8bc-129">Request body</span></span>

<span data-ttu-id="cd8bc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd8bc-131">响应</span><span class="sxs-lookup"><span data-stu-id="cd8bc-131">Response</span></span>

<span data-ttu-id="cd8bc-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd8bc-133">示例</span><span class="sxs-lookup"><span data-stu-id="cd8bc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd8bc-134">请求</span><span class="sxs-lookup"><span data-stu-id="cd8bc-134">Request</span></span>

<span data-ttu-id="cd8bc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-135">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="cd8bc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd8bc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="c"></a>[<span data-ttu-id="cd8bc-137">C#</span><span class="sxs-lookup"><span data-stu-id="cd8bc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd8bc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd8bc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd8bc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd8bc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd8bc-140">Java</span><span class="sxs-lookup"><span data-stu-id="cd8bc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cd8bc-141">响应</span><span class="sxs-lookup"><span data-stu-id="cd8bc-141">Response</span></span>

<span data-ttu-id="cd8bc-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-142">Here is an example of the response.</span></span>

><span data-ttu-id="cd8bc-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd8bc-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
    "createdDateTime": "2020-05-27T19:22:25.692Z",
    "displayName": "General",
    "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
    "membershipType": "standard"
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
