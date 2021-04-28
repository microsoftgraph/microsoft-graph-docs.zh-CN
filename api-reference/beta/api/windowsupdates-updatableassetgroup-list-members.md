---
title: 列出可更新资源组的成员
description: 列出 updatableAssetGroup 资源的成员。 成员为 azureADDevice 类型。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d4e4ffca528bd4e66b0a407fe14f42a8198aa913
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067837"
---
# <a name="list-updatable-asset-group-members"></a><span data-ttu-id="49f1b-104">列出可更新资源组的成员</span><span class="sxs-lookup"><span data-stu-id="49f1b-104">List updatable asset group members</span></span>
<span data-ttu-id="49f1b-105">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="49f1b-105">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f1b-106">列出 [updatableAssetGroup 资源](../resources/windowsupdates-updatableassetgroup.md) 的成员。</span><span class="sxs-lookup"><span data-stu-id="49f1b-106">List the members of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) resource.</span></span> <span data-ttu-id="49f1b-107">成员为 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="49f1b-107">Members are of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) type.</span></span>

<span data-ttu-id="49f1b-108">此操作引用 **updatableAssetGroup** 资源的 members 导航属性。 </span><span class="sxs-lookup"><span data-stu-id="49f1b-108">This operation references the **members** navigation property of an **updatableAssetGroup** resource.</span></span> <span data-ttu-id="49f1b-109">若要引用派生自 [updatableAsset](../resources/windowsupdates-updatableasset.md)的类型的属性，在查询 URL 中包括完全派生的资源类型，即 `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members` 。</span><span class="sxs-lookup"><span data-stu-id="49f1b-109">To reference a property of a type derived from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full derived resource type in the query URL, i.e., `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members`.</span></span>

## <a name="permissions"></a><span data-ttu-id="49f1b-110">权限</span><span class="sxs-lookup"><span data-stu-id="49f1b-110">Permissions</span></span>
<span data-ttu-id="49f1b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49f1b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f1b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="49f1b-113">Permission type</span></span>|<span data-ttu-id="49f1b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49f1b-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f1b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49f1b-115">Delegated (work or school account)</span></span>|<span data-ttu-id="49f1b-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f1b-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="49f1b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49f1b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f1b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="49f1b-118">Not supported.</span></span>|
|<span data-ttu-id="49f1b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="49f1b-119">Application</span></span>|<span data-ttu-id="49f1b-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f1b-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f1b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49f1b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49f1b-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49f1b-122">Optional query parameters</span></span>
<span data-ttu-id="49f1b-123">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="49f1b-123">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="49f1b-124">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含属性的完整资源类型。</span><span class="sxs-lookup"><span data-stu-id="49f1b-124">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="49f1b-125">例如，若要应用于 `$select` [azureADDevice](../resources/windowsupdates-azureaddevice.md)的 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="49f1b-125">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49f1b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="49f1b-126">Request headers</span></span>
|<span data-ttu-id="49f1b-127">名称</span><span class="sxs-lookup"><span data-stu-id="49f1b-127">Name</span></span>|<span data-ttu-id="49f1b-128">说明</span><span class="sxs-lookup"><span data-stu-id="49f1b-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49f1b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="49f1b-129">Authorization</span></span>|<span data-ttu-id="49f1b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49f1b-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f1b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="49f1b-132">Request body</span></span>
<span data-ttu-id="49f1b-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49f1b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49f1b-134">响应</span><span class="sxs-lookup"><span data-stu-id="49f1b-134">Response</span></span>

<span data-ttu-id="49f1b-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="49f1b-135">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49f1b-136">示例</span><span class="sxs-lookup"><span data-stu-id="49f1b-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49f1b-137">请求</span><span class="sxs-lookup"><span data-stu-id="49f1b-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```


### <a name="response"></a><span data-ttu-id="49f1b-138">响应</span><span class="sxs-lookup"><span data-stu-id="49f1b-138">Response</span></span>

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
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "6d49dfaf-9c24-42f7-9628-c136e35774c8"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "1f61492e-4e34-4dee-904a-0d38299e76b2"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "bfe3c2d1-4cef-4952-8c5e-30d56ccf0cdc"
    }
  ]
}
```

