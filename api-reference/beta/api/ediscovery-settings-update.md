---
title: 更新设置
description: 更新 settings 对象的属性。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bbaf760948fc8ee7079e1c746405afddcd73a2b5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240828"
---
# <a name="update-settings"></a><span data-ttu-id="27d96-103">更新设置</span><span class="sxs-lookup"><span data-stu-id="27d96-103">Update settings</span></span>

<span data-ttu-id="27d96-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="27d96-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d96-105">更新 settings [对象的属性](../resources/ediscovery-settings.md) 。</span><span class="sxs-lookup"><span data-stu-id="27d96-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d96-106">权限</span><span class="sxs-lookup"><span data-stu-id="27d96-106">Permissions</span></span>

<span data-ttu-id="27d96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27d96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27d96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="27d96-109">Permission type</span></span>|<span data-ttu-id="27d96-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27d96-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27d96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27d96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27d96-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d96-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="27d96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27d96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27d96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d96-114">Not supported.</span></span>|
|<span data-ttu-id="27d96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="27d96-115">Application</span></span>|<span data-ttu-id="27d96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d96-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27d96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27d96-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="27d96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="27d96-118">Request headers</span></span>

|<span data-ttu-id="27d96-119">名称</span><span class="sxs-lookup"><span data-stu-id="27d96-119">Name</span></span>|<span data-ttu-id="27d96-120">说明</span><span class="sxs-lookup"><span data-stu-id="27d96-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27d96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27d96-121">Authorization</span></span>|<span data-ttu-id="27d96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27d96-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27d96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27d96-124">Content-Type</span></span>|<span data-ttu-id="27d96-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="27d96-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27d96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27d96-127">Request body</span></span>

<span data-ttu-id="27d96-128">在请求正文中，提供 settings 对象的 JSON [表示](../resources/ediscovery-settings.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="27d96-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27d96-129">响应</span><span class="sxs-lookup"><span data-stu-id="27d96-129">Response</span></span>

<span data-ttu-id="27d96-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="27d96-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="27d96-131">示例</span><span class="sxs-lookup"><span data-stu-id="27d96-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27d96-132">请求</span><span class="sxs-lookup"><span data-stu-id="27d96-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="27d96-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d96-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="27d96-134">C#</span><span class="sxs-lookup"><span data-stu-id="27d96-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27d96-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d96-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27d96-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27d96-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27d96-137">Java</span><span class="sxs-lookup"><span data-stu-id="27d96-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27d96-138">响应</span><span class="sxs-lookup"><span data-stu-id="27d96-138">Response</span></span>

<span data-ttu-id="27d96-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="27d96-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
