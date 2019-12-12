---
title: 获取 androidDeviceOwnerCompliancePolicy
description: 读取 androidDeviceOwnerCompliancePolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e1d516bc382d29a1602077807543f7f30f433f4
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953913"
---
# <a name="get-androiddeviceownercompliancepolicy"></a><span data-ttu-id="bab86-103">获取 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bab86-103">Get androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="bab86-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bab86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bab86-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bab86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bab86-106">读取[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bab86-106">Read properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bab86-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bab86-107">Prerequisites</span></span>
<span data-ttu-id="bab86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bab86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab86-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bab86-110">Permission type</span></span>|<span data-ttu-id="bab86-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bab86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bab86-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bab86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bab86-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab86-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bab86-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bab86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bab86-115">Not supported.</span></span>|
|<span data-ttu-id="bab86-116">Application</span><span class="sxs-lookup"><span data-stu-id="bab86-116">Application</span></span>|<span data-ttu-id="bab86-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab86-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bab86-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bab86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab86-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bab86-119">Optional query parameters</span></span>
<span data-ttu-id="bab86-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bab86-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab86-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bab86-121">Request headers</span></span>
|<span data-ttu-id="bab86-122">标头</span><span class="sxs-lookup"><span data-stu-id="bab86-122">Header</span></span>|<span data-ttu-id="bab86-123">值</span><span class="sxs-lookup"><span data-stu-id="bab86-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bab86-124">授权</span><span class="sxs-lookup"><span data-stu-id="bab86-124">Authorization</span></span>|<span data-ttu-id="bab86-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bab86-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bab86-126">接受</span><span class="sxs-lookup"><span data-stu-id="bab86-126">Accept</span></span>|<span data-ttu-id="bab86-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bab86-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab86-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bab86-128">Request body</span></span>
<span data-ttu-id="bab86-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bab86-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab86-130">响应</span><span class="sxs-lookup"><span data-stu-id="bab86-130">Response</span></span>
<span data-ttu-id="bab86-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bab86-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bab86-132">示例</span><span class="sxs-lookup"><span data-stu-id="bab86-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bab86-133">请求</span><span class="sxs-lookup"><span data-stu-id="bab86-133">Request</span></span>
<span data-ttu-id="bab86-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bab86-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="bab86-135">响应</span><span class="sxs-lookup"><span data-stu-id="bab86-135">Response</span></span>
<span data-ttu-id="bab86-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bab86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "be2464b4-64b4-be24-b464-24beb46424be",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "advancedThreatProtectionRequiredSecurityLevel": "secured",
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordMinimumLetterCharacters": 15,
    "passwordMinimumLowerCaseCharacters": 2,
    "passwordMinimumNonLetterCharacters": 2,
    "passwordMinimumNumericCharacters": 0,
    "passwordMinimumSymbolCharacters": 15,
    "passwordMinimumUpperCaseCharacters": 2,
    "passwordRequiredType": "required",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordCountToBlock": 4,
    "storageRequireEncryption": true
  }
}
```





