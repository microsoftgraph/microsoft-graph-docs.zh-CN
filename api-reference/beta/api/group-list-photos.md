---
title: List photos
description: 检索 profilePhoto 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 959c25bc9904a8145240f76baaf3271e29e17eef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514395"
---
# <a name="list-photos"></a><span data-ttu-id="388a5-103">List photos</span><span class="sxs-lookup"><span data-stu-id="388a5-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="388a5-104">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="388a5-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="388a5-105">权限</span><span class="sxs-lookup"><span data-stu-id="388a5-105">Permissions</span></span>
<span data-ttu-id="388a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="388a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="388a5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="388a5-108">Permission type</span></span>      | <span data-ttu-id="388a5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="388a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="388a5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="388a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="388a5-111">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="388a5-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="388a5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="388a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="388a5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="388a5-113">Not supported.</span></span>    |
|<span data-ttu-id="388a5-114">应用</span><span class="sxs-lookup"><span data-stu-id="388a5-114">Application</span></span> | <span data-ttu-id="388a5-115">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="388a5-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="388a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="388a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="388a5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="388a5-117">Optional query parameters</span></span>
<span data-ttu-id="388a5-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="388a5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="388a5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="388a5-119">Request headers</span></span>
| <span data-ttu-id="388a5-120">名称</span><span class="sxs-lookup"><span data-stu-id="388a5-120">Name</span></span>       | <span data-ttu-id="388a5-121">类型</span><span class="sxs-lookup"><span data-stu-id="388a5-121">Type</span></span> | <span data-ttu-id="388a5-122">说明</span><span class="sxs-lookup"><span data-stu-id="388a5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="388a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="388a5-123">Authorization</span></span>  | <span data-ttu-id="388a5-124">string</span><span class="sxs-lookup"><span data-stu-id="388a5-124">string</span></span>  | <span data-ttu-id="388a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="388a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="388a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="388a5-127">Request body</span></span>
<span data-ttu-id="388a5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="388a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="388a5-129">响应</span><span class="sxs-lookup"><span data-stu-id="388a5-129">Response</span></span>
<span data-ttu-id="388a5-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="388a5-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="388a5-131">示例</span><span class="sxs-lookup"><span data-stu-id="388a5-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="388a5-132">请求</span><span class="sxs-lookup"><span data-stu-id="388a5-132">Request</span></span>
<span data-ttu-id="388a5-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="388a5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="388a5-134">响应</span><span class="sxs-lookup"><span data-stu-id="388a5-134">Response</span></span>
<span data-ttu-id="388a5-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="388a5-135">The following is an example of the response.</span></span>
><span data-ttu-id="388a5-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="388a5-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="388a5-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="388a5-137">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
