---
title: 从 educationSchool 删除 educationUser
description: 从学校删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e473730f63fdbc5675270b553b10cda60f064715
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965955"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="578fd-103">从 educationSchool 删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="578fd-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="578fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="578fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="578fd-105">从学校删除用户。</span><span class="sxs-lookup"><span data-stu-id="578fd-105">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="578fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="578fd-106">Permissions</span></span>

<span data-ttu-id="578fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="578fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="578fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="578fd-109">Permission type</span></span>                        | <span data-ttu-id="578fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="578fd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="578fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="578fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="578fd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="578fd-112">Not supported.</span></span>                              |
| <span data-ttu-id="578fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="578fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="578fd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="578fd-114">Not supported.</span></span>                              |
| <span data-ttu-id="578fd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="578fd-115">Application</span></span>                            | <span data-ttu-id="578fd-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578fd-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="578fd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="578fd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="578fd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="578fd-118">Request headers</span></span>

| <span data-ttu-id="578fd-119">标头</span><span class="sxs-lookup"><span data-stu-id="578fd-119">Header</span></span>        | <span data-ttu-id="578fd-120">值</span><span class="sxs-lookup"><span data-stu-id="578fd-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="578fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="578fd-121">Authorization</span></span> | <span data-ttu-id="578fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="578fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="578fd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="578fd-124">Request body</span></span>

<span data-ttu-id="578fd-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="578fd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="578fd-126">响应</span><span class="sxs-lookup"><span data-stu-id="578fd-126">Response</span></span>

<span data-ttu-id="578fd-127">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="578fd-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="578fd-128">示例</span><span class="sxs-lookup"><span data-stu-id="578fd-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="578fd-129">请求</span><span class="sxs-lookup"><span data-stu-id="578fd-129">Request</span></span>

<span data-ttu-id="578fd-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="578fd-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="578fd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="578fd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```
# <a name="c"></a>[<span data-ttu-id="578fd-132">C#</span><span class="sxs-lookup"><span data-stu-id="578fd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="578fd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="578fd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="578fd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="578fd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="578fd-135">Java</span><span class="sxs-lookup"><span data-stu-id="578fd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="578fd-136">响应</span><span class="sxs-lookup"><span data-stu-id="578fd-136">Response</span></span>

<span data-ttu-id="578fd-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="578fd-137">The following is an example of the response.</span></span> 

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


