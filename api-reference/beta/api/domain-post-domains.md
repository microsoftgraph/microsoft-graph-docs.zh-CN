---
title: 创建域
description: 向租户添加域。
author: lleonard-msft
ms.openlocfilehash: eae00bb3da0321d5c06d0fc3e4dc76e3ac410589
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308888"
---
# <a name="create-domain"></a><span data-ttu-id="68954-103">创建域</span><span class="sxs-lookup"><span data-stu-id="68954-103">Create domain</span></span>

> <span data-ttu-id="68954-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68954-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68954-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68954-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68954-106">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="68954-106">Adds a domain to the tenant.</span></span>

<span data-ttu-id="68954-p102">**重要说明**：必须完成所有权验证，才可以使用与 Azure AD 租户关联的域。有关详细信息，请参阅[列出 verificationDnsRecords](domain-list-verificationdnsrecords.md)。需要对根域进行验证。例如，需要对 contoso.com 进行验证。如果已验证根域，则将自动验证该根域的子域。例如，如果已验证 contoso.com，则将自动验证 subdomain.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="68954-p102">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="68954-113">权限</span><span class="sxs-lookup"><span data-stu-id="68954-113">Permissions</span></span>

<span data-ttu-id="68954-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68954-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="68954-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="68954-116">Permission type</span></span>      | <span data-ttu-id="68954-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68954-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68954-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68954-118">Delegated (work or school account)</span></span> | <span data-ttu-id="68954-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68954-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68954-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68954-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68954-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="68954-121">Not supported.</span></span>    |
|<span data-ttu-id="68954-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="68954-122">Application</span></span> | <span data-ttu-id="68954-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68954-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68954-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68954-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="68954-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="68954-125">Request headers</span></span>
| <span data-ttu-id="68954-126">Name</span><span class="sxs-lookup"><span data-stu-id="68954-126">Name</span></span>       | <span data-ttu-id="68954-127">说明</span><span class="sxs-lookup"><span data-stu-id="68954-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="68954-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="68954-128">Authorization</span></span>  | <span data-ttu-id="68954-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68954-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="68954-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68954-131">Content-Type</span></span>  | <span data-ttu-id="68954-132">application/json</span><span class="sxs-lookup"><span data-stu-id="68954-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="68954-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="68954-133">Request body</span></span>
<span data-ttu-id="68954-134">在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68954-134">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="68954-p105">请求正文包含新域的 id 属性。Id 是唯一可以指定，也是必须指定的属性。此 id 属性值是要创建的完全限定的域名。</span><span class="sxs-lookup"><span data-stu-id="68954-p105">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="68954-138">响应</span><span class="sxs-lookup"><span data-stu-id="68954-138">Response</span></span>

<span data-ttu-id="68954-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68954-139">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68954-140">示例</span><span class="sxs-lookup"><span data-stu-id="68954-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68954-141">请求</span><span class="sxs-lookup"><span data-stu-id="68954-141">Request</span></span>

<span data-ttu-id="68954-142">在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68954-142">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="68954-143">响应</span><span class="sxs-lookup"><span data-stu-id="68954-143">Response</span></span>
<span data-ttu-id="68954-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68954-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->