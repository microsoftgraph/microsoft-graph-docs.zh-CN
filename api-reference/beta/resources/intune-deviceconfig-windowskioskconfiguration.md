---
title: windowsKioskConfiguration 资源类型
description: 此实体提供展台资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 122b3d25f822452eac9db90bf6a1933b3c7fca3e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525500"
---
# <a name="windowskioskconfiguration-resource-type"></a><span data-ttu-id="1206a-103">windowsKioskConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="1206a-103">windowsKioskConfiguration resource type</span></span>

<span data-ttu-id="1206a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1206a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1206a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1206a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1206a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1206a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1206a-107">此实体提供展台资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="1206a-107">This entity provides descriptions of the declared methods, properties and relationships exposed by the kiosk resource.</span></span>


<span data-ttu-id="1206a-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1206a-109">方法</span><span class="sxs-lookup"><span data-stu-id="1206a-109">Methods</span></span>
|<span data-ttu-id="1206a-110">方法</span><span class="sxs-lookup"><span data-stu-id="1206a-110">Method</span></span>|<span data-ttu-id="1206a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1206a-111">Return Type</span></span>|<span data-ttu-id="1206a-112">说明</span><span class="sxs-lookup"><span data-stu-id="1206a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1206a-113">列出 windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="1206a-113">List windowsKioskConfigurations</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|<span data-ttu-id="1206a-114">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="1206a-114">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) collection</span></span>|<span data-ttu-id="1206a-115">列出[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1206a-115">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1206a-116">获取 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-116">Get windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[<span data-ttu-id="1206a-117">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-117">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="1206a-118">读取[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1206a-118">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1206a-119">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-119">Create windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[<span data-ttu-id="1206a-120">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-120">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="1206a-121">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1206a-121">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1206a-122">删除 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-122">Delete windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|<span data-ttu-id="1206a-123">无</span><span class="sxs-lookup"><span data-stu-id="1206a-123">None</span></span>|<span data-ttu-id="1206a-124">删除[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1206a-124">Deletes a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>|
|[<span data-ttu-id="1206a-125">更新 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-125">Update windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[<span data-ttu-id="1206a-126">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="1206a-126">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="1206a-127">更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1206a-127">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1206a-128">属性</span><span class="sxs-lookup"><span data-stu-id="1206a-128">Properties</span></span>
|<span data-ttu-id="1206a-129">属性</span><span class="sxs-lookup"><span data-stu-id="1206a-129">Property</span></span>|<span data-ttu-id="1206a-130">类型</span><span class="sxs-lookup"><span data-stu-id="1206a-130">Type</span></span>|<span data-ttu-id="1206a-131">说明</span><span class="sxs-lookup"><span data-stu-id="1206a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1206a-132">id</span><span class="sxs-lookup"><span data-stu-id="1206a-132">id</span></span>|<span data-ttu-id="1206a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1206a-133">String</span></span>|<span data-ttu-id="1206a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1206a-134">Key of the entity.</span></span> <span data-ttu-id="1206a-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1206a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1206a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1206a-137">DateTimeOffset</span></span>|<span data-ttu-id="1206a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1206a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1206a-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1206a-140">roleScopeTagIds</span></span>|<span data-ttu-id="1206a-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-141">String collection</span></span>|<span data-ttu-id="1206a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1206a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1206a-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1206a-144">supportsScopeTags</span></span>|<span data-ttu-id="1206a-145">布尔</span><span class="sxs-lookup"><span data-stu-id="1206a-145">Boolean</span></span>|<span data-ttu-id="1206a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1206a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1206a-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1206a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1206a-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1206a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1206a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1206a-149">This property is read-only.</span></span> <span data-ttu-id="1206a-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1206a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1206a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1206a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1206a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1206a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1206a-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1206a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1206a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1206a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1206a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1206a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1206a-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1206a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1206a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1206a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1206a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1206a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1206a-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1206a-163">createdDateTime</span></span>|<span data-ttu-id="1206a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1206a-164">DateTimeOffset</span></span>|<span data-ttu-id="1206a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1206a-165">DateTime the object was created.</span></span> <span data-ttu-id="1206a-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-167">说明</span><span class="sxs-lookup"><span data-stu-id="1206a-167">description</span></span>|<span data-ttu-id="1206a-168">String</span><span class="sxs-lookup"><span data-stu-id="1206a-168">String</span></span>|<span data-ttu-id="1206a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1206a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1206a-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1206a-171">displayName</span></span>|<span data-ttu-id="1206a-172">String</span><span class="sxs-lookup"><span data-stu-id="1206a-172">String</span></span>|<span data-ttu-id="1206a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1206a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1206a-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-175">version</span><span class="sxs-lookup"><span data-stu-id="1206a-175">version</span></span>|<span data-ttu-id="1206a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1206a-176">Int32</span></span>|<span data-ttu-id="1206a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1206a-177">Version of the device configuration.</span></span> <span data-ttu-id="1206a-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-179">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="1206a-179">kioskProfiles</span></span>|<span data-ttu-id="1206a-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="1206a-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="1206a-181">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="1206a-181">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="1206a-182">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="1206a-182">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="1206a-183">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="1206a-183">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="1206a-184">String</span><span class="sxs-lookup"><span data-stu-id="1206a-184">String</span></span>|<span data-ttu-id="1206a-185">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="1206a-185">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="1206a-186">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="1206a-186">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="1206a-187">布尔</span><span class="sxs-lookup"><span data-stu-id="1206a-187">Boolean</span></span>|<span data-ttu-id="1206a-188">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="1206a-188">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="1206a-189">默认情况下，"主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1206a-189">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="1206a-190">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="1206a-190">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="1206a-191">布尔</span><span class="sxs-lookup"><span data-stu-id="1206a-191">Boolean</span></span>|<span data-ttu-id="1206a-192">启用展台浏览器的导航按钮（前进/后退）。</span><span class="sxs-lookup"><span data-stu-id="1206a-192">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="1206a-193">默认情况下，导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1206a-193">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="1206a-194">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="1206a-194">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="1206a-195">布尔</span><span class="sxs-lookup"><span data-stu-id="1206a-195">Boolean</span></span>|<span data-ttu-id="1206a-196">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="1206a-196">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="1206a-197">默认情况下，"结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="1206a-197">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="1206a-198">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1206a-198">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="1206a-199">Int32</span><span class="sxs-lookup"><span data-stu-id="1206a-199">Int32</span></span>|<span data-ttu-id="1206a-200">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="1206a-200">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="1206a-201">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="1206a-201">Valid values are 1-1440.</span></span> <span data-ttu-id="1206a-202">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="1206a-202">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="1206a-203">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="1206a-203">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="1206a-204">String 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-204">String collection</span></span>|<span data-ttu-id="1206a-205">指定展台浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="1206a-205">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="1206a-206">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="1206a-206">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="1206a-207">String 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-207">String collection</span></span>|<span data-ttu-id="1206a-208">指定展台浏览器允许其导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="1206a-208">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="1206a-209">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="1206a-209">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="1206a-210">布尔</span><span class="sxs-lookup"><span data-stu-id="1206a-210">Boolean</span></span>|<span data-ttu-id="1206a-211">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="1206a-211">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="1206a-212">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="1206a-212">The Default is false.</span></span>|
|<span data-ttu-id="1206a-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="1206a-213">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="1206a-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="1206a-214">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="1206a-215">强制更新对展台设备的计划。</span><span class="sxs-lookup"><span data-stu-id="1206a-215">force update schedule for Kiosk devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1206a-216">关系</span><span class="sxs-lookup"><span data-stu-id="1206a-216">Relationships</span></span>
|<span data-ttu-id="1206a-217">关系</span><span class="sxs-lookup"><span data-stu-id="1206a-217">Relationship</span></span>|<span data-ttu-id="1206a-218">类型</span><span class="sxs-lookup"><span data-stu-id="1206a-218">Type</span></span>|<span data-ttu-id="1206a-219">说明</span><span class="sxs-lookup"><span data-stu-id="1206a-219">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1206a-220">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="1206a-220">groupAssignments</span></span>|<span data-ttu-id="1206a-221">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1206a-221">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1206a-222">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="1206a-222">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="1206a-223">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-223">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-224">assignments</span><span class="sxs-lookup"><span data-stu-id="1206a-224">assignments</span></span>|<span data-ttu-id="1206a-225">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-225">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1206a-226">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="1206a-226">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="1206a-227">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-227">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-228">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1206a-228">deviceStatuses</span></span>|<span data-ttu-id="1206a-229">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-229">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1206a-230">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1206a-230">Device configuration installation status by device.</span></span> <span data-ttu-id="1206a-231">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-231">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-232">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1206a-232">userStatuses</span></span>|<span data-ttu-id="1206a-233">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-233">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1206a-234">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="1206a-234">Device configuration installation status by user.</span></span> <span data-ttu-id="1206a-235">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-235">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-236">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1206a-236">deviceStatusOverview</span></span>|[<span data-ttu-id="1206a-237">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1206a-237">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1206a-238">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-238">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-239">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1206a-239">userStatusOverview</span></span>|[<span data-ttu-id="1206a-240">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1206a-240">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1206a-241">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-241">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1206a-242">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1206a-242">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1206a-243">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1206a-243">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1206a-244">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1206a-244">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1206a-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1206a-245">JSON Representation</span></span>
<span data-ttu-id="1206a-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1206a-246">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "autoLaunch": true,
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "String (timestamp)",
    "recurrence": "String",
    "dayofWeek": "String",
    "dayofMonth": 1024,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```



