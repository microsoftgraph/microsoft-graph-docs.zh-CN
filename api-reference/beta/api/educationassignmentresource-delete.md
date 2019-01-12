---
title: 删除 educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c8154cc9112d62b06d2a93366f01fba3ea7907f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979584"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="7a6f7-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="7a6f7-103">Delete educationAssignmentResource</span></span>

> <span data-ttu-id="7a6f7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a6f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a6f7-106">删除资源，从一个工作分配。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-106">Delete a resource from an assignment.</span></span> <span data-ttu-id="7a6f7-107">仅在类中的教师可以删除的资源。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-107">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="7a6f7-108">工作分配已发布到学生后，教师不能删除标记为"distributeToStudents"的资源。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-108">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="7a6f7-109">权限</span><span class="sxs-lookup"><span data-stu-id="7a6f7-109">Permissions</span></span>
<span data-ttu-id="7a6f7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a6f7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a6f7-112">Permission type</span></span>      | <span data-ttu-id="7a6f7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a6f7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a6f7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a6f7-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="7a6f7-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a6f7-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7a6f7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a6f7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7a6f7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-117">Not supported.</span></span>  |
|<span data-ttu-id="7a6f7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a6f7-118">Application</span></span> | <span data-ttu-id="7a6f7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7a6f7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a6f7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7a6f7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a6f7-121">Request headers</span></span>
| <span data-ttu-id="7a6f7-122">标头</span><span class="sxs-lookup"><span data-stu-id="7a6f7-122">Header</span></span>       | <span data-ttu-id="7a6f7-123">值</span><span class="sxs-lookup"><span data-stu-id="7a6f7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a6f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a6f7-124">Authorization</span></span>  | <span data-ttu-id="7a6f7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a6f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a6f7-127">Request body</span></span>
<span data-ttu-id="7a6f7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7a6f7-129">响应</span><span class="sxs-lookup"><span data-stu-id="7a6f7-129">Response</span></span>
<span data-ttu-id="7a6f7-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a6f7-132">示例</span><span class="sxs-lookup"><span data-stu-id="7a6f7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a6f7-133">请求</span><span class="sxs-lookup"><span data-stu-id="7a6f7-133">Request</span></span>
<span data-ttu-id="7a6f7-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="7a6f7-135">响应</span><span class="sxs-lookup"><span data-stu-id="7a6f7-135">Response</span></span>
<span data-ttu-id="7a6f7-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7a6f7-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
