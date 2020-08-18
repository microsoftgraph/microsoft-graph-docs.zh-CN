---
title: 获取 windowsProtectionState
description: 读取 windowsProtectionState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adbd2aa6e579157ebf1c3e8dab42f12d287a0bfc
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790579"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="dd3dd-103">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="dd3dd-103">Get windowsProtectionState</span></span>

<span data-ttu-id="dd3dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd3dd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd3dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd3dd-107">读取 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd3dd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd3dd-108">Prerequisites</span></span>
<span data-ttu-id="dd3dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd3dd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd3dd-111">Permission type</span></span>|<span data-ttu-id="dd3dd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd3dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd3dd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd3dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd3dd-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd3dd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="dd3dd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd3dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd3dd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-116">Not supported.</span></span>|
|<span data-ttu-id="dd3dd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd3dd-117">Application</span></span>|<span data-ttu-id="dd3dd-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd3dd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd3dd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd3dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd3dd-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd3dd-120">Optional query parameters</span></span>
<span data-ttu-id="dd3dd-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd3dd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd3dd-122">Request headers</span></span>
|<span data-ttu-id="dd3dd-123">标头</span><span class="sxs-lookup"><span data-stu-id="dd3dd-123">Header</span></span>|<span data-ttu-id="dd3dd-124">值</span><span class="sxs-lookup"><span data-stu-id="dd3dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd3dd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd3dd-125">Authorization</span></span>|<span data-ttu-id="dd3dd-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd3dd-127">接受</span><span class="sxs-lookup"><span data-stu-id="dd3dd-127">Accept</span></span>|<span data-ttu-id="dd3dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dd3dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd3dd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd3dd-129">Request body</span></span>
<span data-ttu-id="dd3dd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd3dd-131">响应</span><span class="sxs-lookup"><span data-stu-id="dd3dd-131">Response</span></span>
<span data-ttu-id="dd3dd-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd3dd-133">示例</span><span class="sxs-lookup"><span data-stu-id="dd3dd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd3dd-134">请求</span><span class="sxs-lookup"><span data-stu-id="dd3dd-134">Request</span></span>
<span data-ttu-id="dd3dd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

### <a name="response"></a><span data-ttu-id="dd3dd-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd3dd-136">Response</span></span>
<span data-ttu-id="dd3dd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd3dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```



