---
title: 更新 deviceComplianceSettingState
description: 更新 deviceComplianceSettingState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 735f9f3b564d7e810347d63a1c90233be7ff1de7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578069"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="1ef6e-103">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1ef6e-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="1ef6e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ef6e-105">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ef6e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ef6e-106">Prerequisites</span></span>
<span data-ttu-id="1ef6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef6e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ef6e-109">Permission type</span></span>|<span data-ttu-id="1ef6e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ef6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef6e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ef6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef6e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef6e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ef6e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ef6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef6e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-114">Not supported.</span></span>|
|<span data-ttu-id="1ef6e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ef6e-115">Application</span></span>|<span data-ttu-id="1ef6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ef6e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ef6e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1ef6e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ef6e-118">Request headers</span></span>
|<span data-ttu-id="1ef6e-119">标头</span><span class="sxs-lookup"><span data-stu-id="1ef6e-119">Header</span></span>|<span data-ttu-id="1ef6e-120">值</span><span class="sxs-lookup"><span data-stu-id="1ef6e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ef6e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef6e-121">Authorization</span></span>|<span data-ttu-id="1ef6e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ef6e-123">接受</span><span class="sxs-lookup"><span data-stu-id="1ef6e-123">Accept</span></span>|<span data-ttu-id="1ef6e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ef6e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef6e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ef6e-125">Request body</span></span>
<span data-ttu-id="1ef6e-126">在请求正文中，提供 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="1ef6e-127">下表显示了创建 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="1ef6e-128">属性</span><span class="sxs-lookup"><span data-stu-id="1ef6e-128">Property</span></span>|<span data-ttu-id="1ef6e-129">类型</span><span class="sxs-lookup"><span data-stu-id="1ef6e-129">Type</span></span>|<span data-ttu-id="1ef6e-130">说明</span><span class="sxs-lookup"><span data-stu-id="1ef6e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef6e-131">id</span><span class="sxs-lookup"><span data-stu-id="1ef6e-131">id</span></span>|<span data-ttu-id="1ef6e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1ef6e-132">String</span></span>|<span data-ttu-id="1ef6e-133">实体的键</span><span class="sxs-lookup"><span data-stu-id="1ef6e-133">Key of the entity</span></span>|
|<span data-ttu-id="1ef6e-134">setting</span><span class="sxs-lookup"><span data-stu-id="1ef6e-134">setting</span></span>|<span data-ttu-id="1ef6e-135">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-135">String</span></span>|<span data-ttu-id="1ef6e-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="1ef6e-137">settingName</span><span class="sxs-lookup"><span data-stu-id="1ef6e-137">settingName</span></span>|<span data-ttu-id="1ef6e-138">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-138">String</span></span>|<span data-ttu-id="1ef6e-139">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="1ef6e-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1ef6e-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="1ef6e-140">deviceId</span></span>|<span data-ttu-id="1ef6e-141">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-141">String</span></span>|<span data-ttu-id="1ef6e-142">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="1ef6e-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1ef6e-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="1ef6e-143">deviceName</span></span>|<span data-ttu-id="1ef6e-144">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-144">String</span></span>|<span data-ttu-id="1ef6e-145">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="1ef6e-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1ef6e-146">userId</span><span class="sxs-lookup"><span data-stu-id="1ef6e-146">userId</span></span>|<span data-ttu-id="1ef6e-147">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-147">String</span></span>|<span data-ttu-id="1ef6e-148">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="1ef6e-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="1ef6e-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="1ef6e-149">userEmail</span></span>|<span data-ttu-id="1ef6e-150">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-150">String</span></span>|<span data-ttu-id="1ef6e-151">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="1ef6e-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="1ef6e-152">userName</span><span class="sxs-lookup"><span data-stu-id="1ef6e-152">userName</span></span>|<span data-ttu-id="1ef6e-153">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-153">String</span></span>|<span data-ttu-id="1ef6e-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="1ef6e-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="1ef6e-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ef6e-155">userPrincipalName</span></span>|<span data-ttu-id="1ef6e-156">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-156">String</span></span>|<span data-ttu-id="1ef6e-157">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1ef6e-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1ef6e-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1ef6e-158">deviceModel</span></span>|<span data-ttu-id="1ef6e-159">String</span><span class="sxs-lookup"><span data-stu-id="1ef6e-159">String</span></span>|<span data-ttu-id="1ef6e-160">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="1ef6e-160">The device model that is being reported</span></span>|
|<span data-ttu-id="1ef6e-161">state</span><span class="sxs-lookup"><span data-stu-id="1ef6e-161">state</span></span>|[<span data-ttu-id="1ef6e-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1ef6e-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1ef6e-163">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-163">The compliance state of the setting.</span></span> <span data-ttu-id="1ef6e-164">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1ef6e-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1ef6e-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1ef6e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ef6e-166">DateTimeOffset</span></span>|<span data-ttu-id="1ef6e-167">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="1ef6e-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="1ef6e-168">响应</span><span class="sxs-lookup"><span data-stu-id="1ef6e-168">Response</span></span>
<span data-ttu-id="1ef6e-169">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef6e-170">示例</span><span class="sxs-lookup"><span data-stu-id="1ef6e-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ef6e-171">请求</span><span class="sxs-lookup"><span data-stu-id="1ef6e-171">Request</span></span>
<span data-ttu-id="1ef6e-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="1ef6e-173">响应</span><span class="sxs-lookup"><span data-stu-id="1ef6e-173">Response</span></span>
<span data-ttu-id="1ef6e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ef6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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



