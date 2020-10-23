---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f5190563b412fd5ae99c62a955981913acda1a0f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690250"
---
# <a name="list-owners"></a><span data-ttu-id="98b1c-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="98b1c-104">List owners</span></span>

<span data-ttu-id="98b1c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98b1c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98b1c-106">检索组的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="98b1c-106">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="98b1c-107">所有者是一组可修改组对象的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="98b1c-107">The owners are a set of users or service principals who are allowed to modify the group object.</span></span> <span data-ttu-id="98b1c-108">对于已在 Exchange 中创建的组，或者已从本地环境中同步的组，Microsoft Graph 目前未提供所有者角色。</span><span class="sxs-lookup"><span data-stu-id="98b1c-108">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span>

><span data-ttu-id="98b1c-109">**注意：** 当前，由于向 Microsoft Graph v1.0 终结点分阶段部署服务主体，服务主体未被列为组所有者。</span><span class="sxs-lookup"><span data-stu-id="98b1c-109">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="98b1c-110">权限</span><span class="sxs-lookup"><span data-stu-id="98b1c-110">Permissions</span></span>
<span data-ttu-id="98b1c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98b1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b1c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="98b1c-113">Permission type</span></span>      | <span data-ttu-id="98b1c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98b1c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98b1c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98b1c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="98b1c-116">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b1c-116">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="98b1c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98b1c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98b1c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="98b1c-118">Not supported.</span></span>    |
|<span data-ttu-id="98b1c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="98b1c-119">Application</span></span> | <span data-ttu-id="98b1c-120">Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b1c-120">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="98b1c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98b1c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98b1c-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98b1c-122">Optional query parameters</span></span>
<span data-ttu-id="98b1c-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98b1c-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98b1c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="98b1c-124">Request headers</span></span>
| <span data-ttu-id="98b1c-125">名称</span><span class="sxs-lookup"><span data-stu-id="98b1c-125">Name</span></span>       | <span data-ttu-id="98b1c-126">类型</span><span class="sxs-lookup"><span data-stu-id="98b1c-126">Type</span></span> | <span data-ttu-id="98b1c-127">说明</span><span class="sxs-lookup"><span data-stu-id="98b1c-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98b1c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="98b1c-128">Authorization</span></span>  | <span data-ttu-id="98b1c-129">string</span><span class="sxs-lookup"><span data-stu-id="98b1c-129">string</span></span>  | <span data-ttu-id="98b1c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98b1c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98b1c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="98b1c-132">Request body</span></span>
<span data-ttu-id="98b1c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98b1c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98b1c-134">响应</span><span class="sxs-lookup"><span data-stu-id="98b1c-134">Response</span></span>
<span data-ttu-id="98b1c-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="98b1c-135">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b1c-136">示例</span><span class="sxs-lookup"><span data-stu-id="98b1c-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="98b1c-137">请求</span><span class="sxs-lookup"><span data-stu-id="98b1c-137">Request</span></span>
<span data-ttu-id="98b1c-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98b1c-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98b1c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="98b1c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="98b1c-140">C#</span><span class="sxs-lookup"><span data-stu-id="98b1c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98b1c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98b1c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98b1c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98b1c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98b1c-143">Java</span><span class="sxs-lookup"><span data-stu-id="98b1c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="98b1c-144">响应</span><span class="sxs-lookup"><span data-stu-id="98b1c-144">Response</span></span>
<span data-ttu-id="98b1c-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98b1c-145">The following is an example of the response.</span></span>
><span data-ttu-id="98b1c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="98b1c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

