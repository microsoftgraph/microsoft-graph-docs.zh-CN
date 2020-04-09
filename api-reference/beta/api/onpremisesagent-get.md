---
title: 获取 onPremisesAgent
description: 检索 onPremisesAgent 对象的属性和关系。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d4224e981c7652036459e56549bcfe9a96098423
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199804"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="58aa2-103">获取 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="58aa2-103">Get onPremisesAgent</span></span>

<span data-ttu-id="58aa2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58aa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58aa2-105">检索[onPremisesAgent](../resources/onpremisesagent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58aa2-105">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58aa2-106">权限</span><span class="sxs-lookup"><span data-stu-id="58aa2-106">Permissions</span></span>

<span data-ttu-id="58aa2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58aa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58aa2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58aa2-109">Permission type</span></span>                        | <span data-ttu-id="58aa2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58aa2-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="58aa2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58aa2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="58aa2-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58aa2-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="58aa2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58aa2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58aa2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58aa2-114">Not supported.</span></span> |
| <span data-ttu-id="58aa2-115">Application</span><span class="sxs-lookup"><span data-stu-id="58aa2-115">Application</span></span>                            | <span data-ttu-id="58aa2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58aa2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58aa2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58aa2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58aa2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="58aa2-118">Optional query parameters</span></span>

<span data-ttu-id="58aa2-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="58aa2-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58aa2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58aa2-120">Request headers</span></span>

| <span data-ttu-id="58aa2-121">名称</span><span class="sxs-lookup"><span data-stu-id="58aa2-121">Name</span></span>      |<span data-ttu-id="58aa2-122">说明</span><span class="sxs-lookup"><span data-stu-id="58aa2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58aa2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58aa2-123">Authorization</span></span> | <span data-ttu-id="58aa2-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="58aa2-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58aa2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="58aa2-125">Request body</span></span>

<span data-ttu-id="58aa2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58aa2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58aa2-127">响应</span><span class="sxs-lookup"><span data-stu-id="58aa2-127">Response</span></span>

<span data-ttu-id="58aa2-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[onPremisesAgent](../resources/onpremisesagent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="58aa2-128">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58aa2-129">示例</span><span class="sxs-lookup"><span data-stu-id="58aa2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58aa2-130">请求</span><span class="sxs-lookup"><span data-stu-id="58aa2-130">Request</span></span>

<span data-ttu-id="58aa2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="58aa2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58aa2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="58aa2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="58aa2-133">C#</span><span class="sxs-lookup"><span data-stu-id="58aa2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58aa2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58aa2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58aa2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58aa2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58aa2-136">响应</span><span class="sxs-lookup"><span data-stu-id="58aa2-136">Response</span></span>

<span data-ttu-id="58aa2-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="58aa2-137">The following is an example of the response.</span></span>

> <span data-ttu-id="58aa2-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="58aa2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
    "status": "Active",
    "machineName": "server1.local1.contoso.com",
    "externalIp": "153.69.23.122",
    "agentGroups": [
         {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
         }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
