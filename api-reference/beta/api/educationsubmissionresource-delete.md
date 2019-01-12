---
title: 删除 educationSubmissionResource
description: 删除提交资源。 这仅可通过学生。 如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 657e05a5a60dd90c8fd0c769b7d978c4be617201
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945725"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="47aeb-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="47aeb-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="47aeb-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47aeb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47aeb-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47aeb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47aeb-108">删除提交资源。</span><span class="sxs-lookup"><span data-stu-id="47aeb-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="47aeb-109">这仅可通过学生。</span><span class="sxs-lookup"><span data-stu-id="47aeb-109">This can only be done by the student.</span></span> <span data-ttu-id="47aeb-110">如果工作分配从复制资源，删除当前副本后，将创建的资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="47aeb-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="47aeb-111">这样，您可以"重置"资源到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="47aeb-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="47aeb-112">如果资源从工作分配不复制，但是从学生已添加，将只删除资源。</span><span class="sxs-lookup"><span data-stu-id="47aeb-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="47aeb-113">权限</span><span class="sxs-lookup"><span data-stu-id="47aeb-113">Permissions</span></span>
<span data-ttu-id="47aeb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47aeb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47aeb-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="47aeb-116">Permission type</span></span>      | <span data-ttu-id="47aeb-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47aeb-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47aeb-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47aeb-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="47aeb-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47aeb-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="47aeb-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47aeb-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47aeb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="47aeb-121">Not supported.</span></span>  |
|<span data-ttu-id="47aeb-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="47aeb-122">Application</span></span> | <span data-ttu-id="47aeb-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="47aeb-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47aeb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47aeb-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="47aeb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="47aeb-125">Request headers</span></span>
| <span data-ttu-id="47aeb-126">标头</span><span class="sxs-lookup"><span data-stu-id="47aeb-126">Header</span></span>       | <span data-ttu-id="47aeb-127">值</span><span class="sxs-lookup"><span data-stu-id="47aeb-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47aeb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="47aeb-128">Authorization</span></span>  | <span data-ttu-id="47aeb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47aeb-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47aeb-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="47aeb-131">Request body</span></span>
<span data-ttu-id="47aeb-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47aeb-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="47aeb-133">响应</span><span class="sxs-lookup"><span data-stu-id="47aeb-133">Response</span></span>
<span data-ttu-id="47aeb-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="47aeb-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47aeb-136">示例</span><span class="sxs-lookup"><span data-stu-id="47aeb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47aeb-137">请求</span><span class="sxs-lookup"><span data-stu-id="47aeb-137">Request</span></span>
<span data-ttu-id="47aeb-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47aeb-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="47aeb-139">响应</span><span class="sxs-lookup"><span data-stu-id="47aeb-139">Response</span></span>
<span data-ttu-id="47aeb-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47aeb-140">The following is an example of the response.</span></span> 

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
