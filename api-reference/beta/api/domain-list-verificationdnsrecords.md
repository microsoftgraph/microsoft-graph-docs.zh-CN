---
title: 列出 verificationDnsRecords
description: 检索 domainDnsRecord 对象列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a470f6bddb9cade8083afb3eb5d5cf76cf4dba32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522838"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="4b698-103">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="4b698-103">List verificationDnsRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b698-104">检索 [domainDnsRecord](../resources/domaindnsrecord.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4b698-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="4b698-p101">必须完成所有权验证，才可以使用与 Azure AD 租户关联的域。若要验证该域的所有权，请检索域验证记录并向该阈的区域文件添加详细信息。这可以通过域名注册机构或 DNS 服务器配置完成。</span><span class="sxs-lookup"><span data-stu-id="4b698-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="4b698-p102">需要对根域进行验证。例如，需要对 contoso.com 进行验证。如果已验证根域，则将自动验证该根域的子域。例如，如果已验证 contoso.com，则将自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="4b698-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b698-112">权限</span><span class="sxs-lookup"><span data-stu-id="4b698-112">Permissions</span></span>

<span data-ttu-id="4b698-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b698-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4b698-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b698-115">Permission type</span></span>      | <span data-ttu-id="4b698-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b698-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b698-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b698-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4b698-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b698-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="4b698-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b698-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b698-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b698-120">Not supported.</span></span>    |
|<span data-ttu-id="4b698-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b698-121">Application</span></span> | <span data-ttu-id="4b698-122">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b698-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b698-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b698-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="4b698-124">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="4b698-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4b698-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b698-125">Optional query parameters</span></span>

<span data-ttu-id="4b698-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b698-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b698-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b698-127">Request headers</span></span>

| <span data-ttu-id="4b698-128">名称</span><span class="sxs-lookup"><span data-stu-id="4b698-128">Name</span></span>      |<span data-ttu-id="4b698-129">说明</span><span class="sxs-lookup"><span data-stu-id="4b698-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b698-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b698-130">Authorization</span></span>  | <span data-ttu-id="4b698-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b698-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b698-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b698-133">Content-Type</span></span>  | <span data-ttu-id="4b698-134">application/json</span><span class="sxs-lookup"><span data-stu-id="4b698-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b698-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b698-135">Request body</span></span>

<span data-ttu-id="4b698-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b698-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b698-137">响应</span><span class="sxs-lookup"><span data-stu-id="4b698-137">Response</span></span>

<span data-ttu-id="4b698-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4b698-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b698-139">示例</span><span class="sxs-lookup"><span data-stu-id="4b698-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b698-140">请求</span><span class="sxs-lookup"><span data-stu-id="4b698-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="4b698-141">响应</span><span class="sxs-lookup"><span data-stu-id="4b698-141">Response</span></span>

<span data-ttu-id="4b698-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b698-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
