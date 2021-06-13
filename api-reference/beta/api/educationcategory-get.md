---
title: 获取 educationCategory
description: 检索类别对象。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3d7e64b947d1cd9ffbfa2ad666fbfb3a9c711ebd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911877"
---
# <a name="get-educationcategory"></a><span data-ttu-id="2384e-103">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="2384e-103">Get educationCategory</span></span>

<span data-ttu-id="2384e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2384e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2384e-105">检索 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2384e-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2384e-106">权限</span><span class="sxs-lookup"><span data-stu-id="2384e-106">Permissions</span></span>

<span data-ttu-id="2384e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2384e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2384e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2384e-109">Permission type</span></span>                        | <span data-ttu-id="2384e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2384e-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2384e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2384e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2384e-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2384e-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2384e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2384e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2384e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2384e-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="2384e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2384e-115">Application</span></span>                            | <span data-ttu-id="2384e-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2384e-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2384e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2384e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2384e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2384e-118">Optional query parameters</span></span>

<span data-ttu-id="2384e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2384e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2384e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2384e-120">Request headers</span></span>
| <span data-ttu-id="2384e-121">标头</span><span class="sxs-lookup"><span data-stu-id="2384e-121">Header</span></span>        | <span data-ttu-id="2384e-122">值</span><span class="sxs-lookup"><span data-stu-id="2384e-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2384e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2384e-123">Authorization</span></span> | <span data-ttu-id="2384e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2384e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2384e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2384e-126">Request body</span></span>

<span data-ttu-id="2384e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2384e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2384e-128">响应</span><span class="sxs-lookup"><span data-stu-id="2384e-128">Response</span></span>

<span data-ttu-id="2384e-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2384e-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2384e-130">示例</span><span class="sxs-lookup"><span data-stu-id="2384e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2384e-131">请求</span><span class="sxs-lookup"><span data-stu-id="2384e-131">Request</span></span>

<span data-ttu-id="2384e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2384e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["dacbf757-888d-42ae-b701-5e57cec300ae"],
  "name": "get_class_category"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747
```

##### <a name="response"></a><span data-ttu-id="2384e-133">响应</span><span class="sxs-lookup"><span data-stu-id="2384e-133">Response</span></span>

<span data-ttu-id="2384e-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2384e-134">The following is an example of the response.</span></span>

><span data-ttu-id="2384e-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2384e-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "7f64924d-4cdb-4e54-8c37-c0f3d46f0747"
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