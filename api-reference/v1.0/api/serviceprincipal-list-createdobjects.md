---
title: 'servicePrincipal: List createdObjects'
description: 检索 directoryObject 对象列表。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 09afbf6afb215e9a20ca74e32db39113b8d06adf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134580"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="6e2b7-103">servicePrincipal: List createdObjects</span><span class="sxs-lookup"><span data-stu-id="6e2b7-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="6e2b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e2b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e2b7-105">检索 directoryObject 对象列表。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e2b7-106">权限</span><span class="sxs-lookup"><span data-stu-id="6e2b7-106">Permissions</span></span>
<span data-ttu-id="6e2b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e2b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e2b7-109">Permission type</span></span>      | <span data-ttu-id="6e2b7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e2b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e2b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e2b7-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e2b7-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e2b7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e2b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e2b7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-114">Not supported.</span></span>    |
|<span data-ttu-id="6e2b7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e2b7-115">Application</span></span> | <span data-ttu-id="6e2b7-116">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e2b7-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6e2b7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e2b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e2b7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e2b7-118">Optional query parameters</span></span>
<span data-ttu-id="6e2b7-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e2b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e2b7-120">Request headers</span></span>
| <span data-ttu-id="6e2b7-121">名称</span><span class="sxs-lookup"><span data-stu-id="6e2b7-121">Name</span></span>           | <span data-ttu-id="6e2b7-122">说明</span><span class="sxs-lookup"><span data-stu-id="6e2b7-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6e2b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e2b7-123">Authorization</span></span>  | <span data-ttu-id="6e2b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e2b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e2b7-126">Request body</span></span>
<span data-ttu-id="6e2b7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e2b7-128">响应</span><span class="sxs-lookup"><span data-stu-id="6e2b7-128">Response</span></span>

<span data-ttu-id="6e2b7-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6e2b7-130">示例</span><span class="sxs-lookup"><span data-stu-id="6e2b7-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="6e2b7-131">请求</span><span class="sxs-lookup"><span data-stu-id="6e2b7-131">Request</span></span>
<span data-ttu-id="6e2b7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e2b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e2b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="6e2b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="6e2b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e2b7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e2b7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e2b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e2b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e2b7-137">Java</span><span class="sxs-lookup"><span data-stu-id="6e2b7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e2b7-138">响应</span><span class="sxs-lookup"><span data-stu-id="6e2b7-138">Response</span></span>
<span data-ttu-id="6e2b7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e2b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
