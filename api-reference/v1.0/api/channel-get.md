---
title: 获取频道
description: 检索频道的属性和关系。
author: nkramer
doc_type: apiPageType
ms.prod: microsoft-teams
localization_priority: Normal
ms.openlocfilehash: a7be2c2b5fe3db44e8c514f39731a56d859e1ce2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202896"
---
# <a name="get-channel"></a><span data-ttu-id="2bfc4-103">获取频道</span><span class="sxs-lookup"><span data-stu-id="2bfc4-103">Get channel</span></span>

<span data-ttu-id="2bfc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bfc4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bfc4-105">检索[频道](../resources/channel.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bfc4-106">权限</span><span class="sxs-lookup"><span data-stu-id="2bfc4-106">Permissions</span></span>

<span data-ttu-id="2bfc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bfc4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bfc4-109">Permission type</span></span>      | <span data-ttu-id="2bfc4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bfc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bfc4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bfc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2bfc4-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bfc4-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2bfc4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bfc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bfc4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-114">Not supported.</span></span>    |
|<span data-ttu-id="2bfc4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bfc4-115">Application</span></span> | <span data-ttu-id="2bfc4-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bfc4-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="2bfc4-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="2bfc4-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2bfc4-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2bfc4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bfc4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2bfc4-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2bfc4-121">Optional query parameters</span></span>

<span data-ttu-id="2bfc4-122">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bfc4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bfc4-123">Request headers</span></span>

| <span data-ttu-id="2bfc4-124">标头</span><span class="sxs-lookup"><span data-stu-id="2bfc4-124">Header</span></span>       | <span data-ttu-id="2bfc4-125">值</span><span class="sxs-lookup"><span data-stu-id="2bfc4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2bfc4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bfc4-126">Authorization</span></span>  | <span data-ttu-id="2bfc4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bfc4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bfc4-129">Request body</span></span>

<span data-ttu-id="2bfc4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bfc4-131">响应</span><span class="sxs-lookup"><span data-stu-id="2bfc4-131">Response</span></span>

<span data-ttu-id="2bfc4-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bfc4-133">示例</span><span class="sxs-lookup"><span data-stu-id="2bfc4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bfc4-134">请求</span><span class="sxs-lookup"><span data-stu-id="2bfc4-134">Request</span></span>

<span data-ttu-id="2bfc4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-135">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```


### <a name="response"></a><span data-ttu-id="2bfc4-136">响应</span><span class="sxs-lookup"><span data-stu-id="2bfc4-136">Response</span></span>

<span data-ttu-id="2bfc4-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-137">Here is an example of the response.</span></span>

><span data-ttu-id="2bfc4-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2bfc4-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
