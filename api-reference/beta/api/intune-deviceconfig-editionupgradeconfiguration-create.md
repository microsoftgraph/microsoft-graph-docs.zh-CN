---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67a86f00fb8160d9226de0343b21230977523ef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421240"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="d8e55-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8e55-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="d8e55-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d8e55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8e55-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8e55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8e55-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8e55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e55-107">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8e55-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8e55-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8e55-108">Prerequisites</span></span>
<span data-ttu-id="d8e55-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d8e55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8e55-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8e55-111">Permission type</span></span>|<span data-ttu-id="d8e55-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8e55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e55-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e55-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8e55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e55-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8e55-116">Not supported.</span></span>|
|<span data-ttu-id="d8e55-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8e55-117">Application</span></span>|<span data-ttu-id="d8e55-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8e55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e55-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8e55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8e55-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8e55-120">Request headers</span></span>
|<span data-ttu-id="d8e55-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8e55-121">Header</span></span>|<span data-ttu-id="d8e55-122">值</span><span class="sxs-lookup"><span data-stu-id="d8e55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e55-123">授权</span><span class="sxs-lookup"><span data-stu-id="d8e55-123">Authorization</span></span>|<span data-ttu-id="d8e55-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8e55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8e55-125">Accept</span></span>|<span data-ttu-id="d8e55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e55-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8e55-127">Request body</span></span>
<span data-ttu-id="d8e55-128">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8e55-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="d8e55-129">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8e55-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="d8e55-130">属性</span><span class="sxs-lookup"><span data-stu-id="d8e55-130">Property</span></span>|<span data-ttu-id="d8e55-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8e55-131">Type</span></span>|<span data-ttu-id="d8e55-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8e55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e55-133">id</span><span class="sxs-lookup"><span data-stu-id="d8e55-133">id</span></span>|<span data-ttu-id="d8e55-134">String</span><span class="sxs-lookup"><span data-stu-id="d8e55-134">String</span></span>|<span data-ttu-id="d8e55-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8e55-135">Key of the entity.</span></span> <span data-ttu-id="d8e55-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e55-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d8e55-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e55-138">DateTimeOffset</span></span>|<span data-ttu-id="d8e55-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8e55-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d8e55-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8e55-141">roleScopeTagIds</span></span>|<span data-ttu-id="d8e55-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d8e55-142">String collection</span></span>|<span data-ttu-id="d8e55-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d8e55-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8e55-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8e55-145">supportsScopeTags</span></span>|<span data-ttu-id="d8e55-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e55-146">Boolean</span></span>|<span data-ttu-id="d8e55-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d8e55-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8e55-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d8e55-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8e55-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d8e55-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8e55-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d8e55-150">This property is read-only.</span></span> <span data-ttu-id="d8e55-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e55-152">createdDateTime</span></span>|<span data-ttu-id="d8e55-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e55-153">DateTimeOffset</span></span>|<span data-ttu-id="d8e55-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8e55-154">DateTime the object was created.</span></span> <span data-ttu-id="d8e55-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-156">description</span><span class="sxs-lookup"><span data-stu-id="d8e55-156">description</span></span>|<span data-ttu-id="d8e55-157">String</span><span class="sxs-lookup"><span data-stu-id="d8e55-157">String</span></span>|<span data-ttu-id="d8e55-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d8e55-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8e55-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d8e55-160">displayName</span></span>|<span data-ttu-id="d8e55-161">String</span><span class="sxs-lookup"><span data-stu-id="d8e55-161">String</span></span>|<span data-ttu-id="d8e55-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d8e55-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8e55-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-164">version</span><span class="sxs-lookup"><span data-stu-id="d8e55-164">version</span></span>|<span data-ttu-id="d8e55-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e55-165">Int32</span></span>|<span data-ttu-id="d8e55-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d8e55-166">Version of the device configuration.</span></span> <span data-ttu-id="d8e55-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e55-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e55-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="d8e55-168">licenseType</span></span>|[<span data-ttu-id="d8e55-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="d8e55-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="d8e55-170">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="d8e55-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="d8e55-171">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="d8e55-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="d8e55-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="d8e55-172">targetEdition</span></span>|[<span data-ttu-id="d8e55-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="d8e55-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="d8e55-174">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="d8e55-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="d8e55-175">可能的值为： `windows10Enterprise`， `windows10EnterpriseN`， `windows10Education`， `windows10EducationN`， `windows10MobileEnterprise`， `windows10HolographicEnterprise`， `windows10Professional`， `windows10ProfessionalN`， `windows10ProfessionalEducation`， `windows10ProfessionalEducationN`， `windows10ProfessionalWorkstation`， `windows10ProfessionalWorkstationN`， `notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="d8e55-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="d8e55-176">license</span><span class="sxs-lookup"><span data-stu-id="d8e55-176">license</span></span>|<span data-ttu-id="d8e55-177">String</span><span class="sxs-lookup"><span data-stu-id="d8e55-177">String</span></span>|<span data-ttu-id="d8e55-178">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="d8e55-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="d8e55-179">productKey</span><span class="sxs-lookup"><span data-stu-id="d8e55-179">productKey</span></span>|<span data-ttu-id="d8e55-180">String</span><span class="sxs-lookup"><span data-stu-id="d8e55-180">String</span></span>|<span data-ttu-id="d8e55-181">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="d8e55-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="d8e55-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="d8e55-182">windowsSMode</span></span>|[<span data-ttu-id="d8e55-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8e55-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="d8e55-184">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="d8e55-184">S mode configuration.</span></span> <span data-ttu-id="d8e55-185">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="d8e55-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="d8e55-186">响应</span><span class="sxs-lookup"><span data-stu-id="d8e55-186">Response</span></span>
<span data-ttu-id="d8e55-187">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8e55-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e55-188">示例</span><span class="sxs-lookup"><span data-stu-id="d8e55-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8e55-189">请求</span><span class="sxs-lookup"><span data-stu-id="d8e55-189">Request</span></span>
<span data-ttu-id="d8e55-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8e55-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8e55-191">响应</span><span class="sxs-lookup"><span data-stu-id="d8e55-191">Response</span></span>
<span data-ttu-id="d8e55-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8e55-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




