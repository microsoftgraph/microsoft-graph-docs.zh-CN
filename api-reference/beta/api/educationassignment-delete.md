---
title: 删除 educationAssignment
description: 删除现有的工作分配。 仅在类的教师可以删除工作分配。
ms.openlocfilehash: e9965efa458459cff0c3914dbc12b37153a6ab51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046397"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="aa654-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="aa654-104">Delete educationAssignment</span></span>

> <span data-ttu-id="aa654-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa654-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa654-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa654-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa654-107">删除现有的工作分配。</span><span class="sxs-lookup"><span data-stu-id="aa654-107">Delete an existing assignment.</span></span> <span data-ttu-id="aa654-108">仅在类的教师可以删除工作分配。</span><span class="sxs-lookup"><span data-stu-id="aa654-108">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa654-109">权限</span><span class="sxs-lookup"><span data-stu-id="aa654-109">Permissions</span></span>
<span data-ttu-id="aa654-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa654-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa654-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa654-112">Permission type</span></span>      | <span data-ttu-id="aa654-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa654-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa654-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa654-114">Delegated (work or school account)</span></span>| <span data-ttu-id="aa654-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa654-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="aa654-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa654-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="aa654-117">不受支持。</span><span class="sxs-lookup"><span data-stu-id="aa654-117">Not Supported.</span></span> |
|<span data-ttu-id="aa654-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa654-118">Application</span></span> | <span data-ttu-id="aa654-119">不受支持。</span><span class="sxs-lookup"><span data-stu-id="aa654-119">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="aa654-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa654-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="aa654-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa654-121">Request headers</span></span>
| <span data-ttu-id="aa654-122">标头</span><span class="sxs-lookup"><span data-stu-id="aa654-122">Header</span></span>       | <span data-ttu-id="aa654-123">值</span><span class="sxs-lookup"><span data-stu-id="aa654-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa654-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa654-124">Authorization</span></span>  | <span data-ttu-id="aa654-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa654-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa654-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa654-127">Request body</span></span>
<span data-ttu-id="aa654-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa654-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="aa654-129">响应</span><span class="sxs-lookup"><span data-stu-id="aa654-129">Response</span></span>
<span data-ttu-id="aa654-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aa654-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa654-132">示例</span><span class="sxs-lookup"><span data-stu-id="aa654-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa654-133">请求</span><span class="sxs-lookup"><span data-stu-id="aa654-133">Request</span></span>
<span data-ttu-id="aa654-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa654-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="aa654-135">响应</span><span class="sxs-lookup"><span data-stu-id="aa654-135">Response</span></span>
<span data-ttu-id="aa654-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa654-136">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->