---
title: 删除 educationSchool
description: 删除学校。
author: mmast-msft
ms.openlocfilehash: e104265f718ad69a84b9e2362962d72763e8fc54
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323063"
---
# <a name="delete-educationschool"></a><span data-ttu-id="81c96-103">删除 educationSchool</span><span class="sxs-lookup"><span data-stu-id="81c96-103">Delete educationSchool</span></span>

> <span data-ttu-id="81c96-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81c96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81c96-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81c96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81c96-106">删除学校。</span><span class="sxs-lookup"><span data-stu-id="81c96-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="81c96-107">权限</span><span class="sxs-lookup"><span data-stu-id="81c96-107">Permissions</span></span>
<span data-ttu-id="81c96-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81c96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81c96-110">Permission type</span></span>      | <span data-ttu-id="81c96-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81c96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81c96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81c96-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="81c96-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="81c96-113">Not supported.</span></span>  |
|<span data-ttu-id="81c96-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81c96-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="81c96-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81c96-115">Not supported.</span></span>  |
|<span data-ttu-id="81c96-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="81c96-116">Application</span></span> | <span data-ttu-id="81c96-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c96-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="81c96-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81c96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81c96-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="81c96-119">Request headers</span></span>
| <span data-ttu-id="81c96-120">标头</span><span class="sxs-lookup"><span data-stu-id="81c96-120">Header</span></span>       | <span data-ttu-id="81c96-121">值</span><span class="sxs-lookup"><span data-stu-id="81c96-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81c96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c96-122">Authorization</span></span>  | <span data-ttu-id="81c96-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81c96-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81c96-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="81c96-125">Request body</span></span>
<span data-ttu-id="81c96-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81c96-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="81c96-127">响应</span><span class="sxs-lookup"><span data-stu-id="81c96-127">Response</span></span>
<span data-ttu-id="81c96-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="81c96-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81c96-130">示例</span><span class="sxs-lookup"><span data-stu-id="81c96-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81c96-131">请求</span><span class="sxs-lookup"><span data-stu-id="81c96-131">Request</span></span>
<span data-ttu-id="81c96-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81c96-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="81c96-133">响应</span><span class="sxs-lookup"><span data-stu-id="81c96-133">Response</span></span>
<span data-ttu-id="81c96-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81c96-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->