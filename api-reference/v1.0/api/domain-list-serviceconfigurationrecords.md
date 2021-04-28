---
title: 列出 serviceConfigurationRecords
description: 检索为域启用服务所需的 domainDnsRecord 对象列表。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cb04790296aa1c6e1c934c8d37db28e9d1cd7620
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054061"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="ac654-103">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="ac654-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="ac654-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac654-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac654-105">检索为域启用服务所需的 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ac654-105">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="ac654-106">使用返回的列表将记录添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="ac654-106">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="ac654-107">这可以通过域注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="ac654-107">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac654-108">权限</span><span class="sxs-lookup"><span data-stu-id="ac654-108">Permissions</span></span>

<span data-ttu-id="ac654-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac654-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ac654-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac654-111">Permission type</span></span>      | <span data-ttu-id="ac654-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac654-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac654-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac654-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac654-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac654-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="ac654-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac654-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac654-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac654-116">Not supported.</span></span>    |
|<span data-ttu-id="ac654-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac654-117">Application</span></span> | <span data-ttu-id="ac654-118">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac654-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac654-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac654-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac654-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac654-120">Optional query parameters</span></span>

<span data-ttu-id="ac654-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac654-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac654-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac654-122">Request headers</span></span>

| <span data-ttu-id="ac654-123">名称</span><span class="sxs-lookup"><span data-stu-id="ac654-123">Name</span></span>      |<span data-ttu-id="ac654-124">说明</span><span class="sxs-lookup"><span data-stu-id="ac654-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac654-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac654-125">Authorization</span></span>  | <span data-ttu-id="ac654-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac654-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac654-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac654-128">Content-Type</span></span>  | <span data-ttu-id="ac654-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ac654-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac654-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac654-130">Request body</span></span>

<span data-ttu-id="ac654-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac654-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac654-132">响应</span><span class="sxs-lookup"><span data-stu-id="ac654-132">Response</span></span>

<span data-ttu-id="ac654-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac654-133">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac654-134">示例</span><span class="sxs-lookup"><span data-stu-id="ac654-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac654-135">请求</span><span class="sxs-lookup"><span data-stu-id="ac654-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ac654-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac654-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
# <a name="c"></a>[<span data-ttu-id="ac654-137">C#</span><span class="sxs-lookup"><span data-stu-id="ac654-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac654-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac654-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac654-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac654-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac654-140">Java</span><span class="sxs-lookup"><span data-stu-id="ac654-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ac654-141">响应</span><span class="sxs-lookup"><span data-stu-id="ac654-141">Response</span></span>
<span data-ttu-id="ac654-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac654-142">Note: The response object shown here might be shortened for readability.</span></span>
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
