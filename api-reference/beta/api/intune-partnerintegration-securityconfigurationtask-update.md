---
title: 更新 securityConfigurationTask
description: 更新 securityConfigurationTask 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79916ea63344b5e8f1f4f2ecf9ed55aef904b0ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709206"
---
# <a name="update-securityconfigurationtask"></a><span data-ttu-id="73aa9-103">更新 securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="73aa9-103">Update securityConfigurationTask</span></span>

<span data-ttu-id="73aa9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73aa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73aa9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73aa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73aa9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73aa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73aa9-107">更新 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73aa9-107">Update the properties of a [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73aa9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="73aa9-108">Prerequisites</span></span>
<span data-ttu-id="73aa9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73aa9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="73aa9-111">Permission type</span></span>|<span data-ttu-id="73aa9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73aa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73aa9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73aa9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73aa9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73aa9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73aa9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73aa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73aa9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73aa9-116">Not supported.</span></span>|
|<span data-ttu-id="73aa9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="73aa9-117">Application</span></span>|<span data-ttu-id="73aa9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73aa9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73aa9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73aa9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="73aa9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73aa9-120">Request headers</span></span>
|<span data-ttu-id="73aa9-121">标头</span><span class="sxs-lookup"><span data-stu-id="73aa9-121">Header</span></span>|<span data-ttu-id="73aa9-122">值</span><span class="sxs-lookup"><span data-stu-id="73aa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73aa9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73aa9-123">Authorization</span></span>|<span data-ttu-id="73aa9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73aa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73aa9-125">接受</span><span class="sxs-lookup"><span data-stu-id="73aa9-125">Accept</span></span>|<span data-ttu-id="73aa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73aa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73aa9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73aa9-127">Request body</span></span>
<span data-ttu-id="73aa9-128">在请求正文中，提供 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73aa9-128">In the request body, supply a JSON representation for the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

<span data-ttu-id="73aa9-129">下表显示创建 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73aa9-129">The following table shows the properties that are required when you create the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).</span></span>

