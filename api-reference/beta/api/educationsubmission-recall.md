---
title: educationSubmission： 记忆功能
description: .
ms.openlocfilehash: 8df134a6d8325e5b497baada89bc0fa16d0ee9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042325"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="c6670-103">educationSubmission： 记忆功能</span><span class="sxs-lookup"><span data-stu-id="c6670-103">educationSubmission: recall</span></span>

> <span data-ttu-id="c6670-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6670-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6670-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6670-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6670-106">指示学生想要收回提交。</span><span class="sxs-lookup"><span data-stu-id="c6670-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="c6670-107">此操作仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="c6670-107">This action can only be done by a student.</span></span> <span data-ttu-id="c6670-108">返回到"工作"，它将从"提交"更改提交的状态。</span><span class="sxs-lookup"><span data-stu-id="c6670-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="c6670-109">权限</span><span class="sxs-lookup"><span data-stu-id="c6670-109">Permissions</span></span>
<span data-ttu-id="c6670-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6670-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6670-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6670-112">Permission type</span></span>      | <span data-ttu-id="c6670-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6670-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6670-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6670-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6670-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6670-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c6670-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6670-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6670-117">不支持</span><span class="sxs-lookup"><span data-stu-id="c6670-117">Not supported</span></span>  |
|<span data-ttu-id="c6670-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6670-118">Application</span></span> |<span data-ttu-id="c6670-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6670-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c6670-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6670-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="c6670-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6670-121">Request headers</span></span>
| <span data-ttu-id="c6670-122">标头</span><span class="sxs-lookup"><span data-stu-id="c6670-122">Header</span></span>       | <span data-ttu-id="c6670-123">值</span><span class="sxs-lookup"><span data-stu-id="c6670-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6670-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6670-124">Authorization</span></span>  | <span data-ttu-id="c6670-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6670-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6670-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6670-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c6670-128">响应</span><span class="sxs-lookup"><span data-stu-id="c6670-128">Response</span></span>
<span data-ttu-id="c6670-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c6670-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6670-131">示例</span><span class="sxs-lookup"><span data-stu-id="c6670-131">Example</span></span>
<span data-ttu-id="c6670-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c6670-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6670-133">请求</span><span class="sxs-lookup"><span data-stu-id="c6670-133">Request</span></span>
<span data-ttu-id="c6670-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6670-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="c6670-135">响应</span><span class="sxs-lookup"><span data-stu-id="c6670-135">Response</span></span>
<span data-ttu-id="c6670-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6670-136">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->