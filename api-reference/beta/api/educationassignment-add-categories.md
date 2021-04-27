---
title: 添加 educationCategories
description: 将现有 educationCategory 添加到此 educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c94ffa2f11ae8fd77380fa164affdded4cfb3b2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044408"
---
# <a name="add-educationcategories"></a><span data-ttu-id="f1b25-103">添加 educationCategories</span><span class="sxs-lookup"><span data-stu-id="f1b25-103">Add educationCategories</span></span>

<span data-ttu-id="f1b25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b25-105">将一个或多个现有的 [educationCategory](../resources/educationcategory.md) 对象添加到 [此 educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f1b25-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1b25-106">权限</span><span class="sxs-lookup"><span data-stu-id="f1b25-106">Permissions</span></span>
<span data-ttu-id="f1b25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1b25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b25-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1b25-109">Permission type</span></span>      | <span data-ttu-id="f1b25-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1b25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1b25-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b25-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1b25-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1b25-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f1b25-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b25-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1b25-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1b25-114">Not supported.</span></span>  |
|<span data-ttu-id="f1b25-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1b25-115">Application</span></span> | <span data-ttu-id="f1b25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1b25-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f1b25-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1b25-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f1b25-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1b25-118">Request headers</span></span>
| <span data-ttu-id="f1b25-119">标头</span><span class="sxs-lookup"><span data-stu-id="f1b25-119">Header</span></span>       | <span data-ttu-id="f1b25-120">值</span><span class="sxs-lookup"><span data-stu-id="f1b25-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1b25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b25-121">Authorization</span></span>  | <span data-ttu-id="f1b25-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1b25-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1b25-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1b25-124">Content-Type</span></span>  | <span data-ttu-id="f1b25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b25-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1b25-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1b25-126">Request body</span></span>
<span data-ttu-id="f1b25-127">在请求正文中，odata.id 现有 [educationCategory](../resources/educationcategory.md) () 添加到此分配。</span><span class="sxs-lookup"><span data-stu-id="f1b25-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="f1b25-128">响应</span><span class="sxs-lookup"><span data-stu-id="f1b25-128">Response</span></span>
<span data-ttu-id="f1b25-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f1b25-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1b25-130">示例</span><span class="sxs-lookup"><span data-stu-id="f1b25-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1b25-131">请求</span><span class="sxs-lookup"><span data-stu-id="f1b25-131">Request</span></span>
<span data-ttu-id="f1b25-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f1b25-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="f1b25-133">在请求正文中，odata.id 要添加到此分配的现有 [educationCategory](../resources/educationcategory.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="f1b25-133">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="f1b25-134">响应</span><span class="sxs-lookup"><span data-stu-id="f1b25-134">Response</span></span>
<span data-ttu-id="f1b25-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f1b25-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f1b25-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f1b25-136">**Note:** The response object shown here might be shortened for readability.</span></span>


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
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


