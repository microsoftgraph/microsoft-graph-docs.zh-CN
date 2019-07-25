---
title: 删除 schemaExtension
description: 删除架构扩展定义。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: c3ce95154319519e7dd6b4353389e392f169de35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870680"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="bc3a2-103">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="bc3a2-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc3a2-104">删除[架构扩展](../resources/schemaextension.md)定义。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="bc3a2-p101">仅创建架构扩展的应用（所有者应用）可以删除架构扩展定义，并且仅在该扩展处于 **InDevelopment** 状态下时才可以将其删除。删除架构扩展定义不会影响访问基于此定义已添加到资源实例的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="bc3a2-107">权限</span><span class="sxs-lookup"><span data-stu-id="bc3a2-107">Permissions</span></span>
<span data-ttu-id="bc3a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bc3a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc3a2-110">Permission type</span></span>      | <span data-ttu-id="bc3a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc3a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc3a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc3a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc3a2-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc3a2-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc3a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc3a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc3a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-115">Not supported.</span></span>    |
|<span data-ttu-id="bc3a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc3a2-116">Application</span></span> | <span data-ttu-id="bc3a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc3a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc3a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc3a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc3a2-119">Request headers</span></span>
| <span data-ttu-id="bc3a2-120">名称</span><span class="sxs-lookup"><span data-stu-id="bc3a2-120">Name</span></span>      |<span data-ttu-id="bc3a2-121">说明</span><span class="sxs-lookup"><span data-stu-id="bc3a2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc3a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc3a2-122">Authorization</span></span>  | <span data-ttu-id="bc3a2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc3a2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc3a2-125">Request body</span></span>
<span data-ttu-id="bc3a2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc3a2-127">响应</span><span class="sxs-lookup"><span data-stu-id="bc3a2-127">Response</span></span>

<span data-ttu-id="bc3a2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc3a2-130">示例</span><span class="sxs-lookup"><span data-stu-id="bc3a2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc3a2-131">请求</span><span class="sxs-lookup"><span data-stu-id="bc3a2-131">Request</span></span>
<span data-ttu-id="bc3a2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bc3a2-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bc3a2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc3a2-134">C#</span><span class="sxs-lookup"><span data-stu-id="bc3a2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc3a2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc3a2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc3a2-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="bc3a2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bc3a2-137">Java</span><span class="sxs-lookup"><span data-stu-id="bc3a2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc3a2-138">响应</span><span class="sxs-lookup"><span data-stu-id="bc3a2-138">Response</span></span>
<span data-ttu-id="bc3a2-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bc3a2-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bc3a2-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bc3a2-140">See also</span></span>

- [<span data-ttu-id="bc3a2-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bc3a2-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bc3a2-142">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bc3a2-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
