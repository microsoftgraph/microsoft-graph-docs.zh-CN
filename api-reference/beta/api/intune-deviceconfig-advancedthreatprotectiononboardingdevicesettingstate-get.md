---
title: 获取 advancedThreatProtectionOnboardingDeviceSettingState
description: 读取 advancedThreatProtectionOnboardingDeviceSettingState 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63083ad5dc17460505396cca5fc52632647744b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961425"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="74c62-103">获取 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="74c62-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="74c62-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74c62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74c62-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74c62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74c62-106">读取[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74c62-106">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74c62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="74c62-107">Prerequisites</span></span>
<span data-ttu-id="74c62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74c62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74c62-110">Permission type</span></span>|<span data-ttu-id="74c62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74c62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74c62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74c62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74c62-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74c62-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="74c62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74c62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74c62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74c62-115">Not supported.</span></span>|
|<span data-ttu-id="74c62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="74c62-116">Application</span></span>|<span data-ttu-id="74c62-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="74c62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74c62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74c62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74c62-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74c62-119">Optional query parameters</span></span>
<span data-ttu-id="74c62-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="74c62-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74c62-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="74c62-121">Request headers</span></span>
|<span data-ttu-id="74c62-122">标头</span><span class="sxs-lookup"><span data-stu-id="74c62-122">Header</span></span>|<span data-ttu-id="74c62-123">值</span><span class="sxs-lookup"><span data-stu-id="74c62-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74c62-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="74c62-124">Authorization</span></span>|<span data-ttu-id="74c62-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74c62-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74c62-126">接受</span><span class="sxs-lookup"><span data-stu-id="74c62-126">Accept</span></span>|<span data-ttu-id="74c62-127">application/json</span><span class="sxs-lookup"><span data-stu-id="74c62-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74c62-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="74c62-128">Request body</span></span>
<span data-ttu-id="74c62-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74c62-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c62-130">响应</span><span class="sxs-lookup"><span data-stu-id="74c62-130">Response</span></span>
<span data-ttu-id="74c62-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74c62-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74c62-132">示例</span><span class="sxs-lookup"><span data-stu-id="74c62-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="74c62-133">请求</span><span class="sxs-lookup"><span data-stu-id="74c62-133">Request</span></span>
<span data-ttu-id="74c62-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74c62-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="74c62-135">响应</span><span class="sxs-lookup"><span data-stu-id="74c62-135">Response</span></span>
<span data-ttu-id="74c62-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74c62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
    "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
    "platformType": "windowsRT",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```




