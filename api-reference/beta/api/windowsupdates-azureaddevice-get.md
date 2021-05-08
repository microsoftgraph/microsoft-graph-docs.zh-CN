---
title: 获取 azureADDevice
description: 读取 azureADDevice 对象的属性。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 480940d2b0b13ff32b002d5a1ff4a5922d9db29c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241095"
---
# <a name="get-azureaddevice"></a><span data-ttu-id="f8c6f-103">获取 azureADDevice</span><span class="sxs-lookup"><span data-stu-id="f8c6f-103">Get azureADDevice</span></span>
<span data-ttu-id="f8c6f-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f8c6f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c6f-105">读取 [azureADDevice 对象](../resources/windowsupdates-azureaddevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-105">Read the properties of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8c6f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8c6f-106">Permissions</span></span>
<span data-ttu-id="f8c6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8c6f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8c6f-109">Permission type</span></span>|<span data-ttu-id="f8c6f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8c6f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8c6f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8c6f-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c6f-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f8c6f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8c6f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-114">Not supported.</span></span>|
|<span data-ttu-id="f8c6f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8c6f-115">Application</span></span>|<span data-ttu-id="f8c6f-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c6f-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8c6f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8c6f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8c6f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8c6f-118">Optional query parameters</span></span>
<span data-ttu-id="f8c6f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8c6f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="f8c6f-121">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含完整的资源类型。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="f8c6f-122">例如，若要选择 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8c6f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8c6f-123">Request headers</span></span>
|<span data-ttu-id="f8c6f-124">名称</span><span class="sxs-lookup"><span data-stu-id="f8c6f-124">Name</span></span>|<span data-ttu-id="f8c6f-125">说明</span><span class="sxs-lookup"><span data-stu-id="f8c6f-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8c6f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c6f-126">Authorization</span></span>|<span data-ttu-id="f8c6f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8c6f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8c6f-129">Request body</span></span>
<span data-ttu-id="f8c6f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8c6f-131">响应</span><span class="sxs-lookup"><span data-stu-id="f8c6f-131">Response</span></span>

<span data-ttu-id="f8c6f-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应 [代码和 azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8c6f-132">If successful, this method returns a `200 OK` response code and an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8c6f-133">示例</span><span class="sxs-lookup"><span data-stu-id="f8c6f-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8c6f-134">请求</span><span class="sxs-lookup"><span data-stu-id="f8c6f-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f8c6f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8c6f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```
# <a name="c"></a>[<span data-ttu-id="f8c6f-136">C#</span><span class="sxs-lookup"><span data-stu-id="f8c6f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8c6f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8c6f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8c6f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8c6f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8c6f-139">Java</span><span class="sxs-lookup"><span data-stu-id="f8c6f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8c6f-140">响应</span><span class="sxs-lookup"><span data-stu-id="f8c6f-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

