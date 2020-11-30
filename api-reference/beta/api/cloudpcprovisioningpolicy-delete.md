---
title: 删除 cloudPcProvisioningPolicy
description: 删除 cloudPcProvisioningPolicy 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4f85b29e0375c10f8e3bb9f1132bf7c9a8b0aafd
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378300"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="03bd6-103">删除 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="03bd6-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="03bd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03bd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03bd6-105">删除 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03bd6-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="03bd6-106">无法删除使用中的策略。</span><span class="sxs-lookup"><span data-stu-id="03bd6-106">You can’t delete a policy that’s in use.</span></span>

## <a name="permissions"></a><span data-ttu-id="03bd6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="03bd6-107">Permissions</span></span>

<span data-ttu-id="03bd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03bd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bd6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03bd6-110">Permission type</span></span>|<span data-ttu-id="03bd6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03bd6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03bd6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03bd6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03bd6-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bd6-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="03bd6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03bd6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03bd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03bd6-115">Not supported.</span></span>|
|<span data-ttu-id="03bd6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03bd6-116">Application</span></span>|<span data-ttu-id="03bd6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="03bd6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03bd6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03bd6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03bd6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="03bd6-119">Request headers</span></span>

|<span data-ttu-id="03bd6-120">名称</span><span class="sxs-lookup"><span data-stu-id="03bd6-120">Name</span></span>|<span data-ttu-id="03bd6-121">说明</span><span class="sxs-lookup"><span data-stu-id="03bd6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03bd6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03bd6-122">Authorization</span></span>|<span data-ttu-id="03bd6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03bd6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03bd6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="03bd6-125">Request body</span></span>

<span data-ttu-id="03bd6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03bd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03bd6-127">响应</span><span class="sxs-lookup"><span data-stu-id="03bd6-127">Response</span></span>

<span data-ttu-id="03bd6-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="03bd6-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="03bd6-129">示例</span><span class="sxs-lookup"><span data-stu-id="03bd6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03bd6-130">请求</span><span class="sxs-lookup"><span data-stu-id="03bd6-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="03bd6-131">响应</span><span class="sxs-lookup"><span data-stu-id="03bd6-131">Response</span></span>

<span data-ttu-id="03bd6-132">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03bd6-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
