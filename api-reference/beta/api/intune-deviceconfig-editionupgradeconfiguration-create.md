---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e18b8d9438da649cec250063913afffb47db1bf2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974424"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="fa849-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa849-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="fa849-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa849-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa849-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa849-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa849-106">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa849-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa849-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa849-107">Prerequisites</span></span>
<span data-ttu-id="fa849-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa849-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa849-110">Permission type</span></span>|<span data-ttu-id="fa849-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa849-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa849-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa849-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa849-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa849-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa849-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa849-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa849-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa849-115">Not supported.</span></span>|
|<span data-ttu-id="fa849-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa849-116">Application</span></span>|<span data-ttu-id="fa849-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa849-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa849-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa849-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa849-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa849-119">Request headers</span></span>
|<span data-ttu-id="fa849-120">标头</span><span class="sxs-lookup"><span data-stu-id="fa849-120">Header</span></span>|<span data-ttu-id="fa849-121">值</span><span class="sxs-lookup"><span data-stu-id="fa849-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa849-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa849-122">Authorization</span></span>|<span data-ttu-id="fa849-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa849-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa849-124">接受</span><span class="sxs-lookup"><span data-stu-id="fa849-124">Accept</span></span>|<span data-ttu-id="fa849-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa849-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa849-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa849-126">Request body</span></span>
<span data-ttu-id="fa849-127">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa849-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="fa849-128">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa849-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="fa849-129">属性</span><span class="sxs-lookup"><span data-stu-id="fa849-129">Property</span></span>|<span data-ttu-id="fa849-130">类型</span><span class="sxs-lookup"><span data-stu-id="fa849-130">Type</span></span>|<span data-ttu-id="fa849-131">说明</span><span class="sxs-lookup"><span data-stu-id="fa849-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa849-132">id</span><span class="sxs-lookup"><span data-stu-id="fa849-132">id</span></span>|<span data-ttu-id="fa849-133">String</span><span class="sxs-lookup"><span data-stu-id="fa849-133">String</span></span>|<span data-ttu-id="fa849-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa849-134">Key of the entity.</span></span> <span data-ttu-id="fa849-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa849-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fa849-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa849-137">DateTimeOffset</span></span>|<span data-ttu-id="fa849-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fa849-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fa849-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa849-140">roleScopeTagIds</span></span>|<span data-ttu-id="fa849-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="fa849-141">String collection</span></span>|<span data-ttu-id="fa849-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fa849-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa849-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fa849-144">supportsScopeTags</span></span>|<span data-ttu-id="fa849-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa849-145">Boolean</span></span>|<span data-ttu-id="fa849-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fa849-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fa849-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fa849-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fa849-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fa849-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fa849-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fa849-149">This property is read-only.</span></span> <span data-ttu-id="fa849-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa849-151">createdDateTime</span></span>|<span data-ttu-id="fa849-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa849-152">DateTimeOffset</span></span>|<span data-ttu-id="fa849-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fa849-153">DateTime the object was created.</span></span> <span data-ttu-id="fa849-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-155">description</span><span class="sxs-lookup"><span data-stu-id="fa849-155">description</span></span>|<span data-ttu-id="fa849-156">String</span><span class="sxs-lookup"><span data-stu-id="fa849-156">String</span></span>|<span data-ttu-id="fa849-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fa849-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa849-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fa849-159">displayName</span></span>|<span data-ttu-id="fa849-160">String</span><span class="sxs-lookup"><span data-stu-id="fa849-160">String</span></span>|<span data-ttu-id="fa849-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fa849-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa849-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-163">version</span><span class="sxs-lookup"><span data-stu-id="fa849-163">version</span></span>|<span data-ttu-id="fa849-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fa849-164">Int32</span></span>|<span data-ttu-id="fa849-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fa849-165">Version of the device configuration.</span></span> <span data-ttu-id="fa849-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa849-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa849-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="fa849-167">licenseType</span></span>|[<span data-ttu-id="fa849-168">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="fa849-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="fa849-169">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="fa849-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="fa849-170">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="fa849-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="fa849-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="fa849-171">targetEdition</span></span>|[<span data-ttu-id="fa849-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="fa849-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="fa849-173">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="fa849-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="fa849-174">可能的值是：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="fa849-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="fa849-175">license</span><span class="sxs-lookup"><span data-stu-id="fa849-175">license</span></span>|<span data-ttu-id="fa849-176">String</span><span class="sxs-lookup"><span data-stu-id="fa849-176">String</span></span>|<span data-ttu-id="fa849-177">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="fa849-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="fa849-178">productKey</span><span class="sxs-lookup"><span data-stu-id="fa849-178">productKey</span></span>|<span data-ttu-id="fa849-179">String</span><span class="sxs-lookup"><span data-stu-id="fa849-179">String</span></span>|<span data-ttu-id="fa849-180">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="fa849-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="fa849-181">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="fa849-181">windowsSMode</span></span>|[<span data-ttu-id="fa849-182">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa849-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="fa849-183">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="fa849-183">S mode configuration.</span></span> <span data-ttu-id="fa849-184">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="fa849-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="fa849-185">响应</span><span class="sxs-lookup"><span data-stu-id="fa849-185">Response</span></span>
<span data-ttu-id="fa849-186">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa849-186">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa849-187">示例</span><span class="sxs-lookup"><span data-stu-id="fa849-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa849-188">请求</span><span class="sxs-lookup"><span data-stu-id="fa849-188">Request</span></span>
<span data-ttu-id="fa849-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa849-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fa849-190">响应</span><span class="sxs-lookup"><span data-stu-id="fa849-190">Response</span></span>
<span data-ttu-id="fa849-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa849-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




