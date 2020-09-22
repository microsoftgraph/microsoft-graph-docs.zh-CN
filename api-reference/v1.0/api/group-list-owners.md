---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 767d1d399f7be629d3d4e71fd9412cab863e8c9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063658"
---
# <a name="list-owners"></a><span data-ttu-id="39f17-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="39f17-104">List owners</span></span>

<span data-ttu-id="39f17-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39f17-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39f17-p102">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="39f17-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users or service principals who are allowed to modify the group object.</span></span> 

><span data-ttu-id="39f17-108">**注意：** 当前，由于向 Microsoft Graph v1.0 终结点分阶段部署服务主体，服务主体未被列为组所有者。</span><span class="sxs-lookup"><span data-stu-id="39f17-108">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="39f17-109">权限</span><span class="sxs-lookup"><span data-stu-id="39f17-109">Permissions</span></span>
<span data-ttu-id="39f17-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39f17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f17-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="39f17-112">Permission type</span></span>      | <span data-ttu-id="39f17-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39f17-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39f17-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39f17-114">Delegated (work or school account)</span></span> | <span data-ttu-id="39f17-115">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="39f17-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="39f17-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39f17-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39f17-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="39f17-117">Not supported.</span></span>    |
|<span data-ttu-id="39f17-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="39f17-118">Application</span></span> | <span data-ttu-id="39f17-119">Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All、Group.Read.All 和 User.Read.All 以及 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="39f17-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="39f17-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39f17-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39f17-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39f17-121">Optional query parameters</span></span>
<span data-ttu-id="39f17-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39f17-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39f17-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="39f17-123">Request headers</span></span>
| <span data-ttu-id="39f17-124">名称</span><span class="sxs-lookup"><span data-stu-id="39f17-124">Name</span></span>       | <span data-ttu-id="39f17-125">类型</span><span class="sxs-lookup"><span data-stu-id="39f17-125">Type</span></span> | <span data-ttu-id="39f17-126">说明</span><span class="sxs-lookup"><span data-stu-id="39f17-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39f17-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f17-127">Authorization</span></span>  | <span data-ttu-id="39f17-128">string</span><span class="sxs-lookup"><span data-stu-id="39f17-128">string</span></span>  | <span data-ttu-id="39f17-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39f17-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39f17-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="39f17-131">Request body</span></span>
<span data-ttu-id="39f17-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39f17-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39f17-133">响应</span><span class="sxs-lookup"><span data-stu-id="39f17-133">Response</span></span>
<span data-ttu-id="39f17-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39f17-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f17-135">示例</span><span class="sxs-lookup"><span data-stu-id="39f17-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="39f17-136">请求</span><span class="sxs-lookup"><span data-stu-id="39f17-136">Request</span></span>
<span data-ttu-id="39f17-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39f17-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39f17-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="39f17-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="39f17-139">C#</span><span class="sxs-lookup"><span data-stu-id="39f17-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39f17-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39f17-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39f17-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39f17-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39f17-142">Java</span><span class="sxs-lookup"><span data-stu-id="39f17-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39f17-143">响应</span><span class="sxs-lookup"><span data-stu-id="39f17-143">Response</span></span>
<span data-ttu-id="39f17-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39f17-144">The following is an example of the response.</span></span>
><span data-ttu-id="39f17-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="39f17-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="39f17-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="39f17-146">All the properties will be returned from an actual call.</span></span>
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

