---
title: 将 educationClass 添加到 educationSchool
description: 向学校添加课程。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f3ea3d025e55d9e56bc8488d404ca2c028f3bbb8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517458"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="09e3a-103">将 educationClass 添加到 educationSchool</span><span class="sxs-lookup"><span data-stu-id="09e3a-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="09e3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09e3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09e3a-105">向学校添加课程。</span><span class="sxs-lookup"><span data-stu-id="09e3a-105">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="09e3a-106">权限</span><span class="sxs-lookup"><span data-stu-id="09e3a-106">Permissions</span></span>
<span data-ttu-id="09e3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09e3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09e3a-109">Permission type</span></span>      | <span data-ttu-id="09e3a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09e3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09e3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09e3a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="09e3a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="09e3a-112">Not supported.</span></span>  |
|<span data-ttu-id="09e3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09e3a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="09e3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09e3a-114">Not supported.</span></span>  |
|<span data-ttu-id="09e3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09e3a-115">Application</span></span> | <span data-ttu-id="09e3a-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09e3a-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09e3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09e3a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="09e3a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09e3a-118">Request headers</span></span>
| <span data-ttu-id="09e3a-119">标头</span><span class="sxs-lookup"><span data-stu-id="09e3a-119">Header</span></span>       | <span data-ttu-id="09e3a-120">值</span><span class="sxs-lookup"><span data-stu-id="09e3a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09e3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e3a-121">Authorization</span></span>  | <span data-ttu-id="09e3a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09e3a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09e3a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09e3a-124">Content-Type</span></span>  | <span data-ttu-id="09e3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09e3a-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09e3a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="09e3a-126">Request body</span></span>
<span data-ttu-id="09e3a-127">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09e3a-127">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="09e3a-128">响应</span><span class="sxs-lookup"><span data-stu-id="09e3a-128">Response</span></span>
<span data-ttu-id="09e3a-129">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09e3a-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e3a-130">示例</span><span class="sxs-lookup"><span data-stu-id="09e3a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09e3a-131">请求</span><span class="sxs-lookup"><span data-stu-id="09e3a-131">Request</span></span>
<span data-ttu-id="09e3a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09e3a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09e3a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="09e3a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```
# <a name="javascript"></a>[<span data-ttu-id="09e3a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09e3a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09e3a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09e3a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="09e3a-136">C#</span><span class="sxs-lookup"><span data-stu-id="09e3a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09e3a-137">Java</span><span class="sxs-lookup"><span data-stu-id="09e3a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09e3a-138">响应</span><span class="sxs-lookup"><span data-stu-id="09e3a-138">Response</span></span> 
<span data-ttu-id="09e3a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09e3a-139">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
