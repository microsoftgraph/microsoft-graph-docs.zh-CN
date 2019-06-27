---
title: 获取 securityAction
description: 检索 securityAction 对象的属性和关系。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b856db451fa725f7f5e52e6db3296f2c82910be4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263866"
---
# <a name="get-securityaction"></a><span data-ttu-id="545b3-103">获取 securityAction</span><span class="sxs-lookup"><span data-stu-id="545b3-103">Get securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="545b3-104">检索[securityAction](../resources/securityaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="545b3-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="545b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="545b3-105">Permissions</span></span>

<span data-ttu-id="545b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="545b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="545b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="545b3-108">Permission type</span></span>                        | <span data-ttu-id="545b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="545b3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="545b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="545b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="545b3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="545b3-111">Not supported.</span></span> |
| <span data-ttu-id="545b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="545b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="545b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="545b3-113">Not supported.</span></span> |
| <span data-ttu-id="545b3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="545b3-114">Application</span></span>                            | <span data-ttu-id="545b3-115">SecurityActions、SecurityActions 和所有</span><span class="sxs-lookup"><span data-stu-id="545b3-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="545b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="545b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="545b3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="545b3-117">Optional query parameters</span></span>

<span data-ttu-id="545b3-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="545b3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="545b3-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="545b3-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="545b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="545b3-120">Request headers</span></span>

| <span data-ttu-id="545b3-121">名称</span><span class="sxs-lookup"><span data-stu-id="545b3-121">Name</span></span>      |<span data-ttu-id="545b3-122">说明</span><span class="sxs-lookup"><span data-stu-id="545b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="545b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="545b3-123">Authorization</span></span> | <span data-ttu-id="545b3-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="545b3-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="545b3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="545b3-125">Request body</span></span>

<span data-ttu-id="545b3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="545b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="545b3-127">响应</span><span class="sxs-lookup"><span data-stu-id="545b3-127">Response</span></span>

<span data-ttu-id="545b3-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="545b3-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="545b3-129">示例</span><span class="sxs-lookup"><span data-stu-id="545b3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="545b3-130">请求</span><span class="sxs-lookup"><span data-stu-id="545b3-130">Request</span></span>

<span data-ttu-id="545b3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="545b3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```

### <a name="response"></a><span data-ttu-id="545b3-132">响应</span><span class="sxs-lookup"><span data-stu-id="545b3-132">Response</span></span>

<span data-ttu-id="545b3-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="545b3-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="545b3-134">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="545b3-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="545b3-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="545b3-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="545b3-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="545b3-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="545b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="545b3-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securityaction-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="545b3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="545b3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securityaction-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="545b3-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="545b3-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securityaction-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securityaction-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securityaction-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityaction-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
