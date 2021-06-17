---
title: 删除 cloudPcUserSetting
description: 删除 cloudPcUserSetting 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a3a6c5b7c7c75b89d1c27adcf7b123788f5cfe51
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993647"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="f34df-103">删除 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="f34df-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="f34df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f34df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f34df-105">删除 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f34df-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="f34df-106">权限</span><span class="sxs-lookup"><span data-stu-id="f34df-106">Permissions</span></span>

<span data-ttu-id="f34df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f34df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f34df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f34df-109">Permission type</span></span>|<span data-ttu-id="f34df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f34df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f34df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f34df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f34df-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34df-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f34df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f34df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f34df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f34df-114">Not supported.</span></span>|
|<span data-ttu-id="f34df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f34df-115">Application</span></span>|<span data-ttu-id="f34df-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34df-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f34df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f34df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f34df-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f34df-118">Request headers</span></span>
|<span data-ttu-id="f34df-119">名称</span><span class="sxs-lookup"><span data-stu-id="f34df-119">Name</span></span>|<span data-ttu-id="f34df-120">说明</span><span class="sxs-lookup"><span data-stu-id="f34df-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f34df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f34df-121">Authorization</span></span>|<span data-ttu-id="f34df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f34df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f34df-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f34df-124">Request body</span></span>
<span data-ttu-id="f34df-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f34df-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f34df-126">响应</span><span class="sxs-lookup"><span data-stu-id="f34df-126">Response</span></span>

<span data-ttu-id="f34df-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f34df-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f34df-128">示例</span><span class="sxs-lookup"><span data-stu-id="f34df-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f34df-129">请求</span><span class="sxs-lookup"><span data-stu-id="f34df-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```


### <a name="response"></a><span data-ttu-id="f34df-130">响应</span><span class="sxs-lookup"><span data-stu-id="f34df-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
