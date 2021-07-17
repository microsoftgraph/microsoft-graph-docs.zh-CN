---
title: 删除 externalItem
description: 删除 externalItem 对象。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6cf75898963765192ef5f380bddc10794c616a66
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467287"
---
# <a name="delete-externalitem"></a><span data-ttu-id="164a7-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="164a7-103">Delete externalItem</span></span>
<span data-ttu-id="164a7-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="164a7-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="164a7-105">删除 [externalItem](../resources/externalconnectors-externalitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="164a7-105">Deletes an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="164a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="164a7-106">Permissions</span></span>
<span data-ttu-id="164a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="164a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="164a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="164a7-109">Permission type</span></span>|<span data-ttu-id="164a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="164a7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="164a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="164a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="164a7-112">不适用</span><span class="sxs-lookup"><span data-stu-id="164a7-112">Not applicable</span></span>|
|<span data-ttu-id="164a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="164a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="164a7-114">不适用</span><span class="sxs-lookup"><span data-stu-id="164a7-114">Not applicable</span></span>|
|<span data-ttu-id="164a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="164a7-115">Application</span></span>| <span data-ttu-id="164a7-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="164a7-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="164a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="164a7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /connections/{connectionsId}/items/{externalItemId}
```

## <a name="request-headers"></a><span data-ttu-id="164a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="164a7-118">Request headers</span></span>
|<span data-ttu-id="164a7-119">名称</span><span class="sxs-lookup"><span data-stu-id="164a7-119">Name</span></span>|<span data-ttu-id="164a7-120">说明</span><span class="sxs-lookup"><span data-stu-id="164a7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="164a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="164a7-121">Authorization</span></span>|<span data-ttu-id="164a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="164a7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="164a7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="164a7-124">Request body</span></span>
<span data-ttu-id="164a7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="164a7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="164a7-126">响应</span><span class="sxs-lookup"><span data-stu-id="164a7-126">Response</span></span>

<span data-ttu-id="164a7-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="164a7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="164a7-128">示例</span><span class="sxs-lookup"><span data-stu-id="164a7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="164a7-129">请求</span><span class="sxs-lookup"><span data-stu-id="164a7-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="164a7-130">响应</span><span class="sxs-lookup"><span data-stu-id="164a7-130">Response</span></span>
<span data-ttu-id="164a7-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="164a7-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

