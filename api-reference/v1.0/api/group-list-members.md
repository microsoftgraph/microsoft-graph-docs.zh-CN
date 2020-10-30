---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、组织联系人、设备、服务主体和其他组作为成员。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fce71e0caa13e5b1ba7ac4bf5aab41ecd2e96357
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782551"
---
# <a name="list-members"></a><span data-ttu-id="09aab-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="09aab-104">List members</span></span>

<span data-ttu-id="09aab-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09aab-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09aab-106">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="09aab-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="09aab-107">组可将用户、组织联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="09aab-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="09aab-108">当前，由于在 Graph V1.0 终结点上分阶段部署服务主体，因此未将服务主体列为组成员。</span><span class="sxs-lookup"><span data-stu-id="09aab-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="09aab-109">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="09aab-109">This operation is not transitive.</span></span>

<span data-ttu-id="09aab-110">当组包含超过 100 个成员时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，其中包含指向下一页结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="09aab-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="09aab-111">如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。</span><span class="sxs-lookup"><span data-stu-id="09aab-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="09aab-112">权限</span><span class="sxs-lookup"><span data-stu-id="09aab-112">Permissions</span></span>
<span data-ttu-id="09aab-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09aab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09aab-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="09aab-115">Permission type</span></span>      | <span data-ttu-id="09aab-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09aab-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09aab-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09aab-117">Delegated (work or school account)</span></span> | <span data-ttu-id="09aab-118">User.ReadBasic.All、User.Read.All、GroupMember.Read.All、Group.Read.All、 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="09aab-118">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="09aab-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09aab-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09aab-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="09aab-120">Not supported.</span></span>    |
|<span data-ttu-id="09aab-121">Application</span><span class="sxs-lookup"><span data-stu-id="09aab-121">Application</span></span> | <span data-ttu-id="09aab-122">User.Read.All、GroupMember.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="09aab-122">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="09aab-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09aab-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09aab-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09aab-124">Optional query parameters</span></span>
<span data-ttu-id="09aab-125">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09aab-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09aab-126">请求头</span><span class="sxs-lookup"><span data-stu-id="09aab-126">Request headers</span></span>
| <span data-ttu-id="09aab-127">标头</span><span class="sxs-lookup"><span data-stu-id="09aab-127">Header</span></span>       | <span data-ttu-id="09aab-128">值</span><span class="sxs-lookup"><span data-stu-id="09aab-128">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="09aab-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="09aab-129">Authorization</span></span>  | <span data-ttu-id="09aab-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09aab-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09aab-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="09aab-132">Request body</span></span>
<span data-ttu-id="09aab-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09aab-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09aab-134">响应</span><span class="sxs-lookup"><span data-stu-id="09aab-134">Response</span></span>
<span data-ttu-id="09aab-135">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="09aab-135">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09aab-136">示例</span><span class="sxs-lookup"><span data-stu-id="09aab-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="09aab-137">请求</span><span class="sxs-lookup"><span data-stu-id="09aab-137">Request</span></span>
<span data-ttu-id="09aab-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09aab-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09aab-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="09aab-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="09aab-140">C#</span><span class="sxs-lookup"><span data-stu-id="09aab-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09aab-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09aab-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09aab-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09aab-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09aab-143">Java</span><span class="sxs-lookup"><span data-stu-id="09aab-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09aab-144">响应</span><span class="sxs-lookup"><span data-stu-id="09aab-144">Response</span></span>
<span data-ttu-id="09aab-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09aab-145">The following is an example of the response.</span></span>
><span data-ttu-id="09aab-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09aab-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

