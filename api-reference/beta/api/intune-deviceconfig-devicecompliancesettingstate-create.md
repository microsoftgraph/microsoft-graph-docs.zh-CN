---
title: 创建 deviceComplianceSettingState
description: 创建新的 deviceComplianceSettingState 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd5322a064b0e644decfb0910836d5f7d072783e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755201"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="e53ac-103">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="e53ac-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="e53ac-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e53ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e53ac-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e53ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e53ac-106">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e53ac-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e53ac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e53ac-107">Prerequisites</span></span>
<span data-ttu-id="e53ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e53ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e53ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e53ac-110">Permission type</span></span>|<span data-ttu-id="e53ac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e53ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e53ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e53ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e53ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e53ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e53ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e53ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e53ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e53ac-115">Not supported.</span></span>|
|<span data-ttu-id="e53ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e53ac-116">Application</span></span>|<span data-ttu-id="e53ac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e53ac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e53ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e53ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="e53ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e53ac-119">Request headers</span></span>
|<span data-ttu-id="e53ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="e53ac-120">Header</span></span>|<span data-ttu-id="e53ac-121">值</span><span class="sxs-lookup"><span data-stu-id="e53ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e53ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e53ac-122">Authorization</span></span>|<span data-ttu-id="e53ac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e53ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e53ac-124">接受</span><span class="sxs-lookup"><span data-stu-id="e53ac-124">Accept</span></span>|<span data-ttu-id="e53ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e53ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e53ac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e53ac-126">Request body</span></span>
<span data-ttu-id="e53ac-127">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e53ac-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="e53ac-128">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e53ac-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="e53ac-129">属性</span><span class="sxs-lookup"><span data-stu-id="e53ac-129">Property</span></span>|<span data-ttu-id="e53ac-130">类型</span><span class="sxs-lookup"><span data-stu-id="e53ac-130">Type</span></span>|<span data-ttu-id="e53ac-131">说明</span><span class="sxs-lookup"><span data-stu-id="e53ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e53ac-132">id</span><span class="sxs-lookup"><span data-stu-id="e53ac-132">id</span></span>|<span data-ttu-id="e53ac-133">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-133">String</span></span>|<span data-ttu-id="e53ac-134">实体的键</span><span class="sxs-lookup"><span data-stu-id="e53ac-134">Key of the entity</span></span>|
|<span data-ttu-id="e53ac-135">platformType</span><span class="sxs-lookup"><span data-stu-id="e53ac-135">platformType</span></span>|[<span data-ttu-id="e53ac-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="e53ac-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e53ac-137">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="e53ac-137">Device platform type.</span></span> <span data-ttu-id="e53ac-138">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="e53ac-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e53ac-139">setting</span><span class="sxs-lookup"><span data-stu-id="e53ac-139">setting</span></span>|<span data-ttu-id="e53ac-140">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-140">String</span></span>|<span data-ttu-id="e53ac-141">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="e53ac-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="e53ac-142">settingName</span><span class="sxs-lookup"><span data-stu-id="e53ac-142">settingName</span></span>|<span data-ttu-id="e53ac-143">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-143">String</span></span>|<span data-ttu-id="e53ac-144">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="e53ac-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="e53ac-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="e53ac-145">deviceId</span></span>|<span data-ttu-id="e53ac-146">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-146">String</span></span>|<span data-ttu-id="e53ac-147">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="e53ac-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="e53ac-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="e53ac-148">deviceName</span></span>|<span data-ttu-id="e53ac-149">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-149">String</span></span>|<span data-ttu-id="e53ac-150">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="e53ac-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="e53ac-151">userId</span><span class="sxs-lookup"><span data-stu-id="e53ac-151">userId</span></span>|<span data-ttu-id="e53ac-152">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-152">String</span></span>|<span data-ttu-id="e53ac-153">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="e53ac-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="e53ac-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="e53ac-154">userEmail</span></span>|<span data-ttu-id="e53ac-155">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-155">String</span></span>|<span data-ttu-id="e53ac-156">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="e53ac-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="e53ac-157">userName</span><span class="sxs-lookup"><span data-stu-id="e53ac-157">userName</span></span>|<span data-ttu-id="e53ac-158">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-158">String</span></span>|<span data-ttu-id="e53ac-159">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="e53ac-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="e53ac-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e53ac-160">userPrincipalName</span></span>|<span data-ttu-id="e53ac-161">字符串</span><span class="sxs-lookup"><span data-stu-id="e53ac-161">String</span></span>|<span data-ttu-id="e53ac-162">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e53ac-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="e53ac-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e53ac-163">deviceModel</span></span>|<span data-ttu-id="e53ac-164">String</span><span class="sxs-lookup"><span data-stu-id="e53ac-164">String</span></span>|<span data-ttu-id="e53ac-165">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="e53ac-165">The device model that is being reported</span></span>|
|<span data-ttu-id="e53ac-166">state</span><span class="sxs-lookup"><span data-stu-id="e53ac-166">state</span></span>|[<span data-ttu-id="e53ac-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e53ac-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e53ac-168">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="e53ac-168">The compliance state of the setting.</span></span> <span data-ttu-id="e53ac-169">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e53ac-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e53ac-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e53ac-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e53ac-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53ac-171">DateTimeOffset</span></span>|<span data-ttu-id="e53ac-172">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="e53ac-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="e53ac-173">响应</span><span class="sxs-lookup"><span data-stu-id="e53ac-173">Response</span></span>
<span data-ttu-id="e53ac-174">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e53ac-174">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e53ac-175">示例</span><span class="sxs-lookup"><span data-stu-id="e53ac-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e53ac-176">请求</span><span class="sxs-lookup"><span data-stu-id="e53ac-176">Request</span></span>
<span data-ttu-id="e53ac-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e53ac-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
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

### <a name="response"></a><span data-ttu-id="e53ac-178">响应</span><span class="sxs-lookup"><span data-stu-id="e53ac-178">Response</span></span>
<span data-ttu-id="e53ac-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e53ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




