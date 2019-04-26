---
title: 删除 educationClass
description: 从学校删除课程。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3cf61d77171e7dc3161aa3b3cc48d663de784649
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550348"
---
# <a name="remove-educationclass"></a><span data-ttu-id="19460-103">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="19460-103">Remove educationClass</span></span>

<span data-ttu-id="19460-104">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="19460-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="19460-105">权限</span><span class="sxs-lookup"><span data-stu-id="19460-105">Permissions</span></span>
<span data-ttu-id="19460-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19460-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19460-108">Permission type</span></span>      | <span data-ttu-id="19460-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19460-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19460-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19460-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="19460-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="19460-111">Not supported.</span></span>  |
|<span data-ttu-id="19460-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19460-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="19460-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19460-113">Not supported.</span></span>  |
|<span data-ttu-id="19460-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19460-114">Application</span></span> | <span data-ttu-id="19460-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19460-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19460-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19460-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="19460-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="19460-117">Request headers</span></span>
| <span data-ttu-id="19460-118">标头</span><span class="sxs-lookup"><span data-stu-id="19460-118">Header</span></span>       | <span data-ttu-id="19460-119">值</span><span class="sxs-lookup"><span data-stu-id="19460-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19460-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19460-120">Authorization</span></span>  | <span data-ttu-id="19460-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19460-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19460-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="19460-123">Request body</span></span>
<span data-ttu-id="19460-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19460-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="19460-125">响应</span><span class="sxs-lookup"><span data-stu-id="19460-125">Response</span></span>
<span data-ttu-id="19460-126">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="19460-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="19460-127">示例</span><span class="sxs-lookup"><span data-stu-id="19460-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19460-128">请求</span><span class="sxs-lookup"><span data-stu-id="19460-128">Request</span></span>
<span data-ttu-id="19460-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19460-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="19460-130">响应</span><span class="sxs-lookup"><span data-stu-id="19460-130">Response</span></span>
<span data-ttu-id="19460-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19460-131">The following is an example of the response.</span></span> 

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
