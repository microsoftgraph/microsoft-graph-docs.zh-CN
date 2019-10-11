---
title: 从 educationSchool 删除 educationUser
description: 从学校删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: afafb2c86188fdf879511916449f7e3d8b3ea489
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427828"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="6de02-103">从 educationSchool 删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="6de02-103">Remove educationUser from an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6de02-104">从学校删除用户。</span><span class="sxs-lookup"><span data-stu-id="6de02-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6de02-105">权限</span><span class="sxs-lookup"><span data-stu-id="6de02-105">Permissions</span></span>

<span data-ttu-id="6de02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6de02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6de02-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6de02-108">Permission type</span></span>                        | <span data-ttu-id="6de02-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6de02-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6de02-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6de02-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6de02-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6de02-111">Not supported.</span></span>                              |
| <span data-ttu-id="6de02-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6de02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6de02-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6de02-113">Not supported.</span></span>                              |
| <span data-ttu-id="6de02-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6de02-114">Application</span></span>                            | <span data-ttu-id="6de02-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de02-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="6de02-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6de02-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6de02-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6de02-117">Request headers</span></span>

| <span data-ttu-id="6de02-118">标头</span><span class="sxs-lookup"><span data-stu-id="6de02-118">Header</span></span>        | <span data-ttu-id="6de02-119">值</span><span class="sxs-lookup"><span data-stu-id="6de02-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6de02-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de02-120">Authorization</span></span> | <span data-ttu-id="6de02-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6de02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6de02-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6de02-123">Request body</span></span>

<span data-ttu-id="6de02-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6de02-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6de02-125">响应</span><span class="sxs-lookup"><span data-stu-id="6de02-125">Response</span></span>

<span data-ttu-id="6de02-126">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="6de02-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de02-127">示例</span><span class="sxs-lookup"><span data-stu-id="6de02-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6de02-128">请求</span><span class="sxs-lookup"><span data-stu-id="6de02-128">Request</span></span>

<span data-ttu-id="6de02-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6de02-129">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6de02-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6de02-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/users/13006
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6de02-131">C#</span><span class="sxs-lookup"><span data-stu-id="6de02-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6de02-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6de02-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6de02-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6de02-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6de02-134">响应</span><span class="sxs-lookup"><span data-stu-id="6de02-134">Response</span></span>

<span data-ttu-id="6de02-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6de02-135">The following is an example of the response.</span></span> 

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
