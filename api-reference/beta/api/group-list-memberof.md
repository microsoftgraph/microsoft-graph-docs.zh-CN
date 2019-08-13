---
title: 列出组 memberOf
description: 获取组是其直接成员的组和管理单元。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4847b94b6aa025b03987bd0bec7e63d1b6125a4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323442"
---
# <a name="list-group-memberof"></a><span data-ttu-id="94113-103">列出组 memberOf</span><span class="sxs-lookup"><span data-stu-id="94113-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94113-104">获取组是其直接成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="94113-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="94113-p101">此操作不可传递。与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="94113-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="94113-107">权限</span><span class="sxs-lookup"><span data-stu-id="94113-107">Permissions</span></span>

<span data-ttu-id="94113-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94113-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94113-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94113-110">Permission type</span></span>      | <span data-ttu-id="94113-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94113-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94113-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94113-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94113-113">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94113-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94113-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94113-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94113-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94113-115">Not supported.</span></span>    |
|<span data-ttu-id="94113-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94113-116">Application</span></span> | <span data-ttu-id="94113-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94113-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94113-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94113-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94113-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94113-119">Optional query parameters</span></span>
<span data-ttu-id="94113-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="94113-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94113-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="94113-121">Request headers</span></span>
| <span data-ttu-id="94113-122">名称</span><span class="sxs-lookup"><span data-stu-id="94113-122">Name</span></span>       | <span data-ttu-id="94113-123">类型</span><span class="sxs-lookup"><span data-stu-id="94113-123">Type</span></span> | <span data-ttu-id="94113-124">说明</span><span class="sxs-lookup"><span data-stu-id="94113-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94113-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="94113-125">Authorization</span></span>  | <span data-ttu-id="94113-126">string</span><span class="sxs-lookup"><span data-stu-id="94113-126">string</span></span>  | <span data-ttu-id="94113-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94113-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94113-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="94113-129">Request body</span></span>
<span data-ttu-id="94113-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94113-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94113-131">响应</span><span class="sxs-lookup"><span data-stu-id="94113-131">Response</span></span>
<span data-ttu-id="94113-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="94113-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94113-133">示例</span><span class="sxs-lookup"><span data-stu-id="94113-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="94113-134">请求</span><span class="sxs-lookup"><span data-stu-id="94113-134">Request</span></span>

<span data-ttu-id="94113-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94113-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94113-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="94113-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94113-137">C#</span><span class="sxs-lookup"><span data-stu-id="94113-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94113-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94113-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94113-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="94113-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94113-140">Java</span><span class="sxs-lookup"><span data-stu-id="94113-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94113-141">响应</span><span class="sxs-lookup"><span data-stu-id="94113-141">Response</span></span>

<span data-ttu-id="94113-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94113-142">The following is an example of the response.</span></span>
><span data-ttu-id="94113-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94113-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94113-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94113-144">All the properties will be returned from an actual call.</span></span>
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
