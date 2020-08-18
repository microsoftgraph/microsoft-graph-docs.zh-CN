---
title: 创建 securityConfigurationTask
description: 创建新的 securityConfigurationTask 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a145aed3721a869fb3cf716d6e3fa799a3efa3d2
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793222"
---
# <a name="create-securityconfigurationtask"></a><span data-ttu-id="3f306-103">创建 securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="3f306-103">Create securityConfigurationTask</span></span>

<span data-ttu-id="3f306-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f306-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f306-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f306-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f306-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f306-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f306-107">创建新的 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f306-107">Create a new [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f306-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f306-108">Prerequisites</span></span>
<span data-ttu-id="3f306-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f306-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f306-111">Permission type</span></span>|<span data-ttu-id="3f306-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f306-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f306-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f306-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f306-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f306-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3f306-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f306-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f306-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f306-116">Not supported.</span></span>|
|<span data-ttu-id="3f306-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f306-117">Application</span></span>|<span data-ttu-id="3f306-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f306-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f306-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f306-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="3f306-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f306-120">Request headers</span></span>
|<span data-ttu-id="3f306-121">标头</span><span class="sxs-lookup"><span data-stu-id="3f306-121">Header</span></span>|<span data-ttu-id="3f306-122">值</span><span class="sxs-lookup"><span data-stu-id="3f306-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f306-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f306-123">Authorization</span></span>|<span data-ttu-id="3f306-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f306-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f306-125">接受</span><span class="sxs-lookup"><span data-stu-id="3f306-125">Accept</span></span>|<span data-ttu-id="3f306-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f306-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f306-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f306-127">Request body</span></span>
<span data-ttu-id="3f306-128">在请求正文中，提供 securityConfigurationTask 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f306-128">In the request body, supply a JSON representation for the securityConfigurationTask object.</span></span>

<span data-ttu-id="3f306-129">下表显示创建 securityConfigurationTask 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3f306-129">The following table shows the properties that are required when you create the securityConfigurationTask.</span></span>

