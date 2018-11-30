---
title: educationAssignment： 发布
description: 此操作将工作分配的状态从其原始草稿状态更改为已发布状态中。 仅在类中的教师可以发起此呼叫。 草稿状态工作分配后，学生看不到工作分配，也不会有任何提交对象。 此 API 调用时，创建提交对象，并且学生的列表中显示的工作分配。
ms.openlocfilehash: d5de5a45d437662dbcd2bf869aef93502a3669f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042327"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="f868f-106">educationAssignment： 发布</span><span class="sxs-lookup"><span data-stu-id="f868f-106">educationAssignment: publish</span></span>

> <span data-ttu-id="f868f-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f868f-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f868f-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f868f-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f868f-109">此操作将工作分配的状态从其原始草稿状态更改为已发布状态中。</span><span class="sxs-lookup"><span data-stu-id="f868f-109">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="f868f-110">仅在类中的教师可以发起此呼叫。</span><span class="sxs-lookup"><span data-stu-id="f868f-110">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="f868f-111">草稿状态工作分配后，学生看不到工作分配，也不会有任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="f868f-111">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="f868f-112">此 API 调用时，创建提交对象，并且学生的列表中显示的工作分配。</span><span class="sxs-lookup"><span data-stu-id="f868f-112">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="f868f-113">权限</span><span class="sxs-lookup"><span data-stu-id="f868f-113">Permissions</span></span>
<span data-ttu-id="f868f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f868f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f868f-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="f868f-116">Permission type</span></span>      | <span data-ttu-id="f868f-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f868f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f868f-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f868f-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="f868f-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f868f-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f868f-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f868f-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f868f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="f868f-121">Not supported.</span></span>  |
|<span data-ttu-id="f868f-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="f868f-122">Application</span></span> | <span data-ttu-id="f868f-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="f868f-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f868f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f868f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="f868f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="f868f-125">Request headers</span></span>
| <span data-ttu-id="f868f-126">标头</span><span class="sxs-lookup"><span data-stu-id="f868f-126">Header</span></span>       | <span data-ttu-id="f868f-127">值</span><span class="sxs-lookup"><span data-stu-id="f868f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f868f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f868f-128">Authorization</span></span>  | <span data-ttu-id="f868f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f868f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f868f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f868f-131">Request body</span></span>
<span data-ttu-id="f868f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f868f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f868f-133">响应</span><span class="sxs-lookup"><span data-stu-id="f868f-133">Response</span></span>
<span data-ttu-id="f868f-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f868f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f868f-136">示例</span><span class="sxs-lookup"><span data-stu-id="f868f-136">Example</span></span>
<span data-ttu-id="f868f-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f868f-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f868f-138">请求</span><span class="sxs-lookup"><span data-stu-id="f868f-138">Request</span></span>
<span data-ttu-id="f868f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f868f-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="f868f-140">响应</span><span class="sxs-lookup"><span data-stu-id="f868f-140">Response</span></span>
<span data-ttu-id="f868f-141">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="f868f-141">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
