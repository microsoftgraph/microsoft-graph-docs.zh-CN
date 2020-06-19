---
title: 获取 deviceConfigurationDeviceStatus
description: 读取 deviceConfigurationDeviceStatus 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0b1e6033fc6d21d3a24f22cc6a1897abb921b4c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792938"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="41495-103">获取 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="41495-103">Get deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="41495-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41495-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41495-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41495-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41495-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41495-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41495-107">读取 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41495-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41495-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41495-108">Prerequisites</span></span>
<span data-ttu-id="41495-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="41495-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="41495-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41495-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41495-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41495-111">Permission type</span></span>|<span data-ttu-id="41495-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41495-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41495-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41495-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41495-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41495-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41495-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41495-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41495-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41495-116">Not supported.</span></span>|
|<span data-ttu-id="41495-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41495-117">Application</span></span>|<span data-ttu-id="41495-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41495-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41495-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41495-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41495-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41495-120">Optional query parameters</span></span>
<span data-ttu-id="41495-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41495-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41495-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="41495-122">Request headers</span></span>
|<span data-ttu-id="41495-123">标头</span><span class="sxs-lookup"><span data-stu-id="41495-123">Header</span></span>|<span data-ttu-id="41495-124">值</span><span class="sxs-lookup"><span data-stu-id="41495-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41495-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41495-125">Authorization</span></span>|<span data-ttu-id="41495-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41495-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41495-127">接受</span><span class="sxs-lookup"><span data-stu-id="41495-127">Accept</span></span>|<span data-ttu-id="41495-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41495-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41495-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="41495-129">Request body</span></span>
<span data-ttu-id="41495-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41495-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41495-131">响应</span><span class="sxs-lookup"><span data-stu-id="41495-131">Response</span></span>
<span data-ttu-id="41495-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41495-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41495-133">示例</span><span class="sxs-lookup"><span data-stu-id="41495-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="41495-134">请求</span><span class="sxs-lookup"><span data-stu-id="41495-134">Request</span></span>
<span data-ttu-id="41495-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41495-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="41495-136">响应</span><span class="sxs-lookup"><span data-stu-id="41495-136">Response</span></span>
<span data-ttu-id="41495-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="41495-137">Here is an example of the response.</span></span> <span data-ttu-id="41495-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="41495-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="41495-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="41495-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