|<span data-ttu-id="3f306-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f306-130">Property</span></span>|<span data-ttu-id="3f306-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f306-131">Type</span></span>|<span data-ttu-id="3f306-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f306-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f306-133">id</span><span class="sxs-lookup"><span data-stu-id="3f306-133">id</span></span>|<span data-ttu-id="3f306-134">String</span><span class="sxs-lookup"><span data-stu-id="3f306-134">String</span></span>|<span data-ttu-id="3f306-135">实体键。</span><span class="sxs-lookup"><span data-stu-id="3f306-135">The entity key.</span></span> <span data-ttu-id="3f306-136">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3f306-137">displayName</span></span>|<span data-ttu-id="3f306-138">String</span><span class="sxs-lookup"><span data-stu-id="3f306-138">String</span></span>|<span data-ttu-id="3f306-139">名称。</span><span class="sxs-lookup"><span data-stu-id="3f306-139">The name.</span></span> <span data-ttu-id="3f306-140">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-141">description</span><span class="sxs-lookup"><span data-stu-id="3f306-141">description</span></span>|<span data-ttu-id="3f306-142">String</span><span class="sxs-lookup"><span data-stu-id="3f306-142">String</span></span>|<span data-ttu-id="3f306-143">说明。</span><span class="sxs-lookup"><span data-stu-id="3f306-143">The description.</span></span> <span data-ttu-id="3f306-144">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f306-145">createdDateTime</span></span>|<span data-ttu-id="3f306-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f306-146">DateTimeOffset</span></span>|<span data-ttu-id="3f306-147">创建日期。</span><span class="sxs-lookup"><span data-stu-id="3f306-147">The created date.</span></span> <span data-ttu-id="3f306-148">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="3f306-149">dueDateTime</span></span>|<span data-ttu-id="3f306-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f306-150">DateTimeOffset</span></span>|<span data-ttu-id="3f306-151">到期日期。</span><span class="sxs-lookup"><span data-stu-id="3f306-151">The due date.</span></span> <span data-ttu-id="3f306-152">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-153">“类别”</span><span class="sxs-lookup"><span data-stu-id="3f306-153">category</span></span>|[<span data-ttu-id="3f306-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="3f306-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="3f306-155">类别。</span><span class="sxs-lookup"><span data-stu-id="3f306-155">The category.</span></span> <span data-ttu-id="3f306-156">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="3f306-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3f306-157">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="3f306-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="3f306-158">priority</span><span class="sxs-lookup"><span data-stu-id="3f306-158">priority</span></span>|[<span data-ttu-id="3f306-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="3f306-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="3f306-160">优先级。</span><span class="sxs-lookup"><span data-stu-id="3f306-160">The priority.</span></span> <span data-ttu-id="3f306-161">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="3f306-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3f306-162">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="3f306-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="3f306-163">创建</span><span class="sxs-lookup"><span data-stu-id="3f306-163">creator</span></span>|<span data-ttu-id="3f306-164">String</span><span class="sxs-lookup"><span data-stu-id="3f306-164">String</span></span>|<span data-ttu-id="3f306-165">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3f306-165">The email address of the creator.</span></span> <span data-ttu-id="3f306-166">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="3f306-167">creatorNotes</span></span>|<span data-ttu-id="3f306-168">String</span><span class="sxs-lookup"><span data-stu-id="3f306-168">String</span></span>|<span data-ttu-id="3f306-169">来自创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="3f306-169">Notes from the creator.</span></span> <span data-ttu-id="3f306-170">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3f306-171">assignedTo</span></span>|<span data-ttu-id="3f306-172">String</span><span class="sxs-lookup"><span data-stu-id="3f306-172">String</span></span>|<span data-ttu-id="3f306-173">将此任务分配到的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3f306-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="3f306-174">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3f306-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3f306-175">status</span><span class="sxs-lookup"><span data-stu-id="3f306-175">status</span></span>|[<span data-ttu-id="3f306-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="3f306-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="3f306-177">状态。</span><span class="sxs-lookup"><span data-stu-id="3f306-177">The status.</span></span> <span data-ttu-id="3f306-178">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="3f306-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3f306-179">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="3f306-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="3f306-180">endpointSecurityPolicy</span><span class="sxs-lookup"><span data-stu-id="3f306-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="3f306-181">endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="3f306-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="3f306-182">终结点安全策略类型。</span><span class="sxs-lookup"><span data-stu-id="3f306-182">The endpoint security policy type.</span></span> <span data-ttu-id="3f306-183">可取值为：`unknown`、`antivirus`、`diskEncryption`、`firewall`、`endpointDetectionAndResponse`、`attackSurfaceReduction` 或 `accountProtection`。</span><span class="sxs-lookup"><span data-stu-id="3f306-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="3f306-184">applicablePlatform</span><span class="sxs-lookup"><span data-stu-id="3f306-184">applicablePlatform</span></span>|[<span data-ttu-id="3f306-185">endpointSecurityConfigurationApplicablePlatform</span><span class="sxs-lookup"><span data-stu-id="3f306-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="3f306-186">适用的平台。</span><span class="sxs-lookup"><span data-stu-id="3f306-186">The applicable platform.</span></span> <span data-ttu-id="3f306-187">可取值为：`unknown`、`macOS`、`windows10AndLater`、`windows10AndWindowsServer`。</span><span class="sxs-lookup"><span data-stu-id="3f306-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="3f306-188">endpointSecurityPolicyProfile</span><span class="sxs-lookup"><span data-stu-id="3f306-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="3f306-189">endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="3f306-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="3f306-190">终结点安全策略配置文件。</span><span class="sxs-lookup"><span data-stu-id="3f306-190">The endpoint security policy profile.</span></span> <span data-ttu-id="3f306-191">可能的值为：、、、、、、、、、、、、、、 `unknown` `antivirus` `windowsSecurity` `bitLocker` `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` 。</span><span class="sxs-lookup"><span data-stu-id="3f306-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="3f306-192">insights</span><span class="sxs-lookup"><span data-stu-id="3f306-192">insights</span></span>|<span data-ttu-id="3f306-193">String</span><span class="sxs-lookup"><span data-stu-id="3f306-193">String</span></span>|<span data-ttu-id="3f306-194">有关缓解措施的信息。</span><span class="sxs-lookup"><span data-stu-id="3f306-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="3f306-195">managedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f306-195">managedDeviceCount</span></span>|<span data-ttu-id="3f306-196">Int32</span><span class="sxs-lookup"><span data-stu-id="3f306-196">Int32</span></span>|<span data-ttu-id="3f306-197">易受攻击设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3f306-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="3f306-198">intendedSettings</span><span class="sxs-lookup"><span data-stu-id="3f306-198">intendedSettings</span></span>|<span data-ttu-id="3f306-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f306-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3f306-200">预期的设置及其值。</span><span class="sxs-lookup"><span data-stu-id="3f306-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="3f306-201">响应</span><span class="sxs-lookup"><span data-stu-id="3f306-201">Response</span></span>
<span data-ttu-id="3f306-202">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f306-202">If successful, this method returns a `201 Created` response code and a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f306-203">示例</span><span class="sxs-lookup"><span data-stu-id="3f306-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f306-204">请求</span><span class="sxs-lookup"><span data-stu-id="3f306-204">Request</span></span>
<span data-ttu-id="3f306-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f306-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3f306-206">响应</span><span class="sxs-lookup"><span data-stu-id="3f306-206">Response</span></span>
<span data-ttu-id="3f306-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f306-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "5d630f12-0f12-5d63-120f-635d120f635d",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```



