---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ac9743f0d94b2f4e273674921aadb9fe2e3ed4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963827"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="93d96-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="93d96-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="93d96-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="93d96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93d96-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="93d96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93d96-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="93d96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93d96-107">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93d96-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93d96-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="93d96-108">Prerequisites</span></span>
<span data-ttu-id="93d96-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="93d96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d96-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="93d96-111">Permission type</span></span>|<span data-ttu-id="93d96-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93d96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93d96-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93d96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93d96-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d96-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93d96-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93d96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93d96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="93d96-116">Not supported.</span></span>|
|<span data-ttu-id="93d96-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="93d96-117">Application</span></span>|<span data-ttu-id="93d96-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="93d96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93d96-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93d96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="93d96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="93d96-120">Request headers</span></span>
|<span data-ttu-id="93d96-121">标头</span><span class="sxs-lookup"><span data-stu-id="93d96-121">Header</span></span>|<span data-ttu-id="93d96-122">值</span><span class="sxs-lookup"><span data-stu-id="93d96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93d96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93d96-123">Authorization</span></span>|<span data-ttu-id="93d96-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93d96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93d96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93d96-125">Accept</span></span>|<span data-ttu-id="93d96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93d96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93d96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93d96-127">Request body</span></span>
<span data-ttu-id="93d96-128">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93d96-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="93d96-129">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93d96-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="93d96-130">属性</span><span class="sxs-lookup"><span data-stu-id="93d96-130">Property</span></span>|<span data-ttu-id="93d96-131">类型</span><span class="sxs-lookup"><span data-stu-id="93d96-131">Type</span></span>|<span data-ttu-id="93d96-132">说明</span><span class="sxs-lookup"><span data-stu-id="93d96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93d96-133">id</span><span class="sxs-lookup"><span data-stu-id="93d96-133">id</span></span>|<span data-ttu-id="93d96-134">String</span><span class="sxs-lookup"><span data-stu-id="93d96-134">String</span></span>|<span data-ttu-id="93d96-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93d96-135">Key of the entity.</span></span> <span data-ttu-id="93d96-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93d96-137">lastModifiedDateTime</span></span>|<span data-ttu-id="93d96-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93d96-138">DateTimeOffset</span></span>|<span data-ttu-id="93d96-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93d96-139">DateTime the object was last modified.</span></span> <span data-ttu-id="93d96-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93d96-141">roleScopeTagIds</span></span>|<span data-ttu-id="93d96-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="93d96-142">String collection</span></span>|<span data-ttu-id="93d96-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="93d96-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93d96-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="93d96-145">supportsScopeTags</span></span>|<span data-ttu-id="93d96-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="93d96-146">Boolean</span></span>|<span data-ttu-id="93d96-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="93d96-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="93d96-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="93d96-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="93d96-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="93d96-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="93d96-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="93d96-150">This property is read-only.</span></span> <span data-ttu-id="93d96-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93d96-152">createdDateTime</span></span>|<span data-ttu-id="93d96-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93d96-153">DateTimeOffset</span></span>|<span data-ttu-id="93d96-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93d96-154">DateTime the object was created.</span></span> <span data-ttu-id="93d96-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-156">description</span><span class="sxs-lookup"><span data-stu-id="93d96-156">description</span></span>|<span data-ttu-id="93d96-157">String</span><span class="sxs-lookup"><span data-stu-id="93d96-157">String</span></span>|<span data-ttu-id="93d96-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="93d96-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93d96-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-160">displayName</span><span class="sxs-lookup"><span data-stu-id="93d96-160">displayName</span></span>|<span data-ttu-id="93d96-161">String</span><span class="sxs-lookup"><span data-stu-id="93d96-161">String</span></span>|<span data-ttu-id="93d96-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="93d96-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93d96-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-164">version</span><span class="sxs-lookup"><span data-stu-id="93d96-164">version</span></span>|<span data-ttu-id="93d96-165">Int32</span><span class="sxs-lookup"><span data-stu-id="93d96-165">Int32</span></span>|<span data-ttu-id="93d96-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="93d96-166">Version of the device configuration.</span></span> <span data-ttu-id="93d96-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93d96-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93d96-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="93d96-168">isEnabled</span></span>|<span data-ttu-id="93d96-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="93d96-169">Boolean</span></span>|<span data-ttu-id="93d96-170">在 UI 中启用设置</span><span class="sxs-lookup"><span data-stu-id="93d96-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="93d96-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="93d96-171">activeHoursStart</span></span>|<span data-ttu-id="93d96-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="93d96-172">TimeOfDay</span></span>|<span data-ttu-id="93d96-173">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="93d96-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="93d96-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="93d96-174">activeHoursEnd</span></span>|<span data-ttu-id="93d96-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="93d96-175">TimeOfDay</span></span>|<span data-ttu-id="93d96-176">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="93d96-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="93d96-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="93d96-177">scheduledInstallDays</span></span>|<span data-ttu-id="93d96-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="93d96-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="93d96-179">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="93d96-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="93d96-180">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="93d96-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="93d96-181">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="93d96-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="93d96-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="93d96-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="93d96-183">Int32</span><span class="sxs-lookup"><span data-stu-id="93d96-183">Int32</span></span>|<span data-ttu-id="93d96-184">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="93d96-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="93d96-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="93d96-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="93d96-186">Int32</span><span class="sxs-lookup"><span data-stu-id="93d96-186">Int32</span></span>|<span data-ttu-id="93d96-187">软件更新之前的天数都能看到介于 0 到 90 非独占的 iOS 设备</span><span class="sxs-lookup"><span data-stu-id="93d96-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="93d96-188">响应</span><span class="sxs-lookup"><span data-stu-id="93d96-188">Response</span></span>
<span data-ttu-id="93d96-189">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93d96-189">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93d96-190">示例</span><span class="sxs-lookup"><span data-stu-id="93d96-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="93d96-191">请求</span><span class="sxs-lookup"><span data-stu-id="93d96-191">Request</span></span>
<span data-ttu-id="93d96-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93d96-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 546

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="93d96-193">响应</span><span class="sxs-lookup"><span data-stu-id="93d96-193">Response</span></span>
<span data-ttu-id="93d96-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93d96-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





