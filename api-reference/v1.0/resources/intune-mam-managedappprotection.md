---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33048876cf28de23f9eaf6f562946283b8f19bd7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354410"
---
# <a name="managedappprotection-resource-type"></a><span data-ttu-id="2bead-103">managedAppProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bead-103">managedAppProtection resource type</span></span>

<span data-ttu-id="2bead-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bead-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bead-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bead-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bead-106">用于为指定的一组应用配置详细管理设置的策略</span><span class="sxs-lookup"><span data-stu-id="2bead-106">Policy used to configure detailed management settings for a specified set of apps</span></span>


<span data-ttu-id="2bead-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2bead-108">方法</span><span class="sxs-lookup"><span data-stu-id="2bead-108">Methods</span></span>
|<span data-ttu-id="2bead-109">方法</span><span class="sxs-lookup"><span data-stu-id="2bead-109">Method</span></span>|<span data-ttu-id="2bead-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bead-110">Return Type</span></span>|<span data-ttu-id="2bead-111">说明</span><span class="sxs-lookup"><span data-stu-id="2bead-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2bead-112">List managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="2bead-112">List managedAppProtections</span></span>](../api/intune-mam-managedappprotection-list.md)|<span data-ttu-id="2bead-113">[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2bead-113">[managedAppProtection](../resources/intune-mam-managedappprotection.md) collection</span></span>|<span data-ttu-id="2bead-114">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bead-114">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="2bead-115">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="2bead-115">Get managedAppProtection</span></span>](../api/intune-mam-managedappprotection-get.md)|[<span data-ttu-id="2bead-116">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="2bead-116">managedAppProtection</span></span>](../resources/intune-mam-managedappprotection.md)|<span data-ttu-id="2bead-117">读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bead-117">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>|
|[<span data-ttu-id="2bead-118">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="2bead-118">targetApps action</span></span>](../api/intune-mam-managedappprotection-targetapps.md)|<span data-ttu-id="2bead-119">无</span><span class="sxs-lookup"><span data-stu-id="2bead-119">None</span></span>|<span data-ttu-id="2bead-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2bead-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2bead-121">属性</span><span class="sxs-lookup"><span data-stu-id="2bead-121">Properties</span></span>
|<span data-ttu-id="2bead-122">属性</span><span class="sxs-lookup"><span data-stu-id="2bead-122">Property</span></span>|<span data-ttu-id="2bead-123">类型</span><span class="sxs-lookup"><span data-stu-id="2bead-123">Type</span></span>|<span data-ttu-id="2bead-124">说明</span><span class="sxs-lookup"><span data-stu-id="2bead-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bead-125">displayName</span><span class="sxs-lookup"><span data-stu-id="2bead-125">displayName</span></span>|<span data-ttu-id="2bead-126">字符串</span><span class="sxs-lookup"><span data-stu-id="2bead-126">String</span></span>|<span data-ttu-id="2bead-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="2bead-127">Policy display name.</span></span> <span data-ttu-id="2bead-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-129">description</span><span class="sxs-lookup"><span data-stu-id="2bead-129">description</span></span>|<span data-ttu-id="2bead-130">String</span><span class="sxs-lookup"><span data-stu-id="2bead-130">String</span></span>|<span data-ttu-id="2bead-131">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="2bead-131">The policy's description.</span></span> <span data-ttu-id="2bead-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bead-133">createdDateTime</span></span>|<span data-ttu-id="2bead-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bead-134">DateTimeOffset</span></span>|<span data-ttu-id="2bead-135">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2bead-135">The date and time the policy was created.</span></span> <span data-ttu-id="2bead-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bead-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2bead-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bead-138">DateTimeOffset</span></span>|<span data-ttu-id="2bead-139">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="2bead-139">Last time the policy was modified.</span></span> <span data-ttu-id="2bead-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-141">id</span><span class="sxs-lookup"><span data-stu-id="2bead-141">id</span></span>|<span data-ttu-id="2bead-142">字符串</span><span class="sxs-lookup"><span data-stu-id="2bead-142">String</span></span>|<span data-ttu-id="2bead-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2bead-143">Key of the entity.</span></span> <span data-ttu-id="2bead-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-145">version</span><span class="sxs-lookup"><span data-stu-id="2bead-145">version</span></span>|<span data-ttu-id="2bead-146">String</span><span class="sxs-lookup"><span data-stu-id="2bead-146">String</span></span>|<span data-ttu-id="2bead-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2bead-147">Version of the entity.</span></span> <span data-ttu-id="2bead-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2bead-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2bead-149">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2bead-149">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="2bead-150">持续时间</span><span class="sxs-lookup"><span data-stu-id="2bead-150">Duration</span></span>|<span data-ttu-id="2bead-151">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="2bead-151">The period after which access is checked when the device is not connected to the internet.</span></span>|
|<span data-ttu-id="2bead-152">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2bead-152">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="2bead-153">持续时间</span><span class="sxs-lookup"><span data-stu-id="2bead-153">Duration</span></span>|<span data-ttu-id="2bead-154">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="2bead-154">The period after which access is checked when the device is connected to the internet.</span></span>|
|<span data-ttu-id="2bead-155">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="2bead-155">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="2bead-156">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="2bead-156">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="2bead-157">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="2bead-157">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="2bead-158">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="2bead-158">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2bead-159">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="2bead-159">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="2bead-160">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="2bead-160">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="2bead-161">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="2bead-161">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="2bead-162">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="2bead-162">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2bead-163">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="2bead-163">organizationalCredentialsRequired</span></span>|<span data-ttu-id="2bead-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-164">Boolean</span></span>|<span data-ttu-id="2bead-165">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="2bead-165">Indicates whether organizational credentials are required for app use.</span></span>|
|<span data-ttu-id="2bead-166">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2bead-166">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="2bead-167">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2bead-167">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="2bead-168">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="2bead-168">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="2bead-169">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="2bead-169">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="2bead-170">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-170">dataBackupBlocked</span></span>|<span data-ttu-id="2bead-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-171">Boolean</span></span>|<span data-ttu-id="2bead-172">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="2bead-172">Indicates whether the backup of a managed app's data is blocked.</span></span>|
|<span data-ttu-id="2bead-173">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="2bead-173">deviceComplianceRequired</span></span>|<span data-ttu-id="2bead-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-174">Boolean</span></span>|<span data-ttu-id="2bead-175">指示是否需要设备合规性。</span><span class="sxs-lookup"><span data-stu-id="2bead-175">Indicates whether device compliance is required.</span></span>|
|<span data-ttu-id="2bead-176">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="2bead-176">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="2bead-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-177">Boolean</span></span>|<span data-ttu-id="2bead-178">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="2bead-178">Indicates whether internet links should be opened in the managed browser app.</span></span>|
|<span data-ttu-id="2bead-179">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-179">saveAsBlocked</span></span>|<span data-ttu-id="2bead-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-180">Boolean</span></span>|<span data-ttu-id="2bead-181">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="2bead-181">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span>|
|<span data-ttu-id="2bead-182">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="2bead-182">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="2bead-183">持续时间</span><span class="sxs-lookup"><span data-stu-id="2bead-183">Duration</span></span>|<span data-ttu-id="2bead-184">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="2bead-184">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span>|
|<span data-ttu-id="2bead-185">pinRequired</span><span class="sxs-lookup"><span data-stu-id="2bead-185">pinRequired</span></span>|<span data-ttu-id="2bead-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-186">Boolean</span></span>|<span data-ttu-id="2bead-187">指示是否需要应用级 pin。</span><span class="sxs-lookup"><span data-stu-id="2bead-187">Indicates whether an app-level pin is required.</span></span>|
|<span data-ttu-id="2bead-188">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="2bead-188">maximumPinRetries</span></span>|<span data-ttu-id="2bead-189">Int32</span><span class="sxs-lookup"><span data-stu-id="2bead-189">Int32</span></span>|<span data-ttu-id="2bead-190">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="2bead-190">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span>|
|<span data-ttu-id="2bead-191">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-191">simplePinBlocked</span></span>|<span data-ttu-id="2bead-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-192">Boolean</span></span>|<span data-ttu-id="2bead-193">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="2bead-193">Indicates whether simplePin is blocked.</span></span>|
|<span data-ttu-id="2bead-194">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="2bead-194">minimumPinLength</span></span>|<span data-ttu-id="2bead-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2bead-195">Int32</span></span>|<span data-ttu-id="2bead-196">PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。</span><span class="sxs-lookup"><span data-stu-id="2bead-196">Minimum pin length required for an app-level pin if PinRequired is set to True</span></span>|
|<span data-ttu-id="2bead-197">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="2bead-197">pinCharacterSet</span></span>|[<span data-ttu-id="2bead-198">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="2bead-198">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="2bead-199">PinRequired 设置为 True 时可用于应用级 pin 的字符集。</span><span class="sxs-lookup"><span data-stu-id="2bead-199">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="2bead-200">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="2bead-200">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="2bead-201">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="2bead-201">periodBeforePinReset</span></span>|<span data-ttu-id="2bead-202">Duration</span><span class="sxs-lookup"><span data-stu-id="2bead-202">Duration</span></span>|<span data-ttu-id="2bead-203">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。</span><span class="sxs-lookup"><span data-stu-id="2bead-203">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span>|
|<span data-ttu-id="2bead-204">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="2bead-204">allowedDataStorageLocations</span></span>|<span data-ttu-id="2bead-205">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="2bead-205">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="2bead-206">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="2bead-206">Data storage locations where a user may store managed data.</span></span>|
|<span data-ttu-id="2bead-207">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-207">contactSyncBlocked</span></span>|<span data-ttu-id="2bead-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-208">Boolean</span></span>|<span data-ttu-id="2bead-209">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="2bead-209">Indicates whether contacts can be synced to the user's device.</span></span>|
|<span data-ttu-id="2bead-210">printBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-210">printBlocked</span></span>|<span data-ttu-id="2bead-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-211">Boolean</span></span>|<span data-ttu-id="2bead-212">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="2bead-212">Indicates whether printing is allowed from managed apps.</span></span>|
|<span data-ttu-id="2bead-213">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="2bead-213">fingerprintBlocked</span></span>|<span data-ttu-id="2bead-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-214">Boolean</span></span>|<span data-ttu-id="2bead-215">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。</span><span class="sxs-lookup"><span data-stu-id="2bead-215">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="2bead-216">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="2bead-216">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="2bead-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bead-217">Boolean</span></span>|<span data-ttu-id="2bead-218">指示如果设置了设备 pin，是否需要使用应用 pin。</span><span class="sxs-lookup"><span data-stu-id="2bead-218">Indicates whether use of the app pin is required if the device pin is set.</span></span>|
|<span data-ttu-id="2bead-219">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="2bead-219">minimumRequiredOsVersion</span></span>|<span data-ttu-id="2bead-220">String</span><span class="sxs-lookup"><span data-stu-id="2bead-220">String</span></span>|<span data-ttu-id="2bead-221">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="2bead-221">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2bead-222">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="2bead-222">minimumWarningOsVersion</span></span>|<span data-ttu-id="2bead-223">String</span><span class="sxs-lookup"><span data-stu-id="2bead-223">String</span></span>|<span data-ttu-id="2bead-224">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="2bead-224">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2bead-225">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="2bead-225">minimumRequiredAppVersion</span></span>|<span data-ttu-id="2bead-226">String</span><span class="sxs-lookup"><span data-stu-id="2bead-226">String</span></span>|<span data-ttu-id="2bead-227">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="2bead-227">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2bead-228">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="2bead-228">minimumWarningAppVersion</span></span>|<span data-ttu-id="2bead-229">String</span><span class="sxs-lookup"><span data-stu-id="2bead-229">String</span></span>|<span data-ttu-id="2bead-230">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="2bead-230">Versions less than the specified version will result in warning message on the managed app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bead-231">关系</span><span class="sxs-lookup"><span data-stu-id="2bead-231">Relationships</span></span>
<span data-ttu-id="2bead-232">无</span><span class="sxs-lookup"><span data-stu-id="2bead-232">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bead-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bead-233">JSON Representation</span></span>
<span data-ttu-id="2bead-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bead-234">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->





