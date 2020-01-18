---
title: 列出 claimsMappingPolicies
description: 获取 claimsMappingPolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9aa69d061eb719a5aed5b6ff1d7755fd9e407045
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234155"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="dbe91-103">列出 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="dbe91-103">List claimsMappingPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe91-104">获取[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="dbe91-104">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe91-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="dbe91-105">Permissions</span></span>

<span data-ttu-id="dbe91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbe91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbe91-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbe91-108">Permission type</span></span>                        | <span data-ttu-id="dbe91-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbe91-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dbe91-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe91-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbe91-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbe91-111">Policy.Read.All</span></span> |
| <span data-ttu-id="dbe91-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe91-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbe91-113">Not supported.</span></span> |
| <span data-ttu-id="dbe91-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbe91-114">Application</span></span>                            | <span data-ttu-id="dbe91-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbe91-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe91-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbe91-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbe91-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dbe91-117">Optional query parameters</span></span>

<span data-ttu-id="dbe91-118">`$expand`此方法支持`$filter`、 `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dbe91-118">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="dbe91-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="dbe91-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="dbe91-120">使用`$expand`时，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="dbe91-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbe91-121">请求头</span><span class="sxs-lookup"><span data-stu-id="dbe91-121">Request headers</span></span>

| <span data-ttu-id="dbe91-122">名称</span><span class="sxs-lookup"><span data-stu-id="dbe91-122">Name</span></span>      |<span data-ttu-id="dbe91-123">说明</span><span class="sxs-lookup"><span data-stu-id="dbe91-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbe91-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe91-124">Authorization</span></span> | <span data-ttu-id="dbe91-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dbe91-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbe91-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbe91-126">Request body</span></span>

<span data-ttu-id="dbe91-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbe91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbe91-128">响应</span><span class="sxs-lookup"><span data-stu-id="dbe91-128">Response</span></span>

<span data-ttu-id="dbe91-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbe91-129">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbe91-130">示例</span><span class="sxs-lookup"><span data-stu-id="dbe91-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dbe91-131">请求</span><span class="sxs-lookup"><span data-stu-id="dbe91-131">Request</span></span>

<span data-ttu-id="dbe91-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dbe91-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies
```

### <a name="response"></a><span data-ttu-id="dbe91-133">响应</span><span class="sxs-lookup"><span data-stu-id="dbe91-133">Response</span></span>

<span data-ttu-id="dbe91-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dbe91-134">The following is an example of the response.</span></span>

> <span data-ttu-id="dbe91-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dbe91-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List claimsMappingPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->