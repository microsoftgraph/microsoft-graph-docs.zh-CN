---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45d393cae18a3986508545cc34895ec214ebb370
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979051"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="1d8f6-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d8f6-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="1d8f6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d8f6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d8f6-106">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d8f6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d8f6-107">Prerequisites</span></span>
<span data-ttu-id="1d8f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d8f6-110">Permission type</span></span>|<span data-ttu-id="1d8f6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d8f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d8f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d8f6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8f6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d8f6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d8f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d8f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-115">Not supported.</span></span>|
|<span data-ttu-id="1d8f6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d8f6-116">Application</span></span>|<span data-ttu-id="1d8f6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d8f6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d8f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d8f6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d8f6-119">Request headers</span></span>
|<span data-ttu-id="1d8f6-120">标头</span><span class="sxs-lookup"><span data-stu-id="1d8f6-120">Header</span></span>|<span data-ttu-id="1d8f6-121">值</span><span class="sxs-lookup"><span data-stu-id="1d8f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d8f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8f6-122">Authorization</span></span>|<span data-ttu-id="1d8f6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d8f6-124">接受</span><span class="sxs-lookup"><span data-stu-id="1d8f6-124">Accept</span></span>|<span data-ttu-id="1d8f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d8f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d8f6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d8f6-126">Request body</span></span>
<span data-ttu-id="1d8f6-127">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="1d8f6-128">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="1d8f6-129">属性</span><span class="sxs-lookup"><span data-stu-id="1d8f6-129">Property</span></span>|<span data-ttu-id="1d8f6-130">类型</span><span class="sxs-lookup"><span data-stu-id="1d8f6-130">Type</span></span>|<span data-ttu-id="1d8f6-131">说明</span><span class="sxs-lookup"><span data-stu-id="1d8f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d8f6-132">id</span><span class="sxs-lookup"><span data-stu-id="1d8f6-132">id</span></span>|<span data-ttu-id="1d8f6-133">String</span><span class="sxs-lookup"><span data-stu-id="1d8f6-133">String</span></span>|<span data-ttu-id="1d8f6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-134">Key of the entity.</span></span> <span data-ttu-id="1d8f6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d8f6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d8f6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d8f6-137">DateTimeOffset</span></span>|<span data-ttu-id="1d8f6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d8f6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d8f6-140">roleScopeTagIds</span></span>|<span data-ttu-id="1d8f6-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="1d8f6-141">String collection</span></span>|<span data-ttu-id="1d8f6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d8f6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1d8f6-144">supportsScopeTags</span></span>|<span data-ttu-id="1d8f6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d8f6-145">Boolean</span></span>|<span data-ttu-id="1d8f6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1d8f6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1d8f6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1d8f6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-149">This property is read-only.</span></span> <span data-ttu-id="1d8f6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d8f6-151">createdDateTime</span></span>|<span data-ttu-id="1d8f6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d8f6-152">DateTimeOffset</span></span>|<span data-ttu-id="1d8f6-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-153">DateTime the object was created.</span></span> <span data-ttu-id="1d8f6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-155">description</span><span class="sxs-lookup"><span data-stu-id="1d8f6-155">description</span></span>|<span data-ttu-id="1d8f6-156">String</span><span class="sxs-lookup"><span data-stu-id="1d8f6-156">String</span></span>|<span data-ttu-id="1d8f6-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d8f6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1d8f6-159">displayName</span></span>|<span data-ttu-id="1d8f6-160">String</span><span class="sxs-lookup"><span data-stu-id="1d8f6-160">String</span></span>|<span data-ttu-id="1d8f6-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d8f6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-163">version</span><span class="sxs-lookup"><span data-stu-id="1d8f6-163">version</span></span>|<span data-ttu-id="1d8f6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8f6-164">Int32</span></span>|<span data-ttu-id="1d8f6-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-165">Version of the device configuration.</span></span> <span data-ttu-id="1d8f6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d8f6-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1d8f6-167">isEnabled</span></span>|<span data-ttu-id="1d8f6-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d8f6-168">Boolean</span></span>|<span data-ttu-id="1d8f6-169">在 UI 中是否启用了设置</span><span class="sxs-lookup"><span data-stu-id="1d8f6-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="1d8f6-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="1d8f6-170">activeHoursStart</span></span>|<span data-ttu-id="1d8f6-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1d8f6-171">TimeOfDay</span></span>|<span data-ttu-id="1d8f6-172">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="1d8f6-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="1d8f6-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="1d8f6-173">activeHoursEnd</span></span>|<span data-ttu-id="1d8f6-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1d8f6-174">TimeOfDay</span></span>|<span data-ttu-id="1d8f6-175">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="1d8f6-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="1d8f6-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="1d8f6-176">scheduledInstallDays</span></span>|<span data-ttu-id="1d8f6-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d8f6-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="1d8f6-178">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="1d8f6-179">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1d8f6-180">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1d8f6-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d8f6-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="1d8f6-182">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8f6-182">Int32</span></span>|<span data-ttu-id="1d8f6-183">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="1d8f6-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="1d8f6-184">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="1d8f6-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="1d8f6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1d8f6-185">Int32</span></span>|<span data-ttu-id="1d8f6-186">软件更新在 iOS 设备中可见的天数, 范围从0到 90 (含0到)</span><span class="sxs-lookup"><span data-stu-id="1d8f6-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="1d8f6-187">响应</span><span class="sxs-lookup"><span data-stu-id="1d8f6-187">Response</span></span>
<span data-ttu-id="1d8f6-188">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-188">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d8f6-189">示例</span><span class="sxs-lookup"><span data-stu-id="1d8f6-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d8f6-190">请求</span><span class="sxs-lookup"><span data-stu-id="1d8f6-190">Request</span></span>
<span data-ttu-id="1d8f6-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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

### <a name="response"></a><span data-ttu-id="1d8f6-192">响应</span><span class="sxs-lookup"><span data-stu-id="1d8f6-192">Response</span></span>
<span data-ttu-id="1d8f6-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d8f6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




