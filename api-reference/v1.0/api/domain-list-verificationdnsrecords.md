---
title: 列出 verificationDnsRecords
description: 检索 domainDnsRecord 对象列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e0339b9bf50551d9bcb10ad2c5c582beabc4c9b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927231"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="8f1c3-103">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="8f1c3-103">List verificationDnsRecords</span></span>

<span data-ttu-id="8f1c3-104">检索 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="8f1c3-p101">必须完成所有权验证，才可以使用与 Azure AD 租户关联的域。若要验证该域的所有权，请检索域验证记录并向该阈的区域文件添加详细信息。这可以通过域名注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="8f1c3-p102">需要对根域进行验证。例如，需要对 contoso.com 进行验证。如果已验证根域，则将自动验证该根域的子域。例如，如果已验证 contoso.com，则将自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f1c3-112">权限</span><span class="sxs-lookup"><span data-stu-id="8f1c3-112">Permissions</span></span>

<span data-ttu-id="8f1c3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f1c3-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f1c3-115">Permission type</span></span>      | <span data-ttu-id="8f1c3-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f1c3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f1c3-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f1c3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8f1c3-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f1c3-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="8f1c3-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f1c3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f1c3-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-120">Not supported.</span></span>    |
|<span data-ttu-id="8f1c3-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f1c3-121">Application</span></span> | <span data-ttu-id="8f1c3-122">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f1c3-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f1c3-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f1c3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="8f1c3-124">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8f1c3-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8f1c3-125">Optional query parameters</span></span>

<span data-ttu-id="8f1c3-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f1c3-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f1c3-127">Request headers</span></span>

| <span data-ttu-id="8f1c3-128">名称</span><span class="sxs-lookup"><span data-stu-id="8f1c3-128">Name</span></span>      |<span data-ttu-id="8f1c3-129">说明</span><span class="sxs-lookup"><span data-stu-id="8f1c3-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f1c3-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f1c3-130">Authorization</span></span>  | <span data-ttu-id="8f1c3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f1c3-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f1c3-133">Content-Type</span></span>  | <span data-ttu-id="8f1c3-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8f1c3-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f1c3-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f1c3-135">Request body</span></span>

<span data-ttu-id="8f1c3-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f1c3-137">响应</span><span class="sxs-lookup"><span data-stu-id="8f1c3-137">Response</span></span>

<span data-ttu-id="8f1c3-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f1c3-139">示例</span><span class="sxs-lookup"><span data-stu-id="8f1c3-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f1c3-140">请求</span><span class="sxs-lookup"><span data-stu-id="8f1c3-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="8f1c3-141">响应</span><span class="sxs-lookup"><span data-stu-id="8f1c3-141">Response</span></span>

<span data-ttu-id="8f1c3-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f1c3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
