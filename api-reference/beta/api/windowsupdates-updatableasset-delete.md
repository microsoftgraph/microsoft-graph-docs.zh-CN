---
title: 删除 updatableAsset
description: 删除 updatableAsset 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7dd7aaf3317eef98568ba89fc3e2c158e64e2784
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067838"
---
# <a name="delete-updatableasset"></a><span data-ttu-id="94aec-103">删除 updatableAsset</span><span class="sxs-lookup"><span data-stu-id="94aec-103">Delete updatableAsset</span></span>
<span data-ttu-id="94aec-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="94aec-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94aec-105">删除 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94aec-105">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94aec-106">权限</span><span class="sxs-lookup"><span data-stu-id="94aec-106">Permissions</span></span>
<span data-ttu-id="94aec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94aec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94aec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94aec-109">Permission type</span></span>|<span data-ttu-id="94aec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94aec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94aec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94aec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94aec-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94aec-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="94aec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94aec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94aec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="94aec-114">Not supported.</span></span>|
|<span data-ttu-id="94aec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="94aec-115">Application</span></span>|<span data-ttu-id="94aec-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94aec-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94aec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94aec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="request-headers"></a><span data-ttu-id="94aec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="94aec-118">Request headers</span></span>
|<span data-ttu-id="94aec-119">名称</span><span class="sxs-lookup"><span data-stu-id="94aec-119">Name</span></span>|<span data-ttu-id="94aec-120">说明</span><span class="sxs-lookup"><span data-stu-id="94aec-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94aec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94aec-121">Authorization</span></span>|<span data-ttu-id="94aec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94aec-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94aec-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="94aec-124">Request body</span></span>
<span data-ttu-id="94aec-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94aec-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94aec-126">响应</span><span class="sxs-lookup"><span data-stu-id="94aec-126">Response</span></span>

<span data-ttu-id="94aec-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="94aec-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94aec-129">示例</span><span class="sxs-lookup"><span data-stu-id="94aec-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94aec-130">请求</span><span class="sxs-lookup"><span data-stu-id="94aec-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_updatableasset"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```

### <a name="response"></a><span data-ttu-id="94aec-131">响应</span><span class="sxs-lookup"><span data-stu-id="94aec-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

