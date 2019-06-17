---
title: windowsKioskConfiguration 资源类型
description: 此实体提供展台资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8da4c53d22621f08faf4edb27be2da10ce5674c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978505"
---
# <a name="windowskioskconfiguration-resource-type"></a><span data-ttu-id="90eaf-103">windowsKioskConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="90eaf-103">windowsKioskConfiguration resource type</span></span>

> <span data-ttu-id="90eaf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90eaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90eaf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90eaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90eaf-106">此实体提供展台资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="90eaf-106">This entity provides descriptions of the declared methods, properties and relationships exposed by the kiosk resource.</span></span>


<span data-ttu-id="90eaf-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="90eaf-108">方法</span><span class="sxs-lookup"><span data-stu-id="90eaf-108">Methods</span></span>
|<span data-ttu-id="90eaf-109">方法</span><span class="sxs-lookup"><span data-stu-id="90eaf-109">Method</span></span>|<span data-ttu-id="90eaf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90eaf-110">Return Type</span></span>|<span data-ttu-id="90eaf-111">说明</span><span class="sxs-lookup"><span data-stu-id="90eaf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90eaf-112">列出 windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="90eaf-112">List windowsKioskConfigurations</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|<span data-ttu-id="90eaf-113">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-113">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) collection</span></span>|<span data-ttu-id="90eaf-114">列出[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90eaf-114">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="90eaf-115">获取 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-115">Get windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[<span data-ttu-id="90eaf-116">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-116">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="90eaf-117">读取[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90eaf-117">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="90eaf-118">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-118">Create windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[<span data-ttu-id="90eaf-119">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-119">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="90eaf-120">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90eaf-120">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="90eaf-121">删除 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-121">Delete windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|<span data-ttu-id="90eaf-122">无</span><span class="sxs-lookup"><span data-stu-id="90eaf-122">None</span></span>|<span data-ttu-id="90eaf-123">删除[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="90eaf-123">Deletes a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>|
|[<span data-ttu-id="90eaf-124">更新 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-124">Update windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[<span data-ttu-id="90eaf-125">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="90eaf-125">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="90eaf-126">更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="90eaf-126">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90eaf-127">属性</span><span class="sxs-lookup"><span data-stu-id="90eaf-127">Properties</span></span>
|<span data-ttu-id="90eaf-128">属性</span><span class="sxs-lookup"><span data-stu-id="90eaf-128">Property</span></span>|<span data-ttu-id="90eaf-129">类型</span><span class="sxs-lookup"><span data-stu-id="90eaf-129">Type</span></span>|<span data-ttu-id="90eaf-130">说明</span><span class="sxs-lookup"><span data-stu-id="90eaf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90eaf-131">id</span><span class="sxs-lookup"><span data-stu-id="90eaf-131">id</span></span>|<span data-ttu-id="90eaf-132">字符串</span><span class="sxs-lookup"><span data-stu-id="90eaf-132">String</span></span>|<span data-ttu-id="90eaf-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90eaf-133">Key of the entity.</span></span> <span data-ttu-id="90eaf-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90eaf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="90eaf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90eaf-136">DateTimeOffset</span></span>|<span data-ttu-id="90eaf-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90eaf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="90eaf-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90eaf-139">roleScopeTagIds</span></span>|<span data-ttu-id="90eaf-140">String collection</span><span class="sxs-lookup"><span data-stu-id="90eaf-140">String collection</span></span>|<span data-ttu-id="90eaf-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="90eaf-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90eaf-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="90eaf-143">supportsScopeTags</span></span>|<span data-ttu-id="90eaf-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="90eaf-144">Boolean</span></span>|<span data-ttu-id="90eaf-145">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="90eaf-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90eaf-146">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="90eaf-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90eaf-147">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="90eaf-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90eaf-148">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="90eaf-148">This property is read-only.</span></span> <span data-ttu-id="90eaf-149">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-150">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90eaf-150">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="90eaf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90eaf-151">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="90eaf-152">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="90eaf-152">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="90eaf-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-154">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90eaf-154">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="90eaf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90eaf-155">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="90eaf-156">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="90eaf-156">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="90eaf-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-158">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90eaf-158">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="90eaf-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90eaf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="90eaf-160">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="90eaf-160">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="90eaf-161">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90eaf-162">createdDateTime</span></span>|<span data-ttu-id="90eaf-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90eaf-163">DateTimeOffset</span></span>|<span data-ttu-id="90eaf-164">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90eaf-164">DateTime the object was created.</span></span> <span data-ttu-id="90eaf-165">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-166">说明</span><span class="sxs-lookup"><span data-stu-id="90eaf-166">description</span></span>|<span data-ttu-id="90eaf-167">String</span><span class="sxs-lookup"><span data-stu-id="90eaf-167">String</span></span>|<span data-ttu-id="90eaf-168">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="90eaf-168">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90eaf-169">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-169">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-170">displayName</span><span class="sxs-lookup"><span data-stu-id="90eaf-170">displayName</span></span>|<span data-ttu-id="90eaf-171">String</span><span class="sxs-lookup"><span data-stu-id="90eaf-171">String</span></span>|<span data-ttu-id="90eaf-172">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="90eaf-172">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90eaf-173">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-173">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-174">version</span><span class="sxs-lookup"><span data-stu-id="90eaf-174">version</span></span>|<span data-ttu-id="90eaf-175">Int32</span><span class="sxs-lookup"><span data-stu-id="90eaf-175">Int32</span></span>|<span data-ttu-id="90eaf-176">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="90eaf-176">Version of the device configuration.</span></span> <span data-ttu-id="90eaf-177">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-178">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="90eaf-178">kioskProfiles</span></span>|<span data-ttu-id="90eaf-179">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-179">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="90eaf-180">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="90eaf-180">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="90eaf-181">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="90eaf-181">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="90eaf-182">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="90eaf-182">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="90eaf-183">String</span><span class="sxs-lookup"><span data-stu-id="90eaf-183">String</span></span>|<span data-ttu-id="90eaf-184">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="90eaf-184">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="90eaf-185">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="90eaf-185">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="90eaf-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="90eaf-186">Boolean</span></span>|<span data-ttu-id="90eaf-187">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="90eaf-187">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="90eaf-188">默认情况下, "主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="90eaf-188">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="90eaf-189">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="90eaf-189">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="90eaf-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="90eaf-190">Boolean</span></span>|<span data-ttu-id="90eaf-191">启用展台浏览器的导航按钮 (前进/后退)。</span><span class="sxs-lookup"><span data-stu-id="90eaf-191">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="90eaf-192">默认情况下, 导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="90eaf-192">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="90eaf-193">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="90eaf-193">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="90eaf-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="90eaf-194">Boolean</span></span>|<span data-ttu-id="90eaf-195">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="90eaf-195">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="90eaf-196">默认情况下, "结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="90eaf-196">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="90eaf-197">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="90eaf-197">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="90eaf-198">Int32</span><span class="sxs-lookup"><span data-stu-id="90eaf-198">Int32</span></span>|<span data-ttu-id="90eaf-199">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="90eaf-199">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="90eaf-200">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="90eaf-200">Valid values are 1-1440.</span></span> <span data-ttu-id="90eaf-201">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="90eaf-201">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="90eaf-202">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="90eaf-202">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="90eaf-203">String collection</span><span class="sxs-lookup"><span data-stu-id="90eaf-203">String collection</span></span>|<span data-ttu-id="90eaf-204">指定展台浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="90eaf-204">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="90eaf-205">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="90eaf-205">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="90eaf-206">String collection</span><span class="sxs-lookup"><span data-stu-id="90eaf-206">String collection</span></span>|<span data-ttu-id="90eaf-207">指定展台浏览器允许其导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="90eaf-207">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="90eaf-208">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="90eaf-208">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="90eaf-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="90eaf-209">Boolean</span></span>|<span data-ttu-id="90eaf-210">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="90eaf-210">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="90eaf-211">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="90eaf-211">The Default is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90eaf-212">关系</span><span class="sxs-lookup"><span data-stu-id="90eaf-212">Relationships</span></span>
|<span data-ttu-id="90eaf-213">关系</span><span class="sxs-lookup"><span data-stu-id="90eaf-213">Relationship</span></span>|<span data-ttu-id="90eaf-214">类型</span><span class="sxs-lookup"><span data-stu-id="90eaf-214">Type</span></span>|<span data-ttu-id="90eaf-215">说明</span><span class="sxs-lookup"><span data-stu-id="90eaf-215">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90eaf-216">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="90eaf-216">groupAssignments</span></span>|<span data-ttu-id="90eaf-217">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-217">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="90eaf-218">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="90eaf-218">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="90eaf-219">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-219">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-220">assignments</span><span class="sxs-lookup"><span data-stu-id="90eaf-220">assignments</span></span>|<span data-ttu-id="90eaf-221">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-221">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="90eaf-222">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="90eaf-222">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="90eaf-223">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-223">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-224">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="90eaf-224">deviceStatuses</span></span>|<span data-ttu-id="90eaf-225">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-225">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="90eaf-226">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="90eaf-226">Device configuration installation status by device.</span></span> <span data-ttu-id="90eaf-227">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-227">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-228">userStatuses</span><span class="sxs-lookup"><span data-stu-id="90eaf-228">userStatuses</span></span>|<span data-ttu-id="90eaf-229">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-229">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="90eaf-230">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="90eaf-230">Device configuration installation status by user.</span></span> <span data-ttu-id="90eaf-231">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-231">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-232">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="90eaf-232">deviceStatusOverview</span></span>|[<span data-ttu-id="90eaf-233">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="90eaf-233">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="90eaf-234">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-234">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-235">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="90eaf-235">userStatusOverview</span></span>|[<span data-ttu-id="90eaf-236">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="90eaf-236">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="90eaf-237">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-237">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90eaf-238">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="90eaf-238">deviceSettingStateSummaries</span></span>|<span data-ttu-id="90eaf-239">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90eaf-239">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="90eaf-240">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90eaf-240">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90eaf-241">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90eaf-241">JSON Representation</span></span>
<span data-ttu-id="90eaf-242">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90eaf-242">Here is a JSON representation of the resource.</span></span>
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
  "edgeKioskEnablePublicBrowsing": true
}
```





