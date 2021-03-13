---
title: 删除 directoryObject
description: 删除 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 62a4d9f6d83df0eaa80be7262a9d3057fe28d724
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769977"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="df0ab-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="df0ab-103">Delete directoryObject</span></span>

<span data-ttu-id="df0ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df0ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df0ab-105">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="df0ab-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="df0ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="df0ab-106">Permissions</span></span>
<span data-ttu-id="df0ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df0ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df0ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df0ab-109">Permission type</span></span>      | <span data-ttu-id="df0ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df0ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df0ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df0ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df0ab-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df0ab-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df0ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df0ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df0ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df0ab-114">Not supported.</span></span>    |
|<span data-ttu-id="df0ab-115">Application</span><span class="sxs-lookup"><span data-stu-id="df0ab-115">Application</span></span> | <span data-ttu-id="df0ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df0ab-116">Not supported.</span></span> |

<span data-ttu-id="df0ab-117">**注意：** 用户、组和联系人是 directory 对象的类型。</span><span class="sxs-lookup"><span data-stu-id="df0ab-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="df0ab-118">因此，如果需要删除用户，可以并且应该使用以下权限：User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0ab-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="df0ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df0ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="df0ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df0ab-120">Request headers</span></span>
| <span data-ttu-id="df0ab-121">名称</span><span class="sxs-lookup"><span data-stu-id="df0ab-121">Name</span></span>       | <span data-ttu-id="df0ab-122">类型</span><span class="sxs-lookup"><span data-stu-id="df0ab-122">Type</span></span> | <span data-ttu-id="df0ab-123">说明</span><span class="sxs-lookup"><span data-stu-id="df0ab-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="df0ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df0ab-124">Authorization</span></span>  | <span data-ttu-id="df0ab-125">string</span><span class="sxs-lookup"><span data-stu-id="df0ab-125">string</span></span>  | <span data-ttu-id="df0ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df0ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df0ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="df0ab-128">Request body</span></span>
<span data-ttu-id="df0ab-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df0ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df0ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="df0ab-130">Response</span></span>

<span data-ttu-id="df0ab-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="df0ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0ab-133">示例</span><span class="sxs-lookup"><span data-stu-id="df0ab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df0ab-134">请求</span><span class="sxs-lookup"><span data-stu-id="df0ab-134">Request</span></span>
<span data-ttu-id="df0ab-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df0ab-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df0ab-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="df0ab-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
# <a name="c"></a>[<span data-ttu-id="df0ab-137">C#</span><span class="sxs-lookup"><span data-stu-id="df0ab-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df0ab-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df0ab-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df0ab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df0ab-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df0ab-140">Java</span><span class="sxs-lookup"><span data-stu-id="df0ab-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="df0ab-141">响应</span><span class="sxs-lookup"><span data-stu-id="df0ab-141">Response</span></span>
<span data-ttu-id="df0ab-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="df0ab-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


