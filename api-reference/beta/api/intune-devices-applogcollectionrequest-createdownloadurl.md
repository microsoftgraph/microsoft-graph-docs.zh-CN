---
title: createDownloadUrl 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce6d9d6c4ccd7ac9eaa1f1bc2672b4dc1717ef19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470005"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="34395-103">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="34395-103">createDownloadUrl action</span></span>

<span data-ttu-id="34395-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="34395-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34395-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34395-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34395-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34395-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34395-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34395-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34395-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="34395-108">Prerequisites</span></span>
<span data-ttu-id="34395-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34395-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="34395-111">Permission type</span></span>|<span data-ttu-id="34395-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34395-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34395-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34395-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34395-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34395-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="34395-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34395-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34395-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34395-116">Not supported.</span></span>|
|<span data-ttu-id="34395-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="34395-117">Application</span></span>|<span data-ttu-id="34395-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34395-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34395-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34395-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="34395-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="34395-120">Request headers</span></span>
|<span data-ttu-id="34395-121">标头</span><span class="sxs-lookup"><span data-stu-id="34395-121">Header</span></span>|<span data-ttu-id="34395-122">值</span><span class="sxs-lookup"><span data-stu-id="34395-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34395-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34395-123">Authorization</span></span>|<span data-ttu-id="34395-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34395-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34395-125">接受</span><span class="sxs-lookup"><span data-stu-id="34395-125">Accept</span></span>|<span data-ttu-id="34395-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34395-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34395-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34395-127">Request body</span></span>
<span data-ttu-id="34395-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34395-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34395-129">响应</span><span class="sxs-lookup"><span data-stu-id="34395-129">Response</span></span>
<span data-ttu-id="34395-130">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) 。</span><span class="sxs-lookup"><span data-stu-id="34395-130">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34395-131">示例</span><span class="sxs-lookup"><span data-stu-id="34395-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="34395-132">请求</span><span class="sxs-lookup"><span data-stu-id="34395-132">Request</span></span>
<span data-ttu-id="34395-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34395-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="34395-134">响应</span><span class="sxs-lookup"><span data-stu-id="34395-134">Response</span></span>
<span data-ttu-id="34395-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34395-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





