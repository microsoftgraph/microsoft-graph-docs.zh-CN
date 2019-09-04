---
title: 列出 verificationDnsRecords
description: 检索 domainDnsRecord 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 919996c9e9f6d989f943a6aaba95793f51b694b0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718121"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="96eee-103">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="96eee-103">List verificationDnsRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96eee-104">检索[domainDnsRecord](../resources/domaindnsrecord.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="96eee-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="96eee-105">在验证所有权之前, 不能使用 Azure AD 租户相关联的域。</span><span class="sxs-lookup"><span data-stu-id="96eee-105">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="96eee-106">若要验证域的所有权, 请检索域验证记录并将详细信息添加到域的区域文件中。</span><span class="sxs-lookup"><span data-stu-id="96eee-106">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="96eee-107">可以通过域注册机构或 DNS 服务器配置来完成此操作。</span><span class="sxs-lookup"><span data-stu-id="96eee-107">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="96eee-108">根域需要验证。</span><span class="sxs-lookup"><span data-stu-id="96eee-108">Root domains require verification.</span></span> <span data-ttu-id="96eee-109">例如, contoso.com 需要验证。</span><span class="sxs-lookup"><span data-stu-id="96eee-109">For example, contoso.com requires verification.</span></span> <span data-ttu-id="96eee-110">如果验证了根域, 则会自动验证根域的子域。</span><span class="sxs-lookup"><span data-stu-id="96eee-110">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="96eee-111">例如, 如果 contoso.com 已经过验证, 则会自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="96eee-111">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="96eee-112">权限</span><span class="sxs-lookup"><span data-stu-id="96eee-112">Permissions</span></span>

<span data-ttu-id="96eee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96eee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96eee-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="96eee-115">Permission type</span></span>      | <span data-ttu-id="96eee-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96eee-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96eee-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96eee-117">Delegated (work or school account)</span></span> | <span data-ttu-id="96eee-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96eee-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="96eee-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96eee-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96eee-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="96eee-120">Not supported.</span></span>    |
|<span data-ttu-id="96eee-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="96eee-121">Application</span></span> | <span data-ttu-id="96eee-122">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96eee-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96eee-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96eee-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="96eee-124">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="96eee-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="96eee-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96eee-125">Optional query parameters</span></span>

<span data-ttu-id="96eee-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96eee-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96eee-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="96eee-127">Request headers</span></span>

| <span data-ttu-id="96eee-128">名称</span><span class="sxs-lookup"><span data-stu-id="96eee-128">Name</span></span>      |<span data-ttu-id="96eee-129">说明</span><span class="sxs-lookup"><span data-stu-id="96eee-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96eee-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="96eee-130">Authorization</span></span>  | <span data-ttu-id="96eee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96eee-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96eee-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96eee-133">Content-Type</span></span>  | <span data-ttu-id="96eee-134">application/json</span><span class="sxs-lookup"><span data-stu-id="96eee-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="96eee-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="96eee-135">Request body</span></span>

<span data-ttu-id="96eee-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96eee-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96eee-137">响应</span><span class="sxs-lookup"><span data-stu-id="96eee-137">Response</span></span>

<span data-ttu-id="96eee-138">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[domainDnsRecord](../resources/domaindnsrecord.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="96eee-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96eee-139">示例</span><span class="sxs-lookup"><span data-stu-id="96eee-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96eee-140">请求</span><span class="sxs-lookup"><span data-stu-id="96eee-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96eee-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="96eee-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96eee-142">C#</span><span class="sxs-lookup"><span data-stu-id="96eee-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-verificationdnsrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96eee-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96eee-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-verificationdnsrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96eee-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="96eee-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-verificationdnsrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96eee-145">响应</span><span class="sxs-lookup"><span data-stu-id="96eee-145">Response</span></span>

<span data-ttu-id="96eee-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96eee-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
