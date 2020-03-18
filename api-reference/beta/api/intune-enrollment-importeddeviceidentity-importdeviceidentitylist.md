---
title: importDeviceIdentityList 操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9a7128b4d49137cf722b5556c64049049c8d190
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805212"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="8df14-103">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="8df14-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="8df14-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8df14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8df14-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8df14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df14-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8df14-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df14-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8df14-107">Prerequisites</span></span>
<span data-ttu-id="8df14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8df14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8df14-110">Permission type</span></span>|<span data-ttu-id="8df14-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8df14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8df14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8df14-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df14-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8df14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8df14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8df14-115">Not supported.</span></span>|
|<span data-ttu-id="8df14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8df14-116">Application</span></span>|<span data-ttu-id="8df14-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df14-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8df14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="8df14-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8df14-119">Request headers</span></span>
|<span data-ttu-id="8df14-120">标头</span><span class="sxs-lookup"><span data-stu-id="8df14-120">Header</span></span>|<span data-ttu-id="8df14-121">值</span><span class="sxs-lookup"><span data-stu-id="8df14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df14-122">Authorization</span></span>|<span data-ttu-id="8df14-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8df14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df14-124">接受</span><span class="sxs-lookup"><span data-stu-id="8df14-124">Accept</span></span>|<span data-ttu-id="8df14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8df14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df14-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8df14-126">Request body</span></span>
<span data-ttu-id="8df14-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8df14-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8df14-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8df14-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8df14-129">属性</span><span class="sxs-lookup"><span data-stu-id="8df14-129">Property</span></span>|<span data-ttu-id="8df14-130">类型</span><span class="sxs-lookup"><span data-stu-id="8df14-130">Type</span></span>|<span data-ttu-id="8df14-131">说明</span><span class="sxs-lookup"><span data-stu-id="8df14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df14-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8df14-132">importedDeviceIdentities</span></span>|<span data-ttu-id="8df14-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8df14-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="8df14-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8df14-134">Not yet documented</span></span>|
|<span data-ttu-id="8df14-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8df14-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="8df14-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="8df14-136">Boolean</span></span>|<span data-ttu-id="8df14-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8df14-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8df14-138">响应</span><span class="sxs-lookup"><span data-stu-id="8df14-138">Response</span></span>
<span data-ttu-id="8df14-139">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="8df14-139">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df14-140">示例</span><span class="sxs-lookup"><span data-stu-id="8df14-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df14-141">请求</span><span class="sxs-lookup"><span data-stu-id="8df14-141">Request</span></span>
<span data-ttu-id="8df14-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8df14-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

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
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="8df14-143">响应</span><span class="sxs-lookup"><span data-stu-id="8df14-143">Response</span></span>
<span data-ttu-id="8df14-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8df14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




