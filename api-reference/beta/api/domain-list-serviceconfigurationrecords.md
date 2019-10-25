---
title: 列出 serviceConfigurationRecords
description: 检索为域启用服务所需的 domainDnsRecord 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 509a69c4f2caf254398809debf5e49544a2272ae
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37724653"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="235ef-103">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="235ef-103">List serviceConfigurationRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="235ef-104">检索为域启用服务所需的[domainDnsRecord](../resources/domaindnsrecord.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="235ef-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="235ef-105">使用返回的列表将记录添加到域的区域文件中。</span><span class="sxs-lookup"><span data-stu-id="235ef-105">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="235ef-106">可以通过域注册机构或 DNS 服务器配置来完成此操作。</span><span class="sxs-lookup"><span data-stu-id="235ef-106">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="235ef-107">权限</span><span class="sxs-lookup"><span data-stu-id="235ef-107">Permissions</span></span>

<span data-ttu-id="235ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="235ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="235ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="235ef-110">Permission type</span></span>      | <span data-ttu-id="235ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="235ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="235ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="235ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="235ef-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="235ef-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="235ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="235ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="235ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="235ef-115">Not supported.</span></span>    |
|<span data-ttu-id="235ef-116">Application</span><span class="sxs-lookup"><span data-stu-id="235ef-116">Application</span></span> | <span data-ttu-id="235ef-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="235ef-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="235ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="235ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="235ef-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="235ef-119">Optional query parameters</span></span>

<span data-ttu-id="235ef-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="235ef-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="235ef-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="235ef-121">Request headers</span></span>

| <span data-ttu-id="235ef-122">名称</span><span class="sxs-lookup"><span data-stu-id="235ef-122">Name</span></span>      |<span data-ttu-id="235ef-123">说明</span><span class="sxs-lookup"><span data-stu-id="235ef-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="235ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="235ef-124">Authorization</span></span>  | <span data-ttu-id="235ef-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="235ef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="235ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="235ef-127">Content-Type</span></span>  | <span data-ttu-id="235ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="235ef-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="235ef-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="235ef-129">Request body</span></span>

<span data-ttu-id="235ef-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="235ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="235ef-131">响应</span><span class="sxs-lookup"><span data-stu-id="235ef-131">Response</span></span>

<span data-ttu-id="235ef-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[domainDnsRecord](../resources/domaindnsrecord.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="235ef-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="235ef-133">示例</span><span class="sxs-lookup"><span data-stu-id="235ef-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="235ef-134">请求</span><span class="sxs-lookup"><span data-stu-id="235ef-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="235ef-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="235ef-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="235ef-136">C#</span><span class="sxs-lookup"><span data-stu-id="235ef-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="235ef-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235ef-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="235ef-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235ef-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="235ef-139">响应</span><span class="sxs-lookup"><span data-stu-id="235ef-139">Response</span></span>
<span data-ttu-id="235ef-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="235ef-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
