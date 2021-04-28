---
title: 删除 azureADDevice
description: 删除 azureADDevice 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6cb9d23b01241878eff96e7301f8322baa7f0fb0
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067841"
---
# <a name="delete-azureaddevice"></a><span data-ttu-id="3c990-103">删除 azureADDevice</span><span class="sxs-lookup"><span data-stu-id="3c990-103">Delete azureADDevice</span></span>
<span data-ttu-id="3c990-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3c990-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c990-105">删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c990-105">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

<span data-ttu-id="3c990-106">删除 Azure AD 设备后，它将从部署服务注销，并自动注销该服务管理的所有更新类别，以及从每个 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)中删除。</span><span class="sxs-lookup"><span data-stu-id="3c990-106">When an Azure AD device is deleted, it is unregistered from the deployment service and automatically unenrolled from management by the service for all update categories, as well as removed from every [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c990-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c990-107">Permissions</span></span>
<span data-ttu-id="3c990-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c990-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c990-110">Permission type</span></span>|<span data-ttu-id="3c990-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c990-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c990-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c990-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c990-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c990-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="3c990-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c990-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c990-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c990-115">Not supported.</span></span>|
|<span data-ttu-id="3c990-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c990-116">Application</span></span>|<span data-ttu-id="3c990-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c990-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c990-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c990-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="3c990-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c990-119">Request headers</span></span>
|<span data-ttu-id="3c990-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c990-120">Name</span></span>|<span data-ttu-id="3c990-121">说明</span><span class="sxs-lookup"><span data-stu-id="3c990-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c990-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c990-122">Authorization</span></span>|<span data-ttu-id="3c990-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c990-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c990-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c990-125">Request body</span></span>
<span data-ttu-id="3c990-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c990-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c990-127">响应</span><span class="sxs-lookup"><span data-stu-id="3c990-127">Response</span></span>

<span data-ttu-id="3c990-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c990-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c990-130">示例</span><span class="sxs-lookup"><span data-stu-id="3c990-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c990-131">请求</span><span class="sxs-lookup"><span data-stu-id="3c990-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="3c990-132">响应</span><span class="sxs-lookup"><span data-stu-id="3c990-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

