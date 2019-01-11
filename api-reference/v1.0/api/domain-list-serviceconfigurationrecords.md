---
title: 列出 serviceConfigurationRecords
description: 检索启用域服务所需的 domainDnsRecord 对象列表。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 958115620d9cf1e8a108c08004bfb124328f15b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825331"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="d94cb-103">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="d94cb-103">List serviceConfigurationRecords</span></span>

<span data-ttu-id="d94cb-104">检索启用域服务所需的 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d94cb-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="d94cb-p101">使用返回的列表将记录添加到域的区域文件。这可以通过域名注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="d94cb-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d94cb-107">权限</span><span class="sxs-lookup"><span data-stu-id="d94cb-107">Permissions</span></span>

<span data-ttu-id="d94cb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d94cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d94cb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d94cb-110">Permission type</span></span>      | <span data-ttu-id="d94cb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d94cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d94cb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d94cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d94cb-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d94cb-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="d94cb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d94cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d94cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d94cb-115">Not supported.</span></span>    |
|<span data-ttu-id="d94cb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d94cb-116">Application</span></span> | <span data-ttu-id="d94cb-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94cb-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d94cb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d94cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d94cb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d94cb-119">Optional query parameters</span></span>

<span data-ttu-id="d94cb-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d94cb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d94cb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d94cb-121">Request headers</span></span>

| <span data-ttu-id="d94cb-122">名称</span><span class="sxs-lookup"><span data-stu-id="d94cb-122">Name</span></span>      |<span data-ttu-id="d94cb-123">说明</span><span class="sxs-lookup"><span data-stu-id="d94cb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d94cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d94cb-124">Authorization</span></span>  | <span data-ttu-id="d94cb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d94cb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d94cb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d94cb-127">Content-Type</span></span>  | <span data-ttu-id="d94cb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d94cb-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d94cb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d94cb-129">Request body</span></span>

<span data-ttu-id="d94cb-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d94cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d94cb-131">响应</span><span class="sxs-lookup"><span data-stu-id="d94cb-131">Response</span></span>

<span data-ttu-id="d94cb-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d94cb-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d94cb-133">示例</span><span class="sxs-lookup"><span data-stu-id="d94cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d94cb-134">请求</span><span class="sxs-lookup"><span data-stu-id="d94cb-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="d94cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="d94cb-135">Response</span></span>
<span data-ttu-id="d94cb-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d94cb-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
