---
title: 列出 azureADDevice 资源
description: 获取 azureADDevice 对象及其属性的列表。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 84c70d23b1b8bfadbc1820ea63a0589d972a4b40
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239289"
---
# <a name="list-azureaddevice-resources"></a><span data-ttu-id="c0ed4-103">列出 azureADDevice 资源</span><span class="sxs-lookup"><span data-stu-id="c0ed4-103">List azureADDevice resources</span></span>
<span data-ttu-id="c0ed4-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c0ed4-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0ed4-105">获取 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-105">Get a list of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>

<span data-ttu-id="c0ed4-106">此操作筛选完全限定的资源类型， `microsoft.graph.windowsUpdates.azureADDevice` 该类型继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.azureADDevice`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0ed4-107">权限</span><span class="sxs-lookup"><span data-stu-id="c0ed4-107">Permissions</span></span>
<span data-ttu-id="c0ed4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ed4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0ed4-110">Permission type</span></span>|<span data-ttu-id="c0ed4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0ed4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0ed4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ed4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0ed4-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ed4-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c0ed4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ed4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0ed4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-115">Not supported.</span></span>|
|<span data-ttu-id="c0ed4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0ed4-116">Application</span></span>|<span data-ttu-id="c0ed4-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ed4-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0ed4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0ed4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0ed4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0ed4-119">Optional query parameters</span></span>
<span data-ttu-id="c0ed4-120">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="c0ed4-121">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含完整的资源类型。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="c0ed4-122">例如，若要选择 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0ed4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0ed4-123">Request headers</span></span>
|<span data-ttu-id="c0ed4-124">名称</span><span class="sxs-lookup"><span data-stu-id="c0ed4-124">Name</span></span>|<span data-ttu-id="c0ed4-125">说明</span><span class="sxs-lookup"><span data-stu-id="c0ed4-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0ed4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ed4-126">Authorization</span></span>|<span data-ttu-id="c0ed4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0ed4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0ed4-129">Request body</span></span>
<span data-ttu-id="c0ed4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0ed4-131">响应</span><span class="sxs-lookup"><span data-stu-id="c0ed4-131">Response</span></span>

<span data-ttu-id="c0ed4-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0ed4-132">If successful, this method returns a `200 OK` response code and a collection of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0ed4-133">示例</span><span class="sxs-lookup"><span data-stu-id="c0ed4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0ed4-134">请求</span><span class="sxs-lookup"><span data-stu-id="c0ed4-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0ed4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0ed4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```
# <a name="c"></a>[<span data-ttu-id="c0ed4-136">C#</span><span class="sxs-lookup"><span data-stu-id="c0ed4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0ed4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0ed4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0ed4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0ed4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0ed4-139">Java</span><span class="sxs-lookup"><span data-stu-id="c0ed4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0ed4-140">响应</span><span class="sxs-lookup"><span data-stu-id="c0ed4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.azureADDevice)"
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
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "90b91efa-6d46-42cd-ad4d-381831773a85",
      "errors": [],
      "enrollments": []
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "0ee3eb63-caf3-44ce-9769-b83188cc683d",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": []
    }
  ]
}
```

