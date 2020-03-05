---
title: 列出组 memberOf
description: 获取组是其直接成员的组和管理单元。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b4edb12a1b620c77f844d1e2a5d5f5a7751a249
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419434"
---
# <a name="list-group-memberof"></a><span data-ttu-id="2c046-103">列出组 memberOf</span><span class="sxs-lookup"><span data-stu-id="2c046-103">List group memberOf</span></span>

<span data-ttu-id="2c046-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2c046-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c046-105">获取组是其直接成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="2c046-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="2c046-106">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="2c046-106">This operation is not transitive.</span></span> <span data-ttu-id="2c046-107">与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="2c046-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2c046-108">权限</span><span class="sxs-lookup"><span data-stu-id="2c046-108">Permissions</span></span>

<span data-ttu-id="2c046-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c046-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c046-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c046-111">Permission type</span></span>      | <span data-ttu-id="2c046-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c046-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c046-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c046-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c046-114">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c046-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c046-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c046-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c046-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c046-116">Not supported.</span></span>    |
|<span data-ttu-id="2c046-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c046-117">Application</span></span> | <span data-ttu-id="2c046-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c046-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2c046-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c046-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c046-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c046-120">Optional query parameters</span></span>
<span data-ttu-id="2c046-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c046-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c046-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c046-122">Request headers</span></span>
| <span data-ttu-id="2c046-123">名称</span><span class="sxs-lookup"><span data-stu-id="2c046-123">Name</span></span>       | <span data-ttu-id="2c046-124">类型</span><span class="sxs-lookup"><span data-stu-id="2c046-124">Type</span></span> | <span data-ttu-id="2c046-125">说明</span><span class="sxs-lookup"><span data-stu-id="2c046-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c046-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c046-126">Authorization</span></span>  | <span data-ttu-id="2c046-127">string</span><span class="sxs-lookup"><span data-stu-id="2c046-127">string</span></span>  | <span data-ttu-id="2c046-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c046-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c046-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c046-130">Request body</span></span>
<span data-ttu-id="2c046-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c046-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c046-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c046-132">Response</span></span>
<span data-ttu-id="2c046-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c046-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c046-134">示例</span><span class="sxs-lookup"><span data-stu-id="2c046-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c046-135">请求</span><span class="sxs-lookup"><span data-stu-id="2c046-135">Request</span></span>

<span data-ttu-id="2c046-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c046-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c046-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c046-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="2c046-138">C#</span><span class="sxs-lookup"><span data-stu-id="2c046-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c046-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c046-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c046-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c046-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c046-141">响应</span><span class="sxs-lookup"><span data-stu-id="2c046-141">Response</span></span>

<span data-ttu-id="2c046-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2c046-142">The following is an example of the response.</span></span>
><span data-ttu-id="2c046-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c046-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2c046-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2c046-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
