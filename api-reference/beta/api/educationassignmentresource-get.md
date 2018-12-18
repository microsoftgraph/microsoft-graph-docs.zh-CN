---
title: 获取 educationAssignmentResource
description: '工作分配上获取特定资源的属性。  '
author: dipakboyed
ms.openlocfilehash: 25c448f3247631c9129a837bd00842588bf152d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358812"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="61b64-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="61b64-103">Get educationAssignmentResource</span></span>

> <span data-ttu-id="61b64-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="61b64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61b64-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61b64-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61b64-106">工作分配上获取特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="61b64-106">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="61b64-107">权限</span><span class="sxs-lookup"><span data-stu-id="61b64-107">Permissions</span></span>
<span data-ttu-id="61b64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61b64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61b64-110">Permission type</span></span>      | <span data-ttu-id="61b64-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61b64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61b64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61b64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61b64-113">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b64-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="61b64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61b64-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="61b64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61b64-115">Not supported.</span></span>  |
|<span data-ttu-id="61b64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61b64-116">Application</span></span> |  <span data-ttu-id="61b64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="61b64-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61b64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61b64-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61b64-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61b64-119">Optional query parameters</span></span>
<span data-ttu-id="61b64-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61b64-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61b64-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="61b64-121">Request headers</span></span>
| <span data-ttu-id="61b64-122">标头</span><span class="sxs-lookup"><span data-stu-id="61b64-122">Header</span></span>       | <span data-ttu-id="61b64-123">值</span><span class="sxs-lookup"><span data-stu-id="61b64-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61b64-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="61b64-124">Authorization</span></span>  | <span data-ttu-id="61b64-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61b64-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61b64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="61b64-127">Request body</span></span>
<span data-ttu-id="61b64-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61b64-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="61b64-129">响应</span><span class="sxs-lookup"><span data-stu-id="61b64-129">Response</span></span>
<span data-ttu-id="61b64-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61b64-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61b64-131">示例</span><span class="sxs-lookup"><span data-stu-id="61b64-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61b64-132">请求</span><span class="sxs-lookup"><span data-stu-id="61b64-132">Request</span></span>
<span data-ttu-id="61b64-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61b64-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="61b64-134">响应</span><span class="sxs-lookup"><span data-stu-id="61b64-134">Response</span></span>
<span data-ttu-id="61b64-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61b64-135">The following is an example of the response.</span></span> 

><span data-ttu-id="61b64-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61b64-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="61b64-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61b64-137">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->