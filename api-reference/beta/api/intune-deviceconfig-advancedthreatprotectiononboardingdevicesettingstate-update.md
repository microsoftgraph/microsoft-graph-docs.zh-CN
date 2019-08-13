---
title: 更新 advancedThreatProtectionOnboardingDeviceSettingState
description: 更新 advancedThreatProtectionOnboardingDeviceSettingState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5764de8a6a04e7c16d9b65bf864206931019675b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312927"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="59a67-103">更新 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="59a67-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="59a67-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59a67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59a67-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59a67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a67-106">更新[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="59a67-106">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59a67-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="59a67-107">Prerequisites</span></span>
<span data-ttu-id="59a67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a67-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59a67-110">Permission type</span></span>|<span data-ttu-id="59a67-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59a67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59a67-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59a67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59a67-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a67-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59a67-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59a67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59a67-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59a67-115">Not supported.</span></span>|
|<span data-ttu-id="59a67-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59a67-116">Application</span></span>|<span data-ttu-id="59a67-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a67-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59a67-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59a67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="59a67-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59a67-119">Request headers</span></span>
|<span data-ttu-id="59a67-120">标头</span><span class="sxs-lookup"><span data-stu-id="59a67-120">Header</span></span>|<span data-ttu-id="59a67-121">值</span><span class="sxs-lookup"><span data-stu-id="59a67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59a67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59a67-122">Authorization</span></span>|<span data-ttu-id="59a67-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59a67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59a67-124">接受</span><span class="sxs-lookup"><span data-stu-id="59a67-124">Accept</span></span>|<span data-ttu-id="59a67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59a67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a67-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="59a67-126">Request body</span></span>
<span data-ttu-id="59a67-127">在请求正文中, 提供[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59a67-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="59a67-128">下表显示创建[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59a67-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="59a67-129">属性</span><span class="sxs-lookup"><span data-stu-id="59a67-129">Property</span></span>|<span data-ttu-id="59a67-130">类型</span><span class="sxs-lookup"><span data-stu-id="59a67-130">Type</span></span>|<span data-ttu-id="59a67-131">说明</span><span class="sxs-lookup"><span data-stu-id="59a67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a67-132">id</span><span class="sxs-lookup"><span data-stu-id="59a67-132">id</span></span>|<span data-ttu-id="59a67-133">String</span><span class="sxs-lookup"><span data-stu-id="59a67-133">String</span></span>|<span data-ttu-id="59a67-134">实体的键</span><span class="sxs-lookup"><span data-stu-id="59a67-134">Key of the entity</span></span>|
|<span data-ttu-id="59a67-135">platformType</span><span class="sxs-lookup"><span data-stu-id="59a67-135">platformType</span></span>|[<span data-ttu-id="59a67-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="59a67-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="59a67-137">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="59a67-137">Device platform type.</span></span> <span data-ttu-id="59a67-138">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="59a67-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="59a67-139">setting</span><span class="sxs-lookup"><span data-stu-id="59a67-139">setting</span></span>|<span data-ttu-id="59a67-140">String</span><span class="sxs-lookup"><span data-stu-id="59a67-140">String</span></span>|<span data-ttu-id="59a67-141">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="59a67-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="59a67-142">settingName</span><span class="sxs-lookup"><span data-stu-id="59a67-142">settingName</span></span>|<span data-ttu-id="59a67-143">String</span><span class="sxs-lookup"><span data-stu-id="59a67-143">String</span></span>|<span data-ttu-id="59a67-144">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="59a67-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="59a67-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="59a67-145">deviceId</span></span>|<span data-ttu-id="59a67-146">String</span><span class="sxs-lookup"><span data-stu-id="59a67-146">String</span></span>|<span data-ttu-id="59a67-147">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="59a67-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="59a67-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="59a67-148">deviceName</span></span>|<span data-ttu-id="59a67-149">String</span><span class="sxs-lookup"><span data-stu-id="59a67-149">String</span></span>|<span data-ttu-id="59a67-150">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="59a67-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="59a67-151">userId</span><span class="sxs-lookup"><span data-stu-id="59a67-151">userId</span></span>|<span data-ttu-id="59a67-152">String</span><span class="sxs-lookup"><span data-stu-id="59a67-152">String</span></span>|<span data-ttu-id="59a67-153">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="59a67-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="59a67-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="59a67-154">userEmail</span></span>|<span data-ttu-id="59a67-155">String</span><span class="sxs-lookup"><span data-stu-id="59a67-155">String</span></span>|<span data-ttu-id="59a67-156">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="59a67-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="59a67-157">userName</span><span class="sxs-lookup"><span data-stu-id="59a67-157">userName</span></span>|<span data-ttu-id="59a67-158">String</span><span class="sxs-lookup"><span data-stu-id="59a67-158">String</span></span>|<span data-ttu-id="59a67-159">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="59a67-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="59a67-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="59a67-160">userPrincipalName</span></span>|<span data-ttu-id="59a67-161">字符串</span><span class="sxs-lookup"><span data-stu-id="59a67-161">String</span></span>|<span data-ttu-id="59a67-162">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="59a67-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="59a67-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="59a67-163">deviceModel</span></span>|<span data-ttu-id="59a67-164">String</span><span class="sxs-lookup"><span data-stu-id="59a67-164">String</span></span>|<span data-ttu-id="59a67-165">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="59a67-165">The device model that is being reported</span></span>|
|<span data-ttu-id="59a67-166">state</span><span class="sxs-lookup"><span data-stu-id="59a67-166">state</span></span>|[<span data-ttu-id="59a67-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="59a67-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="59a67-168">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="59a67-168">The compliance state of the setting.</span></span> <span data-ttu-id="59a67-169">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="59a67-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="59a67-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="59a67-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="59a67-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a67-171">DateTimeOffset</span></span>|<span data-ttu-id="59a67-172">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="59a67-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="59a67-173">响应</span><span class="sxs-lookup"><span data-stu-id="59a67-173">Response</span></span>
<span data-ttu-id="59a67-174">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59a67-174">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59a67-175">示例</span><span class="sxs-lookup"><span data-stu-id="59a67-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="59a67-176">请求</span><span class="sxs-lookup"><span data-stu-id="59a67-176">Request</span></span>
<span data-ttu-id="59a67-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59a67-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
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
```

### <a name="response"></a><span data-ttu-id="59a67-178">响应</span><span class="sxs-lookup"><span data-stu-id="59a67-178">Response</span></span>
<span data-ttu-id="59a67-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59a67-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
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
```






