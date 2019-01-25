---
title: 删除 educationSubmissionResource
description: 删除提交资源。 这仅可通过学生。 如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a735cb1451e8d3eb8df13e6fa395c3e02393f451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518980"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="e0e86-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="e0e86-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e86-106">删除提交资源。</span><span class="sxs-lookup"><span data-stu-id="e0e86-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="e0e86-107">这仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="e0e86-107">This can only be done by the student.</span></span> <span data-ttu-id="e0e86-108">如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="e0e86-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="e0e86-109">这样，您可以"重置"资源到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="e0e86-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="e0e86-110">如果资源从工作分配不复制，但是从学生已添加，将只删除资源。</span><span class="sxs-lookup"><span data-stu-id="e0e86-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e86-111">权限</span><span class="sxs-lookup"><span data-stu-id="e0e86-111">Permissions</span></span>
<span data-ttu-id="e0e86-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0e86-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e86-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0e86-114">Permission type</span></span>      | <span data-ttu-id="e0e86-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0e86-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0e86-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0e86-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0e86-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0e86-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e0e86-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0e86-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0e86-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0e86-119">Not supported.</span></span>  |
|<span data-ttu-id="e0e86-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0e86-120">Application</span></span> | <span data-ttu-id="e0e86-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0e86-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e0e86-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0e86-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e0e86-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0e86-123">Request headers</span></span>
| <span data-ttu-id="e0e86-124">标头</span><span class="sxs-lookup"><span data-stu-id="e0e86-124">Header</span></span>       | <span data-ttu-id="e0e86-125">值</span><span class="sxs-lookup"><span data-stu-id="e0e86-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0e86-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0e86-126">Authorization</span></span>  | <span data-ttu-id="e0e86-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0e86-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0e86-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0e86-129">Request body</span></span>
<span data-ttu-id="e0e86-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0e86-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e0e86-131">响应</span><span class="sxs-lookup"><span data-stu-id="e0e86-131">Response</span></span>
<span data-ttu-id="e0e86-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0e86-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0e86-134">示例</span><span class="sxs-lookup"><span data-stu-id="e0e86-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0e86-135">请求</span><span class="sxs-lookup"><span data-stu-id="e0e86-135">Request</span></span>
<span data-ttu-id="e0e86-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0e86-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="e0e86-137">响应</span><span class="sxs-lookup"><span data-stu-id="e0e86-137">Response</span></span>
<span data-ttu-id="e0e86-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0e86-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
