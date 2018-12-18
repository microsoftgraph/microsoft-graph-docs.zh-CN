---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
ms.openlocfilehash: 2597d532d28614bb595ffe44aa6705187619aa44
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315818"
---
# <a name="list-photos"></a><span data-ttu-id="fadee-103">List photos</span><span class="sxs-lookup"><span data-stu-id="fadee-103">List photos</span></span>

> <span data-ttu-id="fadee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fadee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fadee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fadee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fadee-106">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="fadee-106">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fadee-107">权限</span><span class="sxs-lookup"><span data-stu-id="fadee-107">Permissions</span></span>
<span data-ttu-id="fadee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fadee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fadee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fadee-110">Permission type</span></span>      | <span data-ttu-id="fadee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fadee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fadee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fadee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fadee-113">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fadee-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fadee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fadee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fadee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fadee-115">Not supported.</span></span>    |
|<span data-ttu-id="fadee-116">应用</span><span class="sxs-lookup"><span data-stu-id="fadee-116">Application</span></span> | <span data-ttu-id="fadee-117">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fadee-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fadee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fadee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fadee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fadee-119">Optional query parameters</span></span>
<span data-ttu-id="fadee-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fadee-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fadee-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fadee-121">Request headers</span></span>
| <span data-ttu-id="fadee-122">Name</span><span class="sxs-lookup"><span data-stu-id="fadee-122">Name</span></span>       | <span data-ttu-id="fadee-123">类型</span><span class="sxs-lookup"><span data-stu-id="fadee-123">Type</span></span> | <span data-ttu-id="fadee-124">说明</span><span class="sxs-lookup"><span data-stu-id="fadee-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fadee-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fadee-125">Authorization</span></span>  | <span data-ttu-id="fadee-126">string</span><span class="sxs-lookup"><span data-stu-id="fadee-126">string</span></span>  | <span data-ttu-id="fadee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fadee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fadee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fadee-129">Request body</span></span>
<span data-ttu-id="fadee-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fadee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fadee-131">响应</span><span class="sxs-lookup"><span data-stu-id="fadee-131">Response</span></span>
<span data-ttu-id="fadee-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fadee-132">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fadee-133">示例</span><span class="sxs-lookup"><span data-stu-id="fadee-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fadee-134">请求</span><span class="sxs-lookup"><span data-stu-id="fadee-134">Request</span></span>
<span data-ttu-id="fadee-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fadee-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="fadee-136">响应</span><span class="sxs-lookup"><span data-stu-id="fadee-136">Response</span></span>
<span data-ttu-id="fadee-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fadee-137">The following is an example of the response.</span></span>
><span data-ttu-id="fadee-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fadee-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fadee-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fadee-139">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->