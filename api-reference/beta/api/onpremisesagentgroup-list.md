---
title: 列出 onPremisesAgentGroups
description: 检索 onPremisesAgentGroup 对象的列表。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02374b55c5d1905c26675ea5419dce3115e3c4c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969499"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="a852c-103">列出 onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="a852c-103">List onPremisesAgentGroups</span></span>

<span data-ttu-id="a852c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a852c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a852c-105">检索 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a852c-105">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a852c-106">权限</span><span class="sxs-lookup"><span data-stu-id="a852c-106">Permissions</span></span>

<span data-ttu-id="a852c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a852c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a852c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a852c-109">Permission type</span></span>                        | <span data-ttu-id="a852c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a852c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a852c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a852c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a852c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a852c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="a852c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a852c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a852c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a852c-114">Not supported.</span></span> |
| <span data-ttu-id="a852c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a852c-115">Application</span></span>                            | <span data-ttu-id="a852c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a852c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a852c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a852c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a852c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a852c-118">Optional query parameters</span></span>

<span data-ttu-id="a852c-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a852c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a852c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a852c-120">Request headers</span></span>

| <span data-ttu-id="a852c-121">名称</span><span class="sxs-lookup"><span data-stu-id="a852c-121">Name</span></span>      |<span data-ttu-id="a852c-122">说明</span><span class="sxs-lookup"><span data-stu-id="a852c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a852c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a852c-123">Authorization</span></span> | <span data-ttu-id="a852c-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a852c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a852c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a852c-125">Request body</span></span>

<span data-ttu-id="a852c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a852c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a852c-127">响应</span><span class="sxs-lookup"><span data-stu-id="a852c-127">Response</span></span>

<span data-ttu-id="a852c-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a852c-128">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a852c-129">示例</span><span class="sxs-lookup"><span data-stu-id="a852c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a852c-130">请求</span><span class="sxs-lookup"><span data-stu-id="a852c-130">Request</span></span>

<span data-ttu-id="a852c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a852c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a852c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a852c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="c"></a>[<span data-ttu-id="a852c-133">C#</span><span class="sxs-lookup"><span data-stu-id="a852c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a852c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a852c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a852c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a852c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a852c-136">响应</span><span class="sxs-lookup"><span data-stu-id="a852c-136">Response</span></span>

<span data-ttu-id="a852c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a852c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="a852c-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a852c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
                }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


