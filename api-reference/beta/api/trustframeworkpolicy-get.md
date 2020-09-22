---
title: 获取 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户检索现有的 trustFrameworkPolicy 内容。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efb26734bbcb39cdad5fe451e636d836ea615243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095602"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="f07c0-103">获取 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="f07c0-103">Get trustFrameworkPolicy</span></span>

<span data-ttu-id="f07c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f07c0-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="f07c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f07c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f07c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f07c0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f07c0-107">检索现有 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)的内容。</span><span class="sxs-lookup"><span data-stu-id="f07c0-107">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f07c0-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f07c0-108">Permissions</span></span>

<span data-ttu-id="f07c0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f07c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f07c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f07c0-111">Permission type</span></span>      | <span data-ttu-id="f07c0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f07c0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f07c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f07c0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f07c0-114">Policy： Read. All，TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f07c0-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="f07c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f07c0-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f07c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f07c0-116">Not supported.</span></span>|
|<span data-ttu-id="f07c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f07c0-117">Application</span></span>|<span data-ttu-id="f07c0-118">Policy： Read. All，TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f07c0-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="f07c0-119">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="f07c0-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f07c0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f07c0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f07c0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f07c0-121">Optional query parameters</span></span>

<span data-ttu-id="f07c0-122">此方法支持 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f07c0-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f07c0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f07c0-123">Request headers</span></span>

|<span data-ttu-id="f07c0-124">名称</span><span class="sxs-lookup"><span data-stu-id="f07c0-124">Name</span></span>|<span data-ttu-id="f07c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="f07c0-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f07c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f07c0-126">Authorization</span></span>|<span data-ttu-id="f07c0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f07c0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f07c0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f07c0-129">Request body</span></span>

<span data-ttu-id="f07c0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f07c0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f07c0-131">响应</span><span class="sxs-lookup"><span data-stu-id="f07c0-131">Response</span></span>

<span data-ttu-id="f07c0-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [TRUSTFRAMEWORKPOLICY](../resources/trustframeworkpolicy.md) 的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f07c0-132">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="f07c0-133">**注意：** 响应内容类型将为 `application/xml` 。</span><span class="sxs-lookup"><span data-stu-id="f07c0-133">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="f07c0-134">示例</span><span class="sxs-lookup"><span data-stu-id="f07c0-134">Example</span></span>

<span data-ttu-id="f07c0-135">下面的示例检索特定的 **trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="f07c0-135">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f07c0-136">请求</span><span class="sxs-lookup"><span data-stu-id="f07c0-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="f07c0-137">响应</span><span class="sxs-lookup"><span data-stu-id="f07c0-137">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
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
  "description": "Get trustFramework policy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


