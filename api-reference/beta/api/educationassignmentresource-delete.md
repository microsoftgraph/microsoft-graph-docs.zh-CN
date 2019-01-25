---
title: 删除 educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0a6ac6f4cddde9d80e48080b0f54b2610e84782c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513037"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="30248-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="30248-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30248-104">删除资源，从一个工作分配。</span><span class="sxs-lookup"><span data-stu-id="30248-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="30248-105">仅在类中的教师可以删除的资源。</span><span class="sxs-lookup"><span data-stu-id="30248-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="30248-106">工作分配已发布到学生后，教师不能删除标记为"distributeToStudents"的资源。</span><span class="sxs-lookup"><span data-stu-id="30248-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="30248-107">权限</span><span class="sxs-lookup"><span data-stu-id="30248-107">Permissions</span></span>
<span data-ttu-id="30248-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30248-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30248-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="30248-110">Permission type</span></span>      | <span data-ttu-id="30248-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30248-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30248-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30248-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="30248-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30248-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="30248-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30248-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="30248-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="30248-115">Not supported.</span></span>  |
|<span data-ttu-id="30248-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="30248-116">Application</span></span> | <span data-ttu-id="30248-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="30248-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="30248-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30248-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="30248-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="30248-119">Request headers</span></span>
| <span data-ttu-id="30248-120">标头</span><span class="sxs-lookup"><span data-stu-id="30248-120">Header</span></span>       | <span data-ttu-id="30248-121">值</span><span class="sxs-lookup"><span data-stu-id="30248-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30248-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30248-122">Authorization</span></span>  | <span data-ttu-id="30248-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30248-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30248-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="30248-125">Request body</span></span>
<span data-ttu-id="30248-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30248-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="30248-127">响应</span><span class="sxs-lookup"><span data-stu-id="30248-127">Response</span></span>
<span data-ttu-id="30248-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="30248-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30248-130">示例</span><span class="sxs-lookup"><span data-stu-id="30248-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30248-131">请求</span><span class="sxs-lookup"><span data-stu-id="30248-131">Request</span></span>
<span data-ttu-id="30248-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30248-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="30248-133">响应</span><span class="sxs-lookup"><span data-stu-id="30248-133">Response</span></span>
<span data-ttu-id="30248-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30248-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
