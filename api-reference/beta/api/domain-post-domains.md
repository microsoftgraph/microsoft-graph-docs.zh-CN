---
title: 创建域
description: 向租户添加域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d4c6e9731285f5e28829dc2bb5c77faae30775c4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436482"
---
# <a name="create-domain"></a><span data-ttu-id="eaa6d-103">创建域</span><span class="sxs-lookup"><span data-stu-id="eaa6d-103">Create domain</span></span>

<span data-ttu-id="eaa6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaa6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaa6d-105">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-105">Adds a domain to the tenant.</span></span>

<span data-ttu-id="eaa6d-p101">**重要说明**：必须完成所有权验证，才可以使用与 Azure AD 租户关联的域。有关详细信息，请参阅 [列出 verificationDnsRecords](domain-list-verificationdnsrecords.md)。需要对根域进行验证。例如，需要对 contoso.com 进行验证。如果已验证根域，则将自动验证该根域的子域。例如，如果已验证 contoso.com，则将自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa6d-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="eaa6d-112">Permissions</span></span>

<span data-ttu-id="eaa6d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eaa6d-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="eaa6d-115">Permission type</span></span>      | <span data-ttu-id="eaa6d-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eaa6d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa6d-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eaa6d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa6d-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eaa6d-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eaa6d-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eaa6d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa6d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-120">Not supported.</span></span>    |
|<span data-ttu-id="eaa6d-121">Application</span><span class="sxs-lookup"><span data-stu-id="eaa6d-121">Application</span></span> | <span data-ttu-id="eaa6d-122">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa6d-122">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa6d-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eaa6d-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="eaa6d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="eaa6d-124">Request headers</span></span>
| <span data-ttu-id="eaa6d-125">名称</span><span class="sxs-lookup"><span data-stu-id="eaa6d-125">Name</span></span>       | <span data-ttu-id="eaa6d-126">说明</span><span class="sxs-lookup"><span data-stu-id="eaa6d-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eaa6d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa6d-127">Authorization</span></span>  | <span data-ttu-id="eaa6d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="eaa6d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eaa6d-130">Content-Type</span></span>  | <span data-ttu-id="eaa6d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="eaa6d-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaa6d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="eaa6d-132">Request body</span></span>
<span data-ttu-id="eaa6d-133">在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-133">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="eaa6d-p104">请求正文包含新域的 id 属性。Id 是唯一可以指定，也是必须指定的属性。此 id 属性值是要创建的完全限定的域名。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="eaa6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="eaa6d-137">Response</span></span>

<span data-ttu-id="eaa6d-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-138">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa6d-139">示例</span><span class="sxs-lookup"><span data-stu-id="eaa6d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa6d-140">请求</span><span class="sxs-lookup"><span data-stu-id="eaa6d-140">Request</span></span>

<span data-ttu-id="eaa6d-141">在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-141">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/beta/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="eaa6d-142">响应</span><span class="sxs-lookup"><span data-stu-id="eaa6d-142">Response</span></span>
<span data-ttu-id="eaa6d-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eaa6d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


