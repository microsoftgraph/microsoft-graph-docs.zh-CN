---
title: 获取 educationAssignmentResource
description: '获取工作分配的特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 76d9ed55c4e914385ad6282e3bed6025ef5c6036
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457968"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="d74d6-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="d74d6-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d74d6-104">获取工作分配的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d74d6-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="d74d6-105">权限</span><span class="sxs-lookup"><span data-stu-id="d74d6-105">Permissions</span></span>
<span data-ttu-id="d74d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d74d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74d6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d74d6-108">Permission type</span></span>      | <span data-ttu-id="d74d6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d74d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d74d6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d74d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d74d6-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d74d6-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="d74d6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d74d6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d74d6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d74d6-113">Not supported.</span></span>  |
|<span data-ttu-id="d74d6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d74d6-114">Application</span></span> |  <span data-ttu-id="d74d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d74d6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d74d6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d74d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d74d6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d74d6-117">Optional query parameters</span></span>
<span data-ttu-id="d74d6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d74d6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d74d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d74d6-119">Request headers</span></span>
| <span data-ttu-id="d74d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="d74d6-120">Header</span></span>       | <span data-ttu-id="d74d6-121">值</span><span class="sxs-lookup"><span data-stu-id="d74d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d74d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d74d6-122">Authorization</span></span>  | <span data-ttu-id="d74d6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d74d6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d74d6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d74d6-125">Request body</span></span>
<span data-ttu-id="d74d6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d74d6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d74d6-127">响应</span><span class="sxs-lookup"><span data-stu-id="d74d6-127">Response</span></span>
<span data-ttu-id="d74d6-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d74d6-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d74d6-129">示例</span><span class="sxs-lookup"><span data-stu-id="d74d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d74d6-130">请求</span><span class="sxs-lookup"><span data-stu-id="d74d6-130">Request</span></span>
<span data-ttu-id="d74d6-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d74d6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="d74d6-132">响应</span><span class="sxs-lookup"><span data-stu-id="d74d6-132">Response</span></span>
<span data-ttu-id="d74d6-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d74d6-133">The following is an example of the response.</span></span> 

><span data-ttu-id="d74d6-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d74d6-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d74d6-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d74d6-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
