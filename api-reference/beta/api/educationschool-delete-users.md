---
title: 从 educationSchool 删除 educationUser
description: 从学校删除用户。
ms.openlocfilehash: 05ca8d1940580ac2897c842905a754c37a8c8814
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044563"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="6cd42-103">从 educationSchool 删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="6cd42-103">Remove educationUser from an educationSchool</span></span>

> <span data-ttu-id="6cd42-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6cd42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cd42-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6cd42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cd42-106">从学校删除用户。</span><span class="sxs-lookup"><span data-stu-id="6cd42-106">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cd42-107">权限</span><span class="sxs-lookup"><span data-stu-id="6cd42-107">Permissions</span></span>
<span data-ttu-id="6cd42-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cd42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cd42-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cd42-110">Permission type</span></span>      | <span data-ttu-id="6cd42-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cd42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cd42-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cd42-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="6cd42-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cd42-113">Not supported.</span></span>  |
|<span data-ttu-id="6cd42-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cd42-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6cd42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cd42-115">Not supported.</span></span>  |
|<span data-ttu-id="6cd42-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cd42-116">Application</span></span> | <span data-ttu-id="6cd42-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd42-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6cd42-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cd42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/<id>/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6cd42-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cd42-119">Request headers</span></span>
| <span data-ttu-id="6cd42-120">标头</span><span class="sxs-lookup"><span data-stu-id="6cd42-120">Header</span></span>       | <span data-ttu-id="6cd42-121">值</span><span class="sxs-lookup"><span data-stu-id="6cd42-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cd42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cd42-122">Authorization</span></span>  | <span data-ttu-id="6cd42-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cd42-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cd42-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cd42-125">Request body</span></span>
<span data-ttu-id="6cd42-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cd42-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6cd42-127">响应</span><span class="sxs-lookup"><span data-stu-id="6cd42-127">Response</span></span>
<span data-ttu-id="6cd42-128">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="6cd42-128">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd42-129">示例</span><span class="sxs-lookup"><span data-stu-id="6cd42-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cd42-130">请求</span><span class="sxs-lookup"><span data-stu-id="6cd42-130">Request</span></span>
<span data-ttu-id="6cd42-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cd42-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="6cd42-132">响应</span><span class="sxs-lookup"><span data-stu-id="6cd42-132">Response</span></span>
<span data-ttu-id="6cd42-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cd42-133">The following is an example of the response.</span></span> 
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