|<span data-ttu-id="73aa9-130">属性</span><span class="sxs-lookup"><span data-stu-id="73aa9-130">Property</span></span>|<span data-ttu-id="73aa9-131">类型</span><span class="sxs-lookup"><span data-stu-id="73aa9-131">Type</span></span>|<span data-ttu-id="73aa9-132">说明</span><span class="sxs-lookup"><span data-stu-id="73aa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73aa9-133">id</span><span class="sxs-lookup"><span data-stu-id="73aa9-133">id</span></span>|<span data-ttu-id="73aa9-134">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-134">String</span></span>|<span data-ttu-id="73aa9-135">实体键。</span><span class="sxs-lookup"><span data-stu-id="73aa9-135">The entity key.</span></span> <span data-ttu-id="73aa9-136">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="73aa9-137">displayName</span></span>|<span data-ttu-id="73aa9-138">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-138">String</span></span>|<span data-ttu-id="73aa9-139">名称。</span><span class="sxs-lookup"><span data-stu-id="73aa9-139">The name.</span></span> <span data-ttu-id="73aa9-140">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-141">说明</span><span class="sxs-lookup"><span data-stu-id="73aa9-141">description</span></span>|<span data-ttu-id="73aa9-142">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-142">String</span></span>|<span data-ttu-id="73aa9-143">说明。</span><span class="sxs-lookup"><span data-stu-id="73aa9-143">The description.</span></span> <span data-ttu-id="73aa9-144">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73aa9-145">createdDateTime</span></span>|<span data-ttu-id="73aa9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73aa9-146">DateTimeOffset</span></span>|<span data-ttu-id="73aa9-147">创建日期。</span><span class="sxs-lookup"><span data-stu-id="73aa9-147">The created date.</span></span> <span data-ttu-id="73aa9-148">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="73aa9-149">dueDateTime</span></span>|<span data-ttu-id="73aa9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73aa9-150">DateTimeOffset</span></span>|<span data-ttu-id="73aa9-151">到期日期。</span><span class="sxs-lookup"><span data-stu-id="73aa9-151">The due date.</span></span> <span data-ttu-id="73aa9-152">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-153">“类别”</span><span class="sxs-lookup"><span data-stu-id="73aa9-153">category</span></span>|[<span data-ttu-id="73aa9-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="73aa9-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="73aa9-155">类别。</span><span class="sxs-lookup"><span data-stu-id="73aa9-155">The category.</span></span> <span data-ttu-id="73aa9-156">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="73aa9-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="73aa9-157">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="73aa9-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="73aa9-158">priority</span><span class="sxs-lookup"><span data-stu-id="73aa9-158">priority</span></span>|[<span data-ttu-id="73aa9-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="73aa9-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="73aa9-160">优先级。</span><span class="sxs-lookup"><span data-stu-id="73aa9-160">The priority.</span></span> <span data-ttu-id="73aa9-161">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="73aa9-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="73aa9-162">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="73aa9-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="73aa9-163">Creator</span><span class="sxs-lookup"><span data-stu-id="73aa9-163">creator</span></span>|<span data-ttu-id="73aa9-164">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-164">String</span></span>|<span data-ttu-id="73aa9-165">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="73aa9-165">The email address of the creator.</span></span> <span data-ttu-id="73aa9-166">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="73aa9-167">creatorNotes</span></span>|<span data-ttu-id="73aa9-168">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-168">String</span></span>|<span data-ttu-id="73aa9-169">来自创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="73aa9-169">Notes from the creator.</span></span> <span data-ttu-id="73aa9-170">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="73aa9-171">assignedTo</span></span>|<span data-ttu-id="73aa9-172">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-172">String</span></span>|<span data-ttu-id="73aa9-173">将此任务分配到的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="73aa9-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="73aa9-174">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="73aa9-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="73aa9-175">status</span><span class="sxs-lookup"><span data-stu-id="73aa9-175">status</span></span>|[<span data-ttu-id="73aa9-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="73aa9-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="73aa9-177">状态。</span><span class="sxs-lookup"><span data-stu-id="73aa9-177">The status.</span></span> <span data-ttu-id="73aa9-178">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="73aa9-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="73aa9-179">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="73aa9-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="73aa9-180">endpointSecurityPolicy</span><span class="sxs-lookup"><span data-stu-id="73aa9-180">endpointSecurityPolicy</span></span>|[<span data-ttu-id="73aa9-181">endpointSecurityConfigurationType</span><span class="sxs-lookup"><span data-stu-id="73aa9-181">endpointSecurityConfigurationType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|<span data-ttu-id="73aa9-182">终结点安全策略类型。</span><span class="sxs-lookup"><span data-stu-id="73aa9-182">The endpoint security policy type.</span></span> <span data-ttu-id="73aa9-183">可取值为：`unknown`、`antivirus`、`diskEncryption`、`firewall`、`endpointDetectionAndResponse`、`attackSurfaceReduction` 或 `accountProtection`。</span><span class="sxs-lookup"><span data-stu-id="73aa9-183">Possible values are: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.</span></span>|
|<span data-ttu-id="73aa9-184">applicablePlatform</span><span class="sxs-lookup"><span data-stu-id="73aa9-184">applicablePlatform</span></span>|[<span data-ttu-id="73aa9-185">endpointSecurityConfigurationApplicablePlatform</span><span class="sxs-lookup"><span data-stu-id="73aa9-185">endpointSecurityConfigurationApplicablePlatform</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|<span data-ttu-id="73aa9-186">适用的平台。</span><span class="sxs-lookup"><span data-stu-id="73aa9-186">The applicable platform.</span></span> <span data-ttu-id="73aa9-187">可取值为：`unknown`、`macOS`、`windows10AndLater`、`windows10AndWindowsServer`。</span><span class="sxs-lookup"><span data-stu-id="73aa9-187">Possible values are: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.</span></span>|
|<span data-ttu-id="73aa9-188">endpointSecurityPolicyProfile</span><span class="sxs-lookup"><span data-stu-id="73aa9-188">endpointSecurityPolicyProfile</span></span>|[<span data-ttu-id="73aa9-189">endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="73aa9-189">endpointSecurityConfigurationProfileType</span></span>](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|<span data-ttu-id="73aa9-190">终结点安全策略配置文件。</span><span class="sxs-lookup"><span data-stu-id="73aa9-190">The endpoint security policy profile.</span></span> <span data-ttu-id="73aa9-191">可能的值为：、、、、、、、、、、、、、、 `unknown` `antivirus` `windowsSecurity` `bitLocker` `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` 。</span><span class="sxs-lookup"><span data-stu-id="73aa9-191">Possible values are: `unknown`, `antivirus`, `windowsSecurity`, `bitLocker`, `fileVault`, `firewall`, `firewallRules`, `endpointDetectionAndResponse`, `deviceControl`, `appAndBrowserIsolation`, `exploitProtection`, `webProtection`, `applicationControl`, `attackSurfaceReductionRules`, `accountProtection`.</span></span>|
|<span data-ttu-id="73aa9-192">insights</span><span class="sxs-lookup"><span data-stu-id="73aa9-192">insights</span></span>|<span data-ttu-id="73aa9-193">String</span><span class="sxs-lookup"><span data-stu-id="73aa9-193">String</span></span>|<span data-ttu-id="73aa9-194">有关缓解措施的信息。</span><span class="sxs-lookup"><span data-stu-id="73aa9-194">Information about the mitigation.</span></span>|
|<span data-ttu-id="73aa9-195">managedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73aa9-195">managedDeviceCount</span></span>|<span data-ttu-id="73aa9-196">Int32</span><span class="sxs-lookup"><span data-stu-id="73aa9-196">Int32</span></span>|<span data-ttu-id="73aa9-197">易受攻击设备的数量。</span><span class="sxs-lookup"><span data-stu-id="73aa9-197">The number of vulnerable devices.</span></span>|
|<span data-ttu-id="73aa9-198">intendedSettings</span><span class="sxs-lookup"><span data-stu-id="73aa9-198">intendedSettings</span></span>|<span data-ttu-id="73aa9-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73aa9-199">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="73aa9-200">预期的设置及其值。</span><span class="sxs-lookup"><span data-stu-id="73aa9-200">The intended settings and their values.</span></span>|



## <a name="response"></a><span data-ttu-id="73aa9-201">响应</span><span class="sxs-lookup"><span data-stu-id="73aa9-201">Response</span></span>
<span data-ttu-id="73aa9-202">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73aa9-202">If successful, this method returns a `200 OK` response code and an updated [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73aa9-203">示例</span><span class="sxs-lookup"><span data-stu-id="73aa9-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="73aa9-204">请求</span><span class="sxs-lookup"><span data-stu-id="73aa9-204">Request</span></span>
<span data-ttu-id="73aa9-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73aa9-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
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

### <a name="response"></a><span data-ttu-id="73aa9-206">响应</span><span class="sxs-lookup"><span data-stu-id="73aa9-206">Response</span></span>
<span data-ttu-id="73aa9-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73aa9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





