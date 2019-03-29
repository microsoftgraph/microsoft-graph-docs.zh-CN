---
title: 更新 deviceComplianceSettingState
description: 更新 deviceComplianceSettingState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2cba44ee5a012e173f1411da7db53c0d11f4adcb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981592"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="5b296-103">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="5b296-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="5b296-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b296-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b296-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b296-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b296-106">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5b296-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b296-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b296-107">Prerequisites</span></span>
<span data-ttu-id="5b296-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b296-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b296-110">Permission type</span></span>|<span data-ttu-id="5b296-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b296-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b296-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b296-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b296-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b296-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b296-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b296-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b296-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b296-115">Not supported.</span></span>|
|<span data-ttu-id="5b296-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b296-116">Application</span></span>|<span data-ttu-id="5b296-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b296-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b296-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b296-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5b296-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b296-119">Request headers</span></span>
|<span data-ttu-id="5b296-120">标头</span><span class="sxs-lookup"><span data-stu-id="5b296-120">Header</span></span>|<span data-ttu-id="5b296-121">值</span><span class="sxs-lookup"><span data-stu-id="5b296-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b296-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b296-122">Authorization</span></span>|<span data-ttu-id="5b296-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b296-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b296-124">接受</span><span class="sxs-lookup"><span data-stu-id="5b296-124">Accept</span></span>|<span data-ttu-id="5b296-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b296-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b296-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b296-126">Request body</span></span>
<span data-ttu-id="5b296-127">在请求正文中，提供 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b296-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="5b296-128">下表显示了创建 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5b296-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="5b296-129">属性</span><span class="sxs-lookup"><span data-stu-id="5b296-129">Property</span></span>|<span data-ttu-id="5b296-130">类型</span><span class="sxs-lookup"><span data-stu-id="5b296-130">Type</span></span>|<span data-ttu-id="5b296-131">说明</span><span class="sxs-lookup"><span data-stu-id="5b296-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b296-132">id</span><span class="sxs-lookup"><span data-stu-id="5b296-132">id</span></span>|<span data-ttu-id="5b296-133">String</span><span class="sxs-lookup"><span data-stu-id="5b296-133">String</span></span>|<span data-ttu-id="5b296-134">实体的键</span><span class="sxs-lookup"><span data-stu-id="5b296-134">Key of the entity</span></span>|
|<span data-ttu-id="5b296-135">platformType</span><span class="sxs-lookup"><span data-stu-id="5b296-135">platformType</span></span>|[<span data-ttu-id="5b296-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="5b296-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5b296-137">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="5b296-137">Device platform type.</span></span> <span data-ttu-id="5b296-138">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5b296-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5b296-139">setting</span><span class="sxs-lookup"><span data-stu-id="5b296-139">setting</span></span>|<span data-ttu-id="5b296-140">String</span><span class="sxs-lookup"><span data-stu-id="5b296-140">String</span></span>|<span data-ttu-id="5b296-141">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="5b296-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="5b296-142">settingName</span><span class="sxs-lookup"><span data-stu-id="5b296-142">settingName</span></span>|<span data-ttu-id="5b296-143">String</span><span class="sxs-lookup"><span data-stu-id="5b296-143">String</span></span>|<span data-ttu-id="5b296-144">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="5b296-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="5b296-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="5b296-145">deviceId</span></span>|<span data-ttu-id="5b296-146">String</span><span class="sxs-lookup"><span data-stu-id="5b296-146">String</span></span>|<span data-ttu-id="5b296-147">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="5b296-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="5b296-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="5b296-148">deviceName</span></span>|<span data-ttu-id="5b296-149">String</span><span class="sxs-lookup"><span data-stu-id="5b296-149">String</span></span>|<span data-ttu-id="5b296-150">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="5b296-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="5b296-151">userId</span><span class="sxs-lookup"><span data-stu-id="5b296-151">userId</span></span>|<span data-ttu-id="5b296-152">String</span><span class="sxs-lookup"><span data-stu-id="5b296-152">String</span></span>|<span data-ttu-id="5b296-153">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="5b296-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="5b296-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="5b296-154">userEmail</span></span>|<span data-ttu-id="5b296-155">String</span><span class="sxs-lookup"><span data-stu-id="5b296-155">String</span></span>|<span data-ttu-id="5b296-156">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="5b296-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="5b296-157">userName</span><span class="sxs-lookup"><span data-stu-id="5b296-157">userName</span></span>|<span data-ttu-id="5b296-158">String</span><span class="sxs-lookup"><span data-stu-id="5b296-158">String</span></span>|<span data-ttu-id="5b296-159">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="5b296-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="5b296-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b296-160">userPrincipalName</span></span>|<span data-ttu-id="5b296-161">String</span><span class="sxs-lookup"><span data-stu-id="5b296-161">String</span></span>|<span data-ttu-id="5b296-162">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="5b296-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="5b296-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5b296-163">deviceModel</span></span>|<span data-ttu-id="5b296-164">String</span><span class="sxs-lookup"><span data-stu-id="5b296-164">String</span></span>|<span data-ttu-id="5b296-165">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="5b296-165">The device model that is being reported</span></span>|
|<span data-ttu-id="5b296-166">state</span><span class="sxs-lookup"><span data-stu-id="5b296-166">state</span></span>|[<span data-ttu-id="5b296-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5b296-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5b296-168">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5b296-168">The compliance state of the setting.</span></span> <span data-ttu-id="5b296-169">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="5b296-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5b296-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5b296-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5b296-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b296-171">DateTimeOffset</span></span>|<span data-ttu-id="5b296-172">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="5b296-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="5b296-173">响应</span><span class="sxs-lookup"><span data-stu-id="5b296-173">Response</span></span>
<span data-ttu-id="5b296-174">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b296-174">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b296-175">示例</span><span class="sxs-lookup"><span data-stu-id="5b296-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b296-176">请求</span><span class="sxs-lookup"><span data-stu-id="5b296-176">Request</span></span>
<span data-ttu-id="5b296-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b296-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b296-178">响应</span><span class="sxs-lookup"><span data-stu-id="5b296-178">Response</span></span>
<span data-ttu-id="5b296-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b296-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




