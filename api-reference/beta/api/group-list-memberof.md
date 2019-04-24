---
title: 列出组 memberOf
description: 获取组是其直接成员的组和管理单元。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ecf127e7cc4af4aada3d75ef6415a242b0a9411b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502110"
---
# <a name="list-group-memberof"></a><span data-ttu-id="3c2a8-103">列出组 memberOf</span><span class="sxs-lookup"><span data-stu-id="3c2a8-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c2a8-104">获取组是其直接成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="3c2a8-105">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-105">This operation is not transitive.</span></span> <span data-ttu-id="3c2a8-106">与获取用户的 Office 365 组不同, 这将返回所有类型的组, 而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-106">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3c2a8-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c2a8-107">Permissions</span></span>

<span data-ttu-id="3c2a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c2a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c2a8-110">Permission type</span></span>      | <span data-ttu-id="3c2a8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c2a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c2a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c2a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c2a8-113">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c2a8-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c2a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c2a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c2a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-115">Not supported.</span></span>    |
|<span data-ttu-id="3c2a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c2a8-116">Application</span></span> | <span data-ttu-id="3c2a8-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2a8-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c2a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c2a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c2a8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c2a8-119">Optional query parameters</span></span>
<span data-ttu-id="3c2a8-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c2a8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c2a8-121">Request headers</span></span>
| <span data-ttu-id="3c2a8-122">名称</span><span class="sxs-lookup"><span data-stu-id="3c2a8-122">Name</span></span>       | <span data-ttu-id="3c2a8-123">类型</span><span class="sxs-lookup"><span data-stu-id="3c2a8-123">Type</span></span> | <span data-ttu-id="3c2a8-124">说明</span><span class="sxs-lookup"><span data-stu-id="3c2a8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c2a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c2a8-125">Authorization</span></span>  | <span data-ttu-id="3c2a8-126">string</span><span class="sxs-lookup"><span data-stu-id="3c2a8-126">string</span></span>  | <span data-ttu-id="3c2a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c2a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c2a8-129">Request body</span></span>
<span data-ttu-id="3c2a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c2a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="3c2a8-131">Response</span></span>
<span data-ttu-id="3c2a8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c2a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="3c2a8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c2a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="3c2a8-134">Request</span></span>

<span data-ttu-id="3c2a8-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="3c2a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="3c2a8-136">Response</span></span>

<span data-ttu-id="3c2a8-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-137">The following is an example of the response.</span></span>
><span data-ttu-id="3c2a8-138">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c2a8-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3c2a8-139">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
