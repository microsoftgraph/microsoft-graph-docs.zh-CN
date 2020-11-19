---
title: createDownloadUrl 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e9ab5b0e1d780a64f533026d492ffa9ce0e0e02
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286176"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="8651e-103">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="8651e-103">createDownloadUrl action</span></span>

<span data-ttu-id="8651e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8651e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8651e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8651e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8651e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8651e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8651e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8651e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8651e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8651e-108">Prerequisites</span></span>
<span data-ttu-id="8651e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8651e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8651e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8651e-111">Permission type</span></span>|<span data-ttu-id="8651e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8651e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8651e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8651e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8651e-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8651e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8651e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8651e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8651e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8651e-116">Not supported.</span></span>|
|<span data-ttu-id="8651e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8651e-117">Application</span></span>|<span data-ttu-id="8651e-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8651e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8651e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8651e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="8651e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8651e-120">Request headers</span></span>
|<span data-ttu-id="8651e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8651e-121">Header</span></span>|<span data-ttu-id="8651e-122">值</span><span class="sxs-lookup"><span data-stu-id="8651e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8651e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8651e-123">Authorization</span></span>|<span data-ttu-id="8651e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8651e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8651e-125">接受</span><span class="sxs-lookup"><span data-stu-id="8651e-125">Accept</span></span>|<span data-ttu-id="8651e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8651e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8651e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8651e-127">Request body</span></span>
<span data-ttu-id="8651e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8651e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8651e-129">响应</span><span class="sxs-lookup"><span data-stu-id="8651e-129">Response</span></span>
<span data-ttu-id="8651e-130">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) 。</span><span class="sxs-lookup"><span data-stu-id="8651e-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8651e-131">示例</span><span class="sxs-lookup"><span data-stu-id="8651e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8651e-132">请求</span><span class="sxs-lookup"><span data-stu-id="8651e-132">Request</span></span>
<span data-ttu-id="8651e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8651e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="8651e-134">响应</span><span class="sxs-lookup"><span data-stu-id="8651e-134">Response</span></span>
<span data-ttu-id="8651e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8651e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
    "downloadUrl": "https://example.com/downloadUrl/",
    "decryptionKey": "Decryption Key value",
    "appLogDecryptionAlgorithm": "aes256"
  }
}
```




