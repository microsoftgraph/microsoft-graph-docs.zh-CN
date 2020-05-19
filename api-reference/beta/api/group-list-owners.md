---
title: 列出所有者
description: 检索组的所有者列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6aada439df5839b0a6d4d91a2da962874beea5df
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287026"
---
# <a name="list-owners"></a><span data-ttu-id="d14a8-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="d14a8-103">List owners</span></span>

<span data-ttu-id="d14a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d14a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d14a8-p101">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="d14a8-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d14a8-107">权限</span><span class="sxs-lookup"><span data-stu-id="d14a8-107">Permissions</span></span>
<span data-ttu-id="d14a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d14a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d14a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d14a8-110">Permission type</span></span>      | <span data-ttu-id="d14a8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d14a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d14a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d14a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d14a8-113">Group. All 和 User.readbasic.all、Group. all、group. all、group. all、Group. all 和 Application。 read. all 和 Application。 Read. all： all. all. all</span><span class="sxs-lookup"><span data-stu-id="d14a8-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>  |
|<span data-ttu-id="d14a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d14a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d14a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d14a8-115">Not supported.</span></span>    |
|<span data-ttu-id="d14a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d14a8-116">Application</span></span> | <span data-ttu-id="d14a8-117">Group. All 和 User. all、group. all 和 group. all、Group. all 和 Application。 Read. all 和 Application。 all</span><span class="sxs-lookup"><span data-stu-id="d14a8-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d14a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d14a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d14a8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d14a8-119">Optional query parameters</span></span>
<span data-ttu-id="d14a8-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d14a8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d14a8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d14a8-121">Request headers</span></span>
| <span data-ttu-id="d14a8-122">名称</span><span class="sxs-lookup"><span data-stu-id="d14a8-122">Name</span></span>       | <span data-ttu-id="d14a8-123">类型</span><span class="sxs-lookup"><span data-stu-id="d14a8-123">Type</span></span> | <span data-ttu-id="d14a8-124">说明</span><span class="sxs-lookup"><span data-stu-id="d14a8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d14a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d14a8-125">Authorization</span></span>  | <span data-ttu-id="d14a8-126">string</span><span class="sxs-lookup"><span data-stu-id="d14a8-126">string</span></span>  | <span data-ttu-id="d14a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d14a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d14a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d14a8-129">Request body</span></span>
<span data-ttu-id="d14a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d14a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d14a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="d14a8-131">Response</span></span>
<span data-ttu-id="d14a8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d14a8-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d14a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="d14a8-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d14a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="d14a8-134">Request</span></span>
<span data-ttu-id="d14a8-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d14a8-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d14a8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d14a8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="d14a8-137">C#</span><span class="sxs-lookup"><span data-stu-id="d14a8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d14a8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d14a8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d14a8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d14a8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d14a8-140">响应</span><span class="sxs-lookup"><span data-stu-id="d14a8-140">Response</span></span>
<span data-ttu-id="d14a8-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d14a8-141">The following is an example of the response.</span></span>
><span data-ttu-id="d14a8-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d14a8-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d14a8-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d14a8-143">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
