---
title: 删除 unifiedGroupSource
description: 删除 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e2eb86c566703e6c23262a0ddb572e438d33ce
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597592"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="86218-103">删除 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="86218-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="86218-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86218-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86218-105">删除 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86218-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86218-106">权限</span><span class="sxs-lookup"><span data-stu-id="86218-106">Permissions</span></span>

<span data-ttu-id="86218-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86218-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86218-109">Permission type</span></span>|<span data-ttu-id="86218-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86218-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86218-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86218-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86218-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="86218-112">User.Read</span></span>|
|<span data-ttu-id="86218-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86218-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86218-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86218-114">Not supported.</span></span>|
|<span data-ttu-id="86218-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86218-115">Application</span></span>|<span data-ttu-id="86218-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86218-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86218-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86218-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="86218-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="86218-118">Request headers</span></span>

|<span data-ttu-id="86218-119">名称</span><span class="sxs-lookup"><span data-stu-id="86218-119">Name</span></span>|<span data-ttu-id="86218-120">说明</span><span class="sxs-lookup"><span data-stu-id="86218-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86218-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86218-121">Authorization</span></span>|<span data-ttu-id="86218-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86218-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86218-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="86218-124">Request body</span></span>

<span data-ttu-id="86218-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86218-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86218-126">响应</span><span class="sxs-lookup"><span data-stu-id="86218-126">Response</span></span>

<span data-ttu-id="86218-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="86218-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86218-128">示例</span><span class="sxs-lookup"><span data-stu-id="86218-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86218-129">请求</span><span class="sxs-lookup"><span data-stu-id="86218-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

### <a name="response"></a><span data-ttu-id="86218-130">响应</span><span class="sxs-lookup"><span data-stu-id="86218-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
