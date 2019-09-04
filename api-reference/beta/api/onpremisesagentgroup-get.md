---
title: 获取 onPremisesAgentGroup
description: 检索[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c0db16462106002f5496f36c1d14635f287685d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726016"
---
# <a name="get-onpremisesagentgroup"></a><span data-ttu-id="9a401-103">获取 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9a401-103">Get onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a401-104">检索[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a401-104">Retrieve the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a401-105">权限</span><span class="sxs-lookup"><span data-stu-id="9a401-105">Permissions</span></span>

<span data-ttu-id="9a401-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a401-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a401-108">Permission type</span></span>                        | <span data-ttu-id="9a401-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a401-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a401-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a401-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a401-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="9a401-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9a401-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a401-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a401-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a401-113">Not supported.</span></span> |
| <span data-ttu-id="9a401-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a401-114">Application</span></span>                            | <span data-ttu-id="9a401-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a401-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a401-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a401-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a401-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a401-117">Optional query parameters</span></span>

<span data-ttu-id="9a401-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a401-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a401-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a401-119">Request headers</span></span>

| <span data-ttu-id="9a401-120">名称</span><span class="sxs-lookup"><span data-stu-id="9a401-120">Name</span></span>      |<span data-ttu-id="9a401-121">说明</span><span class="sxs-lookup"><span data-stu-id="9a401-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a401-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a401-122">Authorization</span></span> | <span data-ttu-id="9a401-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9a401-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a401-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a401-124">Request body</span></span>

<span data-ttu-id="9a401-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a401-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a401-126">响应</span><span class="sxs-lookup"><span data-stu-id="9a401-126">Response</span></span>

<span data-ttu-id="9a401-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a401-127">If successful, this method returns a `200 OK` response code and the requested [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a401-128">示例</span><span class="sxs-lookup"><span data-stu-id="9a401-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a401-129">请求</span><span class="sxs-lookup"><span data-stu-id="9a401-129">Request</span></span>

<span data-ttu-id="9a401-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a401-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a401-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9a401-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagentgroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/?$expand=publishedResources,agents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a401-132">C#</span><span class="sxs-lookup"><span data-stu-id="9a401-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a401-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a401-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a401-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="9a401-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a401-135">响应</span><span class="sxs-lookup"><span data-stu-id="9a401-135">Response</span></span>

<span data-ttu-id="9a401-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a401-136">The following is an example of the response.</span></span>

> <span data-ttu-id="9a401-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9a401-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
    "displayName": "Group 1",
    "publishingType": "provisioning",
    "isDefault": false,
    "agents": [
            {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active"
            }
    ],
    "publishedResources": [
        {
            "displayName": "Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
