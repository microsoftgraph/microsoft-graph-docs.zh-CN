---
title: windowsKioskConfiguration 资源类型
description: 此实体提供展台资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: edc1b3369a3b3ab0faab2cdb16cc8b9ef396f786
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969014"
---
# <a name="windowskioskconfiguration-resource-type"></a><span data-ttu-id="7b2ea-103">windowsKioskConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b2ea-103">windowsKioskConfiguration resource type</span></span>

> <span data-ttu-id="7b2ea-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b2ea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b2ea-106">此实体提供展台资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-106">This entity provides descriptions of the declared methods, properties and relationships exposed by the kiosk resource.</span></span>


<span data-ttu-id="7b2ea-107">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7b2ea-108">方法</span><span class="sxs-lookup"><span data-stu-id="7b2ea-108">Methods</span></span>
|<span data-ttu-id="7b2ea-109">方法</span><span class="sxs-lookup"><span data-stu-id="7b2ea-109">Method</span></span>|<span data-ttu-id="7b2ea-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7b2ea-110">Return Type</span></span>|<span data-ttu-id="7b2ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b2ea-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b2ea-112">列出 windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="7b2ea-112">List windowsKioskConfigurations</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|<span data-ttu-id="7b2ea-113">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-113">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) collection</span></span>|<span data-ttu-id="7b2ea-114">列出[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-114">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7b2ea-115">获取 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-115">Get windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[<span data-ttu-id="7b2ea-116">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-116">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="7b2ea-117">读取[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-117">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7b2ea-118">创建 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-118">Create windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[<span data-ttu-id="7b2ea-119">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-119">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="7b2ea-120">创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-120">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7b2ea-121">删除 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-121">Delete windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|<span data-ttu-id="7b2ea-122">无</span><span class="sxs-lookup"><span data-stu-id="7b2ea-122">None</span></span>|<span data-ttu-id="7b2ea-123">删除[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-123">Deletes a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>|
|[<span data-ttu-id="7b2ea-124">更新 windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-124">Update windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[<span data-ttu-id="7b2ea-125">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b2ea-125">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="7b2ea-126">更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-126">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b2ea-127">属性</span><span class="sxs-lookup"><span data-stu-id="7b2ea-127">Properties</span></span>
|<span data-ttu-id="7b2ea-128">属性</span><span class="sxs-lookup"><span data-stu-id="7b2ea-128">Property</span></span>|<span data-ttu-id="7b2ea-129">类型</span><span class="sxs-lookup"><span data-stu-id="7b2ea-129">Type</span></span>|<span data-ttu-id="7b2ea-130">说明</span><span class="sxs-lookup"><span data-stu-id="7b2ea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b2ea-131">id</span><span class="sxs-lookup"><span data-stu-id="7b2ea-131">id</span></span>|<span data-ttu-id="7b2ea-132">字符串</span><span class="sxs-lookup"><span data-stu-id="7b2ea-132">String</span></span>|<span data-ttu-id="7b2ea-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-133">Key of the entity.</span></span> <span data-ttu-id="7b2ea-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b2ea-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7b2ea-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b2ea-136">DateTimeOffset</span></span>|<span data-ttu-id="7b2ea-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7b2ea-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b2ea-139">roleScopeTagIds</span></span>|<span data-ttu-id="7b2ea-140">String collection</span><span class="sxs-lookup"><span data-stu-id="7b2ea-140">String collection</span></span>|<span data-ttu-id="7b2ea-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b2ea-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7b2ea-143">supportsScopeTags</span></span>|<span data-ttu-id="7b2ea-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2ea-144">Boolean</span></span>|<span data-ttu-id="7b2ea-145">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b2ea-146">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b2ea-147">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b2ea-148">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-148">This property is read-only.</span></span> <span data-ttu-id="7b2ea-149">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-150">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b2ea-150">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7b2ea-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7b2ea-151">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7b2ea-152">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-152">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7b2ea-153">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-154">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b2ea-154">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7b2ea-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7b2ea-155">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7b2ea-156">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-156">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7b2ea-157">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-158">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b2ea-158">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7b2ea-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7b2ea-159">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7b2ea-160">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-160">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7b2ea-161">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b2ea-162">createdDateTime</span></span>|<span data-ttu-id="7b2ea-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b2ea-163">DateTimeOffset</span></span>|<span data-ttu-id="7b2ea-164">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-164">DateTime the object was created.</span></span> <span data-ttu-id="7b2ea-165">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-166">说明</span><span class="sxs-lookup"><span data-stu-id="7b2ea-166">description</span></span>|<span data-ttu-id="7b2ea-167">String</span><span class="sxs-lookup"><span data-stu-id="7b2ea-167">String</span></span>|<span data-ttu-id="7b2ea-168">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-168">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b2ea-169">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-169">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-170">displayName</span><span class="sxs-lookup"><span data-stu-id="7b2ea-170">displayName</span></span>|<span data-ttu-id="7b2ea-171">String</span><span class="sxs-lookup"><span data-stu-id="7b2ea-171">String</span></span>|<span data-ttu-id="7b2ea-172">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-172">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b2ea-173">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-173">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-174">version</span><span class="sxs-lookup"><span data-stu-id="7b2ea-174">version</span></span>|<span data-ttu-id="7b2ea-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2ea-175">Int32</span></span>|<span data-ttu-id="7b2ea-176">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-176">Version of the device configuration.</span></span> <span data-ttu-id="7b2ea-177">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-178">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="7b2ea-178">kioskProfiles</span></span>|<span data-ttu-id="7b2ea-179">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-179">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="7b2ea-180">此策略设置允许为展台配置定义展台配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-180">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="7b2ea-181">此集合最多可包含3个元素。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-181">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="7b2ea-182">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="7b2ea-182">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="7b2ea-183">String</span><span class="sxs-lookup"><span data-stu-id="7b2ea-183">String</span></span>|<span data-ttu-id="7b2ea-184">指定浏览器在启动时应导航到的默认 URL。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-184">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="7b2ea-185">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="7b2ea-185">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="7b2ea-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2ea-186">Boolean</span></span>|<span data-ttu-id="7b2ea-187">启用展台浏览器的 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-187">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="7b2ea-188">默认情况下, "主页" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-188">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="7b2ea-189">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="7b2ea-189">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="7b2ea-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2ea-190">Boolean</span></span>|<span data-ttu-id="7b2ea-191">启用展台浏览器的导航按钮 (前进/后退)。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-191">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="7b2ea-192">默认情况下, 导航按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-192">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="7b2ea-193">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="7b2ea-193">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="7b2ea-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2ea-194">Boolean</span></span>|<span data-ttu-id="7b2ea-195">启用展台浏览器的结束会话按钮。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-195">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="7b2ea-196">默认情况下, "结束会话" 按钮处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-196">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="7b2ea-197">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="7b2ea-197">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="7b2ea-198">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2ea-198">Int32</span></span>|<span data-ttu-id="7b2ea-199">指定在展台浏览器以全新状态重新启动之前会话处于空闲状态的分钟数。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-199">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="7b2ea-200">有效值为1-1440。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-200">Valid values are 1-1440.</span></span> <span data-ttu-id="7b2ea-201">有效值为1至1440</span><span class="sxs-lookup"><span data-stu-id="7b2ea-201">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="7b2ea-202">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="7b2ea-202">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="7b2ea-203">String collection</span><span class="sxs-lookup"><span data-stu-id="7b2ea-203">String collection</span></span>|<span data-ttu-id="7b2ea-204">指定展台浏览器不应导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="7b2ea-204">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="7b2ea-205">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="7b2ea-205">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="7b2ea-206">String collection</span><span class="sxs-lookup"><span data-stu-id="7b2ea-206">String collection</span></span>|<span data-ttu-id="7b2ea-207">指定展台浏览器允许其导航到的 Url</span><span class="sxs-lookup"><span data-stu-id="7b2ea-207">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="7b2ea-208">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="7b2ea-208">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="7b2ea-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2ea-209">Boolean</span></span>|<span data-ttu-id="7b2ea-210">为 Microsoft Edge 浏览器启用公共浏览展台模式。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-210">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="7b2ea-211">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-211">The Default is false.</span></span>|
|<span data-ttu-id="7b2ea-212">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="7b2ea-212">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="7b2ea-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="7b2ea-213">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="7b2ea-214">强制更新对展台设备的计划。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-214">force update schedule for Kiosk devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b2ea-215">关系</span><span class="sxs-lookup"><span data-stu-id="7b2ea-215">Relationships</span></span>
|<span data-ttu-id="7b2ea-216">关系</span><span class="sxs-lookup"><span data-stu-id="7b2ea-216">Relationship</span></span>|<span data-ttu-id="7b2ea-217">类型</span><span class="sxs-lookup"><span data-stu-id="7b2ea-217">Type</span></span>|<span data-ttu-id="7b2ea-218">说明</span><span class="sxs-lookup"><span data-stu-id="7b2ea-218">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b2ea-219">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="7b2ea-219">groupAssignments</span></span>|<span data-ttu-id="7b2ea-220">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-220">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="7b2ea-221">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-221">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="7b2ea-222">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-222">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-223">assignments</span><span class="sxs-lookup"><span data-stu-id="7b2ea-223">assignments</span></span>|<span data-ttu-id="7b2ea-224">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-224">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7b2ea-225">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-225">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="7b2ea-226">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-226">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-227">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7b2ea-227">deviceStatuses</span></span>|<span data-ttu-id="7b2ea-228">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-228">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7b2ea-229">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-229">Device configuration installation status by device.</span></span> <span data-ttu-id="7b2ea-230">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-230">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-231">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7b2ea-231">userStatuses</span></span>|<span data-ttu-id="7b2ea-232">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-232">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7b2ea-233">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-233">Device configuration installation status by user.</span></span> <span data-ttu-id="7b2ea-234">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-234">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-235">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7b2ea-235">deviceStatusOverview</span></span>|[<span data-ttu-id="7b2ea-236">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7b2ea-236">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7b2ea-237">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-237">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-238">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7b2ea-238">userStatusOverview</span></span>|[<span data-ttu-id="7b2ea-239">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7b2ea-239">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7b2ea-240">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-240">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b2ea-241">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7b2ea-241">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7b2ea-242">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b2ea-242">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7b2ea-243">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b2ea-243">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b2ea-244">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b2ea-244">JSON Representation</span></span>
<span data-ttu-id="7b2ea-245">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b2ea-245">Here is a JSON representation of the resource.</span></span>
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





