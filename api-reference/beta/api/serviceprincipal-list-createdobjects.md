---
title: servicePrincipal： List createdObjects
description: 检索 directoryobject 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 74d23f1fb682cb0c0e06c9d1260d7c478bbdfa43
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219079"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="a7d1e-103">servicePrincipal： List createdObjects</span><span class="sxs-lookup"><span data-stu-id="a7d1e-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="a7d1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7d1e-105">检索 directoryobject 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7d1e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7d1e-106">Permissions</span></span>
<span data-ttu-id="a7d1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d1e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7d1e-109">Permission type</span></span>      | <span data-ttu-id="a7d1e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7d1e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d1e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d1e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7d1e-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7d1e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7d1e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d1e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-114">Not supported.</span></span>    |
|<span data-ttu-id="a7d1e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7d1e-115">Application</span></span> | <span data-ttu-id="a7d1e-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d1e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a7d1e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7d1e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7d1e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7d1e-118">Optional query parameters</span></span>
<span data-ttu-id="a7d1e-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7d1e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7d1e-120">Request headers</span></span>
| <span data-ttu-id="a7d1e-121">名称</span><span class="sxs-lookup"><span data-stu-id="a7d1e-121">Name</span></span>       | <span data-ttu-id="a7d1e-122">类型</span><span class="sxs-lookup"><span data-stu-id="a7d1e-122">Type</span></span> | <span data-ttu-id="a7d1e-123">说明</span><span class="sxs-lookup"><span data-stu-id="a7d1e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7d1e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d1e-124">Authorization</span></span>  | <span data-ttu-id="a7d1e-125">string</span><span class="sxs-lookup"><span data-stu-id="a7d1e-125">string</span></span>  | <span data-ttu-id="a7d1e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7d1e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7d1e-128">Request body</span></span>
<span data-ttu-id="a7d1e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d1e-130">响应</span><span class="sxs-lookup"><span data-stu-id="a7d1e-130">Response</span></span>

<span data-ttu-id="a7d1e-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7d1e-132">示例</span><span class="sxs-lookup"><span data-stu-id="a7d1e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d1e-133">请求</span><span class="sxs-lookup"><span data-stu-id="a7d1e-133">Request</span></span>
<span data-ttu-id="a7d1e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7d1e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d1e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="a7d1e-136">C#</span><span class="sxs-lookup"><span data-stu-id="a7d1e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7d1e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7d1e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7d1e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7d1e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7d1e-139">响应</span><span class="sxs-lookup"><span data-stu-id="a7d1e-139">Response</span></span>
<span data-ttu-id="a7d1e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7d1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
