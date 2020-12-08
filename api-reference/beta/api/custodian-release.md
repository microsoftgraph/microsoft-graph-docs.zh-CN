---
title: 管理员：发布
description: 从案例发布管理员。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 59e3ef5721c10419261443ca57d7584035dc1622
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597507"
---
# <a name="custodian-release"></a><span data-ttu-id="32b64-103">管理员：发布</span><span class="sxs-lookup"><span data-stu-id="32b64-103">custodian: release</span></span>

<span data-ttu-id="32b64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32b64-105">从案例发布管理员。</span><span class="sxs-lookup"><span data-stu-id="32b64-105">Release a custodian from a case.</span></span> <span data-ttu-id="32b64-106">有关详细信息，请参阅 [从案例释放管理员](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case)。</span><span class="sxs-lookup"><span data-stu-id="32b64-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="32b64-107">权限</span><span class="sxs-lookup"><span data-stu-id="32b64-107">Permissions</span></span>

<span data-ttu-id="32b64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32b64-110">Permission type</span></span>|<span data-ttu-id="32b64-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32b64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32b64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32b64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32b64-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="32b64-113">User.Read</span></span>|
|<span data-ttu-id="32b64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32b64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32b64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32b64-115">Not supported.</span></span>|
|<span data-ttu-id="32b64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32b64-116">Application</span></span>|<span data-ttu-id="32b64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="32b64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32b64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32b64-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="32b64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="32b64-119">Request headers</span></span>

|<span data-ttu-id="32b64-120">名称</span><span class="sxs-lookup"><span data-stu-id="32b64-120">Name</span></span>|<span data-ttu-id="32b64-121">说明</span><span class="sxs-lookup"><span data-stu-id="32b64-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32b64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b64-122">Authorization</span></span>|<span data-ttu-id="32b64-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32b64-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32b64-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32b64-125">Content-Type</span></span>|<span data-ttu-id="32b64-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32b64-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32b64-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="32b64-128">Request body</span></span>

<span data-ttu-id="32b64-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32b64-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32b64-130">响应</span><span class="sxs-lookup"><span data-stu-id="32b64-130">Response</span></span>

<span data-ttu-id="32b64-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32b64-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="32b64-132">示例</span><span class="sxs-lookup"><span data-stu-id="32b64-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32b64-133">请求</span><span class="sxs-lookup"><span data-stu-id="32b64-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```

### <a name="response"></a><span data-ttu-id="32b64-134">响应</span><span class="sxs-lookup"><span data-stu-id="32b64-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
