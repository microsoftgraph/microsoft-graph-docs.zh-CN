---
title: 获取 educationCategory
description: 检索 category 对象。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c88e8ae48aade64fb5f219008e277063dae46f1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810875"
---
# <a name="get-educationcategory"></a><span data-ttu-id="0c8fc-103">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="0c8fc-103">Get educationCategory</span></span>

<span data-ttu-id="0c8fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c8fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c8fc-105">检索 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c8fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c8fc-106">Permissions</span></span>

<span data-ttu-id="0c8fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c8fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c8fc-109">Permission type</span></span>                        | <span data-ttu-id="0c8fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c8fc-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0c8fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c8fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c8fc-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0c8fc-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0c8fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c8fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c8fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="0c8fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c8fc-115">Application</span></span>                            | <span data-ttu-id="0c8fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="0c8fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c8fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c8fc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c8fc-118">Optional query parameters</span></span>

<span data-ttu-id="0c8fc-119">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c8fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c8fc-120">Request headers</span></span>
| <span data-ttu-id="0c8fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="0c8fc-121">Header</span></span>        | <span data-ttu-id="0c8fc-122">值</span><span class="sxs-lookup"><span data-stu-id="0c8fc-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="0c8fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c8fc-123">Authorization</span></span> | <span data-ttu-id="0c8fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c8fc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c8fc-126">Request body</span></span>

<span data-ttu-id="0c8fc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c8fc-128">响应</span><span class="sxs-lookup"><span data-stu-id="0c8fc-128">Response</span></span>

<span data-ttu-id="0c8fc-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c8fc-130">示例</span><span class="sxs-lookup"><span data-stu-id="0c8fc-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0c8fc-131">请求</span><span class="sxs-lookup"><span data-stu-id="0c8fc-131">Request</span></span>

<span data-ttu-id="0c8fc-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="0c8fc-133">响应</span><span class="sxs-lookup"><span data-stu-id="0c8fc-133">Response</span></span>

<span data-ttu-id="0c8fc-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-134">The following is an example of the response.</span></span>

><span data-ttu-id="0c8fc-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0c8fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
}
```

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
