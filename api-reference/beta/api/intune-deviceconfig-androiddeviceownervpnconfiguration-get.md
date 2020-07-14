---
title: 获取 androidDeviceOwnerVpnConfiguration
description: 读取 androidDeviceOwnerVpnConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fa7af555496e50d236b733cd507590da5626ced
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123328"
---
# <a name="get-androiddeviceownervpnconfiguration"></a><span data-ttu-id="21547-103">获取 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="21547-103">Get androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="21547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21547-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21547-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21547-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21547-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21547-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21547-107">读取[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21547-107">Read properties and relationships of the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21547-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="21547-108">Prerequisites</span></span>
<span data-ttu-id="21547-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="21547-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="21547-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21547-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21547-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21547-111">Permission type</span></span>|<span data-ttu-id="21547-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21547-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21547-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21547-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21547-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21547-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21547-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21547-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21547-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21547-116">Not supported.</span></span>|
|<span data-ttu-id="21547-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="21547-117">Application</span></span>|<span data-ttu-id="21547-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21547-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21547-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21547-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21547-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="21547-120">Optional query parameters</span></span>
<span data-ttu-id="21547-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="21547-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21547-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="21547-122">Request headers</span></span>
|<span data-ttu-id="21547-123">标头</span><span class="sxs-lookup"><span data-stu-id="21547-123">Header</span></span>|<span data-ttu-id="21547-124">值</span><span class="sxs-lookup"><span data-stu-id="21547-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21547-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="21547-125">Authorization</span></span>|<span data-ttu-id="21547-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21547-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21547-127">接受</span><span class="sxs-lookup"><span data-stu-id="21547-127">Accept</span></span>|<span data-ttu-id="21547-128">application/json</span><span class="sxs-lookup"><span data-stu-id="21547-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21547-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="21547-129">Request body</span></span>
<span data-ttu-id="21547-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21547-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21547-131">响应</span><span class="sxs-lookup"><span data-stu-id="21547-131">Response</span></span>
<span data-ttu-id="21547-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="21547-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21547-133">示例</span><span class="sxs-lookup"><span data-stu-id="21547-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="21547-134">请求</span><span class="sxs-lookup"><span data-stu-id="21547-134">Request</span></span>
<span data-ttu-id="21547-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21547-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="21547-136">响应</span><span class="sxs-lookup"><span data-stu-id="21547-136">Response</span></span>
<span data-ttu-id="21547-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="21547-137">Here is an example of the response.</span></span> <span data-ttu-id="21547-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="21547-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21547-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="21547-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2061

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
    "id": "972962e3-62e3-9729-e362-2997e3622997",
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
    "version": 7,
    "authenticationMethod": "usernameAndPassword",
    "connectionName": "Connection Name value",
    "role": "Role value",
    "realm": "Realm value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "connectionType": "pulseSecure",
    "proxyServer": {
      "@odata.type": "microsoft.graph.vpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4
    },
    "targetedPackageIds": [
      "Targeted Package Ids value"
    ],
    "alwaysOn": true,
    "alwaysOnLockdown": true
  }
}
```



