---
title: 删除 educationSubmissionResource
description: 从提交中删除资源。 此操作仅能由学生完成。 如果从工作分配复制了资源，将在删除当前副本后创建资源的新副本。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 45b165ab8f2a9c07d657ea56b3118f5e14ba5e4b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912259"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="aa906-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="aa906-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="aa906-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa906-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa906-107">从提交中删除资源。</span><span class="sxs-lookup"><span data-stu-id="aa906-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="aa906-108">此操作仅能由学生完成。</span><span class="sxs-lookup"><span data-stu-id="aa906-108">This can only be done by the student.</span></span> <span data-ttu-id="aa906-109">如果从工作分配复制了资源，将在删除当前副本后创建资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="aa906-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="aa906-110">这允许您将资源"重置"到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="aa906-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="aa906-111">如果资源不是从作业中复制的，而是从学生添加的，则只会删除该资源。</span><span class="sxs-lookup"><span data-stu-id="aa906-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa906-112">权限</span><span class="sxs-lookup"><span data-stu-id="aa906-112">Permissions</span></span>
<span data-ttu-id="aa906-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa906-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa906-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa906-115">Permission type</span></span>      | <span data-ttu-id="aa906-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa906-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa906-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa906-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa906-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa906-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="aa906-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa906-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aa906-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa906-120">Not supported.</span></span>  |
|<span data-ttu-id="aa906-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa906-121">Application</span></span> | <span data-ttu-id="aa906-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa906-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa906-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa906-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```

## <a name="request-headers"></a><span data-ttu-id="aa906-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa906-124">Request headers</span></span>
| <span data-ttu-id="aa906-125">标头</span><span class="sxs-lookup"><span data-stu-id="aa906-125">Header</span></span>       | <span data-ttu-id="aa906-126">值</span><span class="sxs-lookup"><span data-stu-id="aa906-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa906-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa906-127">Authorization</span></span>  | <span data-ttu-id="aa906-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa906-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa906-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa906-130">Request body</span></span>
<span data-ttu-id="aa906-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa906-131">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="aa906-132">响应</span><span class="sxs-lookup"><span data-stu-id="aa906-132">Response</span></span>
<span data-ttu-id="aa906-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aa906-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa906-135">示例</span><span class="sxs-lookup"><span data-stu-id="aa906-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa906-136">请求</span><span class="sxs-lookup"><span data-stu-id="aa906-136">Request</span></span>
<span data-ttu-id="aa906-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa906-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```

### <a name="response"></a><span data-ttu-id="aa906-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa906-138">Response</span></span>
<span data-ttu-id="aa906-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa906-139">The following is an example of the response.</span></span> 

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
  ]
}
-->


