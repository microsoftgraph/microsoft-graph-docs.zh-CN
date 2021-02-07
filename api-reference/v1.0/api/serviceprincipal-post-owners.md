---
title: servicePrincipal：添加所有者
description: 使用此 API 添加服务主体的所有者。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f45cd696bbd5926927e43902c3cdfcdbc013f4d2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137261"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="62a8e-103">servicePrincipal：添加所有者</span><span class="sxs-lookup"><span data-stu-id="62a8e-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="62a8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62a8e-105">使用此 API 添加 [servicePrincipal](../resources/serviceprincipal.md) 的所有者。</span><span class="sxs-lookup"><span data-stu-id="62a8e-105">Use this API to add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62a8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="62a8e-106">Permissions</span></span>
<span data-ttu-id="62a8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62a8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62a8e-109">Permission type</span></span>      | <span data-ttu-id="62a8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62a8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62a8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62a8e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="62a8e-112">Application.ReadWrite.All 和 Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62a8e-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62a8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62a8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a8e-114">Not supported.</span></span>    |
|<span data-ttu-id="62a8e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62a8e-115">Application</span></span> | <span data-ttu-id="62a8e-116">Application.ReadWrite.OwnedBy 和 Directory.Read.All、Application.ReadWrite.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="62a8e-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62a8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62a8e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="62a8e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62a8e-118">Request headers</span></span>
| <span data-ttu-id="62a8e-119">名称</span><span class="sxs-lookup"><span data-stu-id="62a8e-119">Name</span></span>       | <span data-ttu-id="62a8e-120">说明</span><span class="sxs-lookup"><span data-stu-id="62a8e-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="62a8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62a8e-121">Authorization</span></span> | <span data-ttu-id="62a8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62a8e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62a8e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62a8e-124">Content-Type</span></span> | <span data-ttu-id="62a8e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62a8e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62a8e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62a8e-127">Request body</span></span>
<span data-ttu-id="62a8e-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62a8e-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="62a8e-129">响应</span><span class="sxs-lookup"><span data-stu-id="62a8e-129">Response</span></span>

<span data-ttu-id="62a8e-130">如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62a8e-130">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62a8e-131">示例</span><span class="sxs-lookup"><span data-stu-id="62a8e-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="62a8e-132">请求</span><span class="sxs-lookup"><span data-stu-id="62a8e-132">Request</span></span>
<span data-ttu-id="62a8e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62a8e-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62a8e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="62a8e-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62a8e-135">C#</span><span class="sxs-lookup"><span data-stu-id="62a8e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62a8e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62a8e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62a8e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62a8e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62a8e-138">Java</span><span class="sxs-lookup"><span data-stu-id="62a8e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="62a8e-139">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62a8e-139">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="62a8e-140">响应</span><span class="sxs-lookup"><span data-stu-id="62a8e-140">Response</span></span>
<span data-ttu-id="62a8e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62a8e-141">The following is an example of the response.</span></span>

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

