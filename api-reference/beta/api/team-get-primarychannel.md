---
title: 获取 primaryChannel
description: 检索允许访问其默认常规通道的团队的导航属性。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0993eb206abb4ddaea321567f4bc21a9ec22fbbe
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863447"
---
# <a name="get-primarychannel"></a><span data-ttu-id="a6c70-103">获取 primaryChannel</span><span class="sxs-lookup"><span data-stu-id="a6c70-103">Get primaryChannel</span></span>

<span data-ttu-id="a6c70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c70-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c70-105">获取[团队](../resources/team.md)的默认[频道](../resources/channel.md)（**常规**）。</span><span class="sxs-lookup"><span data-stu-id="a6c70-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c70-106">权限</span><span class="sxs-lookup"><span data-stu-id="a6c70-106">Permissions</span></span>
<span data-ttu-id="a6c70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6c70-109">Permission type</span></span>      | <span data-ttu-id="a6c70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6c70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c70-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c70-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6c70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6c70-114">Not supported.</span></span>    |
|<span data-ttu-id="a6c70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6c70-115">Application</span></span> | <span data-ttu-id="a6c70-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c70-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a6c70-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a6c70-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a6c70-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="a6c70-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a6c70-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6c70-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6c70-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6c70-120">Optional query parameters</span></span>

<span data-ttu-id="a6c70-121">此方法支持 `$filter` 、 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a6c70-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6c70-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6c70-122">Request headers</span></span>
| <span data-ttu-id="a6c70-123">标头</span><span class="sxs-lookup"><span data-stu-id="a6c70-123">Header</span></span>       | <span data-ttu-id="a6c70-124">值</span><span class="sxs-lookup"><span data-stu-id="a6c70-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6c70-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c70-125">Authorization</span></span>  | <span data-ttu-id="a6c70-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6c70-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6c70-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6c70-128">Request body</span></span>
<span data-ttu-id="a6c70-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6c70-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c70-130">响应</span><span class="sxs-lookup"><span data-stu-id="a6c70-130">Response</span></span>

<span data-ttu-id="a6c70-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6c70-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c70-132">示例</span><span class="sxs-lookup"><span data-stu-id="a6c70-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6c70-133">请求</span><span class="sxs-lookup"><span data-stu-id="a6c70-133">Request</span></span>
<span data-ttu-id="a6c70-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6c70-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6c70-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c70-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="a6c70-136">C#</span><span class="sxs-lookup"><span data-stu-id="a6c70-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6c70-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6c70-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6c70-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6c70-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a6c70-139">响应</span><span class="sxs-lookup"><span data-stu-id="a6c70-139">Response</span></span>
<span data-ttu-id="a6c70-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6c70-140">The following is an example of the response.</span></span> 

><span data-ttu-id="a6c70-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6c70-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
