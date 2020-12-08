---
title: ediscoveryCase： close
description: 关闭电子数据展示事例。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 627c8c1547e8df03c6736f00a5cb571d1c8c93bb
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597577"
---
# <a name="ediscoverycase-close"></a><span data-ttu-id="c7883-103">ediscoveryCase： close</span><span class="sxs-lookup"><span data-stu-id="c7883-103">ediscoveryCase: close</span></span>

<span data-ttu-id="c7883-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7883-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7883-105">关闭电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="c7883-105">Close an eDiscovery case.</span></span> <span data-ttu-id="c7883-106">有关详细信息，请参阅 [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case)。</span><span class="sxs-lookup"><span data-stu-id="c7883-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7883-107">权限</span><span class="sxs-lookup"><span data-stu-id="c7883-107">Permissions</span></span>

<span data-ttu-id="c7883-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7883-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7883-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7883-110">Permission type</span></span>|<span data-ttu-id="c7883-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7883-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7883-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7883-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7883-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="c7883-113">User.Read</span></span>|
|<span data-ttu-id="c7883-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7883-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7883-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7883-115">Not supported.</span></span>|
|<span data-ttu-id="c7883-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7883-116">Application</span></span>|<span data-ttu-id="c7883-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7883-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7883-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7883-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="c7883-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7883-119">Request headers</span></span>

|<span data-ttu-id="c7883-120">名称</span><span class="sxs-lookup"><span data-stu-id="c7883-120">Name</span></span>|<span data-ttu-id="c7883-121">说明</span><span class="sxs-lookup"><span data-stu-id="c7883-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7883-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7883-122">Authorization</span></span>|<span data-ttu-id="c7883-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7883-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7883-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7883-125">Request body</span></span>

<span data-ttu-id="c7883-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7883-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7883-127">响应</span><span class="sxs-lookup"><span data-stu-id="c7883-127">Response</span></span>

<span data-ttu-id="c7883-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c7883-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7883-129">示例</span><span class="sxs-lookup"><span data-stu-id="c7883-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7883-130">请求</span><span class="sxs-lookup"><span data-stu-id="c7883-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "ediscoverycase_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

### <a name="response"></a><span data-ttu-id="c7883-131">响应</span><span class="sxs-lookup"><span data-stu-id="c7883-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
