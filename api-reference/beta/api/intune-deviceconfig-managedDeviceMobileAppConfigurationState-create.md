---
title: 创建 managedDeviceMobileAppConfigurationState
description: 创建新的 managedDeviceMobileAppConfigurationState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ab87332a5dedc2aaffbae19966fce737bcbdf1b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636101"
---
# <a name="create-manageddevicemobileappconfigurationstate"></a><span data-ttu-id="82fe8-103">创建 managedDeviceMobileAppConfigurationState</span><span class="sxs-lookup"><span data-stu-id="82fe8-103">Create managedDeviceMobileAppConfigurationState</span></span>

> <span data-ttu-id="82fe8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82fe8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82fe8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82fe8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82fe8-106">创建新的 managedDeviceMobileAppConfigurationState 对象。</span><span class="sxs-lookup"><span data-stu-id="82fe8-106">Create a new managedDeviceMobileAppConfigurationState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82fe8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="82fe8-107">Prerequisites</span></span>
<span data-ttu-id="82fe8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82fe8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82fe8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82fe8-110">Permission type</span></span>|<span data-ttu-id="82fe8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82fe8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82fe8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82fe8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82fe8-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82fe8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82fe8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82fe8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82fe8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82fe8-115">Not supported.</span></span>|
|<span data-ttu-id="82fe8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82fe8-116">Application</span></span>|<span data-ttu-id="82fe8-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82fe8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82fe8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82fe8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
```

## <a name="request-headers"></a><span data-ttu-id="82fe8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="82fe8-119">Request headers</span></span>
|<span data-ttu-id="82fe8-120">标头</span><span class="sxs-lookup"><span data-stu-id="82fe8-120">Header</span></span>|<span data-ttu-id="82fe8-121">值</span><span class="sxs-lookup"><span data-stu-id="82fe8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82fe8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82fe8-122">Authorization</span></span>|<span data-ttu-id="82fe8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82fe8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82fe8-124">接受</span><span class="sxs-lookup"><span data-stu-id="82fe8-124">Accept</span></span>|<span data-ttu-id="82fe8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82fe8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82fe8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82fe8-126">Request body</span></span>
<span data-ttu-id="82fe8-127">在请求正文中，提供 managedDeviceMobileAppConfigurationState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82fe8-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationState object.</span></span>

<span data-ttu-id="82fe8-128">下表显示创建 managedDeviceMobileAppConfigurationState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82fe8-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationState.</span></span>

|<span data-ttu-id="82fe8-129">属性</span><span class="sxs-lookup"><span data-stu-id="82fe8-129">Property</span></span>|<span data-ttu-id="82fe8-130">类型</span><span class="sxs-lookup"><span data-stu-id="82fe8-130">Type</span></span>|<span data-ttu-id="82fe8-131">说明</span><span class="sxs-lookup"><span data-stu-id="82fe8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82fe8-132">id</span><span class="sxs-lookup"><span data-stu-id="82fe8-132">id</span></span>|<span data-ttu-id="82fe8-133">String</span><span class="sxs-lookup"><span data-stu-id="82fe8-133">String</span></span>|<span data-ttu-id="82fe8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82fe8-134">Key of the entity.</span></span>|
|<span data-ttu-id="82fe8-135">settingStates</span><span class="sxs-lookup"><span data-stu-id="82fe8-135">settingStates</span></span>|<span data-ttu-id="82fe8-136">managedDeviceMobileAppConfigurationSettingState 集合</span><span class="sxs-lookup"><span data-stu-id="82fe8-136">managedDeviceMobileAppConfigurationSettingState collection</span></span>|<span data-ttu-id="82fe8-137">**TODO：添加说明。**</span><span class="sxs-lookup"><span data-stu-id="82fe8-137">**TODO: Add description.**</span></span>|
|<span data-ttu-id="82fe8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="82fe8-138">displayName</span></span>|<span data-ttu-id="82fe8-139">String</span><span class="sxs-lookup"><span data-stu-id="82fe8-139">String</span></span>|<span data-ttu-id="82fe8-140">此 policyBase 的策略名称</span><span class="sxs-lookup"><span data-stu-id="82fe8-140">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="82fe8-141">version</span><span class="sxs-lookup"><span data-stu-id="82fe8-141">version</span></span>|<span data-ttu-id="82fe8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="82fe8-142">Int32</span></span>|<span data-ttu-id="82fe8-143">策略版本</span><span class="sxs-lookup"><span data-stu-id="82fe8-143">The version of the policy</span></span>|
|<span data-ttu-id="82fe8-144">platformType</span><span class="sxs-lookup"><span data-stu-id="82fe8-144">platformType</span></span>|<span data-ttu-id="82fe8-145">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="82fe8-145">policyPlatformType</span></span>|<span data-ttu-id="82fe8-146">应用该策略的平台类型。</span><span class="sxs-lookup"><span data-stu-id="82fe8-146">Platform type that the policy applies to.</span></span> <span data-ttu-id="82fe8-147">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="82fe8-147">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="82fe8-148">state</span><span class="sxs-lookup"><span data-stu-id="82fe8-148">state</span></span>|<span data-ttu-id="82fe8-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="82fe8-149">complianceStatus</span></span>|<span data-ttu-id="82fe8-150">策略的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="82fe8-150">The compliance state of the policy.</span></span> <span data-ttu-id="82fe8-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="82fe8-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="82fe8-152">settingCount</span><span class="sxs-lookup"><span data-stu-id="82fe8-152">settingCount</span></span>|<span data-ttu-id="82fe8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="82fe8-153">Int32</span></span>|<span data-ttu-id="82fe8-154">策略保留的设置计数</span><span class="sxs-lookup"><span data-stu-id="82fe8-154">Count of how many setting a policy holds</span></span>|
|<span data-ttu-id="82fe8-155">userId</span><span class="sxs-lookup"><span data-stu-id="82fe8-155">userId</span></span>|<span data-ttu-id="82fe8-156">String</span><span class="sxs-lookup"><span data-stu-id="82fe8-156">String</span></span>|<span data-ttu-id="82fe8-157">用户唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="82fe8-157">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="82fe8-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82fe8-158">userPrincipalName</span></span>|<span data-ttu-id="82fe8-159">字符串</span><span class="sxs-lookup"><span data-stu-id="82fe8-159">String</span></span>|<span data-ttu-id="82fe8-160">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="82fe8-160">User Principal Name</span></span>|



## <a name="response"></a><span data-ttu-id="82fe8-161">响应</span><span class="sxs-lookup"><span data-stu-id="82fe8-161">Response</span></span>
<span data-ttu-id="82fe8-162">如果成功，此方法在响应`201 Created`正文中返回响应代码和 managedDeviceMobileAppConfigurationState 对象。</span><span class="sxs-lookup"><span data-stu-id="82fe8-162">If successful, this method returns a `201 Created` response code and a managedDeviceMobileAppConfigurationState object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82fe8-163">示例</span><span class="sxs-lookup"><span data-stu-id="82fe8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="82fe8-164">请求</span><span class="sxs-lookup"><span data-stu-id="82fe8-164">Request</span></span>
<span data-ttu-id="82fe8-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82fe8-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
Content-type: application/json
Content-length: 1093

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="82fe8-166">响应</span><span class="sxs-lookup"><span data-stu-id="82fe8-166">Response</span></span>
<span data-ttu-id="82fe8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82fe8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1142

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "659554f2-54f2-6595-f254-9565f2549565",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "androidForWork",
  "state": "notApplicable",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```



