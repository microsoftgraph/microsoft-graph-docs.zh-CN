---
title: 获取 educationAssignmentResource
description: '获取工作分配的特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 18d49ab13e124aebb596aacf5d48ef6f83e3a29b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587390"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="9cf59-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9cf59-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf59-104">获取工作分配的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="9cf59-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="9cf59-105">权限</span><span class="sxs-lookup"><span data-stu-id="9cf59-105">Permissions</span></span>
<span data-ttu-id="9cf59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cf59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf59-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cf59-108">Permission type</span></span>      | <span data-ttu-id="9cf59-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cf59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cf59-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9cf59-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="9cf59-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="9cf59-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf59-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9cf59-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf59-113">Not supported.</span></span>  |
|<span data-ttu-id="9cf59-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cf59-114">Application</span></span> |  <span data-ttu-id="9cf59-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf59-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9cf59-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cf59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9cf59-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9cf59-117">Optional query parameters</span></span>
<span data-ttu-id="9cf59-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9cf59-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cf59-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cf59-119">Request headers</span></span>
| <span data-ttu-id="9cf59-120">标头</span><span class="sxs-lookup"><span data-stu-id="9cf59-120">Header</span></span>       | <span data-ttu-id="9cf59-121">值</span><span class="sxs-lookup"><span data-stu-id="9cf59-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9cf59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cf59-122">Authorization</span></span>  | <span data-ttu-id="9cf59-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cf59-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cf59-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cf59-125">Request body</span></span>
<span data-ttu-id="9cf59-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cf59-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9cf59-127">响应</span><span class="sxs-lookup"><span data-stu-id="9cf59-127">Response</span></span>
<span data-ttu-id="9cf59-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9cf59-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cf59-129">示例</span><span class="sxs-lookup"><span data-stu-id="9cf59-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cf59-130">请求</span><span class="sxs-lookup"><span data-stu-id="9cf59-130">Request</span></span>
<span data-ttu-id="9cf59-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cf59-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="9cf59-132">响应</span><span class="sxs-lookup"><span data-stu-id="9cf59-132">Response</span></span>
<span data-ttu-id="9cf59-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9cf59-133">The following is an example of the response.</span></span> 

><span data-ttu-id="9cf59-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cf59-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9cf59-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cf59-135">All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9cf59-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9cf59-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9cf59-137">语言</span><span class="sxs-lookup"><span data-stu-id="9cf59-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationassignmentresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cf59-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9cf59-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationassignmentresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
