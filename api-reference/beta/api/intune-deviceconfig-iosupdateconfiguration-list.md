---
title: 列出 iosUpdateConfigurations
description: 列出 iosUpdateConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 661ec6fd627516a91fd0586d3c63dcd40b5d1fd6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339027"
---
# <a name="list-iosupdateconfigurations"></a><span data-ttu-id="70853-103">列出 iosUpdateConfigurations</span><span class="sxs-lookup"><span data-stu-id="70853-103">List iosUpdateConfigurations</span></span>

> <span data-ttu-id="70853-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70853-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70853-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70853-106">列出 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="70853-106">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70853-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="70853-107">Prerequisites</span></span>
<span data-ttu-id="70853-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70853-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70853-110">Permission type</span></span>|<span data-ttu-id="70853-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70853-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70853-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70853-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70853-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70853-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70853-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70853-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70853-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70853-115">Not supported.</span></span>|
|<span data-ttu-id="70853-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="70853-116">Application</span></span>|<span data-ttu-id="70853-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70853-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70853-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70853-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70853-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70853-119">Request headers</span></span>
|<span data-ttu-id="70853-120">标头</span><span class="sxs-lookup"><span data-stu-id="70853-120">Header</span></span>|<span data-ttu-id="70853-121">值</span><span class="sxs-lookup"><span data-stu-id="70853-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70853-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70853-122">Authorization</span></span>|<span data-ttu-id="70853-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70853-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70853-124">接受</span><span class="sxs-lookup"><span data-stu-id="70853-124">Accept</span></span>|<span data-ttu-id="70853-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70853-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70853-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70853-126">Request body</span></span>
<span data-ttu-id="70853-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70853-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70853-128">响应</span><span class="sxs-lookup"><span data-stu-id="70853-128">Response</span></span>
<span data-ttu-id="70853-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="70853-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70853-130">示例</span><span class="sxs-lookup"><span data-stu-id="70853-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="70853-131">请求</span><span class="sxs-lookup"><span data-stu-id="70853-131">Request</span></span>
<span data-ttu-id="70853-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70853-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="70853-133">响应</span><span class="sxs-lookup"><span data-stu-id="70853-133">Response</span></span>
<span data-ttu-id="70853-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70853-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
      "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
      "isEnabled": true,
      "activeHoursStart": "12:00:05.5020000",
      "activeHoursEnd": "11:59:00.8990000",
      "scheduledInstallDays": [
        "monday"
      ],
      "utcTimeOffsetInMinutes": 6,
      "enforcedSoftwareUpdateDelayInDays": 1
    }
  ]
}
```






