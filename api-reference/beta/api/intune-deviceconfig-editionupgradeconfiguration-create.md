---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 60694b4aa97b5b57c1dcb5ee15da7ba92350d2a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939453"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="6a659-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a659-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="6a659-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a659-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a659-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a659-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a659-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a659-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a659-107">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a659-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a659-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a659-108">Prerequisites</span></span>
<span data-ttu-id="6a659-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6a659-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a659-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a659-111">Permission type</span></span>|<span data-ttu-id="6a659-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a659-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a659-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a659-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a659-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a659-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a659-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a659-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a659-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a659-116">Not supported.</span></span>|
|<span data-ttu-id="6a659-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a659-117">Application</span></span>|<span data-ttu-id="6a659-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a659-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a659-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a659-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6a659-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a659-120">Request headers</span></span>
|<span data-ttu-id="6a659-121">标头</span><span class="sxs-lookup"><span data-stu-id="6a659-121">Header</span></span>|<span data-ttu-id="6a659-122">值</span><span class="sxs-lookup"><span data-stu-id="6a659-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a659-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a659-123">Authorization</span></span>|<span data-ttu-id="6a659-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a659-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a659-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a659-125">Accept</span></span>|<span data-ttu-id="6a659-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a659-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a659-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a659-127">Request body</span></span>
<span data-ttu-id="6a659-128">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a659-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="6a659-129">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a659-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="6a659-130">属性</span><span class="sxs-lookup"><span data-stu-id="6a659-130">Property</span></span>|<span data-ttu-id="6a659-131">类型</span><span class="sxs-lookup"><span data-stu-id="6a659-131">Type</span></span>|<span data-ttu-id="6a659-132">说明</span><span class="sxs-lookup"><span data-stu-id="6a659-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a659-133">id</span><span class="sxs-lookup"><span data-stu-id="6a659-133">id</span></span>|<span data-ttu-id="6a659-134">String</span><span class="sxs-lookup"><span data-stu-id="6a659-134">String</span></span>|<span data-ttu-id="6a659-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a659-135">Key of the entity.</span></span> <span data-ttu-id="6a659-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a659-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6a659-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a659-138">DateTimeOffset</span></span>|<span data-ttu-id="6a659-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6a659-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6a659-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a659-141">roleScopeTagIds</span></span>|<span data-ttu-id="6a659-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a659-142">String collection</span></span>|<span data-ttu-id="6a659-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6a659-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a659-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a659-145">supportsScopeTags</span></span>|<span data-ttu-id="6a659-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6a659-146">Boolean</span></span>|<span data-ttu-id="6a659-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6a659-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a659-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6a659-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a659-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6a659-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a659-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6a659-150">This property is read-only.</span></span> <span data-ttu-id="6a659-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a659-152">createdDateTime</span></span>|<span data-ttu-id="6a659-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a659-153">DateTimeOffset</span></span>|<span data-ttu-id="6a659-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6a659-154">DateTime the object was created.</span></span> <span data-ttu-id="6a659-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-156">description</span><span class="sxs-lookup"><span data-stu-id="6a659-156">description</span></span>|<span data-ttu-id="6a659-157">String</span><span class="sxs-lookup"><span data-stu-id="6a659-157">String</span></span>|<span data-ttu-id="6a659-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6a659-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a659-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6a659-160">displayName</span></span>|<span data-ttu-id="6a659-161">String</span><span class="sxs-lookup"><span data-stu-id="6a659-161">String</span></span>|<span data-ttu-id="6a659-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6a659-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a659-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-164">version</span><span class="sxs-lookup"><span data-stu-id="6a659-164">version</span></span>|<span data-ttu-id="6a659-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6a659-165">Int32</span></span>|<span data-ttu-id="6a659-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6a659-166">Version of the device configuration.</span></span> <span data-ttu-id="6a659-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a659-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a659-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="6a659-168">licenseType</span></span>|[<span data-ttu-id="6a659-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="6a659-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="6a659-170">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="6a659-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="6a659-171">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="6a659-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="6a659-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="6a659-172">targetEdition</span></span>|[<span data-ttu-id="6a659-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="6a659-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="6a659-174">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="6a659-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="6a659-175">可能的值为： `windows10Enterprise`， `windows10EnterpriseN`， `windows10Education`， `windows10EducationN`， `windows10MobileEnterprise`， `windows10HolographicEnterprise`， `windows10Professional`， `windows10ProfessionalN`， `windows10ProfessionalEducation`， `windows10ProfessionalEducationN`， `windows10ProfessionalWorkstation`， `windows10ProfessionalWorkstationN`， `notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="6a659-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="6a659-176">license</span><span class="sxs-lookup"><span data-stu-id="6a659-176">license</span></span>|<span data-ttu-id="6a659-177">String</span><span class="sxs-lookup"><span data-stu-id="6a659-177">String</span></span>|<span data-ttu-id="6a659-178">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="6a659-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="6a659-179">productKey</span><span class="sxs-lookup"><span data-stu-id="6a659-179">productKey</span></span>|<span data-ttu-id="6a659-180">String</span><span class="sxs-lookup"><span data-stu-id="6a659-180">String</span></span>|<span data-ttu-id="6a659-181">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="6a659-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="6a659-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="6a659-182">windowsSMode</span></span>|[<span data-ttu-id="6a659-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a659-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="6a659-184">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="6a659-184">S mode configuration.</span></span> <span data-ttu-id="6a659-185">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="6a659-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="6a659-186">响应</span><span class="sxs-lookup"><span data-stu-id="6a659-186">Response</span></span>
<span data-ttu-id="6a659-187">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a659-187">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a659-188">示例</span><span class="sxs-lookup"><span data-stu-id="6a659-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a659-189">请求</span><span class="sxs-lookup"><span data-stu-id="6a659-189">Request</span></span>
<span data-ttu-id="6a659-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a659-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6a659-191">响应</span><span class="sxs-lookup"><span data-stu-id="6a659-191">Response</span></span>
<span data-ttu-id="6a659-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a659-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





