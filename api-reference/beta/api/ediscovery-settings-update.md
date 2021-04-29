---
title: 更新设置
description: 更新 settings 对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2892e2ecb3d0eea720267f9cc8ea5ae635bdb303
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080722"
---
# <a name="update-settings"></a><span data-ttu-id="a0679-103">更新设置</span><span class="sxs-lookup"><span data-stu-id="a0679-103">Update settings</span></span>

<span data-ttu-id="a0679-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a0679-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0679-105">更新 settings [对象的属性](../resources/ediscovery-settings.md) 。</span><span class="sxs-lookup"><span data-stu-id="a0679-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0679-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0679-106">Permissions</span></span>

<span data-ttu-id="a0679-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0679-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0679-109">Permission type</span></span>|<span data-ttu-id="a0679-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0679-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0679-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0679-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0679-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0679-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a0679-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0679-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0679-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0679-114">Not supported.</span></span>|
|<span data-ttu-id="a0679-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0679-115">Application</span></span>|<span data-ttu-id="a0679-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0679-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0679-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0679-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="a0679-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0679-118">Request headers</span></span>

|<span data-ttu-id="a0679-119">名称</span><span class="sxs-lookup"><span data-stu-id="a0679-119">Name</span></span>|<span data-ttu-id="a0679-120">说明</span><span class="sxs-lookup"><span data-stu-id="a0679-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0679-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0679-121">Authorization</span></span>|<span data-ttu-id="a0679-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0679-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a0679-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0679-124">Content-Type</span></span>|<span data-ttu-id="a0679-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a0679-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0679-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0679-127">Request body</span></span>

<span data-ttu-id="a0679-128">在请求正文中，提供 settings 对象的 JSON [表示](../resources/ediscovery-settings.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="a0679-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0679-129">响应</span><span class="sxs-lookup"><span data-stu-id="a0679-129">Response</span></span>

<span data-ttu-id="a0679-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a0679-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a0679-131">示例</span><span class="sxs-lookup"><span data-stu-id="a0679-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0679-132">请求</span><span class="sxs-lookup"><span data-stu-id="a0679-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_settings"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings
Content-Type: application/json
Content-length: 350

{
    "redundancyDetection": {
        "isEnabled": false,
        "similarityThreshold": 70,
        "minWords": 12,
        "maxWords": 400000
    },
    "topicModeling": {
        "isEnabled": false,
        "ignoreNumbers": false,
        "topicCount": 50,
        "dynamicallyAdjustTopicCount": false
    },
    "ocr": {
        "isEnabled": true,
        "maxImageSize": 12000
    }
}
```

### <a name="response"></a><span data-ttu-id="a0679-133">响应</span><span class="sxs-lookup"><span data-stu-id="a0679-133">Response</span></span>

<span data-ttu-id="a0679-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0679-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
cache-control: no-cache
client-request-id: e9fc7554-ca5e-0928-fc09-9c5825820c88
content-length: 0
request-id: 1f53bd55-f099-46cb-91df-8f5d466aba3a
```
