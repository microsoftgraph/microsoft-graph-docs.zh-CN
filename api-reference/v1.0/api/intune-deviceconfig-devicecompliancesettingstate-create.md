---
title: 创建 deviceComplianceSettingState
description: 创建新的 deviceComplianceSettingState 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7f702f5b9f4b7ab9de29e725c3ab1414753d180
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514941"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="bbaa2-103">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bbaa2-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="bbaa2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbaa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbaa2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbaa2-106">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbaa2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbaa2-107">Prerequisites</span></span>
<span data-ttu-id="bbaa2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbaa2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbaa2-110">Permission type</span></span>|<span data-ttu-id="bbaa2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bbaa2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbaa2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbaa2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbaa2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbaa2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbaa2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbaa2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbaa2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-115">Not supported.</span></span>|
|<span data-ttu-id="bbaa2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbaa2-116">Application</span></span>|<span data-ttu-id="bbaa2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbaa2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbaa2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="bbaa2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbaa2-119">Request headers</span></span>
|<span data-ttu-id="bbaa2-120">标头</span><span class="sxs-lookup"><span data-stu-id="bbaa2-120">Header</span></span>|<span data-ttu-id="bbaa2-121">值</span><span class="sxs-lookup"><span data-stu-id="bbaa2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbaa2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbaa2-122">Authorization</span></span>|<span data-ttu-id="bbaa2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbaa2-124">接受</span><span class="sxs-lookup"><span data-stu-id="bbaa2-124">Accept</span></span>|<span data-ttu-id="bbaa2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bbaa2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbaa2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbaa2-126">Request body</span></span>
<span data-ttu-id="bbaa2-127">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="bbaa2-128">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="bbaa2-129">属性</span><span class="sxs-lookup"><span data-stu-id="bbaa2-129">Property</span></span>|<span data-ttu-id="bbaa2-130">类型</span><span class="sxs-lookup"><span data-stu-id="bbaa2-130">Type</span></span>|<span data-ttu-id="bbaa2-131">说明</span><span class="sxs-lookup"><span data-stu-id="bbaa2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbaa2-132">id</span><span class="sxs-lookup"><span data-stu-id="bbaa2-132">id</span></span>|<span data-ttu-id="bbaa2-133">String</span><span class="sxs-lookup"><span data-stu-id="bbaa2-133">String</span></span>|<span data-ttu-id="bbaa2-134">实体的键</span><span class="sxs-lookup"><span data-stu-id="bbaa2-134">Key of the entity</span></span>|
|<span data-ttu-id="bbaa2-135">setting</span><span class="sxs-lookup"><span data-stu-id="bbaa2-135">setting</span></span>|<span data-ttu-id="bbaa2-136">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-136">String</span></span>|<span data-ttu-id="bbaa2-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="bbaa2-138">settingName</span><span class="sxs-lookup"><span data-stu-id="bbaa2-138">settingName</span></span>|<span data-ttu-id="bbaa2-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-139">String</span></span>|<span data-ttu-id="bbaa2-140">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="bbaa2-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="bbaa2-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="bbaa2-141">deviceId</span></span>|<span data-ttu-id="bbaa2-142">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-142">String</span></span>|<span data-ttu-id="bbaa2-143">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="bbaa2-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="bbaa2-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="bbaa2-144">deviceName</span></span>|<span data-ttu-id="bbaa2-145">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-145">String</span></span>|<span data-ttu-id="bbaa2-146">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="bbaa2-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="bbaa2-147">userId</span><span class="sxs-lookup"><span data-stu-id="bbaa2-147">userId</span></span>|<span data-ttu-id="bbaa2-148">String</span><span class="sxs-lookup"><span data-stu-id="bbaa2-148">String</span></span>|<span data-ttu-id="bbaa2-149">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="bbaa2-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="bbaa2-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="bbaa2-150">userEmail</span></span>|<span data-ttu-id="bbaa2-151">String</span><span class="sxs-lookup"><span data-stu-id="bbaa2-151">String</span></span>|<span data-ttu-id="bbaa2-152">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="bbaa2-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="bbaa2-153">userName</span><span class="sxs-lookup"><span data-stu-id="bbaa2-153">userName</span></span>|<span data-ttu-id="bbaa2-154">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-154">String</span></span>|<span data-ttu-id="bbaa2-155">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="bbaa2-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="bbaa2-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bbaa2-156">userPrincipalName</span></span>|<span data-ttu-id="bbaa2-157">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-157">String</span></span>|<span data-ttu-id="bbaa2-158">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bbaa2-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="bbaa2-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bbaa2-159">deviceModel</span></span>|<span data-ttu-id="bbaa2-160">字符串</span><span class="sxs-lookup"><span data-stu-id="bbaa2-160">String</span></span>|<span data-ttu-id="bbaa2-161">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="bbaa2-161">The device model that is being reported</span></span>|
|<span data-ttu-id="bbaa2-162">state</span><span class="sxs-lookup"><span data-stu-id="bbaa2-162">state</span></span>|[<span data-ttu-id="bbaa2-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="bbaa2-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bbaa2-164">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-164">The compliance state of the setting.</span></span> <span data-ttu-id="bbaa2-165">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bbaa2-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bbaa2-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bbaa2-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbaa2-167">DateTimeOffset</span></span>|<span data-ttu-id="bbaa2-168">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="bbaa2-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="bbaa2-169">响应</span><span class="sxs-lookup"><span data-stu-id="bbaa2-169">Response</span></span>
<span data-ttu-id="bbaa2-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-170">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbaa2-171">示例</span><span class="sxs-lookup"><span data-stu-id="bbaa2-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbaa2-172">请求</span><span class="sxs-lookup"><span data-stu-id="bbaa2-172">Request</span></span>
<span data-ttu-id="bbaa2-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbaa2-174">响应</span><span class="sxs-lookup"><span data-stu-id="bbaa2-174">Response</span></span>
<span data-ttu-id="bbaa2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbaa2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




