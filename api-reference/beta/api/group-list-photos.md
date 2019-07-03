---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6c32cc184617fd20ad7440fcf273a4481f9070cf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440356"
---
# <a name="list-photos"></a><span data-ttu-id="956b9-103">List photos</span><span class="sxs-lookup"><span data-stu-id="956b9-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956b9-104">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="956b9-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="956b9-105">权限</span><span class="sxs-lookup"><span data-stu-id="956b9-105">Permissions</span></span>
<span data-ttu-id="956b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="956b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956b9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="956b9-108">Permission type</span></span>      | <span data-ttu-id="956b9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="956b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956b9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="956b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="956b9-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956b9-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="956b9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="956b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956b9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="956b9-113">Not supported.</span></span>    |
|<span data-ttu-id="956b9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="956b9-114">Application</span></span> | <span data-ttu-id="956b9-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956b9-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="956b9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="956b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="956b9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="956b9-117">Optional query parameters</span></span>
<span data-ttu-id="956b9-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="956b9-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="956b9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="956b9-119">Request headers</span></span>
| <span data-ttu-id="956b9-120">名称</span><span class="sxs-lookup"><span data-stu-id="956b9-120">Name</span></span>       | <span data-ttu-id="956b9-121">类型</span><span class="sxs-lookup"><span data-stu-id="956b9-121">Type</span></span> | <span data-ttu-id="956b9-122">说明</span><span class="sxs-lookup"><span data-stu-id="956b9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="956b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="956b9-123">Authorization</span></span>  | <span data-ttu-id="956b9-124">string</span><span class="sxs-lookup"><span data-stu-id="956b9-124">string</span></span>  | <span data-ttu-id="956b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="956b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="956b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="956b9-127">Request body</span></span>
<span data-ttu-id="956b9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="956b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="956b9-129">响应</span><span class="sxs-lookup"><span data-stu-id="956b9-129">Response</span></span>
<span data-ttu-id="956b9-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="956b9-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="956b9-131">示例</span><span class="sxs-lookup"><span data-stu-id="956b9-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="956b9-132">请求</span><span class="sxs-lookup"><span data-stu-id="956b9-132">Request</span></span>
<span data-ttu-id="956b9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="956b9-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="956b9-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="956b9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="956b9-135">C#</span><span class="sxs-lookup"><span data-stu-id="956b9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="956b9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="956b9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="956b9-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="956b9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="956b9-138">响应</span><span class="sxs-lookup"><span data-stu-id="956b9-138">Response</span></span>
<span data-ttu-id="956b9-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="956b9-139">The following is an example of the response.</span></span>
><span data-ttu-id="956b9-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="956b9-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="956b9-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="956b9-141">All the properties will be returned from an actual call.</span></span>
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
