---
title: 获取 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户检索现有的 trustFrameworkPolicy 内容。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 697218f1ff488b935b401406fbd30ddd9f5ebf65
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734386"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="81e45-103">获取 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="81e45-103">Get trustFrameworkPolicy</span></span>

><span data-ttu-id="81e45-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81e45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81e45-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81e45-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81e45-106">检索现有[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)的内容。</span><span class="sxs-lookup"><span data-stu-id="81e45-106">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81e45-107">权限</span><span class="sxs-lookup"><span data-stu-id="81e45-107">Permissions</span></span>

<span data-ttu-id="81e45-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="81e45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="81e45-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81e45-110">Permission type</span></span>      | <span data-ttu-id="81e45-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81e45-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81e45-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81e45-112">Delegated (work or school account)</span></span>| <span data-ttu-id="81e45-113">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="81e45-113">Policy.Read.All</span></span>|
|<span data-ttu-id="81e45-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81e45-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="81e45-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81e45-115">Not supported.</span></span>|
|<span data-ttu-id="81e45-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="81e45-116">Application</span></span>|<span data-ttu-id="81e45-117">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="81e45-117">Policy.Read.All</span></span>|

<span data-ttu-id="81e45-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="81e45-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="81e45-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81e45-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81e45-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="81e45-120">Optional query parameters</span></span>

<span data-ttu-id="81e45-121">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="81e45-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81e45-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="81e45-122">Request headers</span></span>

|<span data-ttu-id="81e45-123">名称</span><span class="sxs-lookup"><span data-stu-id="81e45-123">Name</span></span>|<span data-ttu-id="81e45-124">说明</span><span class="sxs-lookup"><span data-stu-id="81e45-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="81e45-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="81e45-125">Authorization</span></span>|<span data-ttu-id="81e45-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81e45-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81e45-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="81e45-128">Request body</span></span>

<span data-ttu-id="81e45-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81e45-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81e45-130">响应</span><span class="sxs-lookup"><span data-stu-id="81e45-130">Response</span></span>

<span data-ttu-id="81e45-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e45-131">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="81e45-132">**注意：** 响应内容类型将为`application/xml`。</span><span class="sxs-lookup"><span data-stu-id="81e45-132">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="81e45-133">示例</span><span class="sxs-lookup"><span data-stu-id="81e45-133">Example</span></span>

<span data-ttu-id="81e45-134">下面的示例检索特定的**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="81e45-134">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="81e45-135">请求</span><span class="sxs-lookup"><span data-stu-id="81e45-135">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="81e45-136">响应</span><span class="sxs-lookup"><span data-stu-id="81e45-136">Response</span></span>

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
