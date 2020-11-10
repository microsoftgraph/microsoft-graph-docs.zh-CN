---
title: 列出频道
description: 检索此团队中的频道列表。
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9984cfbaf303013bf06094b40b873137209c858a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959159"
---
# <a name="list-channels"></a><span data-ttu-id="3fbec-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="3fbec-103">List channels</span></span>

<span data-ttu-id="3fbec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fbec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fbec-105">检索此[团队](../resources/team.md)中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="3fbec-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fbec-106">权限</span><span class="sxs-lookup"><span data-stu-id="3fbec-106">Permissions</span></span>

<span data-ttu-id="3fbec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fbec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fbec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fbec-109">Permission type</span></span>      | <span data-ttu-id="3fbec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fbec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fbec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fbec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fbec-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fbec-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3fbec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fbec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fbec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fbec-114">Not supported.</span></span>    |
|<span data-ttu-id="3fbec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fbec-115">Application</span></span> | <span data-ttu-id="3fbec-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fbec-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3fbec-117">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="3fbec-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="3fbec-118">**注意** ：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="3fbec-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="3fbec-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="3fbec-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3fbec-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fbec-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fbec-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3fbec-121">Optional query parameters</span></span>
<span data-ttu-id="3fbec-122">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3fbec-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fbec-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fbec-123">Request headers</span></span>

| <span data-ttu-id="3fbec-124">标头</span><span class="sxs-lookup"><span data-stu-id="3fbec-124">Header</span></span>       | <span data-ttu-id="3fbec-125">值</span><span class="sxs-lookup"><span data-stu-id="3fbec-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3fbec-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fbec-126">Authorization</span></span>  | <span data-ttu-id="3fbec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3fbec-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fbec-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fbec-129">Request body</span></span>

<span data-ttu-id="3fbec-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3fbec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fbec-131">响应</span><span class="sxs-lookup"><span data-stu-id="3fbec-131">Response</span></span>

<span data-ttu-id="3fbec-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3fbec-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3fbec-133">示例</span><span class="sxs-lookup"><span data-stu-id="3fbec-133">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="3fbec-134">示例 1：列出所有频道</span><span class="sxs-lookup"><span data-stu-id="3fbec-134">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="3fbec-135">请求</span><span class="sxs-lookup"><span data-stu-id="3fbec-135">Request</span></span>

<span data-ttu-id="3fbec-136">以下示例显示列出所有频道的请求。</span><span class="sxs-lookup"><span data-stu-id="3fbec-136">The following example shows a request to list all channels.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fbec-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fbec-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="3fbec-138">C#</span><span class="sxs-lookup"><span data-stu-id="3fbec-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fbec-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fbec-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fbec-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fbec-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fbec-141">Java</span><span class="sxs-lookup"><span data-stu-id="3fbec-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3fbec-142">响应</span><span class="sxs-lookup"><span data-stu-id="3fbec-142">Response</span></span>

<span data-ttu-id="3fbec-143">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="3fbec-143">The following is the response.</span></span>

> <span data-ttu-id="3fbec-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3fbec-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3fbec-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3fbec-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="3fbec-146">示例 2：列出所有私人频道</span><span class="sxs-lookup"><span data-stu-id="3fbec-146">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="3fbec-147">请求</span><span class="sxs-lookup"><span data-stu-id="3fbec-147">Request</span></span>

<span data-ttu-id="3fbec-148">以下示例显示列出所有私人频道的请求。</span><span class="sxs-lookup"><span data-stu-id="3fbec-148">The following example shows a request to list all private channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="3fbec-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fbec-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="3fbec-150">C#</span><span class="sxs-lookup"><span data-stu-id="3fbec-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fbec-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fbec-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fbec-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fbec-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fbec-153">Java</span><span class="sxs-lookup"><span data-stu-id="3fbec-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3fbec-154">响应</span><span class="sxs-lookup"><span data-stu-id="3fbec-154">Response</span></span>

<span data-ttu-id="3fbec-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3fbec-155">The following is an example of the response.</span></span>

> <span data-ttu-id="3fbec-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3fbec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


