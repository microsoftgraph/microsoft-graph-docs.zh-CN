---
title: 获取 primaryChannel
description: 检索允许访问其默认常规通道的团队的导航属性。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c9be54f744e596b41de1d2e994dfe51b0c95e6d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791095"
---
# <a name="get-primarychannel"></a><span data-ttu-id="41b44-103">获取 primaryChannel</span><span class="sxs-lookup"><span data-stu-id="41b44-103">Get primaryChannel</span></span>

<span data-ttu-id="41b44-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41b44-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41b44-105">检索允许访问默认常规[通道](../resources/channel.md)的[团队](../resources/team.md)的导航属性。</span><span class="sxs-lookup"><span data-stu-id="41b44-105">Retrieve the navigation property of a [team](../resources/team.md) that allows access to the default General [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41b44-106">权限</span><span class="sxs-lookup"><span data-stu-id="41b44-106">Permissions</span></span>
<span data-ttu-id="41b44-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="41b44-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="41b44-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b44-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="41b44-109">Permission type</span></span>      | <span data-ttu-id="41b44-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41b44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41b44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41b44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41b44-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b44-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="41b44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41b44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41b44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="41b44-114">Not supported.</span></span>    |
|<span data-ttu-id="41b44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="41b44-115">Application</span></span> | <span data-ttu-id="41b44-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b44-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="41b44-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="41b44-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="41b44-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="41b44-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="41b44-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41b44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel

```

## <a name="optional-query-parameters"></a><span data-ttu-id="41b44-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41b44-120">Optional query parameters</span></span>

<span data-ttu-id="41b44-121">此方法支持 `$filter` 、 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41b44-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41b44-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="41b44-122">Request headers</span></span>
| <span data-ttu-id="41b44-123">标头</span><span class="sxs-lookup"><span data-stu-id="41b44-123">Header</span></span>       | <span data-ttu-id="41b44-124">值</span><span class="sxs-lookup"><span data-stu-id="41b44-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41b44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41b44-125">Authorization</span></span>  | <span data-ttu-id="41b44-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="41b44-126">Bearer {token}.</span></span> <span data-ttu-id="41b44-127">Required.</span><span class="sxs-lookup"><span data-stu-id="41b44-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41b44-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="41b44-128">Request body</span></span>
<span data-ttu-id="41b44-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41b44-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41b44-130">响应</span><span class="sxs-lookup"><span data-stu-id="41b44-130">Response</span></span>

<span data-ttu-id="41b44-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41b44-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41b44-132">示例</span><span class="sxs-lookup"><span data-stu-id="41b44-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="41b44-133">请求</span><span class="sxs-lookup"><span data-stu-id="41b44-133">Request</span></span>
<span data-ttu-id="41b44-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="41b44-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
### <a name="response"></a><span data-ttu-id="41b44-135">响应</span><span class="sxs-lookup"><span data-stu-id="41b44-135">Response</span></span>
<span data-ttu-id="41b44-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="41b44-136">The following is an example of the response.</span></span> 

><span data-ttu-id="41b44-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="41b44-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41b44-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="41b44-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "isFavoriteByDefault": null,
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47",
    "membershipType": "standard"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get primaryChannel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
