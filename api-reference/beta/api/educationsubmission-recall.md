---
title: educationSubmission： 记忆功能
description: '指示学生想要收回提交。 此操作仅可通过学生。 '
author: dipakboyed
ms.openlocfilehash: ad49302ac9010923d0da2e31686ae4f6967bb50b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302315"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="ea867-104">educationSubmission： 记忆功能</span><span class="sxs-lookup"><span data-stu-id="ea867-104">educationSubmission: recall</span></span>

> <span data-ttu-id="ea867-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea867-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea867-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea867-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea867-107">指示学生想要收回提交。</span><span class="sxs-lookup"><span data-stu-id="ea867-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="ea867-108">此操作仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="ea867-108">This action can only be done by a student.</span></span> <span data-ttu-id="ea867-109">返回到"工作"，它将从"提交"更改提交的状态。</span><span class="sxs-lookup"><span data-stu-id="ea867-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="ea867-110">权限</span><span class="sxs-lookup"><span data-stu-id="ea867-110">Permissions</span></span>
<span data-ttu-id="ea867-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea867-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea867-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea867-113">Permission type</span></span>      | <span data-ttu-id="ea867-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea867-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea867-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea867-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ea867-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea867-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ea867-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea867-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ea867-118">不支持</span><span class="sxs-lookup"><span data-stu-id="ea867-118">Not supported</span></span>  |
|<span data-ttu-id="ea867-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea867-119">Application</span></span> |<span data-ttu-id="ea867-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea867-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ea867-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea867-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="ea867-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea867-122">Request headers</span></span>
| <span data-ttu-id="ea867-123">标头</span><span class="sxs-lookup"><span data-stu-id="ea867-123">Header</span></span>       | <span data-ttu-id="ea867-124">值</span><span class="sxs-lookup"><span data-stu-id="ea867-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea867-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea867-125">Authorization</span></span>  | <span data-ttu-id="ea867-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea867-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea867-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea867-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ea867-129">响应</span><span class="sxs-lookup"><span data-stu-id="ea867-129">Response</span></span>
<span data-ttu-id="ea867-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ea867-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea867-132">示例</span><span class="sxs-lookup"><span data-stu-id="ea867-132">Example</span></span>
<span data-ttu-id="ea867-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ea867-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea867-134">请求</span><span class="sxs-lookup"><span data-stu-id="ea867-134">Request</span></span>
<span data-ttu-id="ea867-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea867-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="ea867-136">响应</span><span class="sxs-lookup"><span data-stu-id="ea867-136">Response</span></span>
<span data-ttu-id="ea867-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea867-137">The following is an example of the response.</span></span>

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