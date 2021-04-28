---
title: 删除 updatableAssetGroup
description: 删除 updatableAssetGroup 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 207f9df658365e747089a2d77bf15dcb1d50e795
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068012"
---
# <a name="delete-updatableassetgroup"></a><span data-ttu-id="f94e4-103">删除 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="f94e4-103">Delete updatableAssetGroup</span></span>
<span data-ttu-id="f94e4-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f94e4-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f94e4-105">删除 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f94e4-105">Delete an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="f94e4-106">当 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象时，不会删除其成员 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f94e4-106">When an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object, its member [updatableAsset](../resources/windowsupdates-updatableasset.md) objects are not deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f94e4-107">权限</span><span class="sxs-lookup"><span data-stu-id="f94e4-107">Permissions</span></span>
<span data-ttu-id="f94e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f94e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f94e4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f94e4-110">Permission type</span></span>|<span data-ttu-id="f94e4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f94e4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f94e4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f94e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f94e4-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94e4-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f94e4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f94e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f94e4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f94e4-115">Not supported.</span></span>|
|<span data-ttu-id="f94e4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f94e4-116">Application</span></span>|<span data-ttu-id="f94e4-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94e4-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f94e4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f94e4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="f94e4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f94e4-119">Request headers</span></span>
|<span data-ttu-id="f94e4-120">名称</span><span class="sxs-lookup"><span data-stu-id="f94e4-120">Name</span></span>|<span data-ttu-id="f94e4-121">说明</span><span class="sxs-lookup"><span data-stu-id="f94e4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f94e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f94e4-122">Authorization</span></span>|<span data-ttu-id="f94e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f94e4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f94e4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f94e4-125">Request body</span></span>
<span data-ttu-id="f94e4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f94e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f94e4-127">响应</span><span class="sxs-lookup"><span data-stu-id="f94e4-127">Response</span></span>

<span data-ttu-id="f94e4-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f94e4-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f94e4-130">示例</span><span class="sxs-lookup"><span data-stu-id="f94e4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f94e4-131">请求</span><span class="sxs-lookup"><span data-stu-id="f94e4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_updatableassetgroup"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```


### <a name="response"></a><span data-ttu-id="f94e4-132">响应</span><span class="sxs-lookup"><span data-stu-id="f94e4-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

