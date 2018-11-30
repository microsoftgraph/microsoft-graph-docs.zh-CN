---
title: 列出 memberOf
description: '获取直接成员组构成的组集合。 '
ms.openlocfilehash: 9733fd1bc2def3642913887a228275744e17b61c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009224"
---
# <a name="list-memberof"></a><span data-ttu-id="7f7f9-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="7f7f9-103">List memberOf</span></span>
<span data-ttu-id="7f7f9-104">获取直接成员组构成的组集合。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="7f7f9-p101">此操作不可传递。与获取用户的 Office 365 组不同，该操作将返回所有类型的组，而不仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f7f9-107">权限</span><span class="sxs-lookup"><span data-stu-id="7f7f9-107">Permissions</span></span>
<span data-ttu-id="7f7f9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f7f9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f7f9-110">Permission type</span></span>      | <span data-ttu-id="7f7f9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f7f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f7f9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f7f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f7f9-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f7f9-113">Group.Read.All</span></span>    |
|<span data-ttu-id="7f7f9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f7f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f7f9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-115">Not supported.</span></span>    |
|<span data-ttu-id="7f7f9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f7f9-116">Application</span></span> | <span data-ttu-id="7f7f9-117">Group.Read.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f7f9-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f7f9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f7f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f7f9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f7f9-119">Optional query parameters</span></span>
<span data-ttu-id="7f7f9-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f7f9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f7f9-121">Request headers</span></span>
| <span data-ttu-id="7f7f9-122">名称</span><span class="sxs-lookup"><span data-stu-id="7f7f9-122">Name</span></span>       | <span data-ttu-id="7f7f9-123">类型</span><span class="sxs-lookup"><span data-stu-id="7f7f9-123">Type</span></span> | <span data-ttu-id="7f7f9-124">说明</span><span class="sxs-lookup"><span data-stu-id="7f7f9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f7f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f7f9-125">Authorization</span></span>  | <span data-ttu-id="7f7f9-126">string</span><span class="sxs-lookup"><span data-stu-id="7f7f9-126">string</span></span>  | <span data-ttu-id="7f7f9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f7f9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f7f9-129">Request body</span></span>
<span data-ttu-id="7f7f9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f7f9-131">响应</span><span class="sxs-lookup"><span data-stu-id="7f7f9-131">Response</span></span>
<span data-ttu-id="7f7f9-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f7f9-133">示例</span><span class="sxs-lookup"><span data-stu-id="7f7f9-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7f7f9-134">请求</span><span class="sxs-lookup"><span data-stu-id="7f7f9-134">Request</span></span>
<span data-ttu-id="7f7f9-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="7f7f9-136">响应</span><span class="sxs-lookup"><span data-stu-id="7f7f9-136">Response</span></span>
<span data-ttu-id="7f7f9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-137">The following is an example of the response.</span></span>
><span data-ttu-id="7f7f9-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f7f9-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f7f9-139">All the properties will be returned from an actual call.</span></span>
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