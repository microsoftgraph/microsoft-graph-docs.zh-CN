---
title: 创建 deviceComplianceSettingState
description: 创建新的 deviceComplianceSettingState 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cb1deb234005cfdb7a206ddabbbc562f8e91299
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758377"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="9ad95-103">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="9ad95-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="9ad95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ad95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ad95-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ad95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ad95-106">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ad95-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ad95-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ad95-107">Prerequisites</span></span>
<span data-ttu-id="9ad95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ad95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad95-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ad95-110">Permission type</span></span>|<span data-ttu-id="9ad95-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ad95-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ad95-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ad95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ad95-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad95-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ad95-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ad95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ad95-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ad95-115">Not supported.</span></span>|
|<span data-ttu-id="9ad95-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ad95-116">Application</span></span>|<span data-ttu-id="9ad95-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad95-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ad95-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ad95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="9ad95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ad95-119">Request headers</span></span>
|<span data-ttu-id="9ad95-120">标头</span><span class="sxs-lookup"><span data-stu-id="9ad95-120">Header</span></span>|<span data-ttu-id="9ad95-121">值</span><span class="sxs-lookup"><span data-stu-id="9ad95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ad95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ad95-122">Authorization</span></span>|<span data-ttu-id="9ad95-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ad95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ad95-124">接受</span><span class="sxs-lookup"><span data-stu-id="9ad95-124">Accept</span></span>|<span data-ttu-id="9ad95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ad95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ad95-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ad95-126">Request body</span></span>
<span data-ttu-id="9ad95-127">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ad95-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="9ad95-128">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ad95-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="9ad95-129">属性</span><span class="sxs-lookup"><span data-stu-id="9ad95-129">Property</span></span>|<span data-ttu-id="9ad95-130">类型</span><span class="sxs-lookup"><span data-stu-id="9ad95-130">Type</span></span>|<span data-ttu-id="9ad95-131">说明</span><span class="sxs-lookup"><span data-stu-id="9ad95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ad95-132">id</span><span class="sxs-lookup"><span data-stu-id="9ad95-132">id</span></span>|<span data-ttu-id="9ad95-133">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-133">String</span></span>|<span data-ttu-id="9ad95-134">实体的键</span><span class="sxs-lookup"><span data-stu-id="9ad95-134">Key of the entity</span></span>|
|<span data-ttu-id="9ad95-135">setting</span><span class="sxs-lookup"><span data-stu-id="9ad95-135">setting</span></span>|<span data-ttu-id="9ad95-136">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-136">String</span></span>|<span data-ttu-id="9ad95-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="9ad95-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="9ad95-138">settingName</span><span class="sxs-lookup"><span data-stu-id="9ad95-138">settingName</span></span>|<span data-ttu-id="9ad95-139">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-139">String</span></span>|<span data-ttu-id="9ad95-140">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="9ad95-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="9ad95-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="9ad95-141">deviceId</span></span>|<span data-ttu-id="9ad95-142">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-142">String</span></span>|<span data-ttu-id="9ad95-143">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="9ad95-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="9ad95-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="9ad95-144">deviceName</span></span>|<span data-ttu-id="9ad95-145">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-145">String</span></span>|<span data-ttu-id="9ad95-146">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="9ad95-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="9ad95-147">userId</span><span class="sxs-lookup"><span data-stu-id="9ad95-147">userId</span></span>|<span data-ttu-id="9ad95-148">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-148">String</span></span>|<span data-ttu-id="9ad95-149">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="9ad95-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="9ad95-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="9ad95-150">userEmail</span></span>|<span data-ttu-id="9ad95-151">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-151">String</span></span>|<span data-ttu-id="9ad95-152">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="9ad95-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="9ad95-153">userName</span><span class="sxs-lookup"><span data-stu-id="9ad95-153">userName</span></span>|<span data-ttu-id="9ad95-154">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-154">String</span></span>|<span data-ttu-id="9ad95-155">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="9ad95-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="9ad95-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9ad95-156">userPrincipalName</span></span>|<span data-ttu-id="9ad95-157">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-157">String</span></span>|<span data-ttu-id="9ad95-158">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9ad95-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="9ad95-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9ad95-159">deviceModel</span></span>|<span data-ttu-id="9ad95-160">String</span><span class="sxs-lookup"><span data-stu-id="9ad95-160">String</span></span>|<span data-ttu-id="9ad95-161">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="9ad95-161">The device model that is being reported</span></span>|
|<span data-ttu-id="9ad95-162">state</span><span class="sxs-lookup"><span data-stu-id="9ad95-162">state</span></span>|[<span data-ttu-id="9ad95-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9ad95-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9ad95-164">设置的合规性状态。</span><span class="sxs-lookup"><span data-stu-id="9ad95-164">The compliance state of the setting.</span></span> <span data-ttu-id="9ad95-165">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9ad95-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9ad95-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad95-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9ad95-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad95-167">DateTimeOffset</span></span>|<span data-ttu-id="9ad95-168">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="9ad95-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="9ad95-169">响应</span><span class="sxs-lookup"><span data-stu-id="9ad95-169">Response</span></span>
<span data-ttu-id="9ad95-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ad95-170">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ad95-171">示例</span><span class="sxs-lookup"><span data-stu-id="9ad95-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ad95-172">请求</span><span class="sxs-lookup"><span data-stu-id="9ad95-172">Request</span></span>
<span data-ttu-id="9ad95-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ad95-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
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

### <a name="response"></a><span data-ttu-id="9ad95-174">响应</span><span class="sxs-lookup"><span data-stu-id="9ad95-174">Response</span></span>
<span data-ttu-id="9ad95-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ad95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




