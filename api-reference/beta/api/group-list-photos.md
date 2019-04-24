---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 959c25bc9904a8145240f76baaf3271e29e17eef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502050"
---
# <a name="list-photos"></a><span data-ttu-id="b4ed6-103">List photos</span><span class="sxs-lookup"><span data-stu-id="b4ed6-103">List photos</span></span>
<span data-ttu-id="b4ed6-104">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ed6-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4ed6-105">Permissions</span></span>
<span data-ttu-id="b4ed6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ed6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4ed6-108">Permission type</span></span>      | <span data-ttu-id="b4ed6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ed6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ed6-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ed6-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="b4ed6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ed6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-113">Not supported.</span></span>    |
|<span data-ttu-id="b4ed6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4ed6-114">Application</span></span> | <span data-ttu-id="b4ed6-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ed6-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ed6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4ed6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4ed6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4ed6-117">Optional query parameters</span></span>
<span data-ttu-id="b4ed6-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4ed6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4ed6-119">Request headers</span></span>
| <span data-ttu-id="b4ed6-120">名称</span><span class="sxs-lookup"><span data-stu-id="b4ed6-120">Name</span></span>       | <span data-ttu-id="b4ed6-121">类型</span><span class="sxs-lookup"><span data-stu-id="b4ed6-121">Type</span></span> | <span data-ttu-id="b4ed6-122">说明</span><span class="sxs-lookup"><span data-stu-id="b4ed6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4ed6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ed6-123">Authorization</span></span>  | <span data-ttu-id="b4ed6-124">string</span><span class="sxs-lookup"><span data-stu-id="b4ed6-124">string</span></span>  | <span data-ttu-id="b4ed6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ed6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4ed6-127">Request body</span></span>
<span data-ttu-id="b4ed6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4ed6-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4ed6-129">Response</span></span>
<span data-ttu-id="b4ed6-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ed6-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4ed6-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b4ed6-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4ed6-132">Request</span></span>
<span data-ttu-id="b4ed6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="b4ed6-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4ed6-134">Response</span></span>
<span data-ttu-id="b4ed6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-135">The following is an example of the response.</span></span>
><span data-ttu-id="b4ed6-136">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4ed6-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-137">All the properties will be returned from an actual call.</span></span>
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
