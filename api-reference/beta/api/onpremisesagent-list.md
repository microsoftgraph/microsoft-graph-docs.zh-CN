---
title: 列出 onPremisesAgents
description: 检索 onPremisesAgents 的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c46084b57cf11bd09558b872cf6399571aabcc0e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841176"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="5880d-103">列出 onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="5880d-103">List onPremisesAgents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5880d-104">检索[onPremisesAgent](../resources/onpremisesagent.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5880d-104">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5880d-105">权限</span><span class="sxs-lookup"><span data-stu-id="5880d-105">Permissions</span></span>

<span data-ttu-id="5880d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5880d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5880d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5880d-108">Permission type</span></span>                        | <span data-ttu-id="5880d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5880d-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5880d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5880d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5880d-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="5880d-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5880d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5880d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5880d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5880d-113">Not supported.</span></span> |
| <span data-ttu-id="5880d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5880d-114">Application</span></span>                            | <span data-ttu-id="5880d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5880d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5880d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5880d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5880d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5880d-117">Optional query parameters</span></span>

<span data-ttu-id="5880d-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5880d-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5880d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5880d-119">Request headers</span></span>

| <span data-ttu-id="5880d-120">名称</span><span class="sxs-lookup"><span data-stu-id="5880d-120">Name</span></span>      |<span data-ttu-id="5880d-121">说明</span><span class="sxs-lookup"><span data-stu-id="5880d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5880d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5880d-122">Authorization</span></span> | <span data-ttu-id="5880d-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5880d-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5880d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5880d-124">Request body</span></span>

<span data-ttu-id="5880d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5880d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5880d-126">响应</span><span class="sxs-lookup"><span data-stu-id="5880d-126">Response</span></span>

<span data-ttu-id="5880d-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5880d-127">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5880d-128">示例</span><span class="sxs-lookup"><span data-stu-id="5880d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5880d-129">请求</span><span class="sxs-lookup"><span data-stu-id="5880d-129">Request</span></span>

<span data-ttu-id="5880d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5880d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```

### <a name="response"></a><span data-ttu-id="5880d-131">响应</span><span class="sxs-lookup"><span data-stu-id="5880d-131">Response</span></span>

<span data-ttu-id="5880d-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5880d-132">The following is an example of the response.</span></span>

> <span data-ttu-id="5880d-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5880d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
