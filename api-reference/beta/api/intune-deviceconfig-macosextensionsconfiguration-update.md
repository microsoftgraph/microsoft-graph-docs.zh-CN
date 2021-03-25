---
title: 更新 macOSExtensionsConfiguration
description: 更新 macOSExtensionsConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6deff87a77cff0c3c5581223b5f85b10d93b9856
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151149"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="01d98-103">更新 macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="01d98-103">Update macOSExtensionsConfiguration</span></span>

<span data-ttu-id="01d98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01d98-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01d98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01d98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d98-107">更新 [macOSExtensionsConfiguration 对象](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="01d98-107">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01d98-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="01d98-108">Prerequisites</span></span>
<span data-ttu-id="01d98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01d98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="01d98-111">Permission type</span></span>|<span data-ttu-id="01d98-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01d98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01d98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01d98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01d98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01d98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="01d98-116">Not supported.</span></span>|
|<span data-ttu-id="01d98-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="01d98-117">Application</span></span>|<span data-ttu-id="01d98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01d98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="01d98-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="01d98-120">Request headers</span></span>
|<span data-ttu-id="01d98-121">标头</span><span class="sxs-lookup"><span data-stu-id="01d98-121">Header</span></span>|<span data-ttu-id="01d98-122">值</span><span class="sxs-lookup"><span data-stu-id="01d98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01d98-123">Authorization</span></span>|<span data-ttu-id="01d98-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01d98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d98-125">接受</span><span class="sxs-lookup"><span data-stu-id="01d98-125">Accept</span></span>|<span data-ttu-id="01d98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01d98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d98-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01d98-127">Request body</span></span>
<span data-ttu-id="01d98-128">在请求正文中，提供 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01d98-128">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="01d98-129">下表显示创建 [macOSExtensionsConfiguration 时所需的属性](../resources/intune-deviceconfig-macosextensionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="01d98-129">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="01d98-130">属性</span><span class="sxs-lookup"><span data-stu-id="01d98-130">Property</span></span>|<span data-ttu-id="01d98-131">类型</span><span class="sxs-lookup"><span data-stu-id="01d98-131">Type</span></span>|<span data-ttu-id="01d98-132">说明</span><span class="sxs-lookup"><span data-stu-id="01d98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d98-133">id</span><span class="sxs-lookup"><span data-stu-id="01d98-133">id</span></span>|<span data-ttu-id="01d98-134">String</span><span class="sxs-lookup"><span data-stu-id="01d98-134">String</span></span>|<span data-ttu-id="01d98-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="01d98-135">Key of the entity.</span></span> <span data-ttu-id="01d98-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d98-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01d98-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d98-138">DateTimeOffset</span></span>|<span data-ttu-id="01d98-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01d98-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01d98-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01d98-141">roleScopeTagIds</span></span>|<span data-ttu-id="01d98-142">String collection</span><span class="sxs-lookup"><span data-stu-id="01d98-142">String collection</span></span>|<span data-ttu-id="01d98-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="01d98-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01d98-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01d98-145">supportsScopeTags</span></span>|<span data-ttu-id="01d98-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d98-146">Boolean</span></span>|<span data-ttu-id="01d98-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="01d98-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01d98-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="01d98-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01d98-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="01d98-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01d98-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="01d98-150">This property is read-only.</span></span> <span data-ttu-id="01d98-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01d98-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="01d98-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01d98-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="01d98-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="01d98-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="01d98-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01d98-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="01d98-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01d98-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="01d98-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="01d98-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="01d98-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="01d98-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="01d98-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="01d98-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="01d98-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="01d98-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="01d98-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01d98-164">createdDateTime</span></span>|<span data-ttu-id="01d98-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d98-165">DateTimeOffset</span></span>|<span data-ttu-id="01d98-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01d98-166">DateTime the object was created.</span></span> <span data-ttu-id="01d98-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-168">说明</span><span class="sxs-lookup"><span data-stu-id="01d98-168">description</span></span>|<span data-ttu-id="01d98-169">String</span><span class="sxs-lookup"><span data-stu-id="01d98-169">String</span></span>|<span data-ttu-id="01d98-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="01d98-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01d98-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-172">displayName</span><span class="sxs-lookup"><span data-stu-id="01d98-172">displayName</span></span>|<span data-ttu-id="01d98-173">String</span><span class="sxs-lookup"><span data-stu-id="01d98-173">String</span></span>|<span data-ttu-id="01d98-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="01d98-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01d98-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-176">version</span><span class="sxs-lookup"><span data-stu-id="01d98-176">version</span></span>|<span data-ttu-id="01d98-177">Int32</span><span class="sxs-lookup"><span data-stu-id="01d98-177">Int32</span></span>|<span data-ttu-id="01d98-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="01d98-178">Version of the device configuration.</span></span> <span data-ttu-id="01d98-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01d98-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d98-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="01d98-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="01d98-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d98-181">Boolean</span></span>|<span data-ttu-id="01d98-182">如果设置为 true，则用户可以批准配置配置文件未明确允许的其他内核扩展。</span><span class="sxs-lookup"><span data-stu-id="01d98-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="01d98-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="01d98-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="01d98-184">String collection</span><span class="sxs-lookup"><span data-stu-id="01d98-184">String collection</span></span>|<span data-ttu-id="01d98-185">允许加载此列表中的团队标识符有效签名的所有内核扩展。</span><span class="sxs-lookup"><span data-stu-id="01d98-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="01d98-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="01d98-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="01d98-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01d98-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="01d98-188">将允许加载的内核扩展的列表。</span><span class="sxs-lookup"><span data-stu-id="01d98-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="01d98-189">.</span><span class="sxs-lookup"><span data-stu-id="01d98-189">.</span></span> <span data-ttu-id="01d98-190">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="01d98-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01d98-191">systemExtensionsBlockOverride</span><span class="sxs-lookup"><span data-stu-id="01d98-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="01d98-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d98-192">Boolean</span></span>|<span data-ttu-id="01d98-193">获取或设置是否允许用户批准配置文件未明确允许的其他系统扩展。</span><span class="sxs-lookup"><span data-stu-id="01d98-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="01d98-194">systemExtensionsAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="01d98-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="01d98-195">String collection</span><span class="sxs-lookup"><span data-stu-id="01d98-195">String collection</span></span>|<span data-ttu-id="01d98-196">获取或设置允许的团队标识符列表。</span><span class="sxs-lookup"><span data-stu-id="01d98-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="01d98-197">使用任何指定的团队标识符签名的任何系统扩展都将被批准。</span><span class="sxs-lookup"><span data-stu-id="01d98-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="01d98-198">systemExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="01d98-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="01d98-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01d98-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="01d98-200">获取或设置允许的 macOS 系统扩展的列表。</span><span class="sxs-lookup"><span data-stu-id="01d98-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="01d98-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="01d98-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01d98-202">systemExtensionsAllowedTypes</span><span class="sxs-lookup"><span data-stu-id="01d98-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="01d98-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01d98-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="01d98-204">获取或设置允许的 macOS 系统扩展类型的列表。</span><span class="sxs-lookup"><span data-stu-id="01d98-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="01d98-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="01d98-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="01d98-206">响应</span><span class="sxs-lookup"><span data-stu-id="01d98-206">Response</span></span>
<span data-ttu-id="01d98-207">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01d98-207">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d98-208">示例</span><span class="sxs-lookup"><span data-stu-id="01d98-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="01d98-209">请求</span><span class="sxs-lookup"><span data-stu-id="01d98-209">Request</span></span>
<span data-ttu-id="01d98-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01d98-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1965

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="01d98-211">响应</span><span class="sxs-lookup"><span data-stu-id="01d98-211">Response</span></span>
<span data-ttu-id="01d98-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01d98-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2137

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsBlockOverride": true,
  "systemExtensionsAllowedTeamIdentifiers": [
    "System Extensions Allowed Team Identifiers value"
  ],
  "systemExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ],
  "systemExtensionsAllowedTypes": [
    {
      "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
      "teamIdentifier": "Team Identifier value",
      "allowedTypes": "networkExtensionsAllowed"
    }
  ]
}
```




