---
title: 删除 educationClass
description: 从学校删除课程。
author: mmast-msft
ms.openlocfilehash: 7c69d03670adca93194c5761aa6f943ee9201ac8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319248"
---
# <a name="remove-educationclass"></a><span data-ttu-id="adc5b-103">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="adc5b-103">Remove educationClass</span></span>

> <span data-ttu-id="adc5b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="adc5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adc5b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="adc5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adc5b-106">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="adc5b-106">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="adc5b-107">权限</span><span class="sxs-lookup"><span data-stu-id="adc5b-107">Permissions</span></span>
<span data-ttu-id="adc5b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adc5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adc5b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="adc5b-110">Permission type</span></span>      | <span data-ttu-id="adc5b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adc5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adc5b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adc5b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="adc5b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="adc5b-113">Not supported.</span></span>  |
|<span data-ttu-id="adc5b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adc5b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="adc5b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="adc5b-115">Not supported.</span></span>  |
|<span data-ttu-id="adc5b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="adc5b-116">Application</span></span> | <span data-ttu-id="adc5b-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adc5b-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="adc5b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adc5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="adc5b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="adc5b-119">Request headers</span></span>
| <span data-ttu-id="adc5b-120">标头</span><span class="sxs-lookup"><span data-stu-id="adc5b-120">Header</span></span>       | <span data-ttu-id="adc5b-121">值</span><span class="sxs-lookup"><span data-stu-id="adc5b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="adc5b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="adc5b-122">Authorization</span></span>  | <span data-ttu-id="adc5b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adc5b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="adc5b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="adc5b-125">Request body</span></span>
<span data-ttu-id="adc5b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adc5b-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="adc5b-127">响应</span><span class="sxs-lookup"><span data-stu-id="adc5b-127">Response</span></span>
<span data-ttu-id="adc5b-128">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="adc5b-128">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="adc5b-129">示例</span><span class="sxs-lookup"><span data-stu-id="adc5b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adc5b-130">请求</span><span class="sxs-lookup"><span data-stu-id="adc5b-130">Request</span></span>
<span data-ttu-id="adc5b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adc5b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="adc5b-132">响应</span><span class="sxs-lookup"><span data-stu-id="adc5b-132">Response</span></span>
<span data-ttu-id="adc5b-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adc5b-133">The following is an example of the response.</span></span> 

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