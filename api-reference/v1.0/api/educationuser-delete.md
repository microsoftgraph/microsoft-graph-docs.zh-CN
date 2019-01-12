---
title: 删除 educationUser
description: 删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be2839a866474acbdd196c3b43503a5b69252c26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932334"
---
# <a name="delete-educationuser"></a><span data-ttu-id="a8c1e-103">删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="a8c1e-103">Delete educationUser</span></span>

<span data-ttu-id="a8c1e-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="a8c1e-105">权限</span><span class="sxs-lookup"><span data-stu-id="a8c1e-105">Permissions</span></span>
<span data-ttu-id="a8c1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8c1e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8c1e-108">Permission type</span></span>      | <span data-ttu-id="a8c1e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8c1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8c1e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8c1e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a8c1e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-111">Not supported.</span></span>  |
|<span data-ttu-id="a8c1e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8c1e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a8c1e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-113">Not supported.</span></span>  |
|<span data-ttu-id="a8c1e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8c1e-114">Application</span></span> | <span data-ttu-id="a8c1e-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c1e-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8c1e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8c1e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a8c1e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8c1e-117">Request headers</span></span>
| <span data-ttu-id="a8c1e-118">标头</span><span class="sxs-lookup"><span data-stu-id="a8c1e-118">Header</span></span>       | <span data-ttu-id="a8c1e-119">值</span><span class="sxs-lookup"><span data-stu-id="a8c1e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8c1e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8c1e-120">Authorization</span></span>  | <span data-ttu-id="a8c1e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8c1e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8c1e-123">Request body</span></span>
<span data-ttu-id="a8c1e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a8c1e-125">响应</span><span class="sxs-lookup"><span data-stu-id="a8c1e-125">Response</span></span>
<span data-ttu-id="a8c1e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8c1e-128">示例</span><span class="sxs-lookup"><span data-stu-id="a8c1e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8c1e-129">请求</span><span class="sxs-lookup"><span data-stu-id="a8c1e-129">Request</span></span>
<span data-ttu-id="a8c1e-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="a8c1e-131">响应</span><span class="sxs-lookup"><span data-stu-id="a8c1e-131">Response</span></span>
<span data-ttu-id="a8c1e-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8c1e-132">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
