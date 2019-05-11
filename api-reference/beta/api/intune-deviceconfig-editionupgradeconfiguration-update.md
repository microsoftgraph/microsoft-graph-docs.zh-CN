---
title: 更新 editionUpgradeConfiguration
description: 更新 editionUpgradeConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 132d8614026dbd582f3e5d7b5090b46748c62b30
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33926775"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="d8020-103">更新 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8020-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="d8020-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8020-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8020-106">更新 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8020-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8020-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8020-107">Prerequisites</span></span>
<span data-ttu-id="d8020-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8020-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8020-110">Permission type</span></span>|<span data-ttu-id="d8020-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8020-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8020-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8020-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8020-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8020-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8020-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8020-115">Not supported.</span></span>|
|<span data-ttu-id="d8020-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8020-116">Application</span></span>|<span data-ttu-id="d8020-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8020-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8020-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8020-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8020-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8020-119">Request headers</span></span>
|<span data-ttu-id="d8020-120">标头</span><span class="sxs-lookup"><span data-stu-id="d8020-120">Header</span></span>|<span data-ttu-id="d8020-121">值</span><span class="sxs-lookup"><span data-stu-id="d8020-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8020-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8020-122">Authorization</span></span>|<span data-ttu-id="d8020-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8020-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8020-124">接受</span><span class="sxs-lookup"><span data-stu-id="d8020-124">Accept</span></span>|<span data-ttu-id="d8020-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8020-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8020-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8020-126">Request body</span></span>
<span data-ttu-id="d8020-127">在请求正文中，提供 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8020-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="d8020-128">下表显示创建 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8020-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="d8020-129">属性</span><span class="sxs-lookup"><span data-stu-id="d8020-129">Property</span></span>|<span data-ttu-id="d8020-130">类型</span><span class="sxs-lookup"><span data-stu-id="d8020-130">Type</span></span>|<span data-ttu-id="d8020-131">说明</span><span class="sxs-lookup"><span data-stu-id="d8020-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8020-132">id</span><span class="sxs-lookup"><span data-stu-id="d8020-132">id</span></span>|<span data-ttu-id="d8020-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d8020-133">String</span></span>|<span data-ttu-id="d8020-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8020-134">Key of the entity.</span></span> <span data-ttu-id="d8020-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8020-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d8020-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8020-137">DateTimeOffset</span></span>|<span data-ttu-id="d8020-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8020-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d8020-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8020-140">roleScopeTagIds</span></span>|<span data-ttu-id="d8020-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d8020-141">String collection</span></span>|<span data-ttu-id="d8020-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d8020-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8020-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8020-144">supportsScopeTags</span></span>|<span data-ttu-id="d8020-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8020-145">Boolean</span></span>|<span data-ttu-id="d8020-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d8020-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8020-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d8020-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8020-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d8020-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8020-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d8020-149">This property is read-only.</span></span> <span data-ttu-id="d8020-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8020-151">createdDateTime</span></span>|<span data-ttu-id="d8020-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8020-152">DateTimeOffset</span></span>|<span data-ttu-id="d8020-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8020-153">DateTime the object was created.</span></span> <span data-ttu-id="d8020-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-155">说明</span><span class="sxs-lookup"><span data-stu-id="d8020-155">description</span></span>|<span data-ttu-id="d8020-156">String</span><span class="sxs-lookup"><span data-stu-id="d8020-156">String</span></span>|<span data-ttu-id="d8020-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d8020-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8020-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d8020-159">displayName</span></span>|<span data-ttu-id="d8020-160">String</span><span class="sxs-lookup"><span data-stu-id="d8020-160">String</span></span>|<span data-ttu-id="d8020-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d8020-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8020-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-163">version</span><span class="sxs-lookup"><span data-stu-id="d8020-163">version</span></span>|<span data-ttu-id="d8020-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d8020-164">Int32</span></span>|<span data-ttu-id="d8020-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d8020-165">Version of the device configuration.</span></span> <span data-ttu-id="d8020-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8020-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8020-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="d8020-167">licenseType</span></span>|[<span data-ttu-id="d8020-168">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="d8020-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="d8020-169">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="d8020-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="d8020-170">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="d8020-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="d8020-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="d8020-171">targetEdition</span></span>|[<span data-ttu-id="d8020-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="d8020-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="d8020-173">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="d8020-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="d8020-174">可能的值是：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="d8020-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="d8020-175">license</span><span class="sxs-lookup"><span data-stu-id="d8020-175">license</span></span>|<span data-ttu-id="d8020-176">String</span><span class="sxs-lookup"><span data-stu-id="d8020-176">String</span></span>|<span data-ttu-id="d8020-177">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="d8020-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="d8020-178">productKey</span><span class="sxs-lookup"><span data-stu-id="d8020-178">productKey</span></span>|<span data-ttu-id="d8020-179">String</span><span class="sxs-lookup"><span data-stu-id="d8020-179">String</span></span>|<span data-ttu-id="d8020-180">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="d8020-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="d8020-181">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="d8020-181">windowsSMode</span></span>|[<span data-ttu-id="d8020-182">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8020-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="d8020-183">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="d8020-183">S mode configuration.</span></span> <span data-ttu-id="d8020-184">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="d8020-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="d8020-185">响应</span><span class="sxs-lookup"><span data-stu-id="d8020-185">Response</span></span>
<span data-ttu-id="d8020-186">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8020-186">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8020-187">示例</span><span class="sxs-lookup"><span data-stu-id="d8020-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8020-188">请求</span><span class="sxs-lookup"><span data-stu-id="d8020-188">Request</span></span>
<span data-ttu-id="d8020-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8020-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="d8020-190">响应</span><span class="sxs-lookup"><span data-stu-id="d8020-190">Response</span></span>
<span data-ttu-id="d8020-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8020-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```




