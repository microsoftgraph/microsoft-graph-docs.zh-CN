---
title: 删除 externalConnection
description: 删除 externalConnection 对象。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e365c09fca03a97894a53b23eef2d500527a774f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467210"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="d3309-103">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="d3309-103">Delete externalConnection</span></span>
<span data-ttu-id="d3309-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d3309-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="d3309-105">删除 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3309-105">Deletes an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3309-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3309-106">Permissions</span></span>
<span data-ttu-id="d3309-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3309-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3309-109">Permission type</span></span>|<span data-ttu-id="d3309-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3309-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3309-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3309-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3309-112">不适用</span><span class="sxs-lookup"><span data-stu-id="d3309-112">Not applicable</span></span>|
|<span data-ttu-id="d3309-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3309-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3309-114">不适用</span><span class="sxs-lookup"><span data-stu-id="d3309-114">Not applicable</span></span>|
|<span data-ttu-id="d3309-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3309-115">Application</span></span>| <span data-ttu-id="d3309-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d3309-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3309-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3309-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}
```

## <a name="request-headers"></a><span data-ttu-id="d3309-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3309-118">Request headers</span></span>
|<span data-ttu-id="d3309-119">名称</span><span class="sxs-lookup"><span data-stu-id="d3309-119">Name</span></span>|<span data-ttu-id="d3309-120">说明</span><span class="sxs-lookup"><span data-stu-id="d3309-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3309-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3309-121">Authorization</span></span>|<span data-ttu-id="d3309-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3309-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3309-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3309-124">Request body</span></span>
<span data-ttu-id="d3309-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3309-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3309-126">响应</span><span class="sxs-lookup"><span data-stu-id="d3309-126">Response</span></span>

<span data-ttu-id="d3309-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d3309-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3309-129">示例</span><span class="sxs-lookup"><span data-stu-id="d3309-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3309-130">请求</span><span class="sxs-lookup"><span data-stu-id="d3309-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalconnection"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr
```


### <a name="response"></a><span data-ttu-id="d3309-131">响应</span><span class="sxs-lookup"><span data-stu-id="d3309-131">Response</span></span>
<span data-ttu-id="d3309-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3309-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

