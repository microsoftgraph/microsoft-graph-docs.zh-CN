---
title: 列出 assignmentCategories
description: 检索类别对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5e07a33e8dd3d3e55fc894e58049a301b1b7a756
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912336"
---
# <a name="list-assignmentcategories"></a><span data-ttu-id="8ddd9-103">列出 assignmentCategories</span><span class="sxs-lookup"><span data-stu-id="8ddd9-103">List assignmentCategories</span></span>

<span data-ttu-id="8ddd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ddd9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ddd9-105">检索 [educationCategory 对象](../resources/educationcategory.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ddd9-106">权限</span><span class="sxs-lookup"><span data-stu-id="8ddd9-106">Permissions</span></span>

<span data-ttu-id="8ddd9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ddd9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ddd9-109">Permission type</span></span>                        | <span data-ttu-id="8ddd9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ddd9-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8ddd9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ddd9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ddd9-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ddd9-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8ddd9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ddd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ddd9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="8ddd9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ddd9-115">Application</span></span>                            | <span data-ttu-id="8ddd9-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ddd9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ddd9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ddd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ddd9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8ddd9-118">Optional query parameters</span></span>

<span data-ttu-id="8ddd9-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ddd9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ddd9-120">Request headers</span></span>

| <span data-ttu-id="8ddd9-121">标头</span><span class="sxs-lookup"><span data-stu-id="8ddd9-121">Header</span></span>        | <span data-ttu-id="8ddd9-122">值</span><span class="sxs-lookup"><span data-stu-id="8ddd9-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8ddd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ddd9-123">Authorization</span></span> | <span data-ttu-id="8ddd9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ddd9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ddd9-126">Request body</span></span>

<span data-ttu-id="8ddd9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ddd9-128">响应</span><span class="sxs-lookup"><span data-stu-id="8ddd9-128">Response</span></span>

<span data-ttu-id="8ddd9-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationCategory](../resources/educationcategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ddd9-130">示例</span><span class="sxs-lookup"><span data-stu-id="8ddd9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ddd9-131">请求</span><span class="sxs-lookup"><span data-stu-id="8ddd9-131">Request</span></span>

<span data-ttu-id="8ddd9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["acdefc6b-2dc6-4e71-b1e9-6d9810ab1793"],
  "name": "get_class_categories"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories
```

### <a name="response"></a><span data-ttu-id="8ddd9-133">响应</span><span class="sxs-lookup"><span data-stu-id="8ddd9-133">Response</span></span>

<span data-ttu-id="8ddd9-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8ddd9-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8ddd9-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
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
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
