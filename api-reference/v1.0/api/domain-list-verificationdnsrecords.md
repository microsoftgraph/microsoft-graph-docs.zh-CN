---
title: 列出 verificationDnsRecords
description: 检索 domainDnsRecord 对象的列表。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b611cd9557bc88665a826725396a4c9b17b824cc
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402261"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="59354-103">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="59354-103">List verificationDnsRecords</span></span>

<span data-ttu-id="59354-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59354-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59354-105">检索 [domainDnsRecord](../resources/domaindnsrecord.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="59354-105">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="59354-106">在验证所有权之前，不能使用 Azure AD 租户相关联的域。</span><span class="sxs-lookup"><span data-stu-id="59354-106">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="59354-107">若要验证域的所有权，请检索域验证记录并将详细信息添加到域的区域文件中。</span><span class="sxs-lookup"><span data-stu-id="59354-107">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="59354-108">可以通过域注册机构或 DNS 服务器配置来完成此操作。</span><span class="sxs-lookup"><span data-stu-id="59354-108">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="59354-109">根域需要验证。</span><span class="sxs-lookup"><span data-stu-id="59354-109">Root domains require verification.</span></span> <span data-ttu-id="59354-110">例如，contoso.com 需要验证。</span><span class="sxs-lookup"><span data-stu-id="59354-110">For example, contoso.com requires verification.</span></span> <span data-ttu-id="59354-111">如果验证了根域，则会自动验证根域的子域。</span><span class="sxs-lookup"><span data-stu-id="59354-111">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="59354-112">例如，如果 contoso.com 已经过验证，则会自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="59354-112">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="59354-113">权限</span><span class="sxs-lookup"><span data-stu-id="59354-113">Permissions</span></span>

<span data-ttu-id="59354-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59354-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="59354-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="59354-116">Permission type</span></span>      | <span data-ttu-id="59354-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59354-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59354-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59354-118">Delegated (work or school account)</span></span> | <span data-ttu-id="59354-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="59354-119">Directory.Read.All</span></span>    |
|<span data-ttu-id="59354-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59354-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59354-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="59354-121">Not supported.</span></span>    |
|<span data-ttu-id="59354-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="59354-122">Application</span></span> | <span data-ttu-id="59354-123">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59354-123">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59354-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59354-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="59354-125">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="59354-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="59354-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59354-126">Optional query parameters</span></span>

<span data-ttu-id="59354-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59354-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59354-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="59354-128">Request headers</span></span>

| <span data-ttu-id="59354-129">名称</span><span class="sxs-lookup"><span data-stu-id="59354-129">Name</span></span>      |<span data-ttu-id="59354-130">说明</span><span class="sxs-lookup"><span data-stu-id="59354-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59354-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="59354-131">Authorization</span></span>  | <span data-ttu-id="59354-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59354-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59354-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59354-134">Content-Type</span></span>  | <span data-ttu-id="59354-135">application/json</span><span class="sxs-lookup"><span data-stu-id="59354-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="59354-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="59354-136">Request body</span></span>

<span data-ttu-id="59354-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59354-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59354-138">响应</span><span class="sxs-lookup"><span data-stu-id="59354-138">Response</span></span>

<span data-ttu-id="59354-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [domainDnsRecord](../resources/domaindnsrecord.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="59354-139">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59354-140">示例</span><span class="sxs-lookup"><span data-stu-id="59354-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59354-141">请求</span><span class="sxs-lookup"><span data-stu-id="59354-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="59354-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="59354-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```
# <a name="c"></a>[<span data-ttu-id="59354-143">C#</span><span class="sxs-lookup"><span data-stu-id="59354-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-verificationdnsrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59354-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59354-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-verificationdnsrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59354-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59354-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-verificationdnsrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59354-146">Java</span><span class="sxs-lookup"><span data-stu-id="59354-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-verificationdnsrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59354-147">响应</span><span class="sxs-lookup"><span data-stu-id="59354-147">Response</span></span>

<span data-ttu-id="59354-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59354-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->