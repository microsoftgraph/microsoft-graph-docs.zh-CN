---
title: 更新 trustFrameworkPolicy
description: '此操作将更新现有的 trustFrameworkPolicy 对象，如果不存在，则创建一个。 '
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de1df6c258794165e37d3572d4bee5da84316c83
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215908"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="cbaea-103">更新或创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="cbaea-103">Update or create trustFrameworkPolicy</span></span>

<span data-ttu-id="cbaea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbaea-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="cbaea-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbaea-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbaea-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbaea-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbaea-107">更新现有[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) ，如果不存在，则创建一个。</span><span class="sxs-lookup"><span data-stu-id="cbaea-107">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbaea-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="cbaea-108">Permissions</span></span>

<span data-ttu-id="cbaea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cbaea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="cbaea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbaea-111">Permission type</span></span>      | <span data-ttu-id="cbaea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cbaea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbaea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbaea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbaea-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="cbaea-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="cbaea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbaea-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cbaea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbaea-116">Not supported.</span></span>|
|<span data-ttu-id="cbaea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbaea-117">Application</span></span>|<span data-ttu-id="cbaea-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="cbaea-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="cbaea-119">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="cbaea-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="cbaea-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbaea-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="cbaea-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbaea-121">Request headers</span></span>

|<span data-ttu-id="cbaea-122">名称</span><span class="sxs-lookup"><span data-stu-id="cbaea-122">Name</span></span>|<span data-ttu-id="cbaea-123">说明</span><span class="sxs-lookup"><span data-stu-id="cbaea-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="cbaea-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbaea-124">Authorization</span></span>|<span data-ttu-id="cbaea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cbaea-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cbaea-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbaea-127">Content-Type</span></span>|<span data-ttu-id="cbaea-128">application/xml。</span><span class="sxs-lookup"><span data-stu-id="cbaea-128">application/xml.</span></span> <span data-ttu-id="cbaea-129">必需。</span><span class="sxs-lookup"><span data-stu-id="cbaea-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbaea-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbaea-130">Request body</span></span>

<span data-ttu-id="cbaea-131">在请求正文中，提供[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbaea-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="cbaea-132">**注意：** 内容类型必须为`application/xml`。</span><span class="sxs-lookup"><span data-stu-id="cbaea-132">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="cbaea-133">响应</span><span class="sxs-lookup"><span data-stu-id="cbaea-133">Response</span></span>

<span data-ttu-id="cbaea-134">响应将为以下之一：</span><span class="sxs-lookup"><span data-stu-id="cbaea-134">The response will be one of the following:</span></span>
- <span data-ttu-id="cbaea-135">如果存在[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) ，则成功的请求将返回`200 OK`响应代码。</span><span class="sxs-lookup"><span data-stu-id="cbaea-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="cbaea-136">如果[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)不存在，则成功的请求将返回`201 Created`响应代码。</span><span class="sxs-lookup"><span data-stu-id="cbaea-136">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="cbaea-137">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="cbaea-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="cbaea-138">示例</span><span class="sxs-lookup"><span data-stu-id="cbaea-138">Example</span></span>

<span data-ttu-id="cbaea-139">下面的示例更新**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="cbaea-139">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="cbaea-140">请求</span><span class="sxs-lookup"><span data-stu-id="cbaea-140">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="cbaea-141">响应</span><span class="sxs-lookup"><span data-stu-id="cbaea-141">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
