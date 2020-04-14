---
title: 列出 macOSCompliancePolicies
description: 列出 macOSCompliancePolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c080bdcb04b2468e656dfce3c97a1f46f560e34d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438315"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="bb140-103">列出 macOSCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="bb140-103">List macOSCompliancePolicies</span></span>

<span data-ttu-id="bb140-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb140-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb140-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb140-107">列出 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb140-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb140-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb140-108">Prerequisites</span></span>
<span data-ttu-id="bb140-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb140-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb140-111">Permission type</span></span>|<span data-ttu-id="bb140-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb140-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb140-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb140-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bb140-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb140-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb140-116">Not supported.</span></span>|
|<span data-ttu-id="bb140-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb140-117">Application</span></span>|<span data-ttu-id="bb140-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb140-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb140-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bb140-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb140-120">Request headers</span></span>
|<span data-ttu-id="bb140-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb140-121">Header</span></span>|<span data-ttu-id="bb140-122">值</span><span class="sxs-lookup"><span data-stu-id="bb140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb140-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb140-123">Authorization</span></span>|<span data-ttu-id="bb140-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb140-125">接受</span><span class="sxs-lookup"><span data-stu-id="bb140-125">Accept</span></span>|<span data-ttu-id="bb140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb140-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb140-127">Request body</span></span>
<span data-ttu-id="bb140-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb140-129">响应</span><span class="sxs-lookup"><span data-stu-id="bb140-129">Response</span></span>
<span data-ttu-id="bb140-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb140-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb140-131">示例</span><span class="sxs-lookup"><span data-stu-id="bb140-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb140-132">请求</span><span class="sxs-lookup"><span data-stu-id="bb140-132">Request</span></span>
<span data-ttu-id="bb140-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb140-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="bb140-134">响应</span><span class="sxs-lookup"><span data-stu-id="bb140-134">Response</span></span>
<span data-ttu-id="bb140-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "gatekeeperAllowedAppSource": "macAppStore",
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```



