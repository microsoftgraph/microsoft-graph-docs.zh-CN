---
title: servicePrincipal：添加所有者
description: 使用此 API 添加服务主体的所有者。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: cb0f6f8e2ce809a1e3a3dadda209975205616658
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334803"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="612b1-103">servicePrincipal：添加所有者</span><span class="sxs-lookup"><span data-stu-id="612b1-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="612b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="612b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="612b1-105">使用此 API 添加[servicePrincipal](../resources/serviceprincipal.md)的所有者。</span><span class="sxs-lookup"><span data-stu-id="612b1-105">Use this API to add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="612b1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="612b1-106">Permissions</span></span>
<span data-ttu-id="612b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="612b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="612b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="612b1-109">Permission type</span></span>      | <span data-ttu-id="612b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="612b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="612b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="612b1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="612b1-112">Directory.accessasuser.all 和所有目录。全部，全部。</span><span class="sxs-lookup"><span data-stu-id="612b1-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="612b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="612b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="612b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="612b1-114">Not supported.</span></span>    |
|<span data-ttu-id="612b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="612b1-115">Application</span></span> | <span data-ttu-id="612b1-116">Application.readwrite.ownedby 和 "全部读取"。全部、全部读取全部和全部读取全部。</span><span class="sxs-lookup"><span data-stu-id="612b1-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="612b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="612b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="612b1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="612b1-118">Request headers</span></span>
| <span data-ttu-id="612b1-119">名称</span><span class="sxs-lookup"><span data-stu-id="612b1-119">Name</span></span>       | <span data-ttu-id="612b1-120">说明</span><span class="sxs-lookup"><span data-stu-id="612b1-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="612b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="612b1-121">Authorization</span></span> | <span data-ttu-id="612b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="612b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="612b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="612b1-124">Content-Type</span></span> | <span data-ttu-id="612b1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="612b1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="612b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="612b1-127">Request body</span></span>
<span data-ttu-id="612b1-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="612b1-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="612b1-129">响应</span><span class="sxs-lookup"><span data-stu-id="612b1-129">Response</span></span>

<span data-ttu-id="612b1-130">如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="612b1-130">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="612b1-131">示例</span><span class="sxs-lookup"><span data-stu-id="612b1-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="612b1-132">请求</span><span class="sxs-lookup"><span data-stu-id="612b1-132">Request</span></span>
<span data-ttu-id="612b1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="612b1-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="612b1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="612b1-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="612b1-135">C#</span><span class="sxs-lookup"><span data-stu-id="612b1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="612b1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="612b1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="612b1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="612b1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="612b1-138">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="612b1-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="612b1-139">响应</span><span class="sxs-lookup"><span data-stu-id="612b1-139">Response</span></span>
<span data-ttu-id="612b1-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="612b1-140">The following is an example of the response.</span></span>

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
