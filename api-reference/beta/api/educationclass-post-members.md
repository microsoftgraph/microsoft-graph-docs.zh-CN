---
title: 添加学生
description: 向课程添加成员。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ab601786af11692f89ec902aa39b11f0f69d19e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966535"
---
# <a name="add-a-student"></a><span data-ttu-id="af221-103">添加学生</span><span class="sxs-lookup"><span data-stu-id="af221-103">Add a student</span></span>

<span data-ttu-id="af221-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af221-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af221-105">向课程添加成员。</span><span class="sxs-lookup"><span data-stu-id="af221-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="af221-106">权限</span><span class="sxs-lookup"><span data-stu-id="af221-106">Permissions</span></span>
<span data-ttu-id="af221-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af221-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="af221-109">Permission type</span></span>      | <span data-ttu-id="af221-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af221-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af221-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af221-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="af221-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="af221-112">Not supported.</span></span>  |
|<span data-ttu-id="af221-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af221-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="af221-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="af221-114">Not supported.</span></span>  |
|<span data-ttu-id="af221-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="af221-115">Application</span></span> | <span data-ttu-id="af221-116">Eduroster.read.all 所有加号 Member。 Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="af221-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="af221-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af221-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="af221-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="af221-118">Request headers</span></span>
| <span data-ttu-id="af221-119">标头</span><span class="sxs-lookup"><span data-stu-id="af221-119">Header</span></span>       | <span data-ttu-id="af221-120">值</span><span class="sxs-lookup"><span data-stu-id="af221-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af221-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af221-121">Authorization</span></span>  | <span data-ttu-id="af221-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af221-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af221-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af221-124">Content-Type</span></span>  | <span data-ttu-id="af221-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af221-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af221-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af221-126">Request body</span></span>
<span data-ttu-id="af221-127">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af221-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="af221-128">响应</span><span class="sxs-lookup"><span data-stu-id="af221-128">Response</span></span>
<span data-ttu-id="af221-129">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af221-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af221-130">示例</span><span class="sxs-lookup"><span data-stu-id="af221-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af221-131">请求</span><span class="sxs-lookup"><span data-stu-id="af221-131">Request</span></span>
<span data-ttu-id="af221-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="af221-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af221-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="af221-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```
# <a name="javascript"></a>[<span data-ttu-id="af221-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af221-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af221-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af221-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="af221-136">C#</span><span class="sxs-lookup"><span data-stu-id="af221-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af221-137">Java</span><span class="sxs-lookup"><span data-stu-id="af221-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af221-138">响应</span><span class="sxs-lookup"><span data-stu-id="af221-138">Response</span></span>
<span data-ttu-id="af221-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="af221-139">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


