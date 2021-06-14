---
title: 获取 educationAssignmentResource
description: '获取工作分配上特定资源的属性。  '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11d19047d055ef51f28dca27ea20861e8f9cfa59
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912339"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="66253-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="66253-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="66253-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66253-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66253-105">获取工作分配上特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="66253-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="66253-106">权限</span><span class="sxs-lookup"><span data-stu-id="66253-106">Permissions</span></span>
<span data-ttu-id="66253-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66253-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66253-109">Permission type</span></span>      | <span data-ttu-id="66253-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66253-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66253-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66253-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66253-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66253-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="66253-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66253-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="66253-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="66253-114">Not supported.</span></span>  |
|<span data-ttu-id="66253-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66253-115">Application</span></span> |  <span data-ttu-id="66253-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66253-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="66253-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66253-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66253-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66253-118">Optional query parameters</span></span>
<span data-ttu-id="66253-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66253-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66253-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66253-120">Request headers</span></span>
| <span data-ttu-id="66253-121">标头</span><span class="sxs-lookup"><span data-stu-id="66253-121">Header</span></span>       | <span data-ttu-id="66253-122">值</span><span class="sxs-lookup"><span data-stu-id="66253-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66253-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66253-123">Authorization</span></span>  | <span data-ttu-id="66253-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66253-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66253-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66253-126">Request body</span></span>
<span data-ttu-id="66253-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66253-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66253-128">响应</span><span class="sxs-lookup"><span data-stu-id="66253-128">Response</span></span>
<span data-ttu-id="66253-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66253-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66253-130">示例</span><span class="sxs-lookup"><span data-stu-id="66253-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="66253-131">请求</span><span class="sxs-lookup"><span data-stu-id="66253-131">Request</span></span>
<span data-ttu-id="66253-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66253-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```

### <a name="response"></a><span data-ttu-id="66253-133">响应</span><span class="sxs-lookup"><span data-stu-id="66253-133">Response</span></span>
<span data-ttu-id="66253-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="66253-134">The following is an example of the response.</span></span> 

><span data-ttu-id="66253-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66253-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "displayName": "Shawn Hughes",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Shawn Hughes",
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
  ]
}
-->
