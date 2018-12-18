---
title: 删除 educationSubmissionResource
description: 删除提交资源。 这仅可通过学生。 如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。
author: dipakboyed
ms.openlocfilehash: d56df6cee3884556186554d9c24ae09ed802c4f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313270"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="40704-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="40704-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="40704-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="40704-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40704-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40704-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40704-108">删除提交资源。</span><span class="sxs-lookup"><span data-stu-id="40704-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="40704-109">这仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="40704-109">This can only be done by the student.</span></span> <span data-ttu-id="40704-110">如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="40704-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="40704-111">这样，您可以"重置"资源到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="40704-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="40704-112">如果资源从工作分配不复制，但是从学生已添加，将只删除资源。</span><span class="sxs-lookup"><span data-stu-id="40704-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="40704-113">权限</span><span class="sxs-lookup"><span data-stu-id="40704-113">Permissions</span></span>
<span data-ttu-id="40704-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40704-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40704-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="40704-116">Permission type</span></span>      | <span data-ttu-id="40704-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40704-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40704-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40704-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="40704-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40704-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="40704-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40704-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="40704-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="40704-121">Not supported.</span></span>  |
|<span data-ttu-id="40704-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="40704-122">Application</span></span> | <span data-ttu-id="40704-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="40704-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="40704-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40704-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="40704-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="40704-125">Request headers</span></span>
| <span data-ttu-id="40704-126">标头</span><span class="sxs-lookup"><span data-stu-id="40704-126">Header</span></span>       | <span data-ttu-id="40704-127">值</span><span class="sxs-lookup"><span data-stu-id="40704-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40704-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="40704-128">Authorization</span></span>  | <span data-ttu-id="40704-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40704-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40704-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="40704-131">Request body</span></span>
<span data-ttu-id="40704-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40704-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="40704-133">响应</span><span class="sxs-lookup"><span data-stu-id="40704-133">Response</span></span>
<span data-ttu-id="40704-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="40704-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40704-136">示例</span><span class="sxs-lookup"><span data-stu-id="40704-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40704-137">请求</span><span class="sxs-lookup"><span data-stu-id="40704-137">Request</span></span>
<span data-ttu-id="40704-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40704-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="40704-139">响应</span><span class="sxs-lookup"><span data-stu-id="40704-139">Response</span></span>
<span data-ttu-id="40704-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40704-140">The following is an example of the response.</span></span> 

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