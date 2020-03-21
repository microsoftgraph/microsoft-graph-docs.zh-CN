---
title: 获取 identitySecurityDefaultsEnforcementPolicy
description: 检索 identitysecuritydefaultsenforcementpolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2ae06cd13c4c9f7401e839d8ac570710ac9e41c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895599"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="6b3c4-103">获取 identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="6b3c4-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="6b3c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b3c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b3c4-105">检索[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b3c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b3c4-106">Permissions</span></span>

<span data-ttu-id="6b3c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b3c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b3c4-109">Permission type</span></span>                        | <span data-ttu-id="6b3c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b3c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b3c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b3c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b3c4-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b3c4-112">Policy.Read.All</span></span> |
| <span data-ttu-id="6b3c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b3c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b3c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-114">Not supported.</span></span> |
| <span data-ttu-id="6b3c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b3c4-115">Application</span></span>                            | <span data-ttu-id="6b3c4-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b3c4-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b3c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b3c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b3c4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b3c4-118">Optional query parameters</span></span>

<span data-ttu-id="6b3c4-119">此方法支持`select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="6b3c4-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b3c4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b3c4-121">Request headers</span></span>

| <span data-ttu-id="6b3c4-122">名称</span><span class="sxs-lookup"><span data-stu-id="6b3c4-122">Name</span></span>      |<span data-ttu-id="6b3c4-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b3c4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b3c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b3c4-124">Authorization</span></span> | <span data-ttu-id="6b3c4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b3c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b3c4-127">Request body</span></span>

<span data-ttu-id="6b3c4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b3c4-129">响应</span><span class="sxs-lookup"><span data-stu-id="6b3c4-129">Response</span></span>

<span data-ttu-id="6b3c4-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b3c4-131">示例</span><span class="sxs-lookup"><span data-stu-id="6b3c4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b3c4-132">请求</span><span class="sxs-lookup"><span data-stu-id="6b3c4-132">Request</span></span>

<span data-ttu-id="6b3c4-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```

### <a name="response"></a><span data-ttu-id="6b3c4-134">响应</span><span class="sxs-lookup"><span data-stu-id="6b3c4-134">Response</span></span>

<span data-ttu-id="6b3c4-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="6b3c4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6b3c4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
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
