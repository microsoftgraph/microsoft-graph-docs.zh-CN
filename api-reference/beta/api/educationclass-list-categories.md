---
title: 列出 educationCategories
description: 检索类别对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b4f821313796382b2bb7c9d5620dee96f463b227
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061789"
---
# <a name="list-educationcategories"></a><span data-ttu-id="6efa3-103">列出 educationCategories</span><span class="sxs-lookup"><span data-stu-id="6efa3-103">List educationCategories</span></span>

<span data-ttu-id="6efa3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6efa3-105">检索 [educationCategory 对象](../resources/educationcategory.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="6efa3-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6efa3-106">权限</span><span class="sxs-lookup"><span data-stu-id="6efa3-106">Permissions</span></span>

<span data-ttu-id="6efa3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6efa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6efa3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6efa3-109">Permission type</span></span>                        | <span data-ttu-id="6efa3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6efa3-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6efa3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6efa3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6efa3-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6efa3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="6efa3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6efa3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efa3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6efa3-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="6efa3-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="6efa3-115">Application\*</span></span>                           | <span data-ttu-id="6efa3-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6efa3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="6efa3-117">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="6efa3-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="6efa3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6efa3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6efa3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6efa3-119">Optional query parameters</span></span>

<span data-ttu-id="6efa3-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6efa3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6efa3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6efa3-121">Request headers</span></span>

| <span data-ttu-id="6efa3-122">标头</span><span class="sxs-lookup"><span data-stu-id="6efa3-122">Header</span></span>        | <span data-ttu-id="6efa3-123">值</span><span class="sxs-lookup"><span data-stu-id="6efa3-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6efa3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efa3-124">Authorization</span></span> | <span data-ttu-id="6efa3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6efa3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6efa3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6efa3-127">Request body</span></span>

<span data-ttu-id="6efa3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6efa3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6efa3-129">响应</span><span class="sxs-lookup"><span data-stu-id="6efa3-129">Response</span></span>

<span data-ttu-id="6efa3-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationCategory](../resources/educationcategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6efa3-130">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6efa3-131">示例</span><span class="sxs-lookup"><span data-stu-id="6efa3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6efa3-132">请求</span><span class="sxs-lookup"><span data-stu-id="6efa3-132">Request</span></span>

<span data-ttu-id="6efa3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6efa3-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="6efa3-134">响应</span><span class="sxs-lookup"><span data-stu-id="6efa3-134">Response</span></span>

<span data-ttu-id="6efa3-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6efa3-135">The following is an example of the response.</span></span> 

><span data-ttu-id="6efa3-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6efa3-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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