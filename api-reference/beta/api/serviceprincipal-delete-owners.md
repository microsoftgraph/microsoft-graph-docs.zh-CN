---
title: 删除所有者
description: 从 servicePrincipals 中删除所有者。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1250e9917e3021bd235a2c6552fd5ac7480e14c8
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333791"
---
# <a name="remove-owner"></a><span data-ttu-id="20619-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="20619-103">Remove owner</span></span>

<span data-ttu-id="20619-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20619-105">从[servicePrincipal](../resources/serviceprincipal.md)对象中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="20619-105">Remove an owner from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20619-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="20619-106">Permissions</span></span>
<span data-ttu-id="20619-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20619-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20619-109">Permission type</span></span>      | <span data-ttu-id="20619-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20619-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20619-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20619-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20619-112">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="20619-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="20619-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20619-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20619-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20619-114">Not supported.</span></span>    |
|<span data-ttu-id="20619-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20619-115">Application</span></span> | <span data-ttu-id="20619-116">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="20619-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20619-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20619-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /serviceprincipals/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="20619-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="20619-118">Request headers</span></span>
| <span data-ttu-id="20619-119">名称</span><span class="sxs-lookup"><span data-stu-id="20619-119">Name</span></span> | <span data-ttu-id="20619-120">说明</span><span class="sxs-lookup"><span data-stu-id="20619-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="20619-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20619-121">Authorization</span></span> | <span data-ttu-id="20619-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20619-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="20619-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="20619-124">Request body</span></span>
<span data-ttu-id="20619-125">在请求正文中，提供要作为所有者分配的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="20619-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="20619-126">响应</span><span class="sxs-lookup"><span data-stu-id="20619-126">Response</span></span>

<span data-ttu-id="20619-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="20619-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20619-128">示例</span><span class="sxs-lookup"><span data-stu-id="20619-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="20619-129">请求</span><span class="sxs-lookup"><span data-stu-id="20619-129">Request</span></span>

<span data-ttu-id="20619-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="20619-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20619-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="20619-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/serviceprincipals/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="20619-132">C#</span><span class="sxs-lookup"><span data-stu-id="20619-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20619-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20619-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20619-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20619-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20619-135">Java</span><span class="sxs-lookup"><span data-stu-id="20619-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20619-136">响应</span><span class="sxs-lookup"><span data-stu-id="20619-136">Response</span></span>

<span data-ttu-id="20619-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20619-137">The following is an example of the response.</span></span>

><span data-ttu-id="20619-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20619-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="20619-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20619-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
