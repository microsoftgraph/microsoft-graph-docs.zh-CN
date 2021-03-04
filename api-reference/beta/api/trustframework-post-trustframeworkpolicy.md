---
title: 创建 trustFrameworkPolicy
description: 此操作在 Azure AD B2C 租户中创建新的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9027c578acecbf5e78f52dfcd0026721330a6f4b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443291"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="aa461-103">创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="aa461-103">Create trustFrameworkPolicy</span></span>

<span data-ttu-id="aa461-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa461-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa461-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa461-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa461-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa461-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa461-107">创建新的 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa461-107">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa461-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="aa461-108">Permissions</span></span>

<span data-ttu-id="aa461-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="aa461-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa461-111">Permission type</span></span>      | <span data-ttu-id="aa461-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa461-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa461-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa461-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa461-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="aa461-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="aa461-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa461-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="aa461-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa461-116">Not supported.</span></span>|
|<span data-ttu-id="aa461-117">Application</span><span class="sxs-lookup"><span data-stu-id="aa461-117">Application</span></span>|<span data-ttu-id="aa461-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="aa461-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="aa461-119">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="aa461-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa461-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa461-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="aa461-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa461-121">Request headers</span></span>

|<span data-ttu-id="aa461-122">名称</span><span class="sxs-lookup"><span data-stu-id="aa461-122">Name</span></span>|<span data-ttu-id="aa461-123">说明</span><span class="sxs-lookup"><span data-stu-id="aa461-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="aa461-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa461-124">Authorization</span></span>|<span data-ttu-id="aa461-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa461-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa461-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa461-127">Content-Type</span></span>|<span data-ttu-id="aa461-128">application/xml。</span><span class="sxs-lookup"><span data-stu-id="aa461-128">application/xml.</span></span> <span data-ttu-id="aa461-129">必需。</span><span class="sxs-lookup"><span data-stu-id="aa461-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa461-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa461-130">Request body</span></span>

<span data-ttu-id="aa461-131">在请求正文中，提供 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) 对象的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa461-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="aa461-132">内容类型必须是 `application/xml`。</span><span class="sxs-lookup"><span data-stu-id="aa461-132">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="aa461-133">响应</span><span class="sxs-lookup"><span data-stu-id="aa461-133">Response</span></span>

<span data-ttu-id="aa461-134">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa461-134">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="aa461-135">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="aa461-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="aa461-136">示例</span><span class="sxs-lookup"><span data-stu-id="aa461-136">Example</span></span>

<span data-ttu-id="aa461-137">下面的示例创建 **一个 trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="aa461-137">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="aa461-138">请求</span><span class="sxs-lookup"><span data-stu-id="aa461-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "name": "create_trustframeworkpolicy_from_trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="aa461-139">响应</span><span class="sxs-lookup"><span data-stu-id="aa461-139">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/xml
Location: /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


