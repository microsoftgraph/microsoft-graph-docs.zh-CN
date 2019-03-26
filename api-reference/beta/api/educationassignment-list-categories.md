---
title: 列出类别
description: 列出与此工作分配相关联的所有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 925b2f558b98e50cfcebd7b68c3af52452f2e3df
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800968"
---
# <a name="list-categories"></a><span data-ttu-id="77c61-103">列出类别</span><span class="sxs-lookup"><span data-stu-id="77c61-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c61-104">列出与此工作分配相关联的所有类别。</span><span class="sxs-lookup"><span data-stu-id="77c61-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="77c61-105">权限</span><span class="sxs-lookup"><span data-stu-id="77c61-105">Permissions</span></span>
<span data-ttu-id="77c61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77c61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77c61-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77c61-108">Permission type</span></span>      | <span data-ttu-id="77c61-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77c61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77c61-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77c61-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="77c61-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="77c61-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="77c61-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77c61-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="77c61-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77c61-113">Not supported.</span></span>  |
|<span data-ttu-id="77c61-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77c61-114">Application</span></span> | <span data-ttu-id="77c61-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77c61-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="77c61-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77c61-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77c61-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77c61-117">Optional query parameters</span></span>
<span data-ttu-id="77c61-118">此方法支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77c61-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77c61-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77c61-119">Request headers</span></span>
| <span data-ttu-id="77c61-120">标头</span><span class="sxs-lookup"><span data-stu-id="77c61-120">Header</span></span>       | <span data-ttu-id="77c61-121">值</span><span class="sxs-lookup"><span data-stu-id="77c61-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77c61-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77c61-122">Authorization</span></span>  | <span data-ttu-id="77c61-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77c61-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77c61-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="77c61-125">Request body</span></span>
<span data-ttu-id="77c61-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77c61-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="77c61-127">响应</span><span class="sxs-lookup"><span data-stu-id="77c61-127">Response</span></span>
<span data-ttu-id="77c61-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationCategory](../resources/educationcategory.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="77c61-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77c61-129">示例</span><span class="sxs-lookup"><span data-stu-id="77c61-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77c61-130">请求</span><span class="sxs-lookup"><span data-stu-id="77c61-130">Request</span></span>
<span data-ttu-id="77c61-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77c61-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="77c61-132">响应</span><span class="sxs-lookup"><span data-stu-id="77c61-132">Response</span></span>
<span data-ttu-id="77c61-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77c61-133">The following is an example of the response.</span></span> 

><span data-ttu-id="77c61-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77c61-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77c61-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77c61-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-categories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
