---
title: 列出 onPremisesAgents
description: 检索 onPremisesAgents 的列表。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8416b61583442017f3b1c14f2497d42bcbb9932e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038185"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="98044-103">列出 onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="98044-103">List onPremisesAgents</span></span>

<span data-ttu-id="98044-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98044-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98044-105">检索 [onPremisesAgent 对象](../resources/onpremisesagent.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="98044-105">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="98044-106">权限</span><span class="sxs-lookup"><span data-stu-id="98044-106">Permissions</span></span>

<span data-ttu-id="98044-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98044-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98044-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="98044-109">Permission type</span></span>                        | <span data-ttu-id="98044-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98044-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98044-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98044-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="98044-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98044-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="98044-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98044-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98044-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="98044-114">Not supported.</span></span> |
| <span data-ttu-id="98044-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="98044-115">Application</span></span>                            | <span data-ttu-id="98044-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98044-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98044-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98044-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98044-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98044-118">Optional query parameters</span></span>

<span data-ttu-id="98044-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98044-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98044-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="98044-120">Request headers</span></span>

| <span data-ttu-id="98044-121">名称</span><span class="sxs-lookup"><span data-stu-id="98044-121">Name</span></span>      |<span data-ttu-id="98044-122">说明</span><span class="sxs-lookup"><span data-stu-id="98044-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98044-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98044-123">Authorization</span></span> | <span data-ttu-id="98044-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="98044-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="98044-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="98044-125">Request body</span></span>

<span data-ttu-id="98044-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98044-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98044-127">响应</span><span class="sxs-lookup"><span data-stu-id="98044-127">Response</span></span>

<span data-ttu-id="98044-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="98044-128">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98044-129">示例</span><span class="sxs-lookup"><span data-stu-id="98044-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98044-130">请求</span><span class="sxs-lookup"><span data-stu-id="98044-130">Request</span></span>

<span data-ttu-id="98044-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98044-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98044-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="98044-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="98044-133">C#</span><span class="sxs-lookup"><span data-stu-id="98044-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98044-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98044-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98044-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98044-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98044-136">Java</span><span class="sxs-lookup"><span data-stu-id="98044-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98044-137">响应</span><span class="sxs-lookup"><span data-stu-id="98044-137">Response</span></span>

<span data-ttu-id="98044-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98044-138">The following is an example of the response.</span></span>

> <span data-ttu-id="98044-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="98044-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agentGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



