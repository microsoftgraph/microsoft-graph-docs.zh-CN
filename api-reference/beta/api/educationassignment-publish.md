---
title: educationAssignment： 发布
description: 此操作将工作分配的状态从其原始草稿状态更改为已发布状态中。 仅在类中的教师可以发起此呼叫。 草稿状态工作分配后，学生看不到工作分配，也不会有任何提交对象。 此 API 调用时，创建提交对象，并且学生的列表中显示的工作分配。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: bac9c38d5fbd2ce80693a468c0a2d229085f32cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508711"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="54481-106">educationAssignment： 发布</span><span class="sxs-lookup"><span data-stu-id="54481-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54481-107">此操作将工作分配的状态从其原始草稿状态更改为已发布状态中。</span><span class="sxs-lookup"><span data-stu-id="54481-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="54481-108">仅在类中的教师可以发起此呼叫。</span><span class="sxs-lookup"><span data-stu-id="54481-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="54481-109">草稿状态工作分配后，学生看不到工作分配，也不会有任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="54481-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="54481-110">此 API 调用时，创建提交对象，并且学生的列表中显示的工作分配。</span><span class="sxs-lookup"><span data-stu-id="54481-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="54481-111">权限</span><span class="sxs-lookup"><span data-stu-id="54481-111">Permissions</span></span>
<span data-ttu-id="54481-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54481-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54481-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="54481-114">Permission type</span></span>      | <span data-ttu-id="54481-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54481-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54481-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54481-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="54481-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54481-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="54481-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54481-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="54481-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="54481-119">Not supported.</span></span>  |
|<span data-ttu-id="54481-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="54481-120">Application</span></span> | <span data-ttu-id="54481-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="54481-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="54481-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54481-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="54481-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="54481-123">Request headers</span></span>
| <span data-ttu-id="54481-124">标头</span><span class="sxs-lookup"><span data-stu-id="54481-124">Header</span></span>       | <span data-ttu-id="54481-125">值</span><span class="sxs-lookup"><span data-stu-id="54481-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54481-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="54481-126">Authorization</span></span>  | <span data-ttu-id="54481-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54481-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54481-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="54481-129">Request body</span></span>
<span data-ttu-id="54481-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54481-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54481-131">响应</span><span class="sxs-lookup"><span data-stu-id="54481-131">Response</span></span>
<span data-ttu-id="54481-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="54481-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54481-134">示例</span><span class="sxs-lookup"><span data-stu-id="54481-134">Example</span></span>
<span data-ttu-id="54481-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="54481-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="54481-136">请求</span><span class="sxs-lookup"><span data-stu-id="54481-136">Request</span></span>
<span data-ttu-id="54481-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54481-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="54481-138">响应</span><span class="sxs-lookup"><span data-stu-id="54481-138">Response</span></span>
<span data-ttu-id="54481-139">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="54481-139">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
