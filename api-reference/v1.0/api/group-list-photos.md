---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 62c713c8e7269345aa7b1462e58c71d118a71e3b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889042"
---
# <a name="list-photos"></a><span data-ttu-id="234da-103">List photos</span><span class="sxs-lookup"><span data-stu-id="234da-103">List photos</span></span>
<span data-ttu-id="234da-104">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="234da-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="234da-105">权限</span><span class="sxs-lookup"><span data-stu-id="234da-105">Permissions</span></span>
<span data-ttu-id="234da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="234da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="234da-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="234da-108">Permission type</span></span>      | <span data-ttu-id="234da-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="234da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="234da-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="234da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="234da-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="234da-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="234da-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="234da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="234da-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="234da-113">Not supported.</span></span>    |
|<span data-ttu-id="234da-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="234da-114">Application</span></span> | <span data-ttu-id="234da-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="234da-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="234da-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="234da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="234da-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="234da-117">Optional query parameters</span></span>
<span data-ttu-id="234da-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="234da-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="234da-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="234da-119">Request headers</span></span>
| <span data-ttu-id="234da-120">名称</span><span class="sxs-lookup"><span data-stu-id="234da-120">Name</span></span>       | <span data-ttu-id="234da-121">类型</span><span class="sxs-lookup"><span data-stu-id="234da-121">Type</span></span> | <span data-ttu-id="234da-122">说明</span><span class="sxs-lookup"><span data-stu-id="234da-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="234da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="234da-123">Authorization</span></span>  | <span data-ttu-id="234da-124">string</span><span class="sxs-lookup"><span data-stu-id="234da-124">string</span></span>  | <span data-ttu-id="234da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="234da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="234da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="234da-127">Request body</span></span>
<span data-ttu-id="234da-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="234da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="234da-129">响应</span><span class="sxs-lookup"><span data-stu-id="234da-129">Response</span></span>
<span data-ttu-id="234da-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="234da-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="234da-131">示例</span><span class="sxs-lookup"><span data-stu-id="234da-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="234da-132">请求</span><span class="sxs-lookup"><span data-stu-id="234da-132">Request</span></span>
<span data-ttu-id="234da-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="234da-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="234da-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="234da-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="234da-135">C#</span><span class="sxs-lookup"><span data-stu-id="234da-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="234da-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="234da-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="234da-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="234da-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="234da-138">Java</span><span class="sxs-lookup"><span data-stu-id="234da-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photos-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="234da-139">响应</span><span class="sxs-lookup"><span data-stu-id="234da-139">Response</span></span>
<span data-ttu-id="234da-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="234da-140">The following is an example of the response.</span></span>
><span data-ttu-id="234da-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="234da-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="234da-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="234da-142">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
