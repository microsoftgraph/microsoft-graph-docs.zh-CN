---
title: 删除 schemaExtension
description: 删除架构扩展定义。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: f8e5d78d0f23430bbd693832a918374af736d1bd
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863493"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="133e1-103">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="133e1-103">Delete schemaExtension</span></span>

<span data-ttu-id="133e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="133e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="133e1-105">删除[架构扩展](../resources/schemaextension.md)定义。</span><span class="sxs-lookup"><span data-stu-id="133e1-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="133e1-106">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state.</span><span class="sxs-lookup"><span data-stu-id="133e1-106">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state.</span></span> <span data-ttu-id="133e1-107">Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span><span class="sxs-lookup"><span data-stu-id="133e1-107">Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="133e1-108">权限</span><span class="sxs-lookup"><span data-stu-id="133e1-108">Permissions</span></span>
<span data-ttu-id="133e1-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="133e1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="133e1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="133e1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="133e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="133e1-111">Permission type</span></span>      | <span data-ttu-id="133e1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="133e1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="133e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="133e1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="133e1-114">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="133e1-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="133e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="133e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="133e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="133e1-116">Not supported.</span></span>    |
|<span data-ttu-id="133e1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="133e1-117">Application</span></span> | <span data-ttu-id="133e1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="133e1-118">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="133e1-119">此外，对于委派的流程，登录用户只能删除他们拥有的 Schemaextension （其中 schemaExtension 的**owner**属性是 `appId` 登录用户拥有的应用程序的）。</span><span class="sxs-lookup"><span data-stu-id="133e1-119">Additionally for the delegated flow, the signed-in user can only delete schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="133e1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="133e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="133e1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="133e1-121">Request headers</span></span>
| <span data-ttu-id="133e1-122">名称</span><span class="sxs-lookup"><span data-stu-id="133e1-122">Name</span></span>      |<span data-ttu-id="133e1-123">说明</span><span class="sxs-lookup"><span data-stu-id="133e1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="133e1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="133e1-124">Authorization</span></span>  | <span data-ttu-id="133e1-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="133e1-125">Bearer {token}.</span></span> <span data-ttu-id="133e1-126">Required.</span><span class="sxs-lookup"><span data-stu-id="133e1-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="133e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="133e1-127">Request body</span></span>
<span data-ttu-id="133e1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="133e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="133e1-129">响应</span><span class="sxs-lookup"><span data-stu-id="133e1-129">Response</span></span>

<span data-ttu-id="133e1-130">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="133e1-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="133e1-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="133e1-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="133e1-132">示例</span><span class="sxs-lookup"><span data-stu-id="133e1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="133e1-133">请求</span><span class="sxs-lookup"><span data-stu-id="133e1-133">Request</span></span>
<span data-ttu-id="133e1-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="133e1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="133e1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="133e1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="133e1-136">C#</span><span class="sxs-lookup"><span data-stu-id="133e1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="133e1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="133e1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="133e1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="133e1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="133e1-139">响应</span><span class="sxs-lookup"><span data-stu-id="133e1-139">Response</span></span>
<span data-ttu-id="133e1-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="133e1-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="133e1-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="133e1-141">See also</span></span>

- [<span data-ttu-id="133e1-142">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="133e1-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="133e1-143">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="133e1-143">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
