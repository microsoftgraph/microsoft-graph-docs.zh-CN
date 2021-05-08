---
title: 获取 updatableAsset
description: 读取 updatableAsset 对象的属性和关系。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d89622adca8c28ebae52afa492eb233f0c1c0c72
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241201"
---
# <a name="get-updatableasset"></a><span data-ttu-id="c124d-103">获取 updatableAsset</span><span class="sxs-lookup"><span data-stu-id="c124d-103">Get updatableAsset</span></span>
<span data-ttu-id="c124d-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c124d-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c124d-105">读取 [updatableAsset 对象的属性和](../resources/windowsupdates-updatableasset.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c124d-105">Read the properties and relationships of an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c124d-106">权限</span><span class="sxs-lookup"><span data-stu-id="c124d-106">Permissions</span></span>
<span data-ttu-id="c124d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c124d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c124d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c124d-109">Permission type</span></span>|<span data-ttu-id="c124d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c124d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c124d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c124d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c124d-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c124d-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c124d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c124d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c124d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c124d-114">Not supported.</span></span>|
|<span data-ttu-id="c124d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c124d-115">Application</span></span>|<span data-ttu-id="c124d-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c124d-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c124d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c124d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c124d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c124d-118">Optional query parameters</span></span>
<span data-ttu-id="c124d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c124d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c124d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c124d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="c124d-121">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含属性的完整资源类型。</span><span class="sxs-lookup"><span data-stu-id="c124d-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="c124d-122">例如，若要应用于 `$select` [azureADDevice](../resources/windowsupdates-azureaddevice.md)的 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="c124d-122">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c124d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c124d-123">Request headers</span></span>
|<span data-ttu-id="c124d-124">名称</span><span class="sxs-lookup"><span data-stu-id="c124d-124">Name</span></span>|<span data-ttu-id="c124d-125">说明</span><span class="sxs-lookup"><span data-stu-id="c124d-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c124d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c124d-126">Authorization</span></span>|<span data-ttu-id="c124d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c124d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c124d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c124d-129">Request body</span></span>
<span data-ttu-id="c124d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c124d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c124d-131">响应</span><span class="sxs-lookup"><span data-stu-id="c124d-131">Response</span></span>

<span data-ttu-id="c124d-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c124d-132">If successful, this method returns a `200 OK` response code and an [updatableAsset](../resources/windowsupdates-updatableasset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c124d-133">示例</span><span class="sxs-lookup"><span data-stu-id="c124d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c124d-134">请求</span><span class="sxs-lookup"><span data-stu-id="c124d-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c124d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c124d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```
# <a name="c"></a>[<span data-ttu-id="c124d-136">C#</span><span class="sxs-lookup"><span data-stu-id="c124d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c124d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c124d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c124d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c124d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c124d-139">Java</span><span class="sxs-lookup"><span data-stu-id="c124d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c124d-140">响应</span><span class="sxs-lookup"><span data-stu-id="c124d-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
    "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
  }
}
```

