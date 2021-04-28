---
title: 列出 updatableAssetGroup 资源
description: 获取 updatableAssetGroup 对象及其属性的列表。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4ae3141880a0ded7677184ecdb55d3dd6e554a5f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067348"
---
# <a name="list-updatableassetgroup-resources"></a><span data-ttu-id="dad29-103">列出 updatableAssetGroup 资源</span><span class="sxs-lookup"><span data-stu-id="dad29-103">List updatableAssetGroup resources</span></span>
<span data-ttu-id="dad29-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="dad29-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dad29-105">获取 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="dad29-105">Get a list of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>

<span data-ttu-id="dad29-106">此操作筛选完全限定的资源类型， `microsoft.graph.windowsUpdates.updatableAssetGroup` 该类型继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="dad29-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.updatableAssetGroup`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dad29-107">权限</span><span class="sxs-lookup"><span data-stu-id="dad29-107">Permissions</span></span>
<span data-ttu-id="dad29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dad29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad29-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dad29-110">Permission type</span></span>|<span data-ttu-id="dad29-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dad29-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad29-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dad29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dad29-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad29-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="dad29-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dad29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad29-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dad29-115">Not supported.</span></span>|
|<span data-ttu-id="dad29-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dad29-116">Application</span></span>|<span data-ttu-id="dad29-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad29-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad29-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dad29-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dad29-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dad29-119">Optional query parameters</span></span>
<span data-ttu-id="dad29-120">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="dad29-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dad29-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dad29-121">Request headers</span></span>
|<span data-ttu-id="dad29-122">名称</span><span class="sxs-lookup"><span data-stu-id="dad29-122">Name</span></span>|<span data-ttu-id="dad29-123">说明</span><span class="sxs-lookup"><span data-stu-id="dad29-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dad29-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dad29-124">Authorization</span></span>|<span data-ttu-id="dad29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dad29-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad29-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dad29-127">Request body</span></span>
<span data-ttu-id="dad29-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dad29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dad29-129">响应</span><span class="sxs-lookup"><span data-stu-id="dad29-129">Response</span></span>

<span data-ttu-id="dad29-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dad29-130">If successful, this method returns a `200 OK` response code and a collection of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dad29-131">示例</span><span class="sxs-lookup"><span data-stu-id="dad29-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dad29-132">请求</span><span class="sxs-lookup"><span data-stu-id="dad29-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```


### <a name="response"></a><span data-ttu-id="dad29-133">响应</span><span class="sxs-lookup"><span data-stu-id="dad29-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAssetGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "deb43c16-77ff-465d-aa79-366a107a6c7a"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "312643e6-b805-419f-bdf7-1a104dd6c8b9"
    }
  ]
}
```

