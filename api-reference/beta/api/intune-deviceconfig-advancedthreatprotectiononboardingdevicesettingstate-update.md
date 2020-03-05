---
title: 更新 advancedThreatProtectionOnboardingDeviceSettingState
description: 更新 advancedThreatProtectionOnboardingDeviceSettingState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1805d7e342b6db49ccbdad4a23bcf9f647f22e29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444278"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="41f78-103">更新 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="41f78-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="41f78-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="41f78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41f78-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41f78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41f78-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41f78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41f78-107">更新[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41f78-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41f78-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41f78-108">Prerequisites</span></span>
<span data-ttu-id="41f78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41f78-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41f78-111">Permission type</span></span>|<span data-ttu-id="41f78-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41f78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41f78-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41f78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41f78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41f78-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41f78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41f78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41f78-116">Not supported.</span></span>|
|<span data-ttu-id="41f78-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41f78-117">Application</span></span>|<span data-ttu-id="41f78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41f78-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41f78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="41f78-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41f78-120">Request headers</span></span>
|<span data-ttu-id="41f78-121">标头</span><span class="sxs-lookup"><span data-stu-id="41f78-121">Header</span></span>|<span data-ttu-id="41f78-122">值</span><span class="sxs-lookup"><span data-stu-id="41f78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41f78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41f78-123">Authorization</span></span>|<span data-ttu-id="41f78-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41f78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41f78-125">接受</span><span class="sxs-lookup"><span data-stu-id="41f78-125">Accept</span></span>|<span data-ttu-id="41f78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41f78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41f78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41f78-127">Request body</span></span>
<span data-ttu-id="41f78-128">在请求正文中，提供[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41f78-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="41f78-129">下表显示创建[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41f78-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="41f78-130">属性</span><span class="sxs-lookup"><span data-stu-id="41f78-130">Property</span></span>|<span data-ttu-id="41f78-131">类型</span><span class="sxs-lookup"><span data-stu-id="41f78-131">Type</span></span>|<span data-ttu-id="41f78-132">说明</span><span class="sxs-lookup"><span data-stu-id="41f78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f78-133">id</span><span class="sxs-lookup"><span data-stu-id="41f78-133">id</span></span>|<span data-ttu-id="41f78-134">String</span><span class="sxs-lookup"><span data-stu-id="41f78-134">String</span></span>|<span data-ttu-id="41f78-135">实体的键</span><span class="sxs-lookup"><span data-stu-id="41f78-135">Key of the entity</span></span>|
|<span data-ttu-id="41f78-136">platformType</span><span class="sxs-lookup"><span data-stu-id="41f78-136">platformType</span></span>|[<span data-ttu-id="41f78-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="41f78-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="41f78-138">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="41f78-138">Device platform type.</span></span> <span data-ttu-id="41f78-139">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="41f78-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="41f78-140">setting</span><span class="sxs-lookup"><span data-stu-id="41f78-140">setting</span></span>|<span data-ttu-id="41f78-141">String</span><span class="sxs-lookup"><span data-stu-id="41f78-141">String</span></span>|<span data-ttu-id="41f78-142">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="41f78-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="41f78-143">settingName</span><span class="sxs-lookup"><span data-stu-id="41f78-143">settingName</span></span>|<span data-ttu-id="41f78-144">String</span><span class="sxs-lookup"><span data-stu-id="41f78-144">String</span></span>|<span data-ttu-id="41f78-145">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="41f78-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="41f78-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="41f78-146">deviceId</span></span>|<span data-ttu-id="41f78-147">String</span><span class="sxs-lookup"><span data-stu-id="41f78-147">String</span></span>|<span data-ttu-id="41f78-148">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="41f78-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="41f78-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="41f78-149">deviceName</span></span>|<span data-ttu-id="41f78-150">String</span><span class="sxs-lookup"><span data-stu-id="41f78-150">String</span></span>|<span data-ttu-id="41f78-151">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="41f78-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="41f78-152">userId</span><span class="sxs-lookup"><span data-stu-id="41f78-152">userId</span></span>|<span data-ttu-id="41f78-153">String</span><span class="sxs-lookup"><span data-stu-id="41f78-153">String</span></span>|<span data-ttu-id="41f78-154">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="41f78-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="41f78-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="41f78-155">userEmail</span></span>|<span data-ttu-id="41f78-156">String</span><span class="sxs-lookup"><span data-stu-id="41f78-156">String</span></span>|<span data-ttu-id="41f78-157">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="41f78-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="41f78-158">userName</span><span class="sxs-lookup"><span data-stu-id="41f78-158">userName</span></span>|<span data-ttu-id="41f78-159">String</span><span class="sxs-lookup"><span data-stu-id="41f78-159">String</span></span>|<span data-ttu-id="41f78-160">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="41f78-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="41f78-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41f78-161">userPrincipalName</span></span>|<span data-ttu-id="41f78-162">字符串</span><span class="sxs-lookup"><span data-stu-id="41f78-162">String</span></span>|<span data-ttu-id="41f78-163">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="41f78-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="41f78-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="41f78-164">deviceModel</span></span>|<span data-ttu-id="41f78-165">String</span><span class="sxs-lookup"><span data-stu-id="41f78-165">String</span></span>|<span data-ttu-id="41f78-166">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="41f78-166">The device model that is being reported</span></span>|
|<span data-ttu-id="41f78-167">state</span><span class="sxs-lookup"><span data-stu-id="41f78-167">state</span></span>|[<span data-ttu-id="41f78-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="41f78-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="41f78-169">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="41f78-169">The compliance state of the setting.</span></span> <span data-ttu-id="41f78-170">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="41f78-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="41f78-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="41f78-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="41f78-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41f78-172">DateTimeOffset</span></span>|<span data-ttu-id="41f78-173">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="41f78-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="41f78-174">响应</span><span class="sxs-lookup"><span data-stu-id="41f78-174">Response</span></span>
<span data-ttu-id="41f78-175">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41f78-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f78-176">示例</span><span class="sxs-lookup"><span data-stu-id="41f78-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="41f78-177">请求</span><span class="sxs-lookup"><span data-stu-id="41f78-177">Request</span></span>
<span data-ttu-id="41f78-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41f78-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41f78-179">响应</span><span class="sxs-lookup"><span data-stu-id="41f78-179">Response</span></span>
<span data-ttu-id="41f78-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41f78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





