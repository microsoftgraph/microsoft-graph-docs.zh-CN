---
title: List photos
description: 检索 profilePhoto 对象列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5970958c72b3202aefdc1347814a171674601f9f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052318"
---
# <a name="list-photos"></a><span data-ttu-id="8a043-103">List photos</span><span class="sxs-lookup"><span data-stu-id="8a043-103">List photos</span></span>

<span data-ttu-id="8a043-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a043-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a043-105">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8a043-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a043-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a043-106">Permissions</span></span>
<span data-ttu-id="8a043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a043-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a043-109">Permission type</span></span>      | <span data-ttu-id="8a043-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a043-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a043-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a043-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a043-112">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a043-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="8a043-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a043-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a043-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a043-114">Not supported.</span></span>    |
|<span data-ttu-id="8a043-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a043-115">Application</span></span> | <span data-ttu-id="8a043-116">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a043-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a043-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a043-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a043-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8a043-118">Optional query parameters</span></span>
<span data-ttu-id="8a043-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8a043-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a043-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a043-120">Request headers</span></span>
| <span data-ttu-id="8a043-121">名称</span><span class="sxs-lookup"><span data-stu-id="8a043-121">Name</span></span>       | <span data-ttu-id="8a043-122">类型</span><span class="sxs-lookup"><span data-stu-id="8a043-122">Type</span></span> | <span data-ttu-id="8a043-123">说明</span><span class="sxs-lookup"><span data-stu-id="8a043-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a043-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a043-124">Authorization</span></span>  | <span data-ttu-id="8a043-125">string</span><span class="sxs-lookup"><span data-stu-id="8a043-125">string</span></span>  | <span data-ttu-id="8a043-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a043-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a043-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a043-128">Request body</span></span>
<span data-ttu-id="8a043-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a043-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a043-130">响应</span><span class="sxs-lookup"><span data-stu-id="8a043-130">Response</span></span>
<span data-ttu-id="8a043-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8a043-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a043-132">示例</span><span class="sxs-lookup"><span data-stu-id="8a043-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8a043-133">请求</span><span class="sxs-lookup"><span data-stu-id="8a043-133">Request</span></span>
<span data-ttu-id="8a043-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a043-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a043-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a043-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="8a043-136">C#</span><span class="sxs-lookup"><span data-stu-id="8a043-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a043-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a043-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a043-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a043-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a043-139">Java</span><span class="sxs-lookup"><span data-stu-id="8a043-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photos-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a043-140">响应</span><span class="sxs-lookup"><span data-stu-id="8a043-140">Response</span></span>
<span data-ttu-id="8a043-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a043-141">The following is an example of the response.</span></span>
><span data-ttu-id="8a043-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8a043-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

