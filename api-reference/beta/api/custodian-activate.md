---
title: 保管人：激活
description: 在某个情况下重新激活管理员。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 40ac381da15065a4363471ba9c82c19080b84884
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597565"
---
# <a name="custodian-activate"></a><span data-ttu-id="bdcd8-103">保管人：激活</span><span class="sxs-lookup"><span data-stu-id="bdcd8-103">custodian: activate</span></span>

<span data-ttu-id="bdcd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdcd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdcd8-105">激活已从事例中释放的管理员，使其再次成为事例的一部分。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="bdcd8-106">有关详细信息，请参阅 [在高级电子数据展示事例中管理保管人](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdcd8-107">权限</span><span class="sxs-lookup"><span data-stu-id="bdcd8-107">Permissions</span></span>

<span data-ttu-id="bdcd8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdcd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdcd8-110">Permission type</span></span>|<span data-ttu-id="bdcd8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bdcd8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdcd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdcd8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdcd8-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="bdcd8-113">User.Read</span></span>|
|<span data-ttu-id="bdcd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdcd8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdcd8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-115">Not supported.</span></span>|
|<span data-ttu-id="bdcd8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdcd8-116">Application</span></span>|<span data-ttu-id="bdcd8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdcd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdcd8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="bdcd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdcd8-119">Request headers</span></span>

|<span data-ttu-id="bdcd8-120">名称</span><span class="sxs-lookup"><span data-stu-id="bdcd8-120">Name</span></span>|<span data-ttu-id="bdcd8-121">说明</span><span class="sxs-lookup"><span data-stu-id="bdcd8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bdcd8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdcd8-122">Authorization</span></span>|<span data-ttu-id="bdcd8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bdcd8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdcd8-125">Content-Type</span></span>|<span data-ttu-id="bdcd8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bdcd8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdcd8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdcd8-128">Request body</span></span>

<span data-ttu-id="bdcd8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdcd8-130">响应</span><span class="sxs-lookup"><span data-stu-id="bdcd8-130">Response</span></span>

<span data-ttu-id="bdcd8-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bdcd8-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bdcd8-132">示例</span><span class="sxs-lookup"><span data-stu-id="bdcd8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdcd8-133">请求</span><span class="sxs-lookup"><span data-stu-id="bdcd8-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```

### <a name="response"></a><span data-ttu-id="bdcd8-134">响应</span><span class="sxs-lookup"><span data-stu-id="bdcd8-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
