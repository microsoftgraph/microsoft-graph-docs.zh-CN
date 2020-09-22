---
title: 更新 deviceComplianceSettingState
description: 更新 deviceComplianceSettingState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61e5c5bf78978e181fd68193767e189f08ca7374
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011660"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="a8068-103">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a8068-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="a8068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8068-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a8068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8068-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8068-107">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8068-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8068-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8068-108">Prerequisites</span></span>
<span data-ttu-id="a8068-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8068-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8068-111">Permission type</span></span>|<span data-ttu-id="a8068-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8068-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8068-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8068-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8068-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8068-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8068-116">Not supported.</span></span>|
|<span data-ttu-id="a8068-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8068-117">Application</span></span>|<span data-ttu-id="a8068-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8068-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8068-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a8068-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8068-120">Request headers</span></span>
|<span data-ttu-id="a8068-121">标头</span><span class="sxs-lookup"><span data-stu-id="a8068-121">Header</span></span>|<span data-ttu-id="a8068-122">值</span><span class="sxs-lookup"><span data-stu-id="a8068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8068-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8068-123">Authorization</span></span>|<span data-ttu-id="a8068-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8068-125">接受</span><span class="sxs-lookup"><span data-stu-id="a8068-125">Accept</span></span>|<span data-ttu-id="a8068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8068-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8068-127">Request body</span></span>
<span data-ttu-id="a8068-128">在请求正文中，提供 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8068-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="a8068-129">下表显示了创建 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8068-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="a8068-130">属性</span><span class="sxs-lookup"><span data-stu-id="a8068-130">Property</span></span>|<span data-ttu-id="a8068-131">类型</span><span class="sxs-lookup"><span data-stu-id="a8068-131">Type</span></span>|<span data-ttu-id="a8068-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8068-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8068-133">id</span><span class="sxs-lookup"><span data-stu-id="a8068-133">id</span></span>|<span data-ttu-id="a8068-134">String</span><span class="sxs-lookup"><span data-stu-id="a8068-134">String</span></span>|<span data-ttu-id="a8068-135">实体的键</span><span class="sxs-lookup"><span data-stu-id="a8068-135">Key of the entity</span></span>|
|<span data-ttu-id="a8068-136">platformType</span><span class="sxs-lookup"><span data-stu-id="a8068-136">platformType</span></span>|[<span data-ttu-id="a8068-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="a8068-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a8068-138">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="a8068-138">Device platform type.</span></span> <span data-ttu-id="a8068-139">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="a8068-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a8068-140">setting</span><span class="sxs-lookup"><span data-stu-id="a8068-140">setting</span></span>|<span data-ttu-id="a8068-141">String</span><span class="sxs-lookup"><span data-stu-id="a8068-141">String</span></span>|<span data-ttu-id="a8068-142">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="a8068-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="a8068-143">settingName</span><span class="sxs-lookup"><span data-stu-id="a8068-143">settingName</span></span>|<span data-ttu-id="a8068-144">String</span><span class="sxs-lookup"><span data-stu-id="a8068-144">String</span></span>|<span data-ttu-id="a8068-145">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="a8068-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a8068-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="a8068-146">deviceId</span></span>|<span data-ttu-id="a8068-147">String</span><span class="sxs-lookup"><span data-stu-id="a8068-147">String</span></span>|<span data-ttu-id="a8068-148">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="a8068-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a8068-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="a8068-149">deviceName</span></span>|<span data-ttu-id="a8068-150">String</span><span class="sxs-lookup"><span data-stu-id="a8068-150">String</span></span>|<span data-ttu-id="a8068-151">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="a8068-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a8068-152">userId</span><span class="sxs-lookup"><span data-stu-id="a8068-152">userId</span></span>|<span data-ttu-id="a8068-153">String</span><span class="sxs-lookup"><span data-stu-id="a8068-153">String</span></span>|<span data-ttu-id="a8068-154">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="a8068-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="a8068-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="a8068-155">userEmail</span></span>|<span data-ttu-id="a8068-156">String</span><span class="sxs-lookup"><span data-stu-id="a8068-156">String</span></span>|<span data-ttu-id="a8068-157">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="a8068-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="a8068-158">userName</span><span class="sxs-lookup"><span data-stu-id="a8068-158">userName</span></span>|<span data-ttu-id="a8068-159">String</span><span class="sxs-lookup"><span data-stu-id="a8068-159">String</span></span>|<span data-ttu-id="a8068-160">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="a8068-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="a8068-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a8068-161">userPrincipalName</span></span>|<span data-ttu-id="a8068-162">String</span><span class="sxs-lookup"><span data-stu-id="a8068-162">String</span></span>|<span data-ttu-id="a8068-163">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a8068-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a8068-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a8068-164">deviceModel</span></span>|<span data-ttu-id="a8068-165">String</span><span class="sxs-lookup"><span data-stu-id="a8068-165">String</span></span>|<span data-ttu-id="a8068-166">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="a8068-166">The device model that is being reported</span></span>|
|<span data-ttu-id="a8068-167">state</span><span class="sxs-lookup"><span data-stu-id="a8068-167">state</span></span>|[<span data-ttu-id="a8068-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a8068-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a8068-169">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="a8068-169">The compliance state of the setting.</span></span> <span data-ttu-id="a8068-170">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a8068-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a8068-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8068-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a8068-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8068-172">DateTimeOffset</span></span>|<span data-ttu-id="a8068-173">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="a8068-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="a8068-174">响应</span><span class="sxs-lookup"><span data-stu-id="a8068-174">Response</span></span>
<span data-ttu-id="a8068-175">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8068-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8068-176">示例</span><span class="sxs-lookup"><span data-stu-id="a8068-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8068-177">请求</span><span class="sxs-lookup"><span data-stu-id="a8068-177">Request</span></span>
<span data-ttu-id="a8068-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8068-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8068-179">响应</span><span class="sxs-lookup"><span data-stu-id="a8068-179">Response</span></span>
<span data-ttu-id="a8068-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8068-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






