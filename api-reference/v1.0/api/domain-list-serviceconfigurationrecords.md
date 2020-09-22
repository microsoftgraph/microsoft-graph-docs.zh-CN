---
title: 列出 serviceConfigurationRecords
description: 检索为域启用服务所需的 domainDnsRecord 对象的列表。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7b60fb266f5ed21bb59382fb14ade1964bbf6c9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042273"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="a005d-103">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="a005d-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="a005d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a005d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a005d-105">检索为域启用服务所需的 [domainDnsRecord](../resources/domaindnsrecord.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a005d-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="a005d-106">使用返回的列表将记录添加到域的区域文件中。</span><span class="sxs-lookup"><span data-stu-id="a005d-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="a005d-107">可以通过域注册机构或 DNS 服务器配置来完成此操作。</span><span class="sxs-lookup"><span data-stu-id="a005d-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="a005d-108">权限</span><span class="sxs-lookup"><span data-stu-id="a005d-108">Permissions</span></span>

<span data-ttu-id="a005d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a005d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a005d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a005d-111">Permission type</span></span>      | <span data-ttu-id="a005d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a005d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a005d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a005d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a005d-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a005d-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="a005d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a005d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a005d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a005d-116">Not supported.</span></span>    |
|<span data-ttu-id="a005d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a005d-117">Application</span></span> | <span data-ttu-id="a005d-118">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a005d-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a005d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a005d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a005d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a005d-120">Optional query parameters</span></span>

<span data-ttu-id="a005d-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a005d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a005d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a005d-122">Request headers</span></span>

| <span data-ttu-id="a005d-123">名称</span><span class="sxs-lookup"><span data-stu-id="a005d-123">Name</span></span>      |<span data-ttu-id="a005d-124">说明</span><span class="sxs-lookup"><span data-stu-id="a005d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a005d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a005d-125">Authorization</span></span>  | <span data-ttu-id="a005d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a005d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a005d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a005d-128">Content-Type</span></span>  | <span data-ttu-id="a005d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a005d-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a005d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a005d-130">Request body</span></span>

<span data-ttu-id="a005d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a005d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a005d-132">响应</span><span class="sxs-lookup"><span data-stu-id="a005d-132">Response</span></span>

<span data-ttu-id="a005d-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a005d-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a005d-134">示例</span><span class="sxs-lookup"><span data-stu-id="a005d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a005d-135">请求</span><span class="sxs-lookup"><span data-stu-id="a005d-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a005d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a005d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="a005d-137">C#</span><span class="sxs-lookup"><span data-stu-id="a005d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a005d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a005d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a005d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a005d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a005d-140">Java</span><span class="sxs-lookup"><span data-stu-id="a005d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a005d-141">响应</span><span class="sxs-lookup"><span data-stu-id="a005d-141">Response</span></span>
<span data-ttu-id="a005d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a005d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type":"microsoft.graph.domainDnsMxRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "@odata.type":"microsoft.graph.domainDnsTxtRecord",
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedService": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

