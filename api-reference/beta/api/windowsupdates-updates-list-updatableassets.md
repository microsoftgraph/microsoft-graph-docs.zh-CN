---
title: 列出 updatableAssets
description: 获取 updatableAsset 对象及其属性的列表。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a50e24fec7c80b66eaf9ab58027cc2b3cb8814ec
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151550"
---
# <a name="list-updatableassets"></a><span data-ttu-id="c9779-103">列出 updatableAssets</span><span class="sxs-lookup"><span data-stu-id="c9779-103">List updatableAssets</span></span>
<span data-ttu-id="c9779-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c9779-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9779-105">获取 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c9779-105">Get a list of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects and their properties.</span></span>

<span data-ttu-id="c9779-106">列出可更新资源将 **返回以下派生类型的 updatableAsset** 资源 [：azureADDevice](../resources/windowsupdates-azureADDevice.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md)。</span><span class="sxs-lookup"><span data-stu-id="c9779-106">Listing updatable assets returns **updatableAsset** resources of the following derived types: [azureADDevice](../resources/windowsupdates-azureADDevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span></span>

<span data-ttu-id="c9779-107">使用 [列表 azureADDevice 资源](windowsupdates-updates-list-updatableassets-azureaddevice.md) 或 [list updatableAssetGroup](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) 资源筛选和获取仅派生类型之一的资源。</span><span class="sxs-lookup"><span data-stu-id="c9779-107">Use [list azureADDevice resources](windowsupdates-updates-list-updatableassets-azureaddevice.md) or [list updatableAssetGroup resources](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) to filter and get resources of only one of the derived types.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9779-108">权限</span><span class="sxs-lookup"><span data-stu-id="c9779-108">Permissions</span></span>
<span data-ttu-id="c9779-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9779-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9779-111">Permission type</span></span>|<span data-ttu-id="c9779-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9779-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9779-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9779-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9779-114">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9779-114">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c9779-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9779-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9779-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9779-116">Not supported.</span></span>|
|<span data-ttu-id="c9779-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9779-117">Application</span></span>|<span data-ttu-id="c9779-118">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9779-118">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9779-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9779-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9779-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9779-120">Optional query parameters</span></span>
<span data-ttu-id="c9779-121">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="c9779-121">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="c9779-122">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含属性的完整资源类型。</span><span class="sxs-lookup"><span data-stu-id="c9779-122">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="c9779-123">例如，若要应用于 `$select` [azureADDevice](../resources/windowsupdates-azureaddevice.md)的 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="c9779-123">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9779-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9779-124">Request headers</span></span>
|<span data-ttu-id="c9779-125">名称</span><span class="sxs-lookup"><span data-stu-id="c9779-125">Name</span></span>|<span data-ttu-id="c9779-126">说明</span><span class="sxs-lookup"><span data-stu-id="c9779-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9779-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9779-127">Authorization</span></span>|<span data-ttu-id="c9779-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9779-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9779-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9779-130">Request body</span></span>
<span data-ttu-id="c9779-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9779-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9779-132">响应</span><span class="sxs-lookup"><span data-stu-id="c9779-132">Response</span></span>

<span data-ttu-id="c9779-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c9779-133">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9779-134">示例</span><span class="sxs-lookup"><span data-stu-id="c9779-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9779-135">请求</span><span class="sxs-lookup"><span data-stu-id="c9779-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c9779-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9779-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
```
# <a name="c"></a>[<span data-ttu-id="c9779-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9779-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9779-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9779-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9779-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9779-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9779-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9779-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c9779-141">响应</span><span class="sxs-lookup"><span data-stu-id="c9779-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

