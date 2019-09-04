---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、联系人和其他组作为成员。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9de4f41bfee17a560da5d971ce6ad2e6562b2bf8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726758"
---
# <a name="list-members"></a><span data-ttu-id="524c0-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="524c0-104">List members</span></span>
<span data-ttu-id="524c0-p102">获取组的直接成员列表。组可将用户、联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="524c0-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="524c0-108">权限</span><span class="sxs-lookup"><span data-stu-id="524c0-108">Permissions</span></span>
<span data-ttu-id="524c0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="524c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="524c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="524c0-111">Permission type</span></span>      | <span data-ttu-id="524c0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="524c0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="524c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="524c0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="524c0-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="524c0-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="524c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="524c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="524c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="524c0-116">Not supported.</span></span>    |
|<span data-ttu-id="524c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="524c0-117">Application</span></span> | <span data-ttu-id="524c0-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="524c0-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="524c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="524c0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="524c0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="524c0-120">Optional query parameters</span></span>
<span data-ttu-id="524c0-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="524c0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="524c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="524c0-122">Request headers</span></span>
| <span data-ttu-id="524c0-123">名称</span><span class="sxs-lookup"><span data-stu-id="524c0-123">Name</span></span>       | <span data-ttu-id="524c0-124">类型</span><span class="sxs-lookup"><span data-stu-id="524c0-124">Type</span></span> | <span data-ttu-id="524c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="524c0-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="524c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="524c0-126">Authorization</span></span>  | <span data-ttu-id="524c0-127">string</span><span class="sxs-lookup"><span data-stu-id="524c0-127">string</span></span>  | <span data-ttu-id="524c0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="524c0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="524c0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="524c0-130">Request body</span></span>
<span data-ttu-id="524c0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="524c0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="524c0-132">响应</span><span class="sxs-lookup"><span data-stu-id="524c0-132">Response</span></span>
<span data-ttu-id="524c0-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="524c0-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="524c0-134">示例</span><span class="sxs-lookup"><span data-stu-id="524c0-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="524c0-135">请求</span><span class="sxs-lookup"><span data-stu-id="524c0-135">Request</span></span>
<span data-ttu-id="524c0-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="524c0-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="524c0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="524c0-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="524c0-138">C#</span><span class="sxs-lookup"><span data-stu-id="524c0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="524c0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="524c0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="524c0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="524c0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="524c0-141">Java</span><span class="sxs-lookup"><span data-stu-id="524c0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="524c0-142">响应</span><span class="sxs-lookup"><span data-stu-id="524c0-142">Response</span></span>
<span data-ttu-id="524c0-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="524c0-143">The following is an example of the response.</span></span>
><span data-ttu-id="524c0-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="524c0-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="524c0-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="524c0-145">All the properties will be returned from an actual call.</span></span>
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
