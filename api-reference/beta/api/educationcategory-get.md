---
title: 获取 educationCategory
description: 检索类别对象。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fed72875c029c2080af7f8e2133a2f2a6d94b3ba
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061782"
---
# <a name="get-educationcategory"></a><span data-ttu-id="cd673-103">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="cd673-103">Get educationCategory</span></span>

<span data-ttu-id="cd673-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd673-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd673-105">检索 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd673-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd673-106">权限</span><span class="sxs-lookup"><span data-stu-id="cd673-106">Permissions</span></span>

<span data-ttu-id="cd673-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd673-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd673-109">Permission type</span></span>                        | <span data-ttu-id="cd673-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd673-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cd673-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd673-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd673-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd673-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="cd673-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd673-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd673-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd673-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="cd673-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="cd673-115">Application\*</span></span>                           | <span data-ttu-id="cd673-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd673-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="cd673-117">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="cd673-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="cd673-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd673-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd673-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cd673-119">Optional query parameters</span></span>

<span data-ttu-id="cd673-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cd673-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd673-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd673-121">Request headers</span></span>
| <span data-ttu-id="cd673-122">标头</span><span class="sxs-lookup"><span data-stu-id="cd673-122">Header</span></span>        | <span data-ttu-id="cd673-123">值</span><span class="sxs-lookup"><span data-stu-id="cd673-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="cd673-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd673-124">Authorization</span></span> | <span data-ttu-id="cd673-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd673-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd673-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd673-127">Request body</span></span>

<span data-ttu-id="cd673-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd673-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd673-129">响应</span><span class="sxs-lookup"><span data-stu-id="cd673-129">Response</span></span>

<span data-ttu-id="cd673-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd673-130">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd673-131">示例</span><span class="sxs-lookup"><span data-stu-id="cd673-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cd673-132">请求</span><span class="sxs-lookup"><span data-stu-id="cd673-132">Request</span></span>

<span data-ttu-id="cd673-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cd673-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a><span data-ttu-id="cd673-134">响应</span><span class="sxs-lookup"><span data-stu-id="cd673-134">Response</span></span>

<span data-ttu-id="cd673-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cd673-135">The following is an example of the response.</span></span>

><span data-ttu-id="cd673-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd673-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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