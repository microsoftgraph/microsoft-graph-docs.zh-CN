---
title: 更新 deviceComplianceSettingState
description: 更新 deviceComplianceSettingState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e38e31f91ef4389b2276a93709d175a1a36aa73
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793008"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="8d425-103">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8d425-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="8d425-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d425-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d425-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d425-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d425-107">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d425-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d425-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d425-108">Prerequisites</span></span>
<span data-ttu-id="8d425-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8d425-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8d425-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d425-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d425-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d425-111">Permission type</span></span>|<span data-ttu-id="8d425-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d425-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d425-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d425-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d425-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d425-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d425-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d425-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d425-116">Not supported.</span></span>|
|<span data-ttu-id="8d425-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d425-117">Application</span></span>|<span data-ttu-id="8d425-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d425-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d425-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d425-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8d425-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d425-120">Request headers</span></span>
|<span data-ttu-id="8d425-121">标头</span><span class="sxs-lookup"><span data-stu-id="8d425-121">Header</span></span>|<span data-ttu-id="8d425-122">值</span><span class="sxs-lookup"><span data-stu-id="8d425-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d425-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d425-123">Authorization</span></span>|<span data-ttu-id="8d425-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d425-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d425-125">接受</span><span class="sxs-lookup"><span data-stu-id="8d425-125">Accept</span></span>|<span data-ttu-id="8d425-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d425-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d425-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d425-127">Request body</span></span>
<span data-ttu-id="8d425-128">在请求正文中，提供 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d425-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="8d425-129">下表显示了创建 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d425-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="8d425-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d425-130">Property</span></span>|<span data-ttu-id="8d425-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d425-131">Type</span></span>|<span data-ttu-id="8d425-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d425-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d425-133">id</span><span class="sxs-lookup"><span data-stu-id="8d425-133">id</span></span>|<span data-ttu-id="8d425-134">String</span><span class="sxs-lookup"><span data-stu-id="8d425-134">String</span></span>|<span data-ttu-id="8d425-135">实体的键</span><span class="sxs-lookup"><span data-stu-id="8d425-135">Key of the entity</span></span>|
|<span data-ttu-id="8d425-136">platformType</span><span class="sxs-lookup"><span data-stu-id="8d425-136">platformType</span></span>|[<span data-ttu-id="8d425-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="8d425-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="8d425-138">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="8d425-138">Device platform type.</span></span> <span data-ttu-id="8d425-139">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="8d425-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="8d425-140">setting</span><span class="sxs-lookup"><span data-stu-id="8d425-140">setting</span></span>|<span data-ttu-id="8d425-141">String</span><span class="sxs-lookup"><span data-stu-id="8d425-141">String</span></span>|<span data-ttu-id="8d425-142">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="8d425-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="8d425-143">settingName</span><span class="sxs-lookup"><span data-stu-id="8d425-143">settingName</span></span>|<span data-ttu-id="8d425-144">String</span><span class="sxs-lookup"><span data-stu-id="8d425-144">String</span></span>|<span data-ttu-id="8d425-145">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="8d425-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="8d425-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="8d425-146">deviceId</span></span>|<span data-ttu-id="8d425-147">String</span><span class="sxs-lookup"><span data-stu-id="8d425-147">String</span></span>|<span data-ttu-id="8d425-148">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="8d425-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="8d425-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="8d425-149">deviceName</span></span>|<span data-ttu-id="8d425-150">String</span><span class="sxs-lookup"><span data-stu-id="8d425-150">String</span></span>|<span data-ttu-id="8d425-151">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="8d425-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="8d425-152">userId</span><span class="sxs-lookup"><span data-stu-id="8d425-152">userId</span></span>|<span data-ttu-id="8d425-153">String</span><span class="sxs-lookup"><span data-stu-id="8d425-153">String</span></span>|<span data-ttu-id="8d425-154">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="8d425-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="8d425-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="8d425-155">userEmail</span></span>|<span data-ttu-id="8d425-156">String</span><span class="sxs-lookup"><span data-stu-id="8d425-156">String</span></span>|<span data-ttu-id="8d425-157">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="8d425-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="8d425-158">userName</span><span class="sxs-lookup"><span data-stu-id="8d425-158">userName</span></span>|<span data-ttu-id="8d425-159">String</span><span class="sxs-lookup"><span data-stu-id="8d425-159">String</span></span>|<span data-ttu-id="8d425-160">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="8d425-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="8d425-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d425-161">userPrincipalName</span></span>|<span data-ttu-id="8d425-162">字符串</span><span class="sxs-lookup"><span data-stu-id="8d425-162">String</span></span>|<span data-ttu-id="8d425-163">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="8d425-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="8d425-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8d425-164">deviceModel</span></span>|<span data-ttu-id="8d425-165">String</span><span class="sxs-lookup"><span data-stu-id="8d425-165">String</span></span>|<span data-ttu-id="8d425-166">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="8d425-166">The device model that is being reported</span></span>|
|<span data-ttu-id="8d425-167">state</span><span class="sxs-lookup"><span data-stu-id="8d425-167">state</span></span>|[<span data-ttu-id="8d425-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8d425-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8d425-169">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="8d425-169">The compliance state of the setting.</span></span> <span data-ttu-id="8d425-170">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="8d425-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8d425-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8d425-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8d425-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d425-172">DateTimeOffset</span></span>|<span data-ttu-id="8d425-173">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8d425-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="8d425-174">响应</span><span class="sxs-lookup"><span data-stu-id="8d425-174">Response</span></span>
<span data-ttu-id="8d425-175">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d425-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d425-176">示例</span><span class="sxs-lookup"><span data-stu-id="8d425-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d425-177">请求</span><span class="sxs-lookup"><span data-stu-id="8d425-177">Request</span></span>
<span data-ttu-id="8d425-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d425-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="8d425-179">响应</span><span class="sxs-lookup"><span data-stu-id="8d425-179">Response</span></span>
<span data-ttu-id="8d425-180">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="8d425-180">Here is an example of the response.</span></span> <span data-ttu-id="8d425-181">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="8d425-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8d425-182">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8d425-182">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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



