---
title: 删除 educationCategory
description: 从此 educationAssignment 中删除现有 educationCategory
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: edf054ba1d7b81800a75e260c5a2357ae2d9bcba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044184"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="e93b1-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="e93b1-103">Remove educationCategory</span></span>

<span data-ttu-id="e93b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e93b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e93b1-105">从[educationAssignment](../resources/educationcategory.md)中删除[educationCategory。](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e93b1-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e93b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="e93b1-106">Permissions</span></span>
<span data-ttu-id="e93b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e93b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e93b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e93b1-109">Permission type</span></span>      | <span data-ttu-id="e93b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e93b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e93b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e93b1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e93b1-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e93b1-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e93b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e93b1-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e93b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e93b1-114">Not supported.</span></span>  |
|<span data-ttu-id="e93b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e93b1-115">Application</span></span> | <span data-ttu-id="e93b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e93b1-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e93b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e93b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e93b1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e93b1-118">Request headers</span></span>
| <span data-ttu-id="e93b1-119">标头</span><span class="sxs-lookup"><span data-stu-id="e93b1-119">Header</span></span>       | <span data-ttu-id="e93b1-120">值</span><span class="sxs-lookup"><span data-stu-id="e93b1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e93b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e93b1-121">Authorization</span></span>  | <span data-ttu-id="e93b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e93b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e93b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e93b1-124">Content-Type</span></span>  | <span data-ttu-id="e93b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e93b1-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e93b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e93b1-126">Request body</span></span>
<span data-ttu-id="e93b1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e93b1-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e93b1-128">响应</span><span class="sxs-lookup"><span data-stu-id="e93b1-128">Response</span></span>
<span data-ttu-id="e93b1-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e93b1-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e93b1-130">示例</span><span class="sxs-lookup"><span data-stu-id="e93b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e93b1-131">请求</span><span class="sxs-lookup"><span data-stu-id="e93b1-131">Request</span></span>
<span data-ttu-id="e93b1-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e93b1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="e93b1-133">响应</span><span class="sxs-lookup"><span data-stu-id="e93b1-133">Response</span></span>
<span data-ttu-id="e93b1-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e93b1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="e93b1-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e93b1-135">**Note:** The response object shown here might be shortened for readability.</span></span>


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


