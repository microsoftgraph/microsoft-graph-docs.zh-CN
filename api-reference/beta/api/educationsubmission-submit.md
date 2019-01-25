---
title: educationSubmission： 提交
description: 指示学生完成的工作，并且已准备好分配中分发操作。 仅可由学生执行此操作。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f67e5b07ed1093ee63e9b6fdf7647fa6891dacc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510769"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="981c9-104">educationSubmission： 提交</span><span class="sxs-lookup"><span data-stu-id="981c9-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="981c9-105">指示学生完成的工作，并且已准备好分配中分发操作。</span><span class="sxs-lookup"><span data-stu-id="981c9-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="981c9-106">仅可由学生执行此操作。</span><span class="sxs-lookup"><span data-stu-id="981c9-106">This action can only be taken by the student.</span></span> <span data-ttu-id="981c9-107">这将更改从"工作"到"提交"提交的状态。</span><span class="sxs-lookup"><span data-stu-id="981c9-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="981c9-108">在提交过程中，所有资源将都复制到 submittedResources 地址散列表元中。</span><span class="sxs-lookup"><span data-stu-id="981c9-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="981c9-109">教师将看评分的提交的资源列表。</span><span class="sxs-lookup"><span data-stu-id="981c9-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="981c9-110">权限</span><span class="sxs-lookup"><span data-stu-id="981c9-110">Permissions</span></span>
<span data-ttu-id="981c9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="981c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="981c9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="981c9-113">Permission type</span></span>      | <span data-ttu-id="981c9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="981c9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="981c9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="981c9-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="981c9-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="981c9-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="981c9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="981c9-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="981c9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="981c9-118">Not supported.</span></span>  |
|<span data-ttu-id="981c9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="981c9-119">Application</span></span> | <span data-ttu-id="981c9-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="981c9-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="981c9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="981c9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="981c9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="981c9-122">Request headers</span></span>
| <span data-ttu-id="981c9-123">标头</span><span class="sxs-lookup"><span data-stu-id="981c9-123">Header</span></span>       | <span data-ttu-id="981c9-124">值</span><span class="sxs-lookup"><span data-stu-id="981c9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="981c9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="981c9-125">Authorization</span></span>  | <span data-ttu-id="981c9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="981c9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="981c9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="981c9-128">Request body</span></span>
<span data-ttu-id="981c9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="981c9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="981c9-130">响应</span><span class="sxs-lookup"><span data-stu-id="981c9-130">Response</span></span>
<span data-ttu-id="981c9-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="981c9-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="981c9-133">示例</span><span class="sxs-lookup"><span data-stu-id="981c9-133">Example</span></span>
<span data-ttu-id="981c9-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="981c9-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="981c9-135">请求</span><span class="sxs-lookup"><span data-stu-id="981c9-135">Request</span></span>
<span data-ttu-id="981c9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="981c9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="981c9-137">响应</span><span class="sxs-lookup"><span data-stu-id="981c9-137">Response</span></span>
<span data-ttu-id="981c9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="981c9-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
