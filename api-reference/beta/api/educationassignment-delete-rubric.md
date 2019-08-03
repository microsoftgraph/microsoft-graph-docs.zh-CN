---
title: 从 educationAssignment 中删除 educationRubric
description: 从 educationAssignment 中删除 educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6334e24c01db8f32f643f552b1a64cb2c86967d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173221"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="115f3-103">从 educationAssignment 中删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="115f3-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="115f3-104">从[educationAssignment](../resources/educationassignment.md)中删除[educationRubric](../resources/educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="115f3-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="115f3-105">这不会删除 rubric 本身。</span><span class="sxs-lookup"><span data-stu-id="115f3-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="115f3-106">权限</span><span class="sxs-lookup"><span data-stu-id="115f3-106">Permissions</span></span>

<span data-ttu-id="115f3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="115f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="115f3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="115f3-109">Permission type</span></span>                        | <span data-ttu-id="115f3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="115f3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="115f3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="115f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="115f3-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="115f3-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="115f3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="115f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="115f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="115f3-114">Not supported.</span></span> |
| <span data-ttu-id="115f3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="115f3-115">Application</span></span>                            | <span data-ttu-id="115f3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="115f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="115f3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="115f3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="115f3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="115f3-118">Request headers</span></span>

| <span data-ttu-id="115f3-119">名称</span><span class="sxs-lookup"><span data-stu-id="115f3-119">Name</span></span>          | <span data-ttu-id="115f3-120">说明</span><span class="sxs-lookup"><span data-stu-id="115f3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="115f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="115f3-121">Authorization</span></span> | <span data-ttu-id="115f3-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="115f3-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="115f3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="115f3-123">Request body</span></span>

<span data-ttu-id="115f3-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="115f3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="115f3-125">响应</span><span class="sxs-lookup"><span data-stu-id="115f3-125">Response</span></span>

<span data-ttu-id="115f3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="115f3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="115f3-128">示例</span><span class="sxs-lookup"><span data-stu-id="115f3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="115f3-129">请求</span><span class="sxs-lookup"><span data-stu-id="115f3-129">Request</span></span>

<span data-ttu-id="115f3-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="115f3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="115f3-131">响应</span><span class="sxs-lookup"><span data-stu-id="115f3-131">Response</span></span>

<span data-ttu-id="115f3-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="115f3-132">The following is an example of the response.</span></span>

> <span data-ttu-id="115f3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="115f3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
