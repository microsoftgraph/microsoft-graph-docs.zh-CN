---
title: 列出 windowsUpdateStates
description: 列出 windowsUpdateState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a45cb9a7c38b9be5095d083f7af9910cff923a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966952"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="8603c-103">列出 windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="8603c-103">List windowsUpdateStates</span></span>

<span data-ttu-id="8603c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8603c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8603c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8603c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8603c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8603c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8603c-107">列出 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8603c-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8603c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8603c-108">Prerequisites</span></span>
<span data-ttu-id="8603c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8603c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8603c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8603c-111">Permission type</span></span>|<span data-ttu-id="8603c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8603c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8603c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8603c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8603c-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8603c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8603c-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8603c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="8603c-116">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="8603c-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8603c-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8603c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8603c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8603c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8603c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8603c-119">Not supported.</span></span>|
|<span data-ttu-id="8603c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8603c-120">Application</span></span>||
| <span data-ttu-id="8603c-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8603c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8603c-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8603c-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="8603c-123">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="8603c-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8603c-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8603c-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8603c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8603c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="8603c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8603c-126">Request headers</span></span>
|<span data-ttu-id="8603c-127">标头</span><span class="sxs-lookup"><span data-stu-id="8603c-127">Header</span></span>|<span data-ttu-id="8603c-128">值</span><span class="sxs-lookup"><span data-stu-id="8603c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8603c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8603c-129">Authorization</span></span>|<span data-ttu-id="8603c-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8603c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8603c-131">接受</span><span class="sxs-lookup"><span data-stu-id="8603c-131">Accept</span></span>|<span data-ttu-id="8603c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8603c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8603c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="8603c-133">Request body</span></span>
<span data-ttu-id="8603c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8603c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8603c-135">响应</span><span class="sxs-lookup"><span data-stu-id="8603c-135">Response</span></span>
<span data-ttu-id="8603c-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8603c-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8603c-137">示例</span><span class="sxs-lookup"><span data-stu-id="8603c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8603c-138">请求</span><span class="sxs-lookup"><span data-stu-id="8603c-138">Request</span></span>
<span data-ttu-id="8603c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8603c-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="8603c-140">响应</span><span class="sxs-lookup"><span data-stu-id="8603c-140">Response</span></span>
<span data-ttu-id="8603c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8603c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateState",
      "id": "3d92af00-af00-3d92-00af-923d00af923d",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "status": "pendingInstallation",
      "qualityUpdateVersion": "Quality Update Version value",
      "featureUpdateVersion": "Feature Update Version value",
      "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```









