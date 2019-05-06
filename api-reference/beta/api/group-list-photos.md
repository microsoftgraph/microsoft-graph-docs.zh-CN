---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d1ce8094e34370c5a04d770b46e7d7f9982233e5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592833"
---
# <a name="list-photos"></a><span data-ttu-id="4fbc2-103">List photos</span><span class="sxs-lookup"><span data-stu-id="4fbc2-103">List photos</span></span>
<span data-ttu-id="4fbc2-104">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fbc2-105">权限</span><span class="sxs-lookup"><span data-stu-id="4fbc2-105">Permissions</span></span>
<span data-ttu-id="4fbc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fbc2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fbc2-108">Permission type</span></span>      | <span data-ttu-id="4fbc2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fbc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fbc2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4fbc2-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbc2-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="4fbc2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fbc2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-113">Not supported.</span></span>    |
|<span data-ttu-id="4fbc2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fbc2-114">Application</span></span> | <span data-ttu-id="4fbc2-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbc2-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fbc2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fbc2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4fbc2-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4fbc2-117">Optional query parameters</span></span>
<span data-ttu-id="4fbc2-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fbc2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fbc2-119">Request headers</span></span>
| <span data-ttu-id="4fbc2-120">名称</span><span class="sxs-lookup"><span data-stu-id="4fbc2-120">Name</span></span>       | <span data-ttu-id="4fbc2-121">类型</span><span class="sxs-lookup"><span data-stu-id="4fbc2-121">Type</span></span> | <span data-ttu-id="4fbc2-122">说明</span><span class="sxs-lookup"><span data-stu-id="4fbc2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4fbc2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fbc2-123">Authorization</span></span>  | <span data-ttu-id="4fbc2-124">string</span><span class="sxs-lookup"><span data-stu-id="4fbc2-124">string</span></span>  | <span data-ttu-id="4fbc2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fbc2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fbc2-127">Request body</span></span>
<span data-ttu-id="4fbc2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fbc2-129">响应</span><span class="sxs-lookup"><span data-stu-id="4fbc2-129">Response</span></span>
<span data-ttu-id="4fbc2-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fbc2-131">示例</span><span class="sxs-lookup"><span data-stu-id="4fbc2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4fbc2-132">请求</span><span class="sxs-lookup"><span data-stu-id="4fbc2-132">Request</span></span>
<span data-ttu-id="4fbc2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="4fbc2-134">响应</span><span class="sxs-lookup"><span data-stu-id="4fbc2-134">Response</span></span>
<span data-ttu-id="4fbc2-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-135">The following is an example of the response.</span></span>
><span data-ttu-id="4fbc2-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4fbc2-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4fbc2-137">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4fbc2-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4fbc2-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4fbc2-139">语言</span><span class="sxs-lookup"><span data-stu-id="4fbc2-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fbc2-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="4fbc2-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
