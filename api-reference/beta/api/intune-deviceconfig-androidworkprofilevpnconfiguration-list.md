---
title: 列出 androidWorkProfileVpnConfigurations
description: 列出 androidWorkProfileVpnConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c5f1950e1d42683b3e8d305c8c5386225f7dcecf
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123202"
---
# <a name="list-androidworkprofilevpnconfigurations"></a><span data-ttu-id="87ba1-103">列出 androidWorkProfileVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="87ba1-103">List androidWorkProfileVpnConfigurations</span></span>

<span data-ttu-id="87ba1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87ba1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87ba1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87ba1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87ba1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87ba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ba1-107">列出[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87ba1-107">List properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87ba1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87ba1-108">Prerequisites</span></span>
<span data-ttu-id="87ba1-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="87ba1-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="87ba1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ba1-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ba1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87ba1-111">Permission type</span></span>|<span data-ttu-id="87ba1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="87ba1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ba1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87ba1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87ba1-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87ba1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87ba1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87ba1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87ba1-116">Not supported.</span></span>|
|<span data-ttu-id="87ba1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87ba1-117">Application</span></span>|<span data-ttu-id="87ba1-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87ba1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ba1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87ba1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87ba1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87ba1-120">Request headers</span></span>
|<span data-ttu-id="87ba1-121">标头</span><span class="sxs-lookup"><span data-stu-id="87ba1-121">Header</span></span>|<span data-ttu-id="87ba1-122">值</span><span class="sxs-lookup"><span data-stu-id="87ba1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87ba1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87ba1-123">Authorization</span></span>|<span data-ttu-id="87ba1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87ba1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87ba1-125">接受</span><span class="sxs-lookup"><span data-stu-id="87ba1-125">Accept</span></span>|<span data-ttu-id="87ba1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87ba1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ba1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87ba1-127">Request body</span></span>
<span data-ttu-id="87ba1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87ba1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ba1-129">响应</span><span class="sxs-lookup"><span data-stu-id="87ba1-129">Response</span></span>
<span data-ttu-id="87ba1-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="87ba1-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ba1-131">示例</span><span class="sxs-lookup"><span data-stu-id="87ba1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87ba1-132">请求</span><span class="sxs-lookup"><span data-stu-id="87ba1-132">Request</span></span>
<span data-ttu-id="87ba1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87ba1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="87ba1-134">响应</span><span class="sxs-lookup"><span data-stu-id="87ba1-134">Response</span></span>
<span data-ttu-id="87ba1-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="87ba1-135">Here is an example of the response.</span></span> <span data-ttu-id="87ba1-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="87ba1-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87ba1-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="87ba1-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2592

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
      "id": "32910378-0378-3291-7803-913278039132",
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
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
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
      "fingerprint": "Fingerprint value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "authenticationMethod": "usernameAndPassword",
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
  ]
}
```



