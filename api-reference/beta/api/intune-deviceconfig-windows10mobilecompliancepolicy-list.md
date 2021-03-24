---
title: 列出 windows10MobileCompliancePolicies
description: 列出 windows10MobileCompliancePolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33b64af6cc6c860aad88676b64c9b5e352a22095
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127681"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="bddc6-103">列出 windows10MobileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="bddc6-103">List windows10MobileCompliancePolicies</span></span>

<span data-ttu-id="bddc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bddc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bddc6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bddc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bddc6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bddc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bddc6-107">列出 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bddc6-107">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bddc6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bddc6-108">Prerequisites</span></span>
<span data-ttu-id="bddc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bddc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bddc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bddc6-111">Permission type</span></span>|<span data-ttu-id="bddc6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bddc6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bddc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bddc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bddc6-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bddc6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bddc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bddc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bddc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bddc6-116">Not supported.</span></span>|
|<span data-ttu-id="bddc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bddc6-117">Application</span></span>|<span data-ttu-id="bddc6-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bddc6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bddc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bddc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bddc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bddc6-120">Request headers</span></span>
|<span data-ttu-id="bddc6-121">标头</span><span class="sxs-lookup"><span data-stu-id="bddc6-121">Header</span></span>|<span data-ttu-id="bddc6-122">值</span><span class="sxs-lookup"><span data-stu-id="bddc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bddc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bddc6-123">Authorization</span></span>|<span data-ttu-id="bddc6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bddc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bddc6-125">接受</span><span class="sxs-lookup"><span data-stu-id="bddc6-125">Accept</span></span>|<span data-ttu-id="bddc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bddc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bddc6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bddc6-127">Request body</span></span>
<span data-ttu-id="bddc6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bddc6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bddc6-129">响应</span><span class="sxs-lookup"><span data-stu-id="bddc6-129">Response</span></span>
<span data-ttu-id="bddc6-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bddc6-130">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bddc6-131">示例</span><span class="sxs-lookup"><span data-stu-id="bddc6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bddc6-132">请求</span><span class="sxs-lookup"><span data-stu-id="bddc6-132">Request</span></span>
<span data-ttu-id="bddc6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bddc6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="bddc6-134">响应</span><span class="sxs-lookup"><span data-stu-id="bddc6-134">Response</span></span>
<span data-ttu-id="bddc6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bddc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ]
    }
  ]
}
```




