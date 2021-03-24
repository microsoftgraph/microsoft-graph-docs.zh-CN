---
title: 列出 windowsPhoneEASEmailProfileConfigurations
description: 列出 windowsPhoneEASEmailProfileConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7db5eb9a8a2da232696d5105fb58ae68b4186385
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147089"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="571f1-103">列出 windowsPhoneEASEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="571f1-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

<span data-ttu-id="571f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="571f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="571f1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="571f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="571f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="571f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="571f1-107">列出 [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="571f1-107">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="571f1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="571f1-108">Prerequisites</span></span>
<span data-ttu-id="571f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="571f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="571f1-111">Permission type</span></span>|<span data-ttu-id="571f1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="571f1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="571f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="571f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="571f1-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571f1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="571f1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="571f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="571f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="571f1-116">Not supported.</span></span>|
|<span data-ttu-id="571f1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="571f1-117">Application</span></span>|<span data-ttu-id="571f1-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571f1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="571f1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="571f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="571f1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="571f1-120">Request headers</span></span>
|<span data-ttu-id="571f1-121">标头</span><span class="sxs-lookup"><span data-stu-id="571f1-121">Header</span></span>|<span data-ttu-id="571f1-122">值</span><span class="sxs-lookup"><span data-stu-id="571f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="571f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="571f1-123">Authorization</span></span>|<span data-ttu-id="571f1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="571f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="571f1-125">接受</span><span class="sxs-lookup"><span data-stu-id="571f1-125">Accept</span></span>|<span data-ttu-id="571f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="571f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="571f1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="571f1-127">Request body</span></span>
<span data-ttu-id="571f1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="571f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="571f1-129">响应</span><span class="sxs-lookup"><span data-stu-id="571f1-129">Response</span></span>
<span data-ttu-id="571f1-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="571f1-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571f1-131">示例</span><span class="sxs-lookup"><span data-stu-id="571f1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="571f1-132">请求</span><span class="sxs-lookup"><span data-stu-id="571f1-132">Request</span></span>
<span data-ttu-id="571f1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="571f1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="571f1-134">响应</span><span class="sxs-lookup"><span data-stu-id="571f1-134">Response</span></span>
<span data-ttu-id="571f1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="571f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1956

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
      "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value",
      "accountName": "Account Name value",
      "applyOnlyToWindowsPhone81": true,
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSsl": true
    }
  ]
}
```




