---
title: 'educationSubmission: unsubmit'
description: '指示学生希望后没有打开从事的工作分配的提交操作。 仅可由学生执行此操作。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e8ce4c5d4bf68dca22f686a1b3647c67d7836bed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513506"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="79776-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="79776-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79776-105">指示学生希望后没有打开从事的工作分配的提交操作。</span><span class="sxs-lookup"><span data-stu-id="79776-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="79776-106">仅可由学生执行此操作。</span><span class="sxs-lookup"><span data-stu-id="79776-106">This action can only be taken by the student.</span></span> <span data-ttu-id="79776-107">这将提交的状态从"提交"变为"工作"。</span><span class="sxs-lookup"><span data-stu-id="79776-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="79776-108">在提交过程中，所有资源将都复制从 submittedResources 到 workingResources 地址散列表元。</span><span class="sxs-lookup"><span data-stu-id="79776-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="79776-109">教师将看的分级工作资源列表。</span><span class="sxs-lookup"><span data-stu-id="79776-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="79776-110">权限</span><span class="sxs-lookup"><span data-stu-id="79776-110">Permissions</span></span>
<span data-ttu-id="79776-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79776-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79776-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="79776-113">Permission type</span></span>      | <span data-ttu-id="79776-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79776-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79776-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79776-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="79776-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79776-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="79776-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79776-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="79776-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="79776-118">Not supported.</span></span>  |
|<span data-ttu-id="79776-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="79776-119">Application</span></span> | <span data-ttu-id="79776-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="79776-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="79776-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79776-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="79776-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="79776-122">Request headers</span></span>
| <span data-ttu-id="79776-123">标头</span><span class="sxs-lookup"><span data-stu-id="79776-123">Header</span></span>       | <span data-ttu-id="79776-124">值</span><span class="sxs-lookup"><span data-stu-id="79776-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79776-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79776-125">Authorization</span></span>  | <span data-ttu-id="79776-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79776-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79776-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="79776-128">Request body</span></span>
<span data-ttu-id="79776-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79776-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79776-130">响应</span><span class="sxs-lookup"><span data-stu-id="79776-130">Response</span></span>
<span data-ttu-id="79776-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="79776-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79776-133">示例</span><span class="sxs-lookup"><span data-stu-id="79776-133">Example</span></span>
<span data-ttu-id="79776-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="79776-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79776-135">请求</span><span class="sxs-lookup"><span data-stu-id="79776-135">Request</span></span>
<span data-ttu-id="79776-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79776-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="79776-137">响应</span><span class="sxs-lookup"><span data-stu-id="79776-137">Response</span></span>
<span data-ttu-id="79776-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79776-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
