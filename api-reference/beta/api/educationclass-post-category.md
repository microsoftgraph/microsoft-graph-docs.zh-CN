---
title: 创建 educationCategory
description: 创建新类别。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 943cf7abbd9a91e10249f6cafd675e6844d5b1e9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992338"
---
# <a name="create-educationcategory"></a><span data-ttu-id="eb32c-103">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="eb32c-103">Create educationCategory</span></span>

<span data-ttu-id="eb32c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb32c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb32c-105">在[educationClass 上创建新的 educationCategory。](../resources/educationcategory.md) [](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="eb32c-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb32c-106">权限</span><span class="sxs-lookup"><span data-stu-id="eb32c-106">Permissions</span></span>
<span data-ttu-id="eb32c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb32c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb32c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb32c-109">Permission type</span></span>      | <span data-ttu-id="eb32c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb32c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb32c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb32c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="eb32c-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb32c-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="eb32c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb32c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eb32c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb32c-114">Not supported.</span></span>  |
|<span data-ttu-id="eb32c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb32c-115">Application</span></span> | <span data-ttu-id="eb32c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb32c-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eb32c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb32c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="eb32c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb32c-118">Request headers</span></span>
| <span data-ttu-id="eb32c-119">标头</span><span class="sxs-lookup"><span data-stu-id="eb32c-119">Header</span></span>       | <span data-ttu-id="eb32c-120">值</span><span class="sxs-lookup"><span data-stu-id="eb32c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb32c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb32c-121">Authorization</span></span>  | <span data-ttu-id="eb32c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb32c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb32c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb32c-124">Content-Type</span></span>  | <span data-ttu-id="eb32c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb32c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb32c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb32c-126">Request body</span></span>
<span data-ttu-id="eb32c-127">在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb32c-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="eb32c-128">响应</span><span class="sxs-lookup"><span data-stu-id="eb32c-128">Response</span></span>
<span data-ttu-id="eb32c-129">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb32c-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb32c-130">示例</span><span class="sxs-lookup"><span data-stu-id="eb32c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb32c-131">请求</span><span class="sxs-lookup"><span data-stu-id="eb32c-131">Request</span></span>
<span data-ttu-id="eb32c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb32c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb32c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb32c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["9a5e4047-c1dc-4243-9628-580d3c64b80c"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/9a5e4047-c1dc-4243-9628-580d3c64b80c/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
# <a name="c"></a>[<span data-ttu-id="eb32c-134">C#</span><span class="sxs-lookup"><span data-stu-id="eb32c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationcategory-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb32c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb32c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationcategory-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb32c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb32c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationcategory-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb32c-137">Java</span><span class="sxs-lookup"><span data-stu-id="eb32c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationcategory-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="eb32c-138">在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb32c-138">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="eb32c-139">响应</span><span class="sxs-lookup"><span data-stu-id="eb32c-139">Response</span></span>
<span data-ttu-id="eb32c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb32c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="eb32c-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb32c-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('9a5e4047-c1dc-4243-9628-580d3c64b80c')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


