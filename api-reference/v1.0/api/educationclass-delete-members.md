---
title: 从 educationClass 中删除成员
description: 从 educationClass 删除 educationUser
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d98245691a08ede09d16a290b1aef67935c4753c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783653"
---
# <a name="remove-member-from-educationclass"></a><span data-ttu-id="e775b-103">从 educationClass 中删除成员</span><span class="sxs-lookup"><span data-stu-id="e775b-103">Remove member from educationClass</span></span>

<span data-ttu-id="e775b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e775b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e775b-105">从 [educationClass](../resources/educationclass.md) 删除 [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e775b-105">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

> <span data-ttu-id="e775b-106">**注意：** 教师 _和_ 学生包含在课程 **members** 集合中。</span><span class="sxs-lookup"><span data-stu-id="e775b-106">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="e775b-107">在调用此 API 之前，确定要删除的 **educationUser** 不是教师。</span><span class="sxs-lookup"><span data-stu-id="e775b-107">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span> <span data-ttu-id="e775b-108">要获取教师列表，可调用 [educationclass_list_teachers](educationclass-list-teachers.md) 并验证要删除的用户的用户 ID 不在返回的教师列表中。</span><span class="sxs-lookup"><span data-stu-id="e775b-108">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e775b-109">权限</span><span class="sxs-lookup"><span data-stu-id="e775b-109">Permissions</span></span>
<span data-ttu-id="e775b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e775b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e775b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e775b-112">Permission type</span></span>      | <span data-ttu-id="e775b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e775b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e775b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e775b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e775b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e775b-115">Not supported.</span></span>  |
|<span data-ttu-id="e775b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e775b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e775b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e775b-117">Not supported.</span></span>  |
|<span data-ttu-id="e775b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e775b-118">Application</span></span> | <span data-ttu-id="e775b-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e775b-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e775b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e775b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e775b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e775b-121">Request headers</span></span>
| <span data-ttu-id="e775b-122">标头</span><span class="sxs-lookup"><span data-stu-id="e775b-122">Header</span></span>       | <span data-ttu-id="e775b-123">值</span><span class="sxs-lookup"><span data-stu-id="e775b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e775b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e775b-124">Authorization</span></span>  | <span data-ttu-id="e775b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e775b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e775b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e775b-127">Request body</span></span>
<span data-ttu-id="e775b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e775b-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e775b-129">响应</span><span class="sxs-lookup"><span data-stu-id="e775b-129">Response</span></span>
<span data-ttu-id="e775b-130">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="e775b-130">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e775b-131">示例</span><span class="sxs-lookup"><span data-stu-id="e775b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e775b-132">请求</span><span class="sxs-lookup"><span data-stu-id="e775b-132">Request</span></span>
<span data-ttu-id="e775b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e775b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e775b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e775b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_1"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```
# <a name="c"></a>[<span data-ttu-id="e775b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e775b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e775b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e775b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e775b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e775b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e775b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e775b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e775b-139">响应</span><span class="sxs-lookup"><span data-stu-id="e775b-139">Response</span></span>
<span data-ttu-id="e775b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e775b-140">The following is an example of the response.</span></span> 
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
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
