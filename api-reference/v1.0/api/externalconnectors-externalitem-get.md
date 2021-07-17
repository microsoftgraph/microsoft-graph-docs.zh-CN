---
title: 获取 externalItem
description: 读取 externalItem 对象的属性和关系。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6defb4476d5d34b148e8e18c4757333f9bc3ca81
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467285"
---
# <a name="get-externalitem"></a><span data-ttu-id="52167-103">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="52167-103">Get externalItem</span></span>
<span data-ttu-id="52167-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="52167-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="52167-105">读取 [externalItem 对象的属性和](../resources/externalconnectors-externalitem.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="52167-105">Read the properties and relationships of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52167-106">权限</span><span class="sxs-lookup"><span data-stu-id="52167-106">Permissions</span></span>
<span data-ttu-id="52167-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52167-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52167-109">Permission type</span></span>|<span data-ttu-id="52167-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52167-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52167-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52167-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52167-112">不适用</span><span class="sxs-lookup"><span data-stu-id="52167-112">Not applicable</span></span>|
|<span data-ttu-id="52167-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52167-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52167-114">不适用</span><span class="sxs-lookup"><span data-stu-id="52167-114">Not applicable</span></span>|
|<span data-ttu-id="52167-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52167-115">Application</span></span>| <span data-ttu-id="52167-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52167-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52167-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52167-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/items/{externalItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52167-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="52167-118">Optional query parameters</span></span>
<span data-ttu-id="52167-119">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="52167-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52167-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52167-120">Request headers</span></span>
|<span data-ttu-id="52167-121">名称</span><span class="sxs-lookup"><span data-stu-id="52167-121">Name</span></span>|<span data-ttu-id="52167-122">说明</span><span class="sxs-lookup"><span data-stu-id="52167-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52167-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52167-123">Authorization</span></span>|<span data-ttu-id="52167-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52167-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52167-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="52167-126">Request body</span></span>
<span data-ttu-id="52167-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="52167-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52167-128">响应</span><span class="sxs-lookup"><span data-stu-id="52167-128">Response</span></span>

<span data-ttu-id="52167-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [externalItem](../resources/externalconnectors-externalitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52167-129">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52167-130">示例</span><span class="sxs-lookup"><span data-stu-id="52167-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52167-131">请求</span><span class="sxs-lookup"><span data-stu-id="52167-131">Request</span></span>
<span data-ttu-id="52167-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="52167-132">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="52167-133">响应</span><span class="sxs-lookup"><span data-stu-id="52167-133">Response</span></span>
<span data-ttu-id="52167-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="52167-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```

