---
title: 列出域
description: 检索域对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c957631112ed80161f00e82024b0d380cb8c8c39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433494"
---
# <a name="list-domains"></a><span data-ttu-id="9fba8-103">列出域</span><span class="sxs-lookup"><span data-stu-id="9fba8-103">List domains</span></span>

<span data-ttu-id="9fba8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9fba8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fba8-105">检索域对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9fba8-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fba8-106">权限</span><span class="sxs-lookup"><span data-stu-id="9fba8-106">Permissions</span></span>
<span data-ttu-id="9fba8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fba8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fba8-109">Permission type</span></span>      | <span data-ttu-id="9fba8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fba8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fba8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fba8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9fba8-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fba8-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="9fba8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fba8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fba8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fba8-114">Not supported.</span></span>    |
|<span data-ttu-id="9fba8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fba8-115">Application</span></span> | <span data-ttu-id="9fba8-116">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fba8-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fba8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fba8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9fba8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9fba8-118">Optional query parameters</span></span>
<span data-ttu-id="9fba8-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9fba8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fba8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fba8-120">Request headers</span></span>
| <span data-ttu-id="9fba8-121">名称</span><span class="sxs-lookup"><span data-stu-id="9fba8-121">Name</span></span>      |<span data-ttu-id="9fba8-122">说明</span><span class="sxs-lookup"><span data-stu-id="9fba8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9fba8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fba8-123">Authorization</span></span>  | <span data-ttu-id="9fba8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fba8-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9fba8-126">接受</span><span class="sxs-lookup"><span data-stu-id="9fba8-126">Accept</span></span>         | <span data-ttu-id="9fba8-127">application/json;</span><span class="sxs-lookup"><span data-stu-id="9fba8-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fba8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fba8-128">Request body</span></span>
<span data-ttu-id="9fba8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fba8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fba8-130">响应</span><span class="sxs-lookup"><span data-stu-id="9fba8-130">Response</span></span>

<span data-ttu-id="9fba8-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[domain](../resources/domain.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9fba8-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9fba8-132">示例</span><span class="sxs-lookup"><span data-stu-id="9fba8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fba8-133">请求</span><span class="sxs-lookup"><span data-stu-id="9fba8-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9fba8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fba8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains
```
# <a name="c"></a>[<span data-ttu-id="9fba8-135">C#</span><span class="sxs-lookup"><span data-stu-id="9fba8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fba8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fba8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fba8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fba8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9fba8-138">响应</span><span class="sxs-lookup"><span data-stu-id="9fba8-138">Response</span></span>
<span data-ttu-id="9fba8-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fba8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
