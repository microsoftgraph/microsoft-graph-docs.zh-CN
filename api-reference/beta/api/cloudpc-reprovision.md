---
title: cloudPC：重新设置
description: 重新设置特定云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 33a467fad7368750fda2dd814c414ed01961ecc4
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378290"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="ac257-103">cloudPC：重新设置</span><span class="sxs-lookup"><span data-stu-id="ac257-103">cloudPC: reprovision</span></span>

<span data-ttu-id="ac257-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac257-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac257-105">重新设置特定云电脑。</span><span class="sxs-lookup"><span data-stu-id="ac257-105">Reprovision a specific cloud PC.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac257-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ac257-106">Permissions</span></span>

<span data-ttu-id="ac257-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac257-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac257-109">Permission type</span></span>|<span data-ttu-id="ac257-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ac257-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac257-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac257-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac257-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac257-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ac257-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac257-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac257-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac257-114">Not supported.</span></span>|
|<span data-ttu-id="ac257-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac257-115">Application</span></span>|<span data-ttu-id="ac257-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac257-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac257-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac257-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="ac257-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac257-118">Request headers</span></span>

|<span data-ttu-id="ac257-119">名称</span><span class="sxs-lookup"><span data-stu-id="ac257-119">Name</span></span>|<span data-ttu-id="ac257-120">说明</span><span class="sxs-lookup"><span data-stu-id="ac257-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac257-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac257-121">Authorization</span></span>|<span data-ttu-id="ac257-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac257-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac257-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac257-124">Request body</span></span>

<span data-ttu-id="ac257-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac257-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac257-126">响应</span><span class="sxs-lookup"><span data-stu-id="ac257-126">Response</span></span>

<span data-ttu-id="ac257-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ac257-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ac257-128">示例</span><span class="sxs-lookup"><span data-stu-id="ac257-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac257-129">请求</span><span class="sxs-lookup"><span data-stu-id="ac257-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

### <a name="response"></a><span data-ttu-id="ac257-130">响应</span><span class="sxs-lookup"><span data-stu-id="ac257-130">Response</span></span>

<span data-ttu-id="ac257-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac257-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
