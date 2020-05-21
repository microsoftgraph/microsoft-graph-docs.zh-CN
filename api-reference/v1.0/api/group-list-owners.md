---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2294378620f6d02da7cb98be657fb587a8a7b46b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335409"
---
# <a name="list-owners"></a><span data-ttu-id="69a63-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="69a63-104">List owners</span></span>

<span data-ttu-id="69a63-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69a63-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69a63-p102">检索组所有者的列表。所有者是允许修改组对象的一组非管理员用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="69a63-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users or service principals who are allowed to modify the group object.</span></span> 

><span data-ttu-id="69a63-108">**注意：** 目前，由于将服务主体的暂存部署到 Microsoft Graph v1.0 终结点，服务主体不会作为组所有者列出。</span><span class="sxs-lookup"><span data-stu-id="69a63-108">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="69a63-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="69a63-109">Permissions</span></span>
<span data-ttu-id="69a63-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69a63-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69a63-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="69a63-112">Permission type</span></span>      | <span data-ttu-id="69a63-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69a63-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69a63-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69a63-114">Delegated (work or school account)</span></span> | <span data-ttu-id="69a63-115">Group. All 和 User.readbasic.all、Group. all、group. all、group. all、Group. all 和 Application。 read. all 和 Application。 Read. all： all. all. all</span><span class="sxs-lookup"><span data-stu-id="69a63-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="69a63-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69a63-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69a63-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69a63-117">Not supported.</span></span>    |
|<span data-ttu-id="69a63-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="69a63-118">Application</span></span> | <span data-ttu-id="69a63-119">Group. All 和 User. all、group. all 和 group. all、Group. all 和 Application。 Read. all 和 Application。 all</span><span class="sxs-lookup"><span data-stu-id="69a63-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="69a63-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69a63-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69a63-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69a63-121">Optional query parameters</span></span>
<span data-ttu-id="69a63-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69a63-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69a63-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="69a63-123">Request headers</span></span>
| <span data-ttu-id="69a63-124">名称</span><span class="sxs-lookup"><span data-stu-id="69a63-124">Name</span></span>       | <span data-ttu-id="69a63-125">类型</span><span class="sxs-lookup"><span data-stu-id="69a63-125">Type</span></span> | <span data-ttu-id="69a63-126">说明</span><span class="sxs-lookup"><span data-stu-id="69a63-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69a63-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="69a63-127">Authorization</span></span>  | <span data-ttu-id="69a63-128">string</span><span class="sxs-lookup"><span data-stu-id="69a63-128">string</span></span>  | <span data-ttu-id="69a63-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69a63-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69a63-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="69a63-131">Request body</span></span>
<span data-ttu-id="69a63-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69a63-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69a63-133">响应</span><span class="sxs-lookup"><span data-stu-id="69a63-133">Response</span></span>
<span data-ttu-id="69a63-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69a63-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69a63-135">示例</span><span class="sxs-lookup"><span data-stu-id="69a63-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69a63-136">请求</span><span class="sxs-lookup"><span data-stu-id="69a63-136">Request</span></span>
<span data-ttu-id="69a63-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69a63-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69a63-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="69a63-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="69a63-139">C#</span><span class="sxs-lookup"><span data-stu-id="69a63-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69a63-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69a63-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69a63-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69a63-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69a63-142">Java</span><span class="sxs-lookup"><span data-stu-id="69a63-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69a63-143">响应</span><span class="sxs-lookup"><span data-stu-id="69a63-143">Response</span></span>
<span data-ttu-id="69a63-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="69a63-144">The following is an example of the response.</span></span>
><span data-ttu-id="69a63-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69a63-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69a63-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69a63-146">All the properties will be returned from an actual call.</span></span>
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
