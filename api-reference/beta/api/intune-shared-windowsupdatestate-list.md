---
title: 列出 windowsUpdateStates
description: 列出 windowsUpdateState 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d9837763b952e9f2d980a61a4165a3232b1d5ab
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864716"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="5577a-103">列出 windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="5577a-103">List windowsUpdateStates</span></span>

<span data-ttu-id="5577a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5577a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5577a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5577a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5577a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5577a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5577a-107">列出 [windowsUpdateState 对象的属性和](../resources/intune-shared-windowsupdatestate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="5577a-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5577a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5577a-108">Prerequisites</span></span>
<span data-ttu-id="5577a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5577a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5577a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5577a-111">Permission type</span></span>|<span data-ttu-id="5577a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5577a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5577a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5577a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5577a-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="5577a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5577a-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5577a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5577a-116">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="5577a-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="5577a-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5577a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5577a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5577a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5577a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5577a-119">Not supported.</span></span>|
|<span data-ttu-id="5577a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5577a-120">Application</span></span>||
| <span data-ttu-id="5577a-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="5577a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5577a-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5577a-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5577a-123">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="5577a-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="5577a-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5577a-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5577a-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5577a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="5577a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="5577a-126">Request headers</span></span>
|<span data-ttu-id="5577a-127">标头</span><span class="sxs-lookup"><span data-stu-id="5577a-127">Header</span></span>|<span data-ttu-id="5577a-128">值</span><span class="sxs-lookup"><span data-stu-id="5577a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5577a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="5577a-129">Authorization</span></span>|<span data-ttu-id="5577a-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5577a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5577a-131">接受</span><span class="sxs-lookup"><span data-stu-id="5577a-131">Accept</span></span>|<span data-ttu-id="5577a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5577a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5577a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5577a-133">Request body</span></span>
<span data-ttu-id="5577a-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5577a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5577a-135">响应</span><span class="sxs-lookup"><span data-stu-id="5577a-135">Response</span></span>
<span data-ttu-id="5577a-136">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5577a-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5577a-137">示例</span><span class="sxs-lookup"><span data-stu-id="5577a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5577a-138">请求</span><span class="sxs-lookup"><span data-stu-id="5577a-138">Request</span></span>
<span data-ttu-id="5577a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5577a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="5577a-140">响应</span><span class="sxs-lookup"><span data-stu-id="5577a-140">Response</span></span>
<span data-ttu-id="5577a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5577a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







