---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: a7d5f376bd6d70229d8058084946fd474a692212
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457940"
---
# <a name="delete-educationclass"></a><span data-ttu-id="c15d3-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="c15d3-104">Delete educationClass</span></span>

<span data-ttu-id="c15d3-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="c15d3-105">Delete a class.</span></span> <span data-ttu-id="c15d3-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="c15d3-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c15d3-107">权限</span><span class="sxs-lookup"><span data-stu-id="c15d3-107">Permissions</span></span>
<span data-ttu-id="c15d3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c15d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c15d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c15d3-110">Permission type</span></span>      | <span data-ttu-id="c15d3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c15d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c15d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c15d3-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c15d3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c15d3-113">Not supported.</span></span>  |
|<span data-ttu-id="c15d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c15d3-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c15d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c15d3-115">Not supported.</span></span>  |
|<span data-ttu-id="c15d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c15d3-116">Application</span></span> | <span data-ttu-id="c15d3-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c15d3-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c15d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c15d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c15d3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c15d3-119">Request headers</span></span>
| <span data-ttu-id="c15d3-120">标头</span><span class="sxs-lookup"><span data-stu-id="c15d3-120">Header</span></span>       | <span data-ttu-id="c15d3-121">值</span><span class="sxs-lookup"><span data-stu-id="c15d3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c15d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c15d3-122">Authorization</span></span>  | <span data-ttu-id="c15d3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c15d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c15d3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c15d3-125">Request body</span></span>
<span data-ttu-id="c15d3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c15d3-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c15d3-127">响应</span><span class="sxs-lookup"><span data-stu-id="c15d3-127">Response</span></span>
<span data-ttu-id="c15d3-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c15d3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c15d3-130">示例</span><span class="sxs-lookup"><span data-stu-id="c15d3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c15d3-131">请求</span><span class="sxs-lookup"><span data-stu-id="c15d3-131">Request</span></span>
<span data-ttu-id="c15d3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c15d3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="c15d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="c15d3-133">Response</span></span>
<span data-ttu-id="c15d3-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c15d3-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
