---
title: 列出 deviceManagementScripts
description: 列出 deviceManagementScript 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1293b467b955aee9ca78fd17a34304e89579047
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199744"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="e19de-103">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="e19de-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="e19de-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e19de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e19de-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e19de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e19de-106">列出[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e19de-106">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e19de-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e19de-107">Prerequisites</span></span>
<span data-ttu-id="e19de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e19de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e19de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e19de-110">Permission type</span></span>|<span data-ttu-id="e19de-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e19de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e19de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e19de-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e19de-113">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="e19de-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e19de-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e19de-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="e19de-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="e19de-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e19de-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e19de-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e19de-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e19de-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e19de-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e19de-118">Not supported.</span></span>|
|<span data-ttu-id="e19de-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e19de-119">Application</span></span>||
| <span data-ttu-id="e19de-120">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="e19de-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e19de-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e19de-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="e19de-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="e19de-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e19de-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e19de-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e19de-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e19de-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="e19de-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e19de-125">Request headers</span></span>
|<span data-ttu-id="e19de-126">标头</span><span class="sxs-lookup"><span data-stu-id="e19de-126">Header</span></span>|<span data-ttu-id="e19de-127">值</span><span class="sxs-lookup"><span data-stu-id="e19de-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e19de-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e19de-128">Authorization</span></span>|<span data-ttu-id="e19de-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e19de-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e19de-130">接受</span><span class="sxs-lookup"><span data-stu-id="e19de-130">Accept</span></span>|<span data-ttu-id="e19de-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e19de-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e19de-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e19de-132">Request body</span></span>
<span data-ttu-id="e19de-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e19de-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e19de-134">响应</span><span class="sxs-lookup"><span data-stu-id="e19de-134">Response</span></span>
<span data-ttu-id="e19de-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e19de-135">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e19de-136">示例</span><span class="sxs-lookup"><span data-stu-id="e19de-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="e19de-137">请求</span><span class="sxs-lookup"><span data-stu-id="e19de-137">Request</span></span>
<span data-ttu-id="e19de-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e19de-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="e19de-139">响应</span><span class="sxs-lookup"><span data-stu-id="e19de-139">Response</span></span>
<span data-ttu-id="e19de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e19de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "runAs32Bit": true
    }
  ]
}
```




