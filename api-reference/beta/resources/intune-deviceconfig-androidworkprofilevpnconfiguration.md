---
title: androidWorkProfileVpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 Android 工作配置文件设备连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a78a893cd218f372f8c5f33cf9dc729ffa770c9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021537"
---
# <a name="androidworkprofilevpnconfiguration-resource-type"></a><span data-ttu-id="ff58b-104">androidWorkProfileVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff58b-104">androidWorkProfileVpnConfiguration resource type</span></span>

<span data-ttu-id="ff58b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff58b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff58b-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff58b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff58b-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff58b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff58b-108">通过提供此配置文件中的配置，可以指示 Android 工作配置文件设备连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="ff58b-108">By providing the configurations in this profile you can instruct the Android Work Profile device to connect to desired VPN endpoint.</span></span> <span data-ttu-id="ff58b-109">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="ff58b-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="ff58b-110">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-110">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ff58b-111">方法</span><span class="sxs-lookup"><span data-stu-id="ff58b-111">Methods</span></span>
|<span data-ttu-id="ff58b-112">方法</span><span class="sxs-lookup"><span data-stu-id="ff58b-112">Method</span></span>|<span data-ttu-id="ff58b-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff58b-113">Return Type</span></span>|<span data-ttu-id="ff58b-114">说明</span><span class="sxs-lookup"><span data-stu-id="ff58b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff58b-115">列出 androidWorkProfileVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="ff58b-115">List androidWorkProfileVpnConfigurations</span></span>](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-list.md)|<span data-ttu-id="ff58b-116">[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-116">[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) collection</span></span>|<span data-ttu-id="ff58b-117">列出 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff58b-117">List properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ff58b-118">获取 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-118">Get androidWorkProfileVpnConfiguration</span></span>](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-get.md)|[<span data-ttu-id="ff58b-119">androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-119">androidWorkProfileVpnConfiguration</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|<span data-ttu-id="ff58b-120">读取 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff58b-120">Read properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ff58b-121">创建 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-121">Create androidWorkProfileVpnConfiguration</span></span>](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-create.md)|[<span data-ttu-id="ff58b-122">androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-122">androidWorkProfileVpnConfiguration</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|<span data-ttu-id="ff58b-123">创建新的 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff58b-123">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ff58b-124">删除 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-124">Delete androidWorkProfileVpnConfiguration</span></span>](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-delete.md)|<span data-ttu-id="ff58b-125">无</span><span class="sxs-lookup"><span data-stu-id="ff58b-125">None</span></span>|<span data-ttu-id="ff58b-126">删除 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ff58b-126">Deletes a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>|
|[<span data-ttu-id="ff58b-127">更新 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-127">Update androidWorkProfileVpnConfiguration</span></span>](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-update.md)|[<span data-ttu-id="ff58b-128">androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff58b-128">androidWorkProfileVpnConfiguration</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|<span data-ttu-id="ff58b-129">更新 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff58b-129">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff58b-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff58b-130">Properties</span></span>
|<span data-ttu-id="ff58b-131">属性</span><span class="sxs-lookup"><span data-stu-id="ff58b-131">Property</span></span>|<span data-ttu-id="ff58b-132">类型</span><span class="sxs-lookup"><span data-stu-id="ff58b-132">Type</span></span>|<span data-ttu-id="ff58b-133">说明</span><span class="sxs-lookup"><span data-stu-id="ff58b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff58b-134">id</span><span class="sxs-lookup"><span data-stu-id="ff58b-134">id</span></span>|<span data-ttu-id="ff58b-135">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-135">String</span></span>|<span data-ttu-id="ff58b-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff58b-136">Key of the entity.</span></span> <span data-ttu-id="ff58b-137">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff58b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ff58b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff58b-139">DateTimeOffset</span></span>|<span data-ttu-id="ff58b-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ff58b-140">DateTime the object was last modified.</span></span> <span data-ttu-id="ff58b-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff58b-142">roleScopeTagIds</span></span>|<span data-ttu-id="ff58b-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-143">String collection</span></span>|<span data-ttu-id="ff58b-144">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ff58b-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff58b-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ff58b-146">supportsScopeTags</span></span>|<span data-ttu-id="ff58b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff58b-147">Boolean</span></span>|<span data-ttu-id="ff58b-148">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ff58b-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ff58b-149">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ff58b-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ff58b-150">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ff58b-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ff58b-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ff58b-151">This property is read-only.</span></span> <span data-ttu-id="ff58b-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff58b-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ff58b-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff58b-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ff58b-155">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ff58b-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ff58b-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff58b-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ff58b-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff58b-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ff58b-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ff58b-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ff58b-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff58b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ff58b-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff58b-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ff58b-163">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ff58b-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ff58b-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff58b-165">createdDateTime</span></span>|<span data-ttu-id="ff58b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff58b-166">DateTimeOffset</span></span>|<span data-ttu-id="ff58b-167">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ff58b-167">DateTime the object was created.</span></span> <span data-ttu-id="ff58b-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-169">description</span><span class="sxs-lookup"><span data-stu-id="ff58b-169">description</span></span>|<span data-ttu-id="ff58b-170">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-170">String</span></span>|<span data-ttu-id="ff58b-171">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ff58b-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff58b-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-173">displayName</span><span class="sxs-lookup"><span data-stu-id="ff58b-173">displayName</span></span>|<span data-ttu-id="ff58b-174">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-174">String</span></span>|<span data-ttu-id="ff58b-175">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ff58b-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff58b-176">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-177">version</span><span class="sxs-lookup"><span data-stu-id="ff58b-177">version</span></span>|<span data-ttu-id="ff58b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ff58b-178">Int32</span></span>|<span data-ttu-id="ff58b-179">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ff58b-179">Version of the device configuration.</span></span> <span data-ttu-id="ff58b-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-181">connectionName</span><span class="sxs-lookup"><span data-stu-id="ff58b-181">connectionName</span></span>|<span data-ttu-id="ff58b-182">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-182">String</span></span>|<span data-ttu-id="ff58b-183">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ff58b-183">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ff58b-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="ff58b-184">connectionType</span></span>|[<span data-ttu-id="ff58b-185">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ff58b-185">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="ff58b-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ff58b-186">Connection type.</span></span> <span data-ttu-id="ff58b-187">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`、`microsoftTunnel`、`netMotionMobility`。</span><span class="sxs-lookup"><span data-stu-id="ff58b-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="ff58b-188">role</span><span class="sxs-lookup"><span data-stu-id="ff58b-188">role</span></span>|<span data-ttu-id="ff58b-189">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-189">String</span></span>|<span data-ttu-id="ff58b-190">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="ff58b-190">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ff58b-191">型</span><span class="sxs-lookup"><span data-stu-id="ff58b-191">realm</span></span>|<span data-ttu-id="ff58b-192">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-192">String</span></span>|<span data-ttu-id="ff58b-193">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="ff58b-193">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ff58b-194">台</span><span class="sxs-lookup"><span data-stu-id="ff58b-194">servers</span></span>|<span data-ttu-id="ff58b-195">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-195">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ff58b-196">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ff58b-196">List of VPN Servers on the network.</span></span> <span data-ttu-id="ff58b-197">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ff58b-197">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ff58b-198">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ff58b-198">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ff58b-199">其次</span><span class="sxs-lookup"><span data-stu-id="ff58b-199">fingerprint</span></span>|<span data-ttu-id="ff58b-200">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-200">String</span></span>|<span data-ttu-id="ff58b-201">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="ff58b-201">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ff58b-202">customData</span><span class="sxs-lookup"><span data-stu-id="ff58b-202">customData</span></span>|<span data-ttu-id="ff58b-203">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-203">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ff58b-204">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ff58b-204">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ff58b-205">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ff58b-205">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ff58b-206">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ff58b-206">customKeyValueData</span></span>|<span data-ttu-id="ff58b-207">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-207">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ff58b-208">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ff58b-208">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ff58b-209">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ff58b-209">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ff58b-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff58b-210">authenticationMethod</span></span>|[<span data-ttu-id="ff58b-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff58b-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ff58b-212">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ff58b-212">Authentication method.</span></span> <span data-ttu-id="ff58b-213">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="ff58b-213">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ff58b-214">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ff58b-214">proxyServer</span></span>|[<span data-ttu-id="ff58b-215">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ff58b-215">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ff58b-216">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="ff58b-216">Proxy server.</span></span>|
|<span data-ttu-id="ff58b-217">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="ff58b-217">targetedPackageIds</span></span>|<span data-ttu-id="ff58b-218">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-218">String collection</span></span>|<span data-ttu-id="ff58b-219">目标应用程序包 Id。</span><span class="sxs-lookup"><span data-stu-id="ff58b-219">Targeted App package IDs.</span></span>|
|<span data-ttu-id="ff58b-220">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ff58b-220">targetedMobileApps</span></span>|<span data-ttu-id="ff58b-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ff58b-222">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="ff58b-222">Targeted mobile apps.</span></span> <span data-ttu-id="ff58b-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ff58b-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ff58b-224">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="ff58b-224">alwaysOn</span></span>|<span data-ttu-id="ff58b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff58b-225">Boolean</span></span>|<span data-ttu-id="ff58b-226">是否启用始终启用的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="ff58b-226">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="ff58b-227">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="ff58b-227">alwaysOnLockdown</span></span>|<span data-ttu-id="ff58b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff58b-228">Boolean</span></span>|<span data-ttu-id="ff58b-229">如果启用了 always on VPN 连接，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="ff58b-229">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="ff58b-230">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="ff58b-230">microsoftTunnelSiteId</span></span>|<span data-ttu-id="ff58b-231">String</span><span class="sxs-lookup"><span data-stu-id="ff58b-231">String</span></span>|<span data-ttu-id="ff58b-232">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="ff58b-232">Microsoft Tunnel site ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff58b-233">关系</span><span class="sxs-lookup"><span data-stu-id="ff58b-233">Relationships</span></span>
|<span data-ttu-id="ff58b-234">关系</span><span class="sxs-lookup"><span data-stu-id="ff58b-234">Relationship</span></span>|<span data-ttu-id="ff58b-235">类型</span><span class="sxs-lookup"><span data-stu-id="ff58b-235">Type</span></span>|<span data-ttu-id="ff58b-236">说明</span><span class="sxs-lookup"><span data-stu-id="ff58b-236">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff58b-237">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="ff58b-237">groupAssignments</span></span>|<span data-ttu-id="ff58b-238">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-238">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="ff58b-239">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="ff58b-239">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="ff58b-240">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-240">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-241">assignments</span><span class="sxs-lookup"><span data-stu-id="ff58b-241">assignments</span></span>|<span data-ttu-id="ff58b-242">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-242">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ff58b-243">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="ff58b-243">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="ff58b-244">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-244">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-245">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ff58b-245">deviceStatuses</span></span>|<span data-ttu-id="ff58b-246">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-246">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ff58b-247">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="ff58b-247">Device configuration installation status by device.</span></span> <span data-ttu-id="ff58b-248">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-248">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-249">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ff58b-249">userStatuses</span></span>|<span data-ttu-id="ff58b-250">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-250">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ff58b-251">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="ff58b-251">Device configuration installation status by user.</span></span> <span data-ttu-id="ff58b-252">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-252">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-253">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ff58b-253">deviceStatusOverview</span></span>|[<span data-ttu-id="ff58b-254">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff58b-254">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="ff58b-255">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-255">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-256">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ff58b-256">userStatusOverview</span></span>|[<span data-ttu-id="ff58b-257">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ff58b-257">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="ff58b-258">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-258">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-259">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ff58b-259">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ff58b-260">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff58b-260">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ff58b-261">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff58b-261">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff58b-262">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="ff58b-262">identityCertificate</span></span>|[<span data-ttu-id="ff58b-263">androidWorkProfileCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="ff58b-263">androidWorkProfileCertificateProfileBase</span></span>](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|<span data-ttu-id="ff58b-264">在身份验证方法为证书时，用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="ff58b-264">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff58b-265">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff58b-265">JSON Representation</span></span>
<span data-ttu-id="ff58b-266">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff58b-266">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "connectionType": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "authenticationMethod": "String",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "targetedPackageIds": [
    "String"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "String"
}
```






