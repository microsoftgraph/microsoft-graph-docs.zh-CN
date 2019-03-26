---
title: 添加 educationCategories
description: 将现有 educationCategory 添加到此 educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d5fbf5d6db4ade6e44f65c256879c535d2e2a0e2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800963"
---
# <a name="add-educationcategories"></a><span data-ttu-id="0c3e7-103">添加 educationCategories</span><span class="sxs-lookup"><span data-stu-id="0c3e7-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c3e7-104">将一个或多个现有[educationCategory](../resources/educationcategory.md)对象添加到此[educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c3e7-105">权限</span><span class="sxs-lookup"><span data-stu-id="0c3e7-105">Permissions</span></span>
<span data-ttu-id="0c3e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3e7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c3e7-108">Permission type</span></span>      | <span data-ttu-id="0c3e7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c3e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c3e7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3e7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c3e7-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0c3e7-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0c3e7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3e7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c3e7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-113">Not supported.</span></span>  |
|<span data-ttu-id="0c3e7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c3e7-114">Application</span></span> | <span data-ttu-id="0c3e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0c3e7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c3e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0c3e7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c3e7-117">Request headers</span></span>
| <span data-ttu-id="0c3e7-118">标头</span><span class="sxs-lookup"><span data-stu-id="0c3e7-118">Header</span></span>       | <span data-ttu-id="0c3e7-119">值</span><span class="sxs-lookup"><span data-stu-id="0c3e7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c3e7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c3e7-120">Authorization</span></span>  | <span data-ttu-id="0c3e7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c3e7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c3e7-123">Content-Type</span></span>  | <span data-ttu-id="0c3e7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0c3e7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c3e7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c3e7-125">Request body</span></span>
<span data-ttu-id="0c3e7-126">在请求正文中, 提供要添加到此工作分配的现有[educationCategory](../resources/educationcategory.md)对象的 odata.id。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="0c3e7-127">响应</span><span class="sxs-lookup"><span data-stu-id="0c3e7-127">Response</span></span>
<span data-ttu-id="0c3e7-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c3e7-129">示例</span><span class="sxs-lookup"><span data-stu-id="0c3e7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c3e7-130">请求</span><span class="sxs-lookup"><span data-stu-id="0c3e7-130">Request</span></span>
<span data-ttu-id="0c3e7-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="0c3e7-132">在请求正文中, 提供要添加到此工作分配的现有[educationCategory](../resources/educationcategory.md)对象的 odata.id。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="0c3e7-133">响应</span><span class="sxs-lookup"><span data-stu-id="0c3e7-133">Response</span></span>
<span data-ttu-id="0c3e7-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-134">The following is an example of the response.</span></span> 

><span data-ttu-id="0c3e7-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c3e7-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c3e7-136">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-add-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
