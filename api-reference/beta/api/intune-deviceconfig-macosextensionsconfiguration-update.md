---
title: 更新 macOSExtensionsConfiguration
description: 更新 macOSExtensionsConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58ed32af4f36eef43a81aa111ae5aa7e640c2bb9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065856"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="0fa55-103">更新 macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fa55-103">Update macOSExtensionsConfiguration</span></span>

<span data-ttu-id="0fa55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fa55-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fa55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fa55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fa55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa55-107">更新 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-107">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fa55-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0fa55-108">Prerequisites</span></span>
<span data-ttu-id="0fa55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fa55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa55-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fa55-111">Permission type</span></span>|<span data-ttu-id="0fa55-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0fa55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fa55-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fa55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fa55-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fa55-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fa55-116">Not supported.</span></span>|
|<span data-ttu-id="0fa55-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fa55-117">Application</span></span>|<span data-ttu-id="0fa55-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa55-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fa55-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fa55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0fa55-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fa55-120">Request headers</span></span>
|<span data-ttu-id="0fa55-121">标头</span><span class="sxs-lookup"><span data-stu-id="0fa55-121">Header</span></span>|<span data-ttu-id="0fa55-122">值</span><span class="sxs-lookup"><span data-stu-id="0fa55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fa55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa55-123">Authorization</span></span>|<span data-ttu-id="0fa55-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0fa55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fa55-125">接受</span><span class="sxs-lookup"><span data-stu-id="0fa55-125">Accept</span></span>|<span data-ttu-id="0fa55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fa55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa55-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fa55-127">Request body</span></span>
<span data-ttu-id="0fa55-128">在请求正文中，提供 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fa55-128">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="0fa55-129">下表显示创建 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-129">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="0fa55-130">属性</span><span class="sxs-lookup"><span data-stu-id="0fa55-130">Property</span></span>|<span data-ttu-id="0fa55-131">类型</span><span class="sxs-lookup"><span data-stu-id="0fa55-131">Type</span></span>|<span data-ttu-id="0fa55-132">说明</span><span class="sxs-lookup"><span data-stu-id="0fa55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa55-133">id</span><span class="sxs-lookup"><span data-stu-id="0fa55-133">id</span></span>|<span data-ttu-id="0fa55-134">String</span><span class="sxs-lookup"><span data-stu-id="0fa55-134">String</span></span>|<span data-ttu-id="0fa55-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fa55-135">Key of the entity.</span></span> <span data-ttu-id="0fa55-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa55-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0fa55-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa55-138">DateTimeOffset</span></span>|<span data-ttu-id="0fa55-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa55-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0fa55-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0fa55-141">roleScopeTagIds</span></span>|<span data-ttu-id="0fa55-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-142">String collection</span></span>|<span data-ttu-id="0fa55-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0fa55-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fa55-145">supportsScopeTags</span></span>|<span data-ttu-id="0fa55-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa55-146">Boolean</span></span>|<span data-ttu-id="0fa55-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0fa55-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0fa55-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0fa55-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0fa55-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0fa55-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0fa55-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0fa55-150">This property is read-only.</span></span> <span data-ttu-id="0fa55-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa55-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0fa55-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa55-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0fa55-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0fa55-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0fa55-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa55-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0fa55-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa55-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0fa55-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa55-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0fa55-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa55-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0fa55-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa55-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0fa55-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa55-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0fa55-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa55-164">createdDateTime</span></span>|<span data-ttu-id="0fa55-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa55-165">DateTimeOffset</span></span>|<span data-ttu-id="0fa55-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa55-166">DateTime the object was created.</span></span> <span data-ttu-id="0fa55-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-168">说明</span><span class="sxs-lookup"><span data-stu-id="0fa55-168">description</span></span>|<span data-ttu-id="0fa55-169">String</span><span class="sxs-lookup"><span data-stu-id="0fa55-169">String</span></span>|<span data-ttu-id="0fa55-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0fa55-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0fa55-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0fa55-172">displayName</span></span>|<span data-ttu-id="0fa55-173">String</span><span class="sxs-lookup"><span data-stu-id="0fa55-173">String</span></span>|<span data-ttu-id="0fa55-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0fa55-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0fa55-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-176">version</span><span class="sxs-lookup"><span data-stu-id="0fa55-176">version</span></span>|<span data-ttu-id="0fa55-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0fa55-177">Int32</span></span>|<span data-ttu-id="0fa55-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0fa55-178">Version of the device configuration.</span></span> <span data-ttu-id="0fa55-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-180">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="0fa55-180">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="0fa55-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa55-181">Boolean</span></span>|<span data-ttu-id="0fa55-182">如果设置为 true，则用户可以批准配置文件配置文件未明确允许的其他内核扩展。</span><span class="sxs-lookup"><span data-stu-id="0fa55-182">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="0fa55-183">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="0fa55-183">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="0fa55-184">String 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-184">String collection</span></span>|<span data-ttu-id="0fa55-185">将允许加载此列表中由团队标识符有效签名的所有内核扩展。</span><span class="sxs-lookup"><span data-stu-id="0fa55-185">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="0fa55-186">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="0fa55-186">kernelExtensionsAllowed</span></span>|<span data-ttu-id="0fa55-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-187">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="0fa55-188">将允许加载的内核扩展的列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-188">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="0fa55-189">.</span><span class="sxs-lookup"><span data-stu-id="0fa55-189">.</span></span> <span data-ttu-id="0fa55-190">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa55-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0fa55-191">systemExtensionsBlockOverride</span><span class="sxs-lookup"><span data-stu-id="0fa55-191">systemExtensionsBlockOverride</span></span>|<span data-ttu-id="0fa55-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa55-192">Boolean</span></span>|<span data-ttu-id="0fa55-193">获取或设置是否允许用户批准配置文件未显式允许的其他系统扩展。</span><span class="sxs-lookup"><span data-stu-id="0fa55-193">Gets or sets whether to allow the user to approve additional system extensions not explicitly allowed by configuration profiles.</span></span>|
|<span data-ttu-id="0fa55-194">systemExtensionsAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="0fa55-194">systemExtensionsAllowedTeamIdentifiers</span></span>|<span data-ttu-id="0fa55-195">String 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-195">String collection</span></span>|<span data-ttu-id="0fa55-196">获取或设置允许的团队标识符的列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-196">Gets or sets a list of allowed team identifiers.</span></span> <span data-ttu-id="0fa55-197">任何指定的团队标识符签名的系统扩展都将获得批准。</span><span class="sxs-lookup"><span data-stu-id="0fa55-197">Any system extension signed with any of the specified team identifiers will be approved.</span></span>|
|<span data-ttu-id="0fa55-198">systemExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="0fa55-198">systemExtensionsAllowed</span></span>|<span data-ttu-id="0fa55-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-199">[macOSSystemExtension](../resources/intune-deviceconfig-macossystemextension.md) collection</span></span>|<span data-ttu-id="0fa55-200">获取或设置允许的 macOS 系统扩展列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-200">Gets or sets a list of allowed macOS system extensions.</span></span> <span data-ttu-id="0fa55-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa55-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0fa55-202">systemExtensionsAllowedTypes</span><span class="sxs-lookup"><span data-stu-id="0fa55-202">systemExtensionsAllowedTypes</span></span>|<span data-ttu-id="0fa55-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-203">[macOSSystemExtensionTypeMapping](../resources/intune-deviceconfig-macossystemextensiontypemapping.md) collection</span></span>|<span data-ttu-id="0fa55-204">获取或设置允许的 macOS 系统扩展类型的列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-204">Gets or sets a list of allowed macOS system extension types.</span></span> <span data-ttu-id="0fa55-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa55-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0fa55-206">响应</span><span class="sxs-lookup"><span data-stu-id="0fa55-206">Response</span></span>
<span data-ttu-id="0fa55-207">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fa55-207">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa55-208">示例</span><span class="sxs-lookup"><span data-stu-id="0fa55-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa55-209">请求</span><span class="sxs-lookup"><span data-stu-id="0fa55-209">Request</span></span>
<span data-ttu-id="0fa55-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fa55-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fa55-211">响应</span><span class="sxs-lookup"><span data-stu-id="0fa55-211">Response</span></span>
<span data-ttu-id="0fa55-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






