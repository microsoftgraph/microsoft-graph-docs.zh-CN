---
title: 创建 advancedThreatProtectionOnboardingDeviceSettingState
description: 创建新的 advancedThreatProtectionOnboardingDeviceSettingState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 576ac7eaf5e44cdd3539c1d4a281c3612880e733
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793148"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="f5815-103">创建 advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="f5815-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="f5815-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5815-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5815-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5815-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5815-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5815-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5815-107">创建新的[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f5815-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5815-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5815-108">Prerequisites</span></span>
<span data-ttu-id="f5815-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f5815-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f5815-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5815-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5815-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5815-111">Permission type</span></span>|<span data-ttu-id="f5815-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5815-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5815-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5815-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5815-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5815-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5815-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5815-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5815-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5815-116">Not supported.</span></span>|
|<span data-ttu-id="f5815-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5815-117">Application</span></span>|<span data-ttu-id="f5815-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5815-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5815-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5815-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="f5815-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5815-120">Request headers</span></span>
|<span data-ttu-id="f5815-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5815-121">Header</span></span>|<span data-ttu-id="f5815-122">值</span><span class="sxs-lookup"><span data-stu-id="f5815-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5815-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5815-123">Authorization</span></span>|<span data-ttu-id="f5815-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5815-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5815-125">接受</span><span class="sxs-lookup"><span data-stu-id="f5815-125">Accept</span></span>|<span data-ttu-id="f5815-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5815-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5815-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5815-127">Request body</span></span>
<span data-ttu-id="f5815-128">在请求正文中，提供 advancedThreatProtectionOnboardingDeviceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5815-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="f5815-129">下表显示创建 advancedThreatProtectionOnboardingDeviceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5815-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="f5815-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5815-130">Property</span></span>|<span data-ttu-id="f5815-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5815-131">Type</span></span>|<span data-ttu-id="f5815-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5815-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5815-133">id</span><span class="sxs-lookup"><span data-stu-id="f5815-133">id</span></span>|<span data-ttu-id="f5815-134">String</span><span class="sxs-lookup"><span data-stu-id="f5815-134">String</span></span>|<span data-ttu-id="f5815-135">实体的键</span><span class="sxs-lookup"><span data-stu-id="f5815-135">Key of the entity</span></span>|
|<span data-ttu-id="f5815-136">platformType</span><span class="sxs-lookup"><span data-stu-id="f5815-136">platformType</span></span>|[<span data-ttu-id="f5815-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="f5815-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f5815-138">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="f5815-138">Device platform type.</span></span> <span data-ttu-id="f5815-139">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="f5815-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f5815-140">setting</span><span class="sxs-lookup"><span data-stu-id="f5815-140">setting</span></span>|<span data-ttu-id="f5815-141">String</span><span class="sxs-lookup"><span data-stu-id="f5815-141">String</span></span>|<span data-ttu-id="f5815-142">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="f5815-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="f5815-143">settingName</span><span class="sxs-lookup"><span data-stu-id="f5815-143">settingName</span></span>|<span data-ttu-id="f5815-144">String</span><span class="sxs-lookup"><span data-stu-id="f5815-144">String</span></span>|<span data-ttu-id="f5815-145">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="f5815-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f5815-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="f5815-146">deviceId</span></span>|<span data-ttu-id="f5815-147">String</span><span class="sxs-lookup"><span data-stu-id="f5815-147">String</span></span>|<span data-ttu-id="f5815-148">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="f5815-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f5815-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="f5815-149">deviceName</span></span>|<span data-ttu-id="f5815-150">String</span><span class="sxs-lookup"><span data-stu-id="f5815-150">String</span></span>|<span data-ttu-id="f5815-151">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="f5815-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f5815-152">userId</span><span class="sxs-lookup"><span data-stu-id="f5815-152">userId</span></span>|<span data-ttu-id="f5815-153">String</span><span class="sxs-lookup"><span data-stu-id="f5815-153">String</span></span>|<span data-ttu-id="f5815-154">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="f5815-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="f5815-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="f5815-155">userEmail</span></span>|<span data-ttu-id="f5815-156">String</span><span class="sxs-lookup"><span data-stu-id="f5815-156">String</span></span>|<span data-ttu-id="f5815-157">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="f5815-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="f5815-158">userName</span><span class="sxs-lookup"><span data-stu-id="f5815-158">userName</span></span>|<span data-ttu-id="f5815-159">String</span><span class="sxs-lookup"><span data-stu-id="f5815-159">String</span></span>|<span data-ttu-id="f5815-160">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="f5815-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="f5815-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f5815-161">userPrincipalName</span></span>|<span data-ttu-id="f5815-162">字符串</span><span class="sxs-lookup"><span data-stu-id="f5815-162">String</span></span>|<span data-ttu-id="f5815-163">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f5815-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f5815-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f5815-164">deviceModel</span></span>|<span data-ttu-id="f5815-165">String</span><span class="sxs-lookup"><span data-stu-id="f5815-165">String</span></span>|<span data-ttu-id="f5815-166">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="f5815-166">The device model that is being reported</span></span>|
|<span data-ttu-id="f5815-167">state</span><span class="sxs-lookup"><span data-stu-id="f5815-167">state</span></span>|[<span data-ttu-id="f5815-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f5815-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f5815-169">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="f5815-169">The compliance state of the setting.</span></span> <span data-ttu-id="f5815-170">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f5815-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f5815-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f5815-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f5815-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5815-172">DateTimeOffset</span></span>|<span data-ttu-id="f5815-173">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="f5815-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="f5815-174">响应</span><span class="sxs-lookup"><span data-stu-id="f5815-174">Response</span></span>
<span data-ttu-id="f5815-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f5815-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5815-176">示例</span><span class="sxs-lookup"><span data-stu-id="f5815-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5815-177">请求</span><span class="sxs-lookup"><span data-stu-id="f5815-177">Request</span></span>
<span data-ttu-id="f5815-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5815-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
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

### <a name="response"></a><span data-ttu-id="f5815-179">响应</span><span class="sxs-lookup"><span data-stu-id="f5815-179">Response</span></span>
<span data-ttu-id="f5815-180">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f5815-180">Here is an example of the response.</span></span> <span data-ttu-id="f5815-181">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f5815-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5815-182">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f5815-182">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



