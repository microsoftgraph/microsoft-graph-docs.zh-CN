---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 57ca7bd1e84f507dbf59f515f6f7b2ec1ef020ed
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125216"
---
# <a name="list-owners"></a><span data-ttu-id="2cd68-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="2cd68-104">List owners</span></span>

<span data-ttu-id="2cd68-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cd68-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cd68-p102">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="2cd68-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2cd68-108">权限</span><span class="sxs-lookup"><span data-stu-id="2cd68-108">Permissions</span></span>
<span data-ttu-id="2cd68-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cd68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cd68-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cd68-111">Permission type</span></span>      | <span data-ttu-id="2cd68-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cd68-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cd68-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cd68-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2cd68-114">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cd68-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="2cd68-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cd68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cd68-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cd68-116">Not supported.</span></span>    |
|<span data-ttu-id="2cd68-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cd68-117">Application</span></span> | <span data-ttu-id="2cd68-118">Group.Read.All 和 User.Read.All、Group.Read.All 和User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cd68-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2cd68-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cd68-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2cd68-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2cd68-120">Optional query parameters</span></span>
<span data-ttu-id="2cd68-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2cd68-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cd68-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cd68-122">Request headers</span></span>
| <span data-ttu-id="2cd68-123">名称</span><span class="sxs-lookup"><span data-stu-id="2cd68-123">Name</span></span>       | <span data-ttu-id="2cd68-124">类型</span><span class="sxs-lookup"><span data-stu-id="2cd68-124">Type</span></span> | <span data-ttu-id="2cd68-125">说明</span><span class="sxs-lookup"><span data-stu-id="2cd68-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2cd68-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cd68-126">Authorization</span></span>  | <span data-ttu-id="2cd68-127">string</span><span class="sxs-lookup"><span data-stu-id="2cd68-127">string</span></span>  | <span data-ttu-id="2cd68-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cd68-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cd68-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cd68-130">Request body</span></span>
<span data-ttu-id="2cd68-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cd68-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cd68-132">响应</span><span class="sxs-lookup"><span data-stu-id="2cd68-132">Response</span></span>
<span data-ttu-id="2cd68-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2cd68-133">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cd68-134">示例</span><span class="sxs-lookup"><span data-stu-id="2cd68-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2cd68-135">请求</span><span class="sxs-lookup"><span data-stu-id="2cd68-135">Request</span></span>
<span data-ttu-id="2cd68-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cd68-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cd68-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cd68-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="2cd68-138">C#</span><span class="sxs-lookup"><span data-stu-id="2cd68-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cd68-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cd68-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cd68-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cd68-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cd68-141">Java</span><span class="sxs-lookup"><span data-stu-id="2cd68-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2cd68-142">响应</span><span class="sxs-lookup"><span data-stu-id="2cd68-142">Response</span></span>
<span data-ttu-id="2cd68-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2cd68-143">The following is an example of the response.</span></span>
><span data-ttu-id="2cd68-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2cd68-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2cd68-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cd68-145">All the properties will be returned from an actual call.</span></span>
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
