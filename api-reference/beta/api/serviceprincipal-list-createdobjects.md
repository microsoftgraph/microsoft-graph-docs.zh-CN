---
title: 'servicePrincipal: List createdObjects'
description: 检索 directoryObject 对象列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 23f93a48e808a72e312c55def59fae0a89d6daeb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053487"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="8da0a-103">servicePrincipal: List createdObjects</span><span class="sxs-lookup"><span data-stu-id="8da0a-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="8da0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da0a-105">检索 directoryObject 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8da0a-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8da0a-106">Permissions</span></span>
<span data-ttu-id="8da0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8da0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8da0a-109">Permission type</span></span>      | <span data-ttu-id="8da0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8da0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8da0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8da0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8da0a-112">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8da0a-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8da0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8da0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8da0a-114">Not supported.</span></span>    |
|<span data-ttu-id="8da0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8da0a-115">Application</span></span> | <span data-ttu-id="8da0a-116">Application.Read.All、 Directory.Read.All、 Application.ReadWrite.OwnedBy、 Application.ReadWrite.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da0a-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8da0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8da0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8da0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8da0a-118">Optional query parameters</span></span>
<span data-ttu-id="8da0a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8da0a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8da0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8da0a-120">Request headers</span></span>
| <span data-ttu-id="8da0a-121">名称</span><span class="sxs-lookup"><span data-stu-id="8da0a-121">Name</span></span>           | <span data-ttu-id="8da0a-122">说明</span><span class="sxs-lookup"><span data-stu-id="8da0a-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8da0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da0a-123">Authorization</span></span>  | <span data-ttu-id="8da0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8da0a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8da0a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8da0a-126">Request body</span></span>
<span data-ttu-id="8da0a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8da0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da0a-128">响应</span><span class="sxs-lookup"><span data-stu-id="8da0a-128">Response</span></span>

<span data-ttu-id="8da0a-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8da0a-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="8da0a-130">示例</span><span class="sxs-lookup"><span data-stu-id="8da0a-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="8da0a-131">请求</span><span class="sxs-lookup"><span data-stu-id="8da0a-131">Request</span></span>
<span data-ttu-id="8da0a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8da0a-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8da0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8da0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="8da0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8da0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8da0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8da0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8da0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8da0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8da0a-137">Java</span><span class="sxs-lookup"><span data-stu-id="8da0a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8da0a-138">响应</span><span class="sxs-lookup"><span data-stu-id="8da0a-138">Response</span></span>
<span data-ttu-id="8da0a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8da0a-139">Here is an example of the response.</span></span> 
><span data-ttu-id="8da0a-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8da0a-140">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

