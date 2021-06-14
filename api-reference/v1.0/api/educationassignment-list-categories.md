---
title: 列出类别
description: 列出与此工作分配关联的所有类别。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15e6be29aa4f39772559506043d1de5f5c6bae35
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912295"
---
# <a name="list-categories"></a><span data-ttu-id="53d9b-103">列出类别</span><span class="sxs-lookup"><span data-stu-id="53d9b-103">List categories</span></span>

<span data-ttu-id="53d9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53d9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53d9b-105">列出与工作分配关联的所有类别。</span><span class="sxs-lookup"><span data-stu-id="53d9b-105">List all the categories associated with an assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="53d9b-106">权限</span><span class="sxs-lookup"><span data-stu-id="53d9b-106">Permissions</span></span>
<span data-ttu-id="53d9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d9b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53d9b-109">Permission type</span></span>      | <span data-ttu-id="53d9b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53d9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d9b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53d9b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="53d9b-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53d9b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="53d9b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53d9b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53d9b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53d9b-114">Not supported.</span></span>  |
|<span data-ttu-id="53d9b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53d9b-115">Application</span></span> | <span data-ttu-id="53d9b-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53d9b-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53d9b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53d9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53d9b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53d9b-118">Optional query parameters</span></span>
<span data-ttu-id="53d9b-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53d9b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53d9b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53d9b-120">Request headers</span></span>
| <span data-ttu-id="53d9b-121">标头</span><span class="sxs-lookup"><span data-stu-id="53d9b-121">Header</span></span>       | <span data-ttu-id="53d9b-122">值</span><span class="sxs-lookup"><span data-stu-id="53d9b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53d9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d9b-123">Authorization</span></span>  | <span data-ttu-id="53d9b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53d9b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53d9b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53d9b-126">Request body</span></span>
<span data-ttu-id="53d9b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53d9b-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d9b-128">响应</span><span class="sxs-lookup"><span data-stu-id="53d9b-128">Response</span></span>
<span data-ttu-id="53d9b-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53d9b-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53d9b-130">示例</span><span class="sxs-lookup"><span data-stu-id="53d9b-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="53d9b-131">请求</span><span class="sxs-lookup"><span data-stu-id="53d9b-131">Request</span></span>
<span data-ttu-id="53d9b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53d9b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_assignment_categories"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories
```

### <a name="response"></a><span data-ttu-id="53d9b-133">响应</span><span class="sxs-lookup"><span data-stu-id="53d9b-133">Response</span></span>
<span data-ttu-id="53d9b-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53d9b-134">The following is an example of the response.</span></span> 

><span data-ttu-id="53d9b-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53d9b-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('a17025d0-62a8-4450-9e6e-db31d8c8feb8')/assignments('1fdf61ee-c129-4960-9b7c-8df159aa64b0')/categories",
    "value": [
        {
            "displayName": "Quizzes",
            "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
        }
    ]
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
  "suppressions": []
}
-->
