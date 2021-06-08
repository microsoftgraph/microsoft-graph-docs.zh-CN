---
title: 添加学生
description: 向课程添加成员。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9e0b90e29019eea2e0b232f195017261974bed99
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788085"
---
# <a name="add-a-student"></a><span data-ttu-id="fb491-103">添加学生</span><span class="sxs-lookup"><span data-stu-id="fb491-103">Add a student</span></span>

<span data-ttu-id="fb491-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb491-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb491-105">向课程添加成员。</span><span class="sxs-lookup"><span data-stu-id="fb491-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb491-106">权限</span><span class="sxs-lookup"><span data-stu-id="fb491-106">Permissions</span></span>
<span data-ttu-id="fb491-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb491-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb491-109">Permission type</span></span>      | <span data-ttu-id="fb491-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb491-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb491-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb491-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="fb491-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb491-112">Not supported.</span></span>  |
|<span data-ttu-id="fb491-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb491-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fb491-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb491-114">Not supported.</span></span>  |
|<span data-ttu-id="fb491-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb491-115">Application</span></span> | <span data-ttu-id="fb491-116">EduRoster.ReadWrite.All 加上 Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="fb491-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fb491-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb491-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fb491-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb491-118">Request headers</span></span>
| <span data-ttu-id="fb491-119">标头</span><span class="sxs-lookup"><span data-stu-id="fb491-119">Header</span></span>       | <span data-ttu-id="fb491-120">值</span><span class="sxs-lookup"><span data-stu-id="fb491-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb491-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb491-121">Authorization</span></span>  | <span data-ttu-id="fb491-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb491-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fb491-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb491-124">Content-Type</span></span>  | <span data-ttu-id="fb491-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb491-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb491-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb491-126">Request body</span></span>
<span data-ttu-id="fb491-127">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb491-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fb491-128">响应</span><span class="sxs-lookup"><span data-stu-id="fb491-128">Response</span></span>
<span data-ttu-id="fb491-129">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb491-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb491-130">示例</span><span class="sxs-lookup"><span data-stu-id="fb491-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb491-131">请求</span><span class="sxs-lookup"><span data-stu-id="fb491-131">Request</span></span>
<span data-ttu-id="fb491-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb491-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb491-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb491-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```
# <a name="javascript"></a>[<span data-ttu-id="fb491-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb491-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb491-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb491-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fb491-136">C#</span><span class="sxs-lookup"><span data-stu-id="fb491-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb491-137">Java</span><span class="sxs-lookup"><span data-stu-id="fb491-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fb491-138">响应</span><span class="sxs-lookup"><span data-stu-id="fb491-138">Response</span></span>
<span data-ttu-id="fb491-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb491-139">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

