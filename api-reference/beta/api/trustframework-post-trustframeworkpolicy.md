---
title: 创建 trustFrameworkPolicy
description: 此操作将在 Azure AD B2C 租户中创建一个新的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4dc64ed9d1db3354926f0f2395e6c2cef84cff28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548003"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="27606-103">创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="27606-103">Create trustFrameworkPolicy</span></span>

> <span data-ttu-id="27606-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27606-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27606-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27606-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27606-106">创建新的[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27606-106">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27606-107">权限</span><span class="sxs-lookup"><span data-stu-id="27606-107">Permissions</span></span>

<span data-ttu-id="27606-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="27606-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="27606-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27606-110">Permission type</span></span>      | <span data-ttu-id="27606-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27606-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27606-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27606-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27606-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="27606-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="27606-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27606-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="27606-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27606-115">Not supported.</span></span>|
|<span data-ttu-id="27606-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="27606-116">Application</span></span>|<span data-ttu-id="27606-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="27606-117">Not supported.</span></span>|

<span data-ttu-id="27606-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="27606-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="27606-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27606-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="27606-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27606-120">Request headers</span></span>

|<span data-ttu-id="27606-121">名称</span><span class="sxs-lookup"><span data-stu-id="27606-121">Name</span></span>|<span data-ttu-id="27606-122">说明</span><span class="sxs-lookup"><span data-stu-id="27606-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="27606-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27606-123">Authorization</span></span>|<span data-ttu-id="27606-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27606-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27606-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27606-126">Content-Type</span></span>|<span data-ttu-id="27606-127">application/xml。</span><span class="sxs-lookup"><span data-stu-id="27606-127">application/xml.</span></span> <span data-ttu-id="27606-128">必需。</span><span class="sxs-lookup"><span data-stu-id="27606-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27606-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="27606-129">Request body</span></span>

<span data-ttu-id="27606-130">在请求正文中, 提供[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27606-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="27606-131">内容类型必须是 `application/xml`。</span><span class="sxs-lookup"><span data-stu-id="27606-131">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="27606-132">响应</span><span class="sxs-lookup"><span data-stu-id="27606-132">Response</span></span>

<span data-ttu-id="27606-133">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27606-133">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="27606-134">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="27606-134">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="27606-135">示例</span><span class="sxs-lookup"><span data-stu-id="27606-135">Example</span></span>

<span data-ttu-id="27606-136">下面的示例创建一个**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="27606-136">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="27606-137">请求</span><span class="sxs-lookup"><span data-stu-id="27606-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create__trustframeworkpolicy_from__trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type:application/xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="27606-138">响应</span><span class="sxs-lookup"><span data-stu-id="27606-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFramework.policy"
} -->
```http
HTTP/1.1 201 Created
Content-Type application/xml
Location /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/
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
