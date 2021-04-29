---
title: 获取设置
description: 读取 settings 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1d4db6227db2793211f900adce5bbe2ca6a68efa
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080723"
---
# <a name="get-settings"></a><span data-ttu-id="0eeb2-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="0eeb2-103">Get settings</span></span>

<span data-ttu-id="0eeb2-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0eeb2-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eeb2-105">读取 settings [对象的属性和](../resources/ediscovery-settings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-105">Read the properties and relationships of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eeb2-106">权限</span><span class="sxs-lookup"><span data-stu-id="0eeb2-106">Permissions</span></span>

<span data-ttu-id="0eeb2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eeb2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0eeb2-109">Permission type</span></span>|<span data-ttu-id="0eeb2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0eeb2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eeb2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0eeb2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0eeb2-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eeb2-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0eeb2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0eeb2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eeb2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-114">Not supported.</span></span>|
|<span data-ttu-id="0eeb2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0eeb2-115">Application</span></span>|<span data-ttu-id="0eeb2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eeb2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0eeb2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eeb2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0eeb2-118">Optional query parameters</span></span>

<span data-ttu-id="0eeb2-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0eeb2-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eeb2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0eeb2-121">Request headers</span></span>

|<span data-ttu-id="0eeb2-122">名称</span><span class="sxs-lookup"><span data-stu-id="0eeb2-122">Name</span></span>|<span data-ttu-id="0eeb2-123">说明</span><span class="sxs-lookup"><span data-stu-id="0eeb2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0eeb2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eeb2-124">Authorization</span></span>|<span data-ttu-id="0eeb2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eeb2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0eeb2-127">Request body</span></span>

<span data-ttu-id="0eeb2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eeb2-129">响应</span><span class="sxs-lookup"><span data-stu-id="0eeb2-129">Response</span></span>

<span data-ttu-id="0eeb2-130">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/ediscovery-settings.md) 代码和 settings 对象。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-130">If successful, this method returns a `200 OK` response code and a [settings](../resources/ediscovery-settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0eeb2-131">示例</span><span class="sxs-lookup"><span data-stu-id="0eeb2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0eeb2-132">请求</span><span class="sxs-lookup"><span data-stu-id="0eeb2-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings
```

### <a name="response"></a><span data-ttu-id="0eeb2-133">响应</span><span class="sxs-lookup"><span data-stu-id="0eeb2-133">Response</span></span>

<span data-ttu-id="0eeb2-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0eeb2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.settings"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/settings/$entity",
    "id": "5b840b94-f821-4c4a-8cad-3a90062bf51a",
    "redundancyDetection": {
        "isEnabled": true,
        "similarityThreshold": 65,
        "minWords": 10,
        "maxWords": 500000
    },
    "topicModeling": {
        "isEnabled": true,
        "ignoreNumbers": true,
        "topicCount": 100,
        "dynamicallyAdjustTopicCount": true
    },
    "ocr": {
        "isEnabled": false,
        "maxImageSize": 24576,
        "timeout": "PT1M"
    }
}
```
