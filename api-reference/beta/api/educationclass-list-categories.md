---
title: 列出 educationCategories
description: 检索 category 对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f647c0b5241dc7ab98d0fda5f3ccce8233a6b557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426694"
---
# <a name="list-educationcategories"></a><span data-ttu-id="d3597-103">列出 educationCategories</span><span class="sxs-lookup"><span data-stu-id="d3597-103">List educationCategories</span></span>

<span data-ttu-id="d3597-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d3597-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3597-105">检索[educationCategory](../resources/educationcategory.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d3597-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3597-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3597-106">Permissions</span></span>

<span data-ttu-id="d3597-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3597-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3597-109">Permission type</span></span>                        | <span data-ttu-id="d3597-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3597-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d3597-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3597-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3597-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d3597-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d3597-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3597-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3597-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3597-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="d3597-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3597-115">Application</span></span>                            | <span data-ttu-id="d3597-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3597-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="d3597-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3597-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3597-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3597-118">Optional query parameters</span></span>

<span data-ttu-id="d3597-119">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3597-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3597-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3597-120">Request headers</span></span>

| <span data-ttu-id="d3597-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3597-121">Header</span></span>        | <span data-ttu-id="d3597-122">值</span><span class="sxs-lookup"><span data-stu-id="d3597-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d3597-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3597-123">Authorization</span></span> | <span data-ttu-id="d3597-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3597-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3597-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3597-126">Request body</span></span>

<span data-ttu-id="d3597-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3597-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3597-128">响应</span><span class="sxs-lookup"><span data-stu-id="d3597-128">Response</span></span>

<span data-ttu-id="d3597-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationCategory](../resources/educationcategory.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d3597-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3597-130">示例</span><span class="sxs-lookup"><span data-stu-id="d3597-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d3597-131">请求</span><span class="sxs-lookup"><span data-stu-id="d3597-131">Request</span></span>

<span data-ttu-id="d3597-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3597-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="d3597-133">响应</span><span class="sxs-lookup"><span data-stu-id="d3597-133">Response</span></span>

<span data-ttu-id="d3597-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3597-134">The following is an example of the response.</span></span> 

><span data-ttu-id="d3597-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3597-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
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
