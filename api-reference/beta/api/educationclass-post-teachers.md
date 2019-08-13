---
title: 添加教师
description: 向课程添加教师。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a9b422d349e465ffd7e14a0543938e3fa8e33616
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323988"
---
# <a name="add-teacher"></a><span data-ttu-id="d73c4-103">添加教师</span><span class="sxs-lookup"><span data-stu-id="d73c4-103">Add teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d73c4-104">向课程添加教师。</span><span class="sxs-lookup"><span data-stu-id="d73c4-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d73c4-105">权限</span><span class="sxs-lookup"><span data-stu-id="d73c4-105">Permissions</span></span>
<span data-ttu-id="d73c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d73c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d73c4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d73c4-108">Permission type</span></span>      | <span data-ttu-id="d73c4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d73c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d73c4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d73c4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d73c4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73c4-111">Not supported.</span></span>  |
|<span data-ttu-id="d73c4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d73c4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d73c4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73c4-113">Not supported.</span></span>  |
|<span data-ttu-id="d73c4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d73c4-114">Application</span></span> | <span data-ttu-id="d73c4-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73c4-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d73c4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d73c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d73c4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d73c4-117">Request headers</span></span>
| <span data-ttu-id="d73c4-118">标头</span><span class="sxs-lookup"><span data-stu-id="d73c4-118">Header</span></span>       | <span data-ttu-id="d73c4-119">值</span><span class="sxs-lookup"><span data-stu-id="d73c4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d73c4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73c4-120">Authorization</span></span>  | <span data-ttu-id="d73c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d73c4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d73c4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d73c4-123">Content-Type</span></span>  | <span data-ttu-id="d73c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d73c4-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d73c4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d73c4-125">Request body</span></span>
<span data-ttu-id="d73c4-126">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d73c4-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d73c4-127">响应</span><span class="sxs-lookup"><span data-stu-id="d73c4-127">Response</span></span>
<span data-ttu-id="d73c4-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d73c4-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d73c4-129">示例</span><span class="sxs-lookup"><span data-stu-id="d73c4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d73c4-130">请求</span><span class="sxs-lookup"><span data-stu-id="d73c4-130">Request</span></span>
<span data-ttu-id="d73c4-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d73c4-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d73c4-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d73c4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d73c4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d73c4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d73c4-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="d73c4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="d73c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="d73c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d73c4-136">Java</span><span class="sxs-lookup"><span data-stu-id="d73c4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d73c4-137">响应</span><span class="sxs-lookup"><span data-stu-id="d73c4-137">Response</span></span>
<span data-ttu-id="d73c4-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d73c4-138">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="d73c4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d73c4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
