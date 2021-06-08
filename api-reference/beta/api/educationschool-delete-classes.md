---
title: 删除 educationClass
description: 从学校删除课程。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 97d49aa9809d7abe4371480ce952b14d27fd270a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786339"
---
# <a name="remove-educationclass"></a><span data-ttu-id="2356e-103">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="2356e-103">Remove educationClass</span></span>

<span data-ttu-id="2356e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2356e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2356e-105">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="2356e-105">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="2356e-106">权限</span><span class="sxs-lookup"><span data-stu-id="2356e-106">Permissions</span></span>
<span data-ttu-id="2356e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2356e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2356e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2356e-109">Permission type</span></span>      | <span data-ttu-id="2356e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2356e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2356e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2356e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2356e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2356e-112">Not supported.</span></span>  |
|<span data-ttu-id="2356e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2356e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2356e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2356e-114">Not supported.</span></span>  |
|<span data-ttu-id="2356e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2356e-115">Application</span></span> | <span data-ttu-id="2356e-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2356e-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2356e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2356e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2356e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2356e-118">Request headers</span></span>
| <span data-ttu-id="2356e-119">标头</span><span class="sxs-lookup"><span data-stu-id="2356e-119">Header</span></span>       | <span data-ttu-id="2356e-120">值</span><span class="sxs-lookup"><span data-stu-id="2356e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2356e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2356e-121">Authorization</span></span>  | <span data-ttu-id="2356e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2356e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2356e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2356e-124">Request body</span></span>
<span data-ttu-id="2356e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2356e-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2356e-126">响应</span><span class="sxs-lookup"><span data-stu-id="2356e-126">Response</span></span>
<span data-ttu-id="2356e-127">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="2356e-127">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="2356e-128">示例</span><span class="sxs-lookup"><span data-stu-id="2356e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2356e-129">请求</span><span class="sxs-lookup"><span data-stu-id="2356e-129">Request</span></span>
<span data-ttu-id="2356e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2356e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2356e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2356e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_3"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```
# <a name="c"></a>[<span data-ttu-id="2356e-132">C#</span><span class="sxs-lookup"><span data-stu-id="2356e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2356e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2356e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2356e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2356e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2356e-135">Java</span><span class="sxs-lookup"><span data-stu-id="2356e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2356e-136">响应</span><span class="sxs-lookup"><span data-stu-id="2356e-136">Response</span></span>
<span data-ttu-id="2356e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2356e-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


