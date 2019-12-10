---
title: searchExistingIdentities 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 100c5ca348fc0031da048d5eba04d9e6889ad79f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943843"
---
# <a name="searchexistingidentities-action"></a><span data-ttu-id="75c15-103">searchExistingIdentities 操作</span><span class="sxs-lookup"><span data-stu-id="75c15-103">searchExistingIdentities action</span></span>

> <span data-ttu-id="75c15-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75c15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c15-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75c15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c15-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="75c15-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75c15-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="75c15-107">Prerequisites</span></span>
<span data-ttu-id="75c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c15-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75c15-110">Permission type</span></span>|<span data-ttu-id="75c15-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75c15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75c15-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75c15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75c15-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="75c15-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="75c15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75c15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75c15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75c15-115">Not supported.</span></span>|
|<span data-ttu-id="75c15-116">Application</span><span class="sxs-lookup"><span data-stu-id="75c15-116">Application</span></span>|<span data-ttu-id="75c15-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="75c15-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75c15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75c15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
```

## <a name="request-headers"></a><span data-ttu-id="75c15-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75c15-119">Request headers</span></span>
|<span data-ttu-id="75c15-120">标头</span><span class="sxs-lookup"><span data-stu-id="75c15-120">Header</span></span>|<span data-ttu-id="75c15-121">值</span><span class="sxs-lookup"><span data-stu-id="75c15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75c15-122">授权</span><span class="sxs-lookup"><span data-stu-id="75c15-122">Authorization</span></span>|<span data-ttu-id="75c15-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="75c15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75c15-124">接受</span><span class="sxs-lookup"><span data-stu-id="75c15-124">Accept</span></span>|<span data-ttu-id="75c15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75c15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75c15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="75c15-126">Request body</span></span>
<span data-ttu-id="75c15-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75c15-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="75c15-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="75c15-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="75c15-129">属性</span><span class="sxs-lookup"><span data-stu-id="75c15-129">Property</span></span>|<span data-ttu-id="75c15-130">类型</span><span class="sxs-lookup"><span data-stu-id="75c15-130">Type</span></span>|<span data-ttu-id="75c15-131">说明</span><span class="sxs-lookup"><span data-stu-id="75c15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c15-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="75c15-132">importedDeviceIdentities</span></span>|<span data-ttu-id="75c15-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="75c15-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="75c15-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="75c15-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="75c15-135">响应</span><span class="sxs-lookup"><span data-stu-id="75c15-135">Response</span></span>
<span data-ttu-id="75c15-136">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合。</span><span class="sxs-lookup"><span data-stu-id="75c15-136">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75c15-137">示例</span><span class="sxs-lookup"><span data-stu-id="75c15-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="75c15-138">请求</span><span class="sxs-lookup"><span data-stu-id="75c15-138">Request</span></span>
<span data-ttu-id="75c15-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75c15-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/searchExistingIdentities

Content-type: application/json
Content-length: 596

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="75c15-140">响应</span><span class="sxs-lookup"><span data-stu-id="75c15-140">Response</span></span>
<span data-ttu-id="75c15-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75c15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```





