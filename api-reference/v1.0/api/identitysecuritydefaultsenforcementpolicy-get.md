---
title: 获取 identitySecurityDefaultsEnforcementPolicy
description: 检索 identitysecuritydefaultsenforcementpolicy 对象的属性和关系。
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48a28d0aa32d8abc23f0c731a0ca4cb89d774e34
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384487"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="9b39a-103">获取 identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="9b39a-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="9b39a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b39a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b39a-105">检索[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b39a-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b39a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b39a-106">Permissions</span></span>

<span data-ttu-id="9b39a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b39a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b39a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b39a-109">Permission type</span></span>                        | <span data-ttu-id="9b39a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b39a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b39a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b39a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b39a-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b39a-112">Policy.Read.All</span></span> |
| <span data-ttu-id="9b39a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b39a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b39a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b39a-114">Not supported.</span></span> |
| <span data-ttu-id="9b39a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b39a-115">Application</span></span>                            | <span data-ttu-id="9b39a-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b39a-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b39a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b39a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b39a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b39a-118">Optional query parameters</span></span>

<span data-ttu-id="9b39a-119">此方法支持 `select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9b39a-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9b39a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9b39a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b39a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b39a-121">Request headers</span></span>

| <span data-ttu-id="9b39a-122">名称</span><span class="sxs-lookup"><span data-stu-id="9b39a-122">Name</span></span>      |<span data-ttu-id="9b39a-123">说明</span><span class="sxs-lookup"><span data-stu-id="9b39a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b39a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b39a-124">Authorization</span></span> | <span data-ttu-id="9b39a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b39a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b39a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b39a-127">Request body</span></span>

<span data-ttu-id="9b39a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b39a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b39a-129">响应</span><span class="sxs-lookup"><span data-stu-id="9b39a-129">Response</span></span>

<span data-ttu-id="9b39a-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b39a-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b39a-131">示例</span><span class="sxs-lookup"><span data-stu-id="9b39a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b39a-132">请求</span><span class="sxs-lookup"><span data-stu-id="9b39a-132">Request</span></span>

<span data-ttu-id="9b39a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b39a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```

### <a name="response"></a><span data-ttu-id="9b39a-134">响应</span><span class="sxs-lookup"><span data-stu-id="9b39a-134">Response</span></span>

<span data-ttu-id="9b39a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b39a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="9b39a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b39a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
