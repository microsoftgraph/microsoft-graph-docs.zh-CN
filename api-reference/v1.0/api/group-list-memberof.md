---
title: 列出 memberOf
description: '获取直接成员组构成的组集合。 '
author: dkershaw10
ms.openlocfilehash: 5cd563c8697a0d93ca2d11c42b3b8c19b0ce7ec9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323581"
---
# <a name="list-memberof"></a><span data-ttu-id="69942-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="69942-103">List memberOf</span></span>
<span data-ttu-id="69942-104">获取直接成员组构成的组集合。</span><span class="sxs-lookup"><span data-stu-id="69942-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="69942-p101">此操作不可传递。与获取用户的 Office 365 组不同，该操作将返回所有类型的组，而不仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="69942-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="69942-107">权限</span><span class="sxs-lookup"><span data-stu-id="69942-107">Permissions</span></span>
<span data-ttu-id="69942-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69942-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69942-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69942-110">Permission type</span></span>      | <span data-ttu-id="69942-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69942-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69942-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69942-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69942-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="69942-113">Group.Read.All</span></span>    |
|<span data-ttu-id="69942-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69942-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69942-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69942-115">Not supported.</span></span>    |
|<span data-ttu-id="69942-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69942-116">Application</span></span> | <span data-ttu-id="69942-117">Group.Read.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="69942-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69942-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69942-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69942-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69942-119">Optional query parameters</span></span>
<span data-ttu-id="69942-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69942-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69942-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="69942-121">Request headers</span></span>
| <span data-ttu-id="69942-122">Name</span><span class="sxs-lookup"><span data-stu-id="69942-122">Name</span></span>       | <span data-ttu-id="69942-123">类型</span><span class="sxs-lookup"><span data-stu-id="69942-123">Type</span></span> | <span data-ttu-id="69942-124">说明</span><span class="sxs-lookup"><span data-stu-id="69942-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69942-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="69942-125">Authorization</span></span>  | <span data-ttu-id="69942-126">string</span><span class="sxs-lookup"><span data-stu-id="69942-126">string</span></span>  | <span data-ttu-id="69942-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69942-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69942-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="69942-129">Request body</span></span>
<span data-ttu-id="69942-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69942-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69942-131">响应</span><span class="sxs-lookup"><span data-stu-id="69942-131">Response</span></span>
<span data-ttu-id="69942-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69942-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69942-133">示例</span><span class="sxs-lookup"><span data-stu-id="69942-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69942-134">请求</span><span class="sxs-lookup"><span data-stu-id="69942-134">Request</span></span>
<span data-ttu-id="69942-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69942-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="69942-136">响应</span><span class="sxs-lookup"><span data-stu-id="69942-136">Response</span></span>
<span data-ttu-id="69942-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69942-137">The following is an example of the response.</span></span>
><span data-ttu-id="69942-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69942-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69942-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69942-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->