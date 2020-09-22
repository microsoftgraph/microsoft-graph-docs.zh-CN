---
title: 获取 deviceConfigurationUserOverview
description: 读取 deviceConfigurationUserOverview 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa467bc5322132edb3a9a1228fc4d1cbc89dc486
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032360"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="4bed6-103">获取 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4bed6-103">Get deviceConfigurationUserOverview</span></span>

<span data-ttu-id="4bed6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bed6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bed6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bed6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bed6-107">读取 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bed6-107">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bed6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4bed6-108">Prerequisites</span></span>
<span data-ttu-id="4bed6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bed6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bed6-111">Permission type</span></span>|<span data-ttu-id="4bed6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4bed6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bed6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bed6-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bed6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4bed6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bed6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bed6-116">Not supported.</span></span>|
|<span data-ttu-id="4bed6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bed6-117">Application</span></span>|<span data-ttu-id="4bed6-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bed6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bed6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bed6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4bed6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4bed6-120">Optional query parameters</span></span>
<span data-ttu-id="4bed6-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4bed6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bed6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bed6-122">Request headers</span></span>
|<span data-ttu-id="4bed6-123">标头</span><span class="sxs-lookup"><span data-stu-id="4bed6-123">Header</span></span>|<span data-ttu-id="4bed6-124">值</span><span class="sxs-lookup"><span data-stu-id="4bed6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bed6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bed6-125">Authorization</span></span>|<span data-ttu-id="4bed6-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4bed6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bed6-127">接受</span><span class="sxs-lookup"><span data-stu-id="4bed6-127">Accept</span></span>|<span data-ttu-id="4bed6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4bed6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bed6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bed6-129">Request body</span></span>
<span data-ttu-id="4bed6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4bed6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bed6-131">响应</span><span class="sxs-lookup"><span data-stu-id="4bed6-131">Response</span></span>
<span data-ttu-id="4bed6-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bed6-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bed6-133">示例</span><span class="sxs-lookup"><span data-stu-id="4bed6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bed6-134">请求</span><span class="sxs-lookup"><span data-stu-id="4bed6-134">Request</span></span>
<span data-ttu-id="4bed6-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bed6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="4bed6-136">响应</span><span class="sxs-lookup"><span data-stu-id="4bed6-136">Response</span></span>
<span data-ttu-id="4bed6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4bed6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```






