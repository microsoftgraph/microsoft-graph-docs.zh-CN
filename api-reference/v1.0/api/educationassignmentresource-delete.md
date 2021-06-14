---
title: 删除 educationAssignmentResource
description: 删除附加到工作分配的特定资源。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f6e86992537e366d5f0972f323729796f197e2b5
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912346"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="9c7b6-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9c7b6-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="9c7b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c7b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c7b6-105">删除附加到工作分配的特定资源。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-105">Delete a specific resource attached to an assignment.</span></span>

<span data-ttu-id="9c7b6-106">一般情况下，只有班级中的教师可以删除资源。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-106">In general, only teachers in the class can remove a resource.</span></span> <span data-ttu-id="9c7b6-107">但是，教师无法在向学生发布作业后删除标记为"distributeToStudents"的资源。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-107">However, teachers cannot remove resources marked as "distributeToStudents", after the assignment has been published to students.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c7b6-108">权限</span><span class="sxs-lookup"><span data-stu-id="9c7b6-108">Permissions</span></span>
<span data-ttu-id="9c7b6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c7b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c7b6-111">Permission type</span></span>      | <span data-ttu-id="9c7b6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c7b6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c7b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c7b6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9c7b6-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c7b6-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9c7b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c7b6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9c7b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-116">Not supported.</span></span>  |
|<span data-ttu-id="9c7b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c7b6-117">Application</span></span> | <span data-ttu-id="9c7b6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9c7b6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c7b6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c

```
## <a name="request-headers"></a><span data-ttu-id="9c7b6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c7b6-120">Request headers</span></span>
| <span data-ttu-id="9c7b6-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c7b6-121">Header</span></span>       | <span data-ttu-id="9c7b6-122">值</span><span class="sxs-lookup"><span data-stu-id="9c7b6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c7b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c7b6-123">Authorization</span></span>  | <span data-ttu-id="9c7b6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c7b6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c7b6-126">Request body</span></span>
<span data-ttu-id="9c7b6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-127">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9c7b6-128">响应</span><span class="sxs-lookup"><span data-stu-id="9c7b6-128">Response</span></span>
<span data-ttu-id="9c7b6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c7b6-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c7b6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c7b6-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c7b6-132">Request</span></span>
<span data-ttu-id="9c7b6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources/22002
```

### <a name="response"></a><span data-ttu-id="9c7b6-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c7b6-134">Response</span></span>
<span data-ttu-id="9c7b6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c7b6-135">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


