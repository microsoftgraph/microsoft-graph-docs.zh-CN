---
title: 创建 deviceComplianceSettingState
description: 创建新的 deviceComplianceSettingState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1914c143bc4c5c7bb40acfcdd4b57cead1070a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956981"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="03513-103">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03513-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="03513-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03513-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03513-105">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03513-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03513-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="03513-106">Prerequisites</span></span>
<span data-ttu-id="03513-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="03513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03513-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="03513-109">Permission type</span></span>|<span data-ttu-id="03513-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03513-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03513-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03513-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03513-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03513-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03513-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03513-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03513-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="03513-114">Not supported.</span></span>|
|<span data-ttu-id="03513-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="03513-115">Application</span></span>|<span data-ttu-id="03513-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03513-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03513-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03513-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="03513-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="03513-118">Request headers</span></span>
|<span data-ttu-id="03513-119">标头</span><span class="sxs-lookup"><span data-stu-id="03513-119">Header</span></span>|<span data-ttu-id="03513-120">值</span><span class="sxs-lookup"><span data-stu-id="03513-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03513-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03513-121">Authorization</span></span>|<span data-ttu-id="03513-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03513-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03513-123">Accept</span><span class="sxs-lookup"><span data-stu-id="03513-123">Accept</span></span>|<span data-ttu-id="03513-124">application/json</span><span class="sxs-lookup"><span data-stu-id="03513-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03513-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="03513-125">Request body</span></span>
<span data-ttu-id="03513-126">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03513-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="03513-127">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03513-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="03513-128">属性</span><span class="sxs-lookup"><span data-stu-id="03513-128">Property</span></span>|<span data-ttu-id="03513-129">类型</span><span class="sxs-lookup"><span data-stu-id="03513-129">Type</span></span>|<span data-ttu-id="03513-130">说明</span><span class="sxs-lookup"><span data-stu-id="03513-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03513-131">id</span><span class="sxs-lookup"><span data-stu-id="03513-131">id</span></span>|<span data-ttu-id="03513-132">String</span><span class="sxs-lookup"><span data-stu-id="03513-132">String</span></span>|<span data-ttu-id="03513-133">实体的键</span><span class="sxs-lookup"><span data-stu-id="03513-133">Key of the entity</span></span>|
|<span data-ttu-id="03513-134">setting</span><span class="sxs-lookup"><span data-stu-id="03513-134">setting</span></span>|<span data-ttu-id="03513-135">String</span><span class="sxs-lookup"><span data-stu-id="03513-135">String</span></span>|<span data-ttu-id="03513-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="03513-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="03513-137">settingName</span><span class="sxs-lookup"><span data-stu-id="03513-137">settingName</span></span>|<span data-ttu-id="03513-138">String</span><span class="sxs-lookup"><span data-stu-id="03513-138">String</span></span>|<span data-ttu-id="03513-139">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="03513-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="03513-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="03513-140">deviceId</span></span>|<span data-ttu-id="03513-141">String</span><span class="sxs-lookup"><span data-stu-id="03513-141">String</span></span>|<span data-ttu-id="03513-142">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="03513-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="03513-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="03513-143">deviceName</span></span>|<span data-ttu-id="03513-144">String</span><span class="sxs-lookup"><span data-stu-id="03513-144">String</span></span>|<span data-ttu-id="03513-145">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="03513-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="03513-146">userId</span><span class="sxs-lookup"><span data-stu-id="03513-146">userId</span></span>|<span data-ttu-id="03513-147">String</span><span class="sxs-lookup"><span data-stu-id="03513-147">String</span></span>|<span data-ttu-id="03513-148">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="03513-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="03513-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="03513-149">userEmail</span></span>|<span data-ttu-id="03513-150">String</span><span class="sxs-lookup"><span data-stu-id="03513-150">String</span></span>|<span data-ttu-id="03513-151">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="03513-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="03513-152">userName</span><span class="sxs-lookup"><span data-stu-id="03513-152">userName</span></span>|<span data-ttu-id="03513-153">String</span><span class="sxs-lookup"><span data-stu-id="03513-153">String</span></span>|<span data-ttu-id="03513-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="03513-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="03513-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03513-155">userPrincipalName</span></span>|<span data-ttu-id="03513-156">String</span><span class="sxs-lookup"><span data-stu-id="03513-156">String</span></span>|<span data-ttu-id="03513-157">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="03513-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="03513-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="03513-158">deviceModel</span></span>|<span data-ttu-id="03513-159">String</span><span class="sxs-lookup"><span data-stu-id="03513-159">String</span></span>|<span data-ttu-id="03513-160">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="03513-160">The device model that is being reported</span></span>|
|<span data-ttu-id="03513-161">state</span><span class="sxs-lookup"><span data-stu-id="03513-161">state</span></span>|[<span data-ttu-id="03513-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="03513-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="03513-163">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="03513-163">The compliance state of the setting.</span></span> <span data-ttu-id="03513-164">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="03513-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="03513-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="03513-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="03513-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03513-166">DateTimeOffset</span></span>|<span data-ttu-id="03513-167">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="03513-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="03513-168">响应</span><span class="sxs-lookup"><span data-stu-id="03513-168">Response</span></span>
<span data-ttu-id="03513-169">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03513-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03513-170">示例</span><span class="sxs-lookup"><span data-stu-id="03513-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="03513-171">请求</span><span class="sxs-lookup"><span data-stu-id="03513-171">Request</span></span>
<span data-ttu-id="03513-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03513-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03513-173">响应</span><span class="sxs-lookup"><span data-stu-id="03513-173">Response</span></span>
<span data-ttu-id="03513-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03513-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



