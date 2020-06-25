---
title: 获取 primaryChannel
description: 检索允许访问其默认常规通道的团队的导航属性。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0c4b209a4f510db2c5a4cd84bbc8bf7064a7935f
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863889"
---
# <a name="get-primarychannel"></a><span data-ttu-id="61760-103">获取 primaryChannel</span><span class="sxs-lookup"><span data-stu-id="61760-103">Get primaryChannel</span></span>

<span data-ttu-id="61760-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61760-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61760-105">获取[团队](../resources/team.md)的默认[频道](../resources/channel.md)（**常规**）。</span><span class="sxs-lookup"><span data-stu-id="61760-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61760-106">权限</span><span class="sxs-lookup"><span data-stu-id="61760-106">Permissions</span></span>
<span data-ttu-id="61760-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="61760-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="61760-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61760-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61760-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="61760-109">Permission type</span></span>      | <span data-ttu-id="61760-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61760-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61760-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61760-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61760-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61760-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="61760-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61760-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61760-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="61760-114">Not supported.</span></span>    |
|<span data-ttu-id="61760-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="61760-115">Application</span></span> | <span data-ttu-id="61760-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61760-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="61760-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="61760-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="61760-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="61760-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="61760-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61760-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61760-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61760-120">Optional query parameters</span></span>

<span data-ttu-id="61760-121">此方法支持 `$filter` 、 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61760-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61760-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="61760-122">Request headers</span></span>
| <span data-ttu-id="61760-123">标头</span><span class="sxs-lookup"><span data-stu-id="61760-123">Header</span></span>       | <span data-ttu-id="61760-124">值</span><span class="sxs-lookup"><span data-stu-id="61760-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61760-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="61760-125">Authorization</span></span>  | <span data-ttu-id="61760-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="61760-126">Bearer {token}.</span></span> <span data-ttu-id="61760-127">Required.</span><span class="sxs-lookup"><span data-stu-id="61760-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61760-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="61760-128">Request body</span></span>
<span data-ttu-id="61760-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61760-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61760-130">响应</span><span class="sxs-lookup"><span data-stu-id="61760-130">Response</span></span>

<span data-ttu-id="61760-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61760-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61760-132">示例</span><span class="sxs-lookup"><span data-stu-id="61760-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="61760-133">请求</span><span class="sxs-lookup"><span data-stu-id="61760-133">Request</span></span>
<span data-ttu-id="61760-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61760-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61760-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="61760-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="61760-136">C#</span><span class="sxs-lookup"><span data-stu-id="61760-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61760-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61760-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61760-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61760-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61760-139">Java</span><span class="sxs-lookup"><span data-stu-id="61760-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-primarychannel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="61760-140">响应</span><span class="sxs-lookup"><span data-stu-id="61760-140">Response</span></span>
<span data-ttu-id="61760-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61760-141">The following is an example of the response.</span></span> 

><span data-ttu-id="61760-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="61760-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="61760-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="61760-143">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47"
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
