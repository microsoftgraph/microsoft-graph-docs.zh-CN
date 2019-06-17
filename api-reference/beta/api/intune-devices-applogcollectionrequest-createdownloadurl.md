---
title: createDownloadUrl 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41b20d2c6638d7943bb52e487ffb5dba4c8eecce
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959374"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="46c97-103">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="46c97-103">createDownloadUrl action</span></span>

> <span data-ttu-id="46c97-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46c97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46c97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46c97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46c97-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="46c97-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46c97-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="46c97-107">Prerequisites</span></span>
<span data-ttu-id="46c97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46c97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46c97-110">Permission type</span></span>|<span data-ttu-id="46c97-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46c97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46c97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46c97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46c97-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c97-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="46c97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46c97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46c97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c97-115">Not supported.</span></span>|
|<span data-ttu-id="46c97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46c97-116">Application</span></span>|<span data-ttu-id="46c97-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46c97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46c97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="46c97-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46c97-119">Request headers</span></span>
|<span data-ttu-id="46c97-120">标头</span><span class="sxs-lookup"><span data-stu-id="46c97-120">Header</span></span>|<span data-ttu-id="46c97-121">值</span><span class="sxs-lookup"><span data-stu-id="46c97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46c97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46c97-122">Authorization</span></span>|<span data-ttu-id="46c97-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46c97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46c97-124">接受</span><span class="sxs-lookup"><span data-stu-id="46c97-124">Accept</span></span>|<span data-ttu-id="46c97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46c97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46c97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="46c97-126">Request body</span></span>
<span data-ttu-id="46c97-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46c97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46c97-128">响应</span><span class="sxs-lookup"><span data-stu-id="46c97-128">Response</span></span>
<span data-ttu-id="46c97-129">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) 。</span><span class="sxs-lookup"><span data-stu-id="46c97-129">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c97-130">示例</span><span class="sxs-lookup"><span data-stu-id="46c97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46c97-131">请求</span><span class="sxs-lookup"><span data-stu-id="46c97-131">Request</span></span>
<span data-ttu-id="46c97-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46c97-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="46c97-133">响应</span><span class="sxs-lookup"><span data-stu-id="46c97-133">Response</span></span>
<span data-ttu-id="46c97-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46c97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





