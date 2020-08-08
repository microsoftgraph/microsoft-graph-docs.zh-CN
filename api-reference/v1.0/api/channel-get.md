---
title: 获取频道
description: 检索频道的属性和关系。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fbe5833d25f844b06f70fb4e2b242e6883724d20
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589289"
---
# <a name="get-channel"></a><span data-ttu-id="c86a9-103">获取频道</span><span class="sxs-lookup"><span data-stu-id="c86a9-103">Get channel</span></span>

<span data-ttu-id="c86a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c86a9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="c86a9-105">检索[频道](../resources/channel.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c86a9-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c86a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="c86a9-106">Permissions</span></span>
<span data-ttu-id="c86a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c86a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c86a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c86a9-109">Permission type</span></span>      | <span data-ttu-id="c86a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c86a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c86a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c86a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c86a9-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86a9-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c86a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c86a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c86a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c86a9-114">Not supported.</span></span>    |
|<span data-ttu-id="c86a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c86a9-115">Application</span></span> | <span data-ttu-id="c86a9-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86a9-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c86a9-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="c86a9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c86a9-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="c86a9-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c86a9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c86a9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c86a9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c86a9-120">Optional query parameters</span></span>

<span data-ttu-id="c86a9-121">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c86a9-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c86a9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c86a9-122">Request headers</span></span>
| <span data-ttu-id="c86a9-123">标头</span><span class="sxs-lookup"><span data-stu-id="c86a9-123">Header</span></span>       | <span data-ttu-id="c86a9-124">值</span><span class="sxs-lookup"><span data-stu-id="c86a9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c86a9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c86a9-125">Authorization</span></span>  | <span data-ttu-id="c86a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c86a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c86a9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c86a9-128">Request body</span></span>
<span data-ttu-id="c86a9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c86a9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c86a9-130">响应</span><span class="sxs-lookup"><span data-stu-id="c86a9-130">Response</span></span>

<span data-ttu-id="c86a9-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c86a9-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c86a9-132">示例</span><span class="sxs-lookup"><span data-stu-id="c86a9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c86a9-133">请求</span><span class="sxs-lookup"><span data-stu-id="c86a9-133">Request</span></span>
<span data-ttu-id="c86a9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c86a9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c86a9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c86a9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="c86a9-136">C#</span><span class="sxs-lookup"><span data-stu-id="c86a9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c86a9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c86a9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c86a9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c86a9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c86a9-139">Java</span><span class="sxs-lookup"><span data-stu-id="c86a9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c86a9-140">响应</span><span class="sxs-lookup"><span data-stu-id="c86a9-140">Response</span></span>
<span data-ttu-id="c86a9-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c86a9-141">Here is an example of the response.</span></span> 

><span data-ttu-id="c86a9-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c86a9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
