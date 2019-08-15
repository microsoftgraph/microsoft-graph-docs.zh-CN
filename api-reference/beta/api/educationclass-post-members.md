---
title: 添加学生
description: 向课程添加成员。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e7df4cbb24cc2287e2289fcd21eab4a80f8b6581
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416350"
---
# <a name="add-a-student"></a><span data-ttu-id="a5407-103">添加学生</span><span class="sxs-lookup"><span data-stu-id="a5407-103">Add a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5407-104">向课程添加成员。</span><span class="sxs-lookup"><span data-stu-id="a5407-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5407-105">权限</span><span class="sxs-lookup"><span data-stu-id="a5407-105">Permissions</span></span>
<span data-ttu-id="a5407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5407-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5407-108">Permission type</span></span>      | <span data-ttu-id="a5407-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5407-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5407-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5407-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5407-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5407-111">Not supported.</span></span>  |
|<span data-ttu-id="a5407-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5407-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5407-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5407-113">Not supported.</span></span>  |
|<span data-ttu-id="a5407-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5407-114">Application</span></span> | <span data-ttu-id="a5407-115">Eduroster.read.all 所有加号 Member。 Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="a5407-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5407-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5407-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a5407-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5407-117">Request headers</span></span>
| <span data-ttu-id="a5407-118">标头</span><span class="sxs-lookup"><span data-stu-id="a5407-118">Header</span></span>       | <span data-ttu-id="a5407-119">值</span><span class="sxs-lookup"><span data-stu-id="a5407-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5407-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5407-120">Authorization</span></span>  | <span data-ttu-id="a5407-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5407-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5407-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5407-123">Content-Type</span></span>  | <span data-ttu-id="a5407-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a5407-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5407-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5407-125">Request body</span></span>
<span data-ttu-id="a5407-126">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5407-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a5407-127">响应</span><span class="sxs-lookup"><span data-stu-id="a5407-127">Response</span></span>
<span data-ttu-id="a5407-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5407-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5407-129">示例</span><span class="sxs-lookup"><span data-stu-id="a5407-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5407-130">请求</span><span class="sxs-lookup"><span data-stu-id="a5407-130">Request</span></span>
<span data-ttu-id="a5407-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a5407-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5407-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a5407-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5407-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5407-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5407-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="a5407-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="a5407-135">C#</span><span class="sxs-lookup"><span data-stu-id="a5407-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5407-136">响应</span><span class="sxs-lookup"><span data-stu-id="a5407-136">Response</span></span>
<span data-ttu-id="a5407-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a5407-137">The following is an example of the response.</span></span> 


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
