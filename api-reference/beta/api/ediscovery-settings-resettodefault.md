---
title: 设置：resetToDefault
description: 将大小写设置重置为默认值。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3bc0cbcad51243e7f264ce69e92370cba864df54
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239663"
---
# <a name="settings-resettodefault"></a><span data-ttu-id="98d5d-103">设置：resetToDefault</span><span class="sxs-lookup"><span data-stu-id="98d5d-103">settings: resetToDefault</span></span>

<span data-ttu-id="98d5d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="98d5d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d5d-105">将大小写设置重置为默认值。</span><span class="sxs-lookup"><span data-stu-id="98d5d-105">Reset the case settings to the default values.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d5d-106">权限</span><span class="sxs-lookup"><span data-stu-id="98d5d-106">Permissions</span></span>

<span data-ttu-id="98d5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98d5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="98d5d-109">Permission type</span></span>|<span data-ttu-id="98d5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98d5d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98d5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98d5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="98d5d-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d5d-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="98d5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98d5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98d5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d5d-114">Not supported.</span></span>|
|<span data-ttu-id="98d5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="98d5d-115">Application</span></span>|<span data-ttu-id="98d5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d5d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98d5d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98d5d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

## <a name="request-headers"></a><span data-ttu-id="98d5d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="98d5d-118">Request headers</span></span>

|<span data-ttu-id="98d5d-119">名称</span><span class="sxs-lookup"><span data-stu-id="98d5d-119">Name</span></span>|<span data-ttu-id="98d5d-120">说明</span><span class="sxs-lookup"><span data-stu-id="98d5d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="98d5d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d5d-121">Authorization</span></span>|<span data-ttu-id="98d5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98d5d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d5d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="98d5d-124">Request body</span></span>

<span data-ttu-id="98d5d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98d5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d5d-126">响应</span><span class="sxs-lookup"><span data-stu-id="98d5d-126">Response</span></span>

<span data-ttu-id="98d5d-127">如果成功，此操作返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="98d5d-127">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="98d5d-128">示例</span><span class="sxs-lookup"><span data-stu-id="98d5d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98d5d-129">请求</span><span class="sxs-lookup"><span data-stu-id="98d5d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98d5d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="98d5d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```
# <a name="c"></a>[<span data-ttu-id="98d5d-131">C#</span><span class="sxs-lookup"><span data-stu-id="98d5d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/settings-resettodefault-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98d5d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98d5d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/settings-resettodefault-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98d5d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98d5d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/settings-resettodefault-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98d5d-134">Java</span><span class="sxs-lookup"><span data-stu-id="98d5d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/settings-resettodefault-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98d5d-135">响应</span><span class="sxs-lookup"><span data-stu-id="98d5d-135">Response</span></span>

<span data-ttu-id="98d5d-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="98d5d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
