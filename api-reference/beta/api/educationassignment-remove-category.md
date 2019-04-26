---
title: 删除 educationCategory
description: 从此 educationAssignment 中删除现有 educationCategory
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 9c92ab53cd62a7ed32aff6300386e2e76699275e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324740"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="a239c-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="a239c-103">Remove educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a239c-104">从[educationAssignment](../resources/educationassignment.md)中删除[educationCategory](../resources/educationcategory.md) 。</span><span class="sxs-lookup"><span data-stu-id="a239c-104">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a239c-105">权限</span><span class="sxs-lookup"><span data-stu-id="a239c-105">Permissions</span></span>
<span data-ttu-id="a239c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a239c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a239c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a239c-108">Permission type</span></span>      | <span data-ttu-id="a239c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a239c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a239c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a239c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a239c-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="a239c-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a239c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a239c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a239c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a239c-113">Not supported.</span></span>  |
|<span data-ttu-id="a239c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a239c-114">Application</span></span> | <span data-ttu-id="a239c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a239c-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="a239c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a239c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a239c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a239c-117">Request headers</span></span>
| <span data-ttu-id="a239c-118">标头</span><span class="sxs-lookup"><span data-stu-id="a239c-118">Header</span></span>       | <span data-ttu-id="a239c-119">值</span><span class="sxs-lookup"><span data-stu-id="a239c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a239c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a239c-120">Authorization</span></span>  | <span data-ttu-id="a239c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a239c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a239c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a239c-123">Content-Type</span></span>  | <span data-ttu-id="a239c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a239c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a239c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a239c-125">Request body</span></span>
<span data-ttu-id="a239c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a239c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a239c-127">响应</span><span class="sxs-lookup"><span data-stu-id="a239c-127">Response</span></span>
<span data-ttu-id="a239c-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a239c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a239c-129">示例</span><span class="sxs-lookup"><span data-stu-id="a239c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a239c-130">请求</span><span class="sxs-lookup"><span data-stu-id="a239c-130">Request</span></span>
<span data-ttu-id="a239c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a239c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="a239c-132">响应</span><span class="sxs-lookup"><span data-stu-id="a239c-132">Response</span></span>
<span data-ttu-id="a239c-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a239c-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a239c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a239c-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a239c-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a239c-135">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
