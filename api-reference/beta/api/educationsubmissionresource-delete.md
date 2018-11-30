---
title: 删除 educationSubmissionResource
description: " 资源到其原始状态。 如果资源从工作分配不复制，但是从学生已添加，将只删除资源。"
ms.openlocfilehash: 9eb5b08e2e5481e707cc6c1e0b0f8339e3d22ad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046429"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="d2e0b-104">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d2e0b-104">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="d2e0b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2e0b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2e0b-107">删除提交资源。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="d2e0b-108">这仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-108">This can only be done by the student.</span></span> <span data-ttu-id="d2e0b-109">如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="d2e0b-110">这样，您可以"重置"资源到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="d2e0b-111">如果资源从工作分配不复制，但是从学生已添加，将只删除资源。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e0b-112">权限</span><span class="sxs-lookup"><span data-stu-id="d2e0b-112">Permissions</span></span>
<span data-ttu-id="d2e0b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e0b-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2e0b-115">Permission type</span></span>      | <span data-ttu-id="d2e0b-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2e0b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2e0b-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e0b-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2e0b-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2e0b-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d2e0b-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e0b-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2e0b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-120">Not supported.</span></span>  |
|<span data-ttu-id="d2e0b-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2e0b-121">Application</span></span> | <span data-ttu-id="d2e0b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2e0b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2e0b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d2e0b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2e0b-124">Request headers</span></span>
| <span data-ttu-id="d2e0b-125">标头</span><span class="sxs-lookup"><span data-stu-id="d2e0b-125">Header</span></span>       | <span data-ttu-id="d2e0b-126">值</span><span class="sxs-lookup"><span data-stu-id="d2e0b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2e0b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2e0b-127">Authorization</span></span>  | <span data-ttu-id="d2e0b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2e0b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2e0b-130">Request body</span></span>
<span data-ttu-id="d2e0b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d2e0b-132">响应</span><span class="sxs-lookup"><span data-stu-id="d2e0b-132">Response</span></span>
<span data-ttu-id="d2e0b-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e0b-135">示例</span><span class="sxs-lookup"><span data-stu-id="d2e0b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2e0b-136">请求</span><span class="sxs-lookup"><span data-stu-id="d2e0b-136">Request</span></span>
<span data-ttu-id="d2e0b-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="d2e0b-138">响应</span><span class="sxs-lookup"><span data-stu-id="d2e0b-138">Response</span></span>
<span data-ttu-id="d2e0b-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2e0b-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->