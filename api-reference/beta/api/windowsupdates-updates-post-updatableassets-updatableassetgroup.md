---
title: 创建 updatableAssetGroup
description: 创建新的 updatableAssetGroup 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 9e3abe53f8e18236cb83fa9105d3890bc21dcce9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067319"
---
# <a name="create-updatableassetgroup"></a><span data-ttu-id="f0d9c-103">创建 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="f0d9c-103">Create updatableAssetGroup</span></span>
<span data-ttu-id="f0d9c-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f0d9c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0d9c-105">创建新的 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-105">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="f0d9c-106">**updatableAssetGroup** 资源继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-106">The **updatableAssetGroup** resource inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0d9c-107">权限</span><span class="sxs-lookup"><span data-stu-id="f0d9c-107">Permissions</span></span>
<span data-ttu-id="f0d9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0d9c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0d9c-110">Permission type</span></span>|<span data-ttu-id="f0d9c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0d9c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0d9c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0d9c-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0d9c-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f0d9c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0d9c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-115">Not supported.</span></span>|
|<span data-ttu-id="f0d9c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0d9c-116">Application</span></span>|<span data-ttu-id="f0d9c-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0d9c-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0d9c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0d9c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets
```

## <a name="request-headers"></a><span data-ttu-id="f0d9c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0d9c-119">Request headers</span></span>
|<span data-ttu-id="f0d9c-120">名称</span><span class="sxs-lookup"><span data-stu-id="f0d9c-120">Name</span></span>|<span data-ttu-id="f0d9c-121">说明</span><span class="sxs-lookup"><span data-stu-id="f0d9c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0d9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d9c-122">Authorization</span></span>|<span data-ttu-id="f0d9c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f0d9c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0d9c-125">Content-Type</span></span>|<span data-ttu-id="f0d9c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f0d9c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0d9c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0d9c-128">Request body</span></span>
<span data-ttu-id="f0d9c-129">在请求正文中，提供 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-129">In the request body, supply a JSON representation of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="f0d9c-130">无需任何属性。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-130">No properties are required.</span></span>


## <a name="response"></a><span data-ttu-id="f0d9c-131">响应</span><span class="sxs-lookup"><span data-stu-id="f0d9c-131">Response</span></span>

<span data-ttu-id="f0d9c-132">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0d9c-132">If successful, this method returns a `201 Created` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0d9c-133">示例</span><span class="sxs-lookup"><span data-stu-id="f0d9c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0d9c-134">请求</span><span class="sxs-lookup"><span data-stu-id="f0d9c-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_updatableassetgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
Content-Type: application/json
Content-length: 76

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup"
}
```


### <a name="response"></a><span data-ttu-id="f0d9c-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0d9c-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
}
```

