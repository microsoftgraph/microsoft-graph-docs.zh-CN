---
title: 列出 settingStateDeviceSummaries
description: 列出 settingStateDeviceSummary 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32d08368b7ea55df94e9fa567a2227f036d0baba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407688"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="08249-103">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="08249-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="08249-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="08249-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08249-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08249-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08249-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08249-107">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="08249-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08249-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08249-108">Prerequisites</span></span>
<span data-ttu-id="08249-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="08249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08249-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08249-111">Permission type</span></span>|<span data-ttu-id="08249-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08249-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08249-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08249-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08249-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08249-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="08249-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08249-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08249-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08249-116">Not supported.</span></span>|
|<span data-ttu-id="08249-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08249-117">Application</span></span>|<span data-ttu-id="08249-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="08249-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08249-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08249-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="08249-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08249-120">Request headers</span></span>
|<span data-ttu-id="08249-121">标头</span><span class="sxs-lookup"><span data-stu-id="08249-121">Header</span></span>|<span data-ttu-id="08249-122">值</span><span class="sxs-lookup"><span data-stu-id="08249-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08249-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08249-123">Authorization</span></span>|<span data-ttu-id="08249-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08249-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08249-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08249-125">Accept</span></span>|<span data-ttu-id="08249-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08249-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08249-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08249-127">Request body</span></span>
<span data-ttu-id="08249-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08249-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08249-129">响应</span><span class="sxs-lookup"><span data-stu-id="08249-129">Response</span></span>
<span data-ttu-id="08249-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="08249-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08249-131">示例</span><span class="sxs-lookup"><span data-stu-id="08249-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="08249-132">请求</span><span class="sxs-lookup"><span data-stu-id="08249-132">Request</span></span>
<span data-ttu-id="08249-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08249-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="08249-134">响应</span><span class="sxs-lookup"><span data-stu-id="08249-134">Response</span></span>
<span data-ttu-id="08249-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08249-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




