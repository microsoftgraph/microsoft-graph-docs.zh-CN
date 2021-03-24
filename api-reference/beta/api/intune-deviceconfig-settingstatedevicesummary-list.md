---
title: 列出 settingStateDeviceSummaries
description: 列出 settingStateDeviceSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 470da5c14bd2648cb9d94bac2a1daed4984d0939
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127877"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="c4ecf-103">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="c4ecf-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="c4ecf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ecf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4ecf-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ecf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ecf-107">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ecf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4ecf-108">Prerequisites</span></span>
<span data-ttu-id="c4ecf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ecf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4ecf-111">Permission type</span></span>|<span data-ttu-id="c4ecf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4ecf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ecf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4ecf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ecf-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ecf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4ecf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4ecf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ecf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-116">Not supported.</span></span>|
|<span data-ttu-id="c4ecf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4ecf-117">Application</span></span>|<span data-ttu-id="c4ecf-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ecf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ecf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4ecf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c4ecf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4ecf-120">Request headers</span></span>
|<span data-ttu-id="c4ecf-121">标头</span><span class="sxs-lookup"><span data-stu-id="c4ecf-121">Header</span></span>|<span data-ttu-id="c4ecf-122">值</span><span class="sxs-lookup"><span data-stu-id="c4ecf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ecf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4ecf-123">Authorization</span></span>|<span data-ttu-id="c4ecf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ecf-125">接受</span><span class="sxs-lookup"><span data-stu-id="c4ecf-125">Accept</span></span>|<span data-ttu-id="c4ecf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ecf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ecf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4ecf-127">Request body</span></span>
<span data-ttu-id="c4ecf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ecf-129">响应</span><span class="sxs-lookup"><span data-stu-id="c4ecf-129">Response</span></span>
<span data-ttu-id="c4ecf-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ecf-131">示例</span><span class="sxs-lookup"><span data-stu-id="c4ecf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ecf-132">请求</span><span class="sxs-lookup"><span data-stu-id="c4ecf-132">Request</span></span>
<span data-ttu-id="c4ecf-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="c4ecf-134">响应</span><span class="sxs-lookup"><span data-stu-id="c4ecf-134">Response</span></span>
<span data-ttu-id="c4ecf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4ecf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```




