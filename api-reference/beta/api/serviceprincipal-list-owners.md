---
title: 'servicePrincipals: 列出所有者'
description: 检索 servicePrincipal 的所有者的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 64ce3cee24711d72ec651675e49adf2e73ac1164
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134293"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="f8c0e-103">servicePrincipals: 列出所有者</span><span class="sxs-lookup"><span data-stu-id="f8c0e-103">servicePrincipals: List owners</span></span>

<span data-ttu-id="f8c0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8c0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c0e-105">检索 [servicePrincipal](../resources/serviceprincipal.md) 的所有者的列表。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-105">Retrieve a list of owners of the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8c0e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8c0e-106">Permissions</span></span>
<span data-ttu-id="f8c0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8c0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8c0e-109">Permission type</span></span>      | <span data-ttu-id="f8c0e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8c0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8c0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8c0e-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8c0e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8c0e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8c0e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-114">Not supported.</span></span>    |
|<span data-ttu-id="f8c0e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8c0e-115">Application</span></span> | <span data-ttu-id="f8c0e-116">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c0e-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f8c0e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8c0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8c0e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8c0e-118">Optional query parameters</span></span>
<span data-ttu-id="f8c0e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8c0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8c0e-120">Request headers</span></span>
| <span data-ttu-id="f8c0e-121">名称</span><span class="sxs-lookup"><span data-stu-id="f8c0e-121">Name</span></span>           | <span data-ttu-id="f8c0e-122">说明</span><span class="sxs-lookup"><span data-stu-id="f8c0e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f8c0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c0e-123">Authorization</span></span>  | <span data-ttu-id="f8c0e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8c0e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8c0e-126">Request body</span></span>
<span data-ttu-id="f8c0e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8c0e-128">响应</span><span class="sxs-lookup"><span data-stu-id="f8c0e-128">Response</span></span>

<span data-ttu-id="f8c0e-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="f8c0e-130">示例</span><span class="sxs-lookup"><span data-stu-id="f8c0e-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f8c0e-131">请求</span><span class="sxs-lookup"><span data-stu-id="f8c0e-131">Request</span></span>
<span data-ttu-id="f8c0e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f8c0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8c0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="f8c0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="f8c0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8c0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8c0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8c0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8c0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8c0e-137">Java</span><span class="sxs-lookup"><span data-stu-id="f8c0e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8c0e-138">响应</span><span class="sxs-lookup"><span data-stu-id="f8c0e-138">Response</span></span>
<span data-ttu-id="f8c0e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="f8c0e-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8c0e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

