---
title: 删除 educationClass
description: 从学校删除课程。
ms.openlocfilehash: 9e5641fa2a3718a388e20b7d980bae0b6916eda2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045659"
---
# <a name="remove-educationclass"></a><span data-ttu-id="8d36d-103">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="8d36d-103">Remove educationClass</span></span>

> <span data-ttu-id="8d36d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d36d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d36d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d36d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d36d-106">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="8d36d-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d36d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8d36d-107">Permissions</span></span>
<span data-ttu-id="8d36d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d36d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d36d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d36d-110">Permission type</span></span>      | <span data-ttu-id="8d36d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d36d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d36d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d36d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d36d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d36d-113">Not supported.</span></span>  |
|<span data-ttu-id="8d36d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d36d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8d36d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d36d-115">Not supported.</span></span>  |
|<span data-ttu-id="8d36d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d36d-116">Application</span></span> | <span data-ttu-id="8d36d-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d36d-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d36d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d36d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8d36d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d36d-119">Request headers</span></span>
| <span data-ttu-id="8d36d-120">标头</span><span class="sxs-lookup"><span data-stu-id="8d36d-120">Header</span></span>       | <span data-ttu-id="8d36d-121">值</span><span class="sxs-lookup"><span data-stu-id="8d36d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d36d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d36d-122">Authorization</span></span>  | <span data-ttu-id="8d36d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d36d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d36d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d36d-125">Request body</span></span>
<span data-ttu-id="8d36d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d36d-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8d36d-127">响应</span><span class="sxs-lookup"><span data-stu-id="8d36d-127">Response</span></span>
<span data-ttu-id="8d36d-128">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="8d36d-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d36d-129">示例</span><span class="sxs-lookup"><span data-stu-id="8d36d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d36d-130">请求</span><span class="sxs-lookup"><span data-stu-id="8d36d-130">Request</span></span>
<span data-ttu-id="8d36d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d36d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="8d36d-132">响应</span><span class="sxs-lookup"><span data-stu-id="8d36d-132">Response</span></span>
<span data-ttu-id="8d36d-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d36d-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->