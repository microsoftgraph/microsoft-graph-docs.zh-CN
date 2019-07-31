---
title: 获取 educationCategory
description: 检索 category 对象。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b25b41168cc08986c5cc21ab2e5932e5c037993d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955521"
---
# <a name="get-educationcategory"></a><span data-ttu-id="70200-103">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="70200-103">Get educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70200-104">检索[educationCategory](../resources/educationcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70200-104">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70200-105">权限</span><span class="sxs-lookup"><span data-stu-id="70200-105">Permissions</span></span>

<span data-ttu-id="70200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70200-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="70200-108">Permission type</span></span>                        | <span data-ttu-id="70200-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70200-109">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="70200-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70200-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="70200-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="70200-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="70200-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70200-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70200-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="70200-113">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="70200-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="70200-114">Application</span></span>                            | <span data-ttu-id="70200-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70200-115">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="70200-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70200-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70200-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70200-117">Optional query parameters</span></span>

<span data-ttu-id="70200-118">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="70200-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70200-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70200-119">Request headers</span></span>
| <span data-ttu-id="70200-120">标头</span><span class="sxs-lookup"><span data-stu-id="70200-120">Header</span></span>        | <span data-ttu-id="70200-121">值</span><span class="sxs-lookup"><span data-stu-id="70200-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="70200-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70200-122">Authorization</span></span> | <span data-ttu-id="70200-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70200-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70200-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="70200-125">Request body</span></span>

<span data-ttu-id="70200-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70200-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70200-127">响应</span><span class="sxs-lookup"><span data-stu-id="70200-127">Response</span></span>

<span data-ttu-id="70200-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationCategory](../resources/educationcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70200-128">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70200-129">示例</span><span class="sxs-lookup"><span data-stu-id="70200-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70200-130">请求</span><span class="sxs-lookup"><span data-stu-id="70200-130">Request</span></span>

<span data-ttu-id="70200-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70200-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="70200-132">响应</span><span class="sxs-lookup"><span data-stu-id="70200-132">Response</span></span>

<span data-ttu-id="70200-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70200-133">The following is an example of the response.</span></span> 

><span data-ttu-id="70200-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="70200-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
