---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b97b4b1453253ecd6fc5b5d77515b8b28586b19f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254126"
---
# <a name="managedappprotection-resource-type"></a><span data-ttu-id="b3912-103">managedAppProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3912-103">managedAppProtection resource type</span></span>

> <span data-ttu-id="b3912-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3912-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3912-105">用于为指定的一组应用配置详细管理设置的策略</span><span class="sxs-lookup"><span data-stu-id="b3912-105">Policy used to configure detailed management settings for a specified set of apps</span></span>


<span data-ttu-id="b3912-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b3912-107">方法</span><span class="sxs-lookup"><span data-stu-id="b3912-107">Methods</span></span>
|<span data-ttu-id="b3912-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3912-108">Method</span></span>|<span data-ttu-id="b3912-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3912-109">Return Type</span></span>|<span data-ttu-id="b3912-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3912-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3912-111">List managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="b3912-111">List managedAppProtections</span></span>](../api/intune-mam-managedappprotection-list.md)|<span data-ttu-id="b3912-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3912-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) collection</span></span>|<span data-ttu-id="b3912-113">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3912-113">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="b3912-114">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b3912-114">Get managedAppProtection</span></span>](../api/intune-mam-managedappprotection-get.md)|[<span data-ttu-id="b3912-115">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b3912-115">managedAppProtection</span></span>](../resources/intune-mam-managedappprotection.md)|<span data-ttu-id="b3912-116">读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3912-116">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>|
|[<span data-ttu-id="b3912-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="b3912-117">targetApps action</span></span>](../api/intune-mam-managedappprotection-targetapps.md)|<span data-ttu-id="b3912-118">无</span><span class="sxs-lookup"><span data-stu-id="b3912-118">None</span></span>|<span data-ttu-id="b3912-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3912-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b3912-120">属性</span><span class="sxs-lookup"><span data-stu-id="b3912-120">Properties</span></span>
|<span data-ttu-id="b3912-121">属性</span><span class="sxs-lookup"><span data-stu-id="b3912-121">Property</span></span>|<span data-ttu-id="b3912-122">类型</span><span class="sxs-lookup"><span data-stu-id="b3912-122">Type</span></span>|<span data-ttu-id="b3912-123">说明</span><span class="sxs-lookup"><span data-stu-id="b3912-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3912-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b3912-124">displayName</span></span>|<span data-ttu-id="b3912-125">String</span><span class="sxs-lookup"><span data-stu-id="b3912-125">String</span></span>|<span data-ttu-id="b3912-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="b3912-126">Policy display name.</span></span> <span data-ttu-id="b3912-127">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-128">description</span><span class="sxs-lookup"><span data-stu-id="b3912-128">description</span></span>|<span data-ttu-id="b3912-129">String</span><span class="sxs-lookup"><span data-stu-id="b3912-129">String</span></span>|<span data-ttu-id="b3912-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b3912-130">The policy's description.</span></span> <span data-ttu-id="b3912-131">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3912-132">createdDateTime</span></span>|<span data-ttu-id="b3912-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3912-133">DateTimeOffset</span></span>|<span data-ttu-id="b3912-134">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b3912-134">The date and time the policy was created.</span></span> <span data-ttu-id="b3912-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3912-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b3912-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3912-137">DateTimeOffset</span></span>|<span data-ttu-id="b3912-138">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="b3912-138">Last time the policy was modified.</span></span> <span data-ttu-id="b3912-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-140">id</span><span class="sxs-lookup"><span data-stu-id="b3912-140">id</span></span>|<span data-ttu-id="b3912-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b3912-141">String</span></span>|<span data-ttu-id="b3912-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3912-142">Key of the entity.</span></span> <span data-ttu-id="b3912-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-144">version</span><span class="sxs-lookup"><span data-stu-id="b3912-144">version</span></span>|<span data-ttu-id="b3912-145">String</span><span class="sxs-lookup"><span data-stu-id="b3912-145">String</span></span>|<span data-ttu-id="b3912-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b3912-146">Version of the entity.</span></span> <span data-ttu-id="b3912-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3912-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3912-148">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="b3912-148">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="b3912-149">持续时间</span><span class="sxs-lookup"><span data-stu-id="b3912-149">Duration</span></span>|<span data-ttu-id="b3912-150">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="b3912-150">The period after which access is checked when the device is not connected to the internet.</span></span>|
|<span data-ttu-id="b3912-151">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="b3912-151">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="b3912-152">持续时间</span><span class="sxs-lookup"><span data-stu-id="b3912-152">Duration</span></span>|<span data-ttu-id="b3912-153">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="b3912-153">The period after which access is checked when the device is connected to the internet.</span></span>|
|<span data-ttu-id="b3912-154">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="b3912-154">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="b3912-155">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="b3912-155">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="b3912-156">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="b3912-156">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="b3912-157">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b3912-157">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="b3912-158">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="b3912-158">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="b3912-159">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="b3912-159">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="b3912-160">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="b3912-160">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="b3912-161">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b3912-161">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="b3912-162">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="b3912-162">organizationalCredentialsRequired</span></span>|<span data-ttu-id="b3912-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-163">Boolean</span></span>|<span data-ttu-id="b3912-164">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="b3912-164">Indicates whether organizational credentials are required for app use.</span></span>|
|<span data-ttu-id="b3912-165">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b3912-165">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="b3912-166">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b3912-166">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="b3912-167">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="b3912-167">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="b3912-168">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="b3912-168">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="b3912-169">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-169">dataBackupBlocked</span></span>|<span data-ttu-id="b3912-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-170">Boolean</span></span>|<span data-ttu-id="b3912-171">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="b3912-171">Indicates whether the backup of a managed app's data is blocked.</span></span>|
|<span data-ttu-id="b3912-172">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="b3912-172">deviceComplianceRequired</span></span>|<span data-ttu-id="b3912-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-173">Boolean</span></span>|<span data-ttu-id="b3912-174">指示是否需要设备合规性。</span><span class="sxs-lookup"><span data-stu-id="b3912-174">Indicates whether device compliance is required.</span></span>|
|<span data-ttu-id="b3912-175">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="b3912-175">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="b3912-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-176">Boolean</span></span>|<span data-ttu-id="b3912-177">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="b3912-177">Indicates whether internet links should be opened in the managed browser app.</span></span>|
|<span data-ttu-id="b3912-178">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-178">saveAsBlocked</span></span>|<span data-ttu-id="b3912-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-179">Boolean</span></span>|<span data-ttu-id="b3912-180">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="b3912-180">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span>|
|<span data-ttu-id="b3912-181">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="b3912-181">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="b3912-182">Duration</span><span class="sxs-lookup"><span data-stu-id="b3912-182">Duration</span></span>|<span data-ttu-id="b3912-183">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="b3912-183">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span>|
|<span data-ttu-id="b3912-184">pinRequired</span><span class="sxs-lookup"><span data-stu-id="b3912-184">pinRequired</span></span>|<span data-ttu-id="b3912-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-185">Boolean</span></span>|<span data-ttu-id="b3912-186">指示是否需要应用级 pin。</span><span class="sxs-lookup"><span data-stu-id="b3912-186">Indicates whether an app-level pin is required.</span></span>|
|<span data-ttu-id="b3912-187">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="b3912-187">maximumPinRetries</span></span>|<span data-ttu-id="b3912-188">Int32</span><span class="sxs-lookup"><span data-stu-id="b3912-188">Int32</span></span>|<span data-ttu-id="b3912-189">在阻止或擦除托管应用之前, 不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="b3912-189">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span>|
|<span data-ttu-id="b3912-190">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-190">simplePinBlocked</span></span>|<span data-ttu-id="b3912-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-191">Boolean</span></span>|<span data-ttu-id="b3912-192">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="b3912-192">Indicates whether simplePin is blocked.</span></span>|
|<span data-ttu-id="b3912-193">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="b3912-193">minimumPinLength</span></span>|<span data-ttu-id="b3912-194">Int32</span><span class="sxs-lookup"><span data-stu-id="b3912-194">Int32</span></span>|<span data-ttu-id="b3912-195">PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。</span><span class="sxs-lookup"><span data-stu-id="b3912-195">Minimum pin length required for an app-level pin if PinRequired is set to True</span></span>|
|<span data-ttu-id="b3912-196">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="b3912-196">pinCharacterSet</span></span>|[<span data-ttu-id="b3912-197">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="b3912-197">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="b3912-198">PinRequired 设置为 True 时可用于应用级 pin 的字符集。</span><span class="sxs-lookup"><span data-stu-id="b3912-198">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="b3912-199">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="b3912-199">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="b3912-200">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="b3912-200">periodBeforePinReset</span></span>|<span data-ttu-id="b3912-201">Duration</span><span class="sxs-lookup"><span data-stu-id="b3912-201">Duration</span></span>|<span data-ttu-id="b3912-202">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。</span><span class="sxs-lookup"><span data-stu-id="b3912-202">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span>|
|<span data-ttu-id="b3912-203">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="b3912-203">allowedDataStorageLocations</span></span>|<span data-ttu-id="b3912-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3912-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="b3912-205">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="b3912-205">Data storage locations where a user may store managed data.</span></span>|
|<span data-ttu-id="b3912-206">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-206">contactSyncBlocked</span></span>|<span data-ttu-id="b3912-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-207">Boolean</span></span>|<span data-ttu-id="b3912-208">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="b3912-208">Indicates whether contacts can be synced to the user's device.</span></span>|
|<span data-ttu-id="b3912-209">printBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-209">printBlocked</span></span>|<span data-ttu-id="b3912-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-210">Boolean</span></span>|<span data-ttu-id="b3912-211">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="b3912-211">Indicates whether printing is allowed from managed apps.</span></span>|
|<span data-ttu-id="b3912-212">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="b3912-212">fingerprintBlocked</span></span>|<span data-ttu-id="b3912-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-213">Boolean</span></span>|<span data-ttu-id="b3912-214">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。</span><span class="sxs-lookup"><span data-stu-id="b3912-214">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="b3912-215">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="b3912-215">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="b3912-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3912-216">Boolean</span></span>|<span data-ttu-id="b3912-217">指示如果设置了设备 pin，是否需要使用应用 pin。</span><span class="sxs-lookup"><span data-stu-id="b3912-217">Indicates whether use of the app pin is required if the device pin is set.</span></span>|
|<span data-ttu-id="b3912-218">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3912-218">minimumRequiredOsVersion</span></span>|<span data-ttu-id="b3912-219">String</span><span class="sxs-lookup"><span data-stu-id="b3912-219">String</span></span>|<span data-ttu-id="b3912-220">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b3912-220">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="b3912-221">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3912-221">minimumWarningOsVersion</span></span>|<span data-ttu-id="b3912-222">String</span><span class="sxs-lookup"><span data-stu-id="b3912-222">String</span></span>|<span data-ttu-id="b3912-223">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="b3912-223">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span>|
|<span data-ttu-id="b3912-224">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="b3912-224">minimumRequiredAppVersion</span></span>|<span data-ttu-id="b3912-225">String</span><span class="sxs-lookup"><span data-stu-id="b3912-225">String</span></span>|<span data-ttu-id="b3912-226">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b3912-226">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="b3912-227">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="b3912-227">minimumWarningAppVersion</span></span>|<span data-ttu-id="b3912-228">String</span><span class="sxs-lookup"><span data-stu-id="b3912-228">String</span></span>|<span data-ttu-id="b3912-229">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="b3912-229">Versions less than the specified version will result in warning message on the managed app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3912-230">关系</span><span class="sxs-lookup"><span data-stu-id="b3912-230">Relationships</span></span>
<span data-ttu-id="b3912-231">无</span><span class="sxs-lookup"><span data-stu-id="b3912-231">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3912-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3912-232">JSON Representation</span></span>
<span data-ttu-id="b3912-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3912-233">Here is a JSON representation of the resource.</span></span>
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

