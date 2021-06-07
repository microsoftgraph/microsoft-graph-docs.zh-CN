---
title: 列出 deviceConfigurationDeviceStatuses
description: 列出 deviceConfigurationDeviceStatus 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4901514966a86328401529739d15c851fa4bfffa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752698"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="dabaf-103">列出 deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="dabaf-103">List deviceConfigurationDeviceStatuses</span></span>

<span data-ttu-id="dabaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dabaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dabaf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dabaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dabaf-106">列出 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dabaf-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dabaf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dabaf-107">Prerequisites</span></span>
<span data-ttu-id="dabaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dabaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dabaf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dabaf-110">Permission type</span></span>|<span data-ttu-id="dabaf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dabaf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dabaf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dabaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dabaf-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dabaf-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dabaf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dabaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dabaf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dabaf-115">Not supported.</span></span>|
|<span data-ttu-id="dabaf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dabaf-116">Application</span></span>|<span data-ttu-id="dabaf-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dabaf-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dabaf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dabaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="dabaf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dabaf-119">Request headers</span></span>
|<span data-ttu-id="dabaf-120">标头</span><span class="sxs-lookup"><span data-stu-id="dabaf-120">Header</span></span>|<span data-ttu-id="dabaf-121">值</span><span class="sxs-lookup"><span data-stu-id="dabaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dabaf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dabaf-122">Authorization</span></span>|<span data-ttu-id="dabaf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dabaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dabaf-124">接受</span><span class="sxs-lookup"><span data-stu-id="dabaf-124">Accept</span></span>|<span data-ttu-id="dabaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dabaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dabaf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dabaf-126">Request body</span></span>
<span data-ttu-id="dabaf-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dabaf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dabaf-128">响应</span><span class="sxs-lookup"><span data-stu-id="dabaf-128">Response</span></span>
<span data-ttu-id="dabaf-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dabaf-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dabaf-130">示例</span><span class="sxs-lookup"><span data-stu-id="dabaf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dabaf-131">请求</span><span class="sxs-lookup"><span data-stu-id="dabaf-131">Request</span></span>
<span data-ttu-id="dabaf-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dabaf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="dabaf-133">响应</span><span class="sxs-lookup"><span data-stu-id="dabaf-133">Response</span></span>
<span data-ttu-id="dabaf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dabaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




