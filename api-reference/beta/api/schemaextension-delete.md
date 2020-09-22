---
title: 删除 schemaExtension
description: 删除架构扩展定义。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: a2ba1ca24916d452232c4088a7b750267dcf761a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058744"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="856cf-103">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="856cf-103">Delete schemaExtension</span></span>

<span data-ttu-id="856cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="856cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="856cf-105">删除[架构扩展](../resources/schemaextension.md)定义。</span><span class="sxs-lookup"><span data-stu-id="856cf-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="856cf-p101">仅创建架构扩展的应用（所有者应用）可以删除架构扩展定义，并且仅在该扩展处于 **InDevelopment** 状态下时才可以将其删除。删除架构扩展定义不会影响访问基于此定义已添加到资源实例的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="856cf-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="856cf-108">权限</span><span class="sxs-lookup"><span data-stu-id="856cf-108">Permissions</span></span>
<span data-ttu-id="856cf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="856cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="856cf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="856cf-111">Permission type</span></span>      | <span data-ttu-id="856cf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="856cf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="856cf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="856cf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="856cf-114">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="856cf-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="856cf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="856cf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="856cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="856cf-116">Not supported.</span></span>    |
|<span data-ttu-id="856cf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="856cf-117">Application</span></span> | <span data-ttu-id="856cf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="856cf-118">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="856cf-119">此外，对于委派的流程，登录用户只能删除他们自己 (的 Schemaextension，其中 schemaExtension 的 **owner** 属性是 `appId` 登录用户拥有) 的应用程序的所有者属性。</span><span class="sxs-lookup"><span data-stu-id="856cf-119">Additionally for the delegated flow, the signed-in user can only delete schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="856cf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="856cf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="856cf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="856cf-121">Request headers</span></span>
| <span data-ttu-id="856cf-122">名称</span><span class="sxs-lookup"><span data-stu-id="856cf-122">Name</span></span>      |<span data-ttu-id="856cf-123">说明</span><span class="sxs-lookup"><span data-stu-id="856cf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="856cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="856cf-124">Authorization</span></span>  | <span data-ttu-id="856cf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="856cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="856cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="856cf-127">Request body</span></span>
<span data-ttu-id="856cf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="856cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="856cf-129">响应</span><span class="sxs-lookup"><span data-stu-id="856cf-129">Response</span></span>

<span data-ttu-id="856cf-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="856cf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="856cf-132">示例</span><span class="sxs-lookup"><span data-stu-id="856cf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="856cf-133">请求</span><span class="sxs-lookup"><span data-stu-id="856cf-133">Request</span></span>
<span data-ttu-id="856cf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="856cf-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="856cf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="856cf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="856cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="856cf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="856cf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="856cf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="856cf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="856cf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="856cf-139">响应</span><span class="sxs-lookup"><span data-stu-id="856cf-139">Response</span></span>
<span data-ttu-id="856cf-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="856cf-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="856cf-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="856cf-141">See also</span></span>

- [<span data-ttu-id="856cf-142">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="856cf-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="856cf-143">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="856cf-143">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


