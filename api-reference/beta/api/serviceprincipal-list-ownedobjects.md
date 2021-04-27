---
title: servicePrincipals： ownedObjects 列表
description: 检索 servicePrincipal 所拥有的对象列表。  这可能包含应用程序或组。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fbb61ab1fd37c8bf322b144974eee7b799bf6650
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051884"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="b1f7f-104">servicePrincipals： ownedObjects 列表</span><span class="sxs-lookup"><span data-stu-id="b1f7f-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="b1f7f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1f7f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1f7f-106">检索[servicePrincipal](../resources/serviceprincipal.md)所拥有的对象列表。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="b1f7f-107">这可能包含应用程序或组。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1f7f-108">权限</span><span class="sxs-lookup"><span data-stu-id="b1f7f-108">Permissions</span></span>
<span data-ttu-id="b1f7f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1f7f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1f7f-111">Permission type</span></span>      | <span data-ttu-id="b1f7f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1f7f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1f7f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1f7f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1f7f-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1f7f-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1f7f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1f7f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1f7f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-116">Not supported.</span></span>    |
|<span data-ttu-id="b1f7f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1f7f-117">Application</span></span> | <span data-ttu-id="b1f7f-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f7f-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b1f7f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1f7f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1f7f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b1f7f-120">Optional query parameters</span></span>
<span data-ttu-id="b1f7f-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1f7f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1f7f-122">Request headers</span></span>
| <span data-ttu-id="b1f7f-123">名称</span><span class="sxs-lookup"><span data-stu-id="b1f7f-123">Name</span></span>           | <span data-ttu-id="b1f7f-124">说明</span><span class="sxs-lookup"><span data-stu-id="b1f7f-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b1f7f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1f7f-125">Authorization</span></span>  | <span data-ttu-id="b1f7f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1f7f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1f7f-128">Request body</span></span>
<span data-ttu-id="b1f7f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1f7f-130">响应</span><span class="sxs-lookup"><span data-stu-id="b1f7f-130">Response</span></span>

<span data-ttu-id="b1f7f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="b1f7f-132">示例</span><span class="sxs-lookup"><span data-stu-id="b1f7f-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b1f7f-133">请求</span><span class="sxs-lookup"><span data-stu-id="b1f7f-133">Request</span></span>
<span data-ttu-id="b1f7f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1f7f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1f7f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="b1f7f-136">C#</span><span class="sxs-lookup"><span data-stu-id="b1f7f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1f7f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1f7f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1f7f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1f7f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1f7f-139">Java</span><span class="sxs-lookup"><span data-stu-id="b1f7f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b1f7f-140">响应</span><span class="sxs-lookup"><span data-stu-id="b1f7f-140">Response</span></span>
<span data-ttu-id="b1f7f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-141">Here is an example of the response.</span></span> 
><span data-ttu-id="b1f7f-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1f7f-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

