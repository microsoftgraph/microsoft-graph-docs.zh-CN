---
title: 删除 educationCategory
description: 从此 educationAssignment 中删除现有 educationCategory
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: edcc71fcacf96dacdd9200e48f2ddedbbcda381e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002532"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="ff360-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="ff360-103">Remove educationCategory</span></span>

<span data-ttu-id="ff360-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff360-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff360-105">从[educationAssignment](../resources/educationassignment.md)中删除[educationCategory](../resources/educationcategory.md) 。</span><span class="sxs-lookup"><span data-stu-id="ff360-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff360-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff360-106">Permissions</span></span>
<span data-ttu-id="ff360-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff360-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff360-109">Permission type</span></span>      | <span data-ttu-id="ff360-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff360-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff360-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff360-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff360-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="ff360-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ff360-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff360-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ff360-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff360-114">Not supported.</span></span>  |
|<span data-ttu-id="ff360-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff360-115">Application</span></span> | <span data-ttu-id="ff360-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff360-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ff360-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff360-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ff360-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff360-118">Request headers</span></span>
| <span data-ttu-id="ff360-119">标头</span><span class="sxs-lookup"><span data-stu-id="ff360-119">Header</span></span>       | <span data-ttu-id="ff360-120">值</span><span class="sxs-lookup"><span data-stu-id="ff360-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff360-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff360-121">Authorization</span></span>  | <span data-ttu-id="ff360-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff360-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff360-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff360-124">Content-Type</span></span>  | <span data-ttu-id="ff360-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff360-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff360-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff360-126">Request body</span></span>
<span data-ttu-id="ff360-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff360-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ff360-128">响应</span><span class="sxs-lookup"><span data-stu-id="ff360-128">Response</span></span>
<span data-ttu-id="ff360-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ff360-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff360-130">示例</span><span class="sxs-lookup"><span data-stu-id="ff360-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff360-131">请求</span><span class="sxs-lookup"><span data-stu-id="ff360-131">Request</span></span>
<span data-ttu-id="ff360-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff360-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="ff360-133">响应</span><span class="sxs-lookup"><span data-stu-id="ff360-133">Response</span></span>
<span data-ttu-id="ff360-134">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="ff360-134">The following is an example of the response.</span></span> 

><span data-ttu-id="ff360-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ff360-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff360-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff360-136">All of the properties will be returned from an actual call.</span></span>


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


