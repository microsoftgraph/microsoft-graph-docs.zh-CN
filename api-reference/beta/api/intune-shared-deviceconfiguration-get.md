---
title: 获取 deviceConfiguration
description: 读取 deviceConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d218722f01726d0a11c13154b2ae8aca36b164fc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866404"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="a05e6-103">获取 deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a05e6-103">Get deviceConfiguration</span></span>

<span data-ttu-id="a05e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a05e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a05e6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a05e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a05e6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a05e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a05e6-107">读取 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a05e6-107">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a05e6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a05e6-108">Prerequisites</span></span>
<span data-ttu-id="a05e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a05e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a05e6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a05e6-111">Permission type</span></span>|<span data-ttu-id="a05e6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a05e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a05e6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a05e6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a05e6-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="a05e6-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a05e6-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05e6-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a05e6-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="a05e6-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a05e6-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05e6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a05e6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a05e6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a05e6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a05e6-119">Not supported.</span></span>|
|<span data-ttu-id="a05e6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="a05e6-120">Application</span></span>||
| <span data-ttu-id="a05e6-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="a05e6-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a05e6-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05e6-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a05e6-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="a05e6-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a05e6-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a05e6-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a05e6-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a05e6-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a05e6-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a05e6-126">Optional query parameters</span></span>
<span data-ttu-id="a05e6-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a05e6-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a05e6-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="a05e6-128">Request headers</span></span>
|<span data-ttu-id="a05e6-129">标头</span><span class="sxs-lookup"><span data-stu-id="a05e6-129">Header</span></span>|<span data-ttu-id="a05e6-130">值</span><span class="sxs-lookup"><span data-stu-id="a05e6-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a05e6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a05e6-131">Authorization</span></span>|<span data-ttu-id="a05e6-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a05e6-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a05e6-133">接受</span><span class="sxs-lookup"><span data-stu-id="a05e6-133">Accept</span></span>|<span data-ttu-id="a05e6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="a05e6-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a05e6-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="a05e6-135">Request body</span></span>
<span data-ttu-id="a05e6-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a05e6-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a05e6-137">响应</span><span class="sxs-lookup"><span data-stu-id="a05e6-137">Response</span></span>
<span data-ttu-id="a05e6-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a05e6-138">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a05e6-139">示例</span><span class="sxs-lookup"><span data-stu-id="a05e6-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a05e6-140">请求</span><span class="sxs-lookup"><span data-stu-id="a05e6-140">Request</span></span>
<span data-ttu-id="a05e6-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a05e6-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a05e6-142">响应</span><span class="sxs-lookup"><span data-stu-id="a05e6-142">Response</span></span>
<span data-ttu-id="a05e6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a05e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```







