---
title: 获取 primaryChannel
description: 检索允许访问默认“常规”频道的团队的导航属性。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce7d7bd956eaa1f96cf456a767aeb2950102046f
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531416"
---
# <a name="get-primarychannel"></a><span data-ttu-id="8109c-103">获取 primaryChannel</span><span class="sxs-lookup"><span data-stu-id="8109c-103">Get primaryChannel</span></span>

<span data-ttu-id="8109c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8109c-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8109c-105">获取[团队](../resources/team.md)的默认[频道](../resources/channel.md)（**常规**）。</span><span class="sxs-lookup"><span data-stu-id="8109c-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8109c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8109c-106">Permissions</span></span>
<span data-ttu-id="8109c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8109c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8109c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8109c-109">Permission type</span></span>      | <span data-ttu-id="8109c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8109c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8109c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8109c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8109c-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8109c-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8109c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8109c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8109c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8109c-114">Not supported.</span></span>    |
|<span data-ttu-id="8109c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8109c-115">Application</span></span> | <span data-ttu-id="8109c-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8109c-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8109c-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="8109c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8109c-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="8109c-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8109c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8109c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8109c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8109c-120">Optional query parameters</span></span>

<span data-ttu-id="8109c-121">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8109c-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8109c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8109c-122">Request headers</span></span>
| <span data-ttu-id="8109c-123">标头</span><span class="sxs-lookup"><span data-stu-id="8109c-123">Header</span></span>       | <span data-ttu-id="8109c-124">值</span><span class="sxs-lookup"><span data-stu-id="8109c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8109c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8109c-125">Authorization</span></span>  | <span data-ttu-id="8109c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8109c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8109c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8109c-128">Request body</span></span>
<span data-ttu-id="8109c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8109c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8109c-130">响应</span><span class="sxs-lookup"><span data-stu-id="8109c-130">Response</span></span>

<span data-ttu-id="8109c-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8109c-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8109c-132">示例</span><span class="sxs-lookup"><span data-stu-id="8109c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="8109c-133">请求</span><span class="sxs-lookup"><span data-stu-id="8109c-133">Request</span></span>
<span data-ttu-id="8109c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8109c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8109c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8109c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="8109c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8109c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8109c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8109c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8109c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8109c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8109c-139">响应</span><span class="sxs-lookup"><span data-stu-id="8109c-139">Response</span></span>
<span data-ttu-id="8109c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8109c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="8109c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8109c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
