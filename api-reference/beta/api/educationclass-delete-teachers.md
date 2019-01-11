---
title: 删除 teacher
description: 从课程中删除教师。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 5a5e5f2fed8a22bf00ca4e29cca51d87b6dc9a8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865133"
---
# <a name="remove-teacher"></a><span data-ttu-id="4e61e-103">删除 teacher</span><span class="sxs-lookup"><span data-stu-id="4e61e-103">Remove teacher</span></span>

> <span data-ttu-id="4e61e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4e61e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e61e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4e61e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e61e-106">从课程中删除教师。</span><span class="sxs-lookup"><span data-stu-id="4e61e-106">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e61e-107">权限</span><span class="sxs-lookup"><span data-stu-id="4e61e-107">Permissions</span></span>
<span data-ttu-id="4e61e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e61e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e61e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e61e-110">Permission type</span></span>      | <span data-ttu-id="4e61e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e61e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e61e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e61e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e61e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e61e-113">Not supported.</span></span>  |
|<span data-ttu-id="4e61e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e61e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4e61e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e61e-115">Not supported.</span></span>  |
|<span data-ttu-id="4e61e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e61e-116">Application</span></span> | <span data-ttu-id="4e61e-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e61e-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4e61e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e61e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4e61e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e61e-119">Request headers</span></span>
| <span data-ttu-id="4e61e-120">标头</span><span class="sxs-lookup"><span data-stu-id="4e61e-120">Header</span></span>       | <span data-ttu-id="4e61e-121">值</span><span class="sxs-lookup"><span data-stu-id="4e61e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e61e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e61e-122">Authorization</span></span>  | <span data-ttu-id="4e61e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e61e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e61e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e61e-125">Request body</span></span>
<span data-ttu-id="4e61e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e61e-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4e61e-127">响应</span><span class="sxs-lookup"><span data-stu-id="4e61e-127">Response</span></span>
<span data-ttu-id="4e61e-128">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="4e61e-128">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e61e-129">示例</span><span class="sxs-lookup"><span data-stu-id="4e61e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e61e-130">请求</span><span class="sxs-lookup"><span data-stu-id="4e61e-130">Request</span></span>
<span data-ttu-id="4e61e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e61e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/<id>/teachers/14012
```

##### <a name="response"></a><span data-ttu-id="4e61e-132">响应</span><span class="sxs-lookup"><span data-stu-id="4e61e-132">Response</span></span>
<span data-ttu-id="4e61e-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e61e-133">The following is an example of the response.</span></span> 
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
