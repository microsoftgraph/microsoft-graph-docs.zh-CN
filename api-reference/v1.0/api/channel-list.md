---
title: 列出频道
description: 检索此团队中的频道列表。
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 967a8cbfc1a3ec909b3fb7e5e36c7c3e7f00730a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509213"
---
# <a name="list-channels"></a><span data-ttu-id="6b950-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="6b950-103">List channels</span></span>

<span data-ttu-id="6b950-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b950-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6b950-105">检索此[团队](../resources/team.md)中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="6b950-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b950-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b950-106">Permissions</span></span>

<span data-ttu-id="6b950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b950-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b950-109">Permission type</span></span>      | <span data-ttu-id="6b950-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b950-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b950-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b950-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b950-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b950-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6b950-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b950-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b950-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b950-114">Not supported.</span></span>    |
|<span data-ttu-id="6b950-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b950-115">Application</span></span> | <span data-ttu-id="6b950-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b950-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="6b950-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6b950-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6b950-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="6b950-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b950-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b950-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b950-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b950-120">Optional query parameters</span></span>

<span data-ttu-id="6b950-121">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b950-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b950-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b950-122">Request headers</span></span>

| <span data-ttu-id="6b950-123">标头</span><span class="sxs-lookup"><span data-stu-id="6b950-123">Header</span></span>       | <span data-ttu-id="6b950-124">值</span><span class="sxs-lookup"><span data-stu-id="6b950-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b950-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b950-125">Authorization</span></span>  | <span data-ttu-id="6b950-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b950-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b950-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b950-128">Request body</span></span>

<span data-ttu-id="6b950-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b950-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b950-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b950-130">Response</span></span>

<span data-ttu-id="6b950-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6b950-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b950-132">示例</span><span class="sxs-lookup"><span data-stu-id="6b950-132">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="6b950-133">示例 1：列出所有频道</span><span class="sxs-lookup"><span data-stu-id="6b950-133">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="6b950-134">请求</span><span class="sxs-lookup"><span data-stu-id="6b950-134">Request</span></span>

<span data-ttu-id="6b950-135">以下示例显示列出所有频道的请求。</span><span class="sxs-lookup"><span data-stu-id="6b950-135">The following example shows a request to list all channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="6b950-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b950-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[<span data-ttu-id="6b950-137">C#</span><span class="sxs-lookup"><span data-stu-id="6b950-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b950-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b950-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b950-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b950-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b950-140">Java</span><span class="sxs-lookup"><span data-stu-id="6b950-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6b950-141">响应</span><span class="sxs-lookup"><span data-stu-id="6b950-141">Response</span></span>

<span data-ttu-id="6b950-142">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="6b950-142">The following is the response.</span></span>

> <span data-ttu-id="6b950-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b950-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="6b950-144">示例 2：列出所有私人频道</span><span class="sxs-lookup"><span data-stu-id="6b950-144">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="6b950-145">请求</span><span class="sxs-lookup"><span data-stu-id="6b950-145">Request</span></span>

<span data-ttu-id="6b950-146">以下示例显示列出所有私人频道的请求。</span><span class="sxs-lookup"><span data-stu-id="6b950-146">The following example shows a request to list all private channels.</span></span>



# <a name="http"></a>[<span data-ttu-id="6b950-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b950-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="6b950-148">C#</span><span class="sxs-lookup"><span data-stu-id="6b950-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b950-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b950-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b950-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b950-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b950-151">Java</span><span class="sxs-lookup"><span data-stu-id="6b950-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6b950-152">响应</span><span class="sxs-lookup"><span data-stu-id="6b950-152">Response</span></span>

<span data-ttu-id="6b950-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b950-153">The following is an example of the response.</span></span>

> <span data-ttu-id="6b950-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b950-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "19:982abbfca323a582f0a6d00ae2deca@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "test private team",
      "membershipType": "private"
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
