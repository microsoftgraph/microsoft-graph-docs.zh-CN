---
title: List photos
description: 检索 profilePhoto 对象列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c0bd09498d679cf1b2f042f7af6e3385cdd2cc6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410026"
---
# <a name="list-photos"></a><span data-ttu-id="30e7e-103">List photos</span><span class="sxs-lookup"><span data-stu-id="30e7e-103">List photos</span></span>

<span data-ttu-id="30e7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30e7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30e7e-105">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="30e7e-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="30e7e-106">权限</span><span class="sxs-lookup"><span data-stu-id="30e7e-106">Permissions</span></span>
<span data-ttu-id="30e7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="30e7e-109">Permission type</span></span>      | <span data-ttu-id="30e7e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30e7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30e7e-112">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e7e-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="30e7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="30e7e-114">Not supported.</span></span>    |
|<span data-ttu-id="30e7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="30e7e-115">Application</span></span> | <span data-ttu-id="30e7e-116">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e7e-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30e7e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30e7e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30e7e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="30e7e-118">Optional query parameters</span></span>
<span data-ttu-id="30e7e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="30e7e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30e7e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="30e7e-120">Request headers</span></span>
| <span data-ttu-id="30e7e-121">名称</span><span class="sxs-lookup"><span data-stu-id="30e7e-121">Name</span></span>       | <span data-ttu-id="30e7e-122">类型</span><span class="sxs-lookup"><span data-stu-id="30e7e-122">Type</span></span> | <span data-ttu-id="30e7e-123">说明</span><span class="sxs-lookup"><span data-stu-id="30e7e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30e7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="30e7e-124">Authorization</span></span>  | <span data-ttu-id="30e7e-125">string</span><span class="sxs-lookup"><span data-stu-id="30e7e-125">string</span></span>  | <span data-ttu-id="30e7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30e7e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30e7e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="30e7e-128">Request body</span></span>
<span data-ttu-id="30e7e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30e7e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30e7e-130">响应</span><span class="sxs-lookup"><span data-stu-id="30e7e-130">Response</span></span>
<span data-ttu-id="30e7e-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30e7e-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e7e-132">示例</span><span class="sxs-lookup"><span data-stu-id="30e7e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="30e7e-133">请求</span><span class="sxs-lookup"><span data-stu-id="30e7e-133">Request</span></span>
<span data-ttu-id="30e7e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30e7e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30e7e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="30e7e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="30e7e-136">C#</span><span class="sxs-lookup"><span data-stu-id="30e7e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30e7e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30e7e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30e7e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30e7e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="30e7e-139">响应</span><span class="sxs-lookup"><span data-stu-id="30e7e-139">Response</span></span>
<span data-ttu-id="30e7e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="30e7e-140">The following is an example of the response.</span></span>
><span data-ttu-id="30e7e-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30e7e-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="30e7e-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="30e7e-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
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
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
