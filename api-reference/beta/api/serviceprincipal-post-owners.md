---
title: 'servicePrincipal: 添加所有者'
description: 添加服务主体的所有者。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fb13fe1249cedc3a1adce81e9d13f1559e06970e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979626"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="365d9-103">servicePrincipal: 添加所有者</span><span class="sxs-lookup"><span data-stu-id="365d9-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="365d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="365d9-105">添加 [servicePrincipal](../resources/serviceprincipal.md) 的所有者。</span><span class="sxs-lookup"><span data-stu-id="365d9-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="365d9-106">权限</span><span class="sxs-lookup"><span data-stu-id="365d9-106">Permissions</span></span>
<span data-ttu-id="365d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="365d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365d9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="365d9-109">Permission type</span></span>      | <span data-ttu-id="365d9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="365d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="365d9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="365d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="365d9-112">Application.ReadWrite.All 和Directory.Read.All、 Application.ReadWrite.All 和Directory.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="365d9-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="365d9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="365d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="365d9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="365d9-114">Not supported.</span></span>    |
|<span data-ttu-id="365d9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="365d9-115">Application</span></span> | <span data-ttu-id="365d9-116">Application.ReadWrite.OwnedBy 和Directory.Read.All、 Application.ReadWrite.All 和Directory.Read.All、 Application.ReadWrite.OwnedBy 和Directory.ReadWrite.All、 Application.ReadWrite.All 和Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365d9-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="365d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="365d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="365d9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="365d9-118">Request headers</span></span>
| <span data-ttu-id="365d9-119">名称</span><span class="sxs-lookup"><span data-stu-id="365d9-119">Name</span></span>       | <span data-ttu-id="365d9-120">说明</span><span class="sxs-lookup"><span data-stu-id="365d9-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="365d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="365d9-121">Authorization</span></span> | <span data-ttu-id="365d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="365d9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="365d9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="365d9-124">Request body</span></span>
<span data-ttu-id="365d9-125">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="365d9-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="365d9-126">响应</span><span class="sxs-lookup"><span data-stu-id="365d9-126">Response</span></span>

<span data-ttu-id="365d9-127">如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="365d9-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="365d9-128">示例</span><span class="sxs-lookup"><span data-stu-id="365d9-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="365d9-129">请求</span><span class="sxs-lookup"><span data-stu-id="365d9-129">Request</span></span>
<span data-ttu-id="365d9-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="365d9-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="365d9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="365d9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="365d9-132">C#</span><span class="sxs-lookup"><span data-stu-id="365d9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="365d9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="365d9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="365d9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="365d9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="365d9-135">Java</span><span class="sxs-lookup"><span data-stu-id="365d9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="365d9-136">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="365d9-136">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="365d9-137">响应</span><span class="sxs-lookup"><span data-stu-id="365d9-137">Response</span></span>
<span data-ttu-id="365d9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="365d9-138">The following is an example of the response.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


