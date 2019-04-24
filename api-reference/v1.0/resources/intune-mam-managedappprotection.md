---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b97b4b1453253ecd6fc5b5d77515b8b28586b19f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465228"
---
# <a name="managedappprotection-resource-type"></a><span data-ttu-id="2ad41-103">managedAppProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ad41-103">managedAppProtection resource type</span></span>

> <span data-ttu-id="2ad41-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ad41-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad41-105">用于为指定的一组应用配置详细管理设置的策略</span><span class="sxs-lookup"><span data-stu-id="2ad41-105">Policy used to configure detailed management settings for a specified set of apps</span></span>


<span data-ttu-id="2ad41-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2ad41-107">方法</span><span class="sxs-lookup"><span data-stu-id="2ad41-107">Methods</span></span>
|<span data-ttu-id="2ad41-108">方法</span><span class="sxs-lookup"><span data-stu-id="2ad41-108">Method</span></span>|<span data-ttu-id="2ad41-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ad41-109">Return Type</span></span>|<span data-ttu-id="2ad41-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ad41-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ad41-111">List managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="2ad41-111">List managedAppProtections</span></span>](../api/intune-mam-managedappprotection-list.md)|<span data-ttu-id="2ad41-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ad41-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) collection</span></span>|<span data-ttu-id="2ad41-113">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ad41-113">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="2ad41-114">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="2ad41-114">Get managedAppProtection</span></span>](../api/intune-mam-managedappprotection-get.md)|[<span data-ttu-id="2ad41-115">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="2ad41-115">managedAppProtection</span></span>](../resources/intune-mam-managedappprotection.md)|<span data-ttu-id="2ad41-116">读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ad41-116">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>|
|[<span data-ttu-id="2ad41-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="2ad41-117">targetApps action</span></span>](../api/intune-mam-managedappprotection-targetapps.md)|<span data-ttu-id="2ad41-118">无</span><span class="sxs-lookup"><span data-stu-id="2ad41-118">None</span></span>|<span data-ttu-id="2ad41-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ad41-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ad41-120">属性</span><span class="sxs-lookup"><span data-stu-id="2ad41-120">Properties</span></span>
|<span data-ttu-id="2ad41-121">属性</span><span class="sxs-lookup"><span data-stu-id="2ad41-121">Property</span></span>|<span data-ttu-id="2ad41-122">类型</span><span class="sxs-lookup"><span data-stu-id="2ad41-122">Type</span></span>|<span data-ttu-id="2ad41-123">说明</span><span class="sxs-lookup"><span data-stu-id="2ad41-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad41-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad41-124">displayName</span></span>|<span data-ttu-id="2ad41-125">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad41-125">String</span></span>|<span data-ttu-id="2ad41-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ad41-126">Policy display name.</span></span> <span data-ttu-id="2ad41-127">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-128">description</span><span class="sxs-lookup"><span data-stu-id="2ad41-128">description</span></span>|<span data-ttu-id="2ad41-129">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad41-129">String</span></span>|<span data-ttu-id="2ad41-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="2ad41-130">The policy's description.</span></span> <span data-ttu-id="2ad41-131">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad41-132">createdDateTime</span></span>|<span data-ttu-id="2ad41-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad41-133">DateTimeOffset</span></span>|<span data-ttu-id="2ad41-134">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ad41-134">The date and time the policy was created.</span></span> <span data-ttu-id="2ad41-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad41-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ad41-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad41-137">DateTimeOffset</span></span>|<span data-ttu-id="2ad41-138">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="2ad41-138">Last time the policy was modified.</span></span> <span data-ttu-id="2ad41-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-140">id</span><span class="sxs-lookup"><span data-stu-id="2ad41-140">id</span></span>|<span data-ttu-id="2ad41-141">String</span><span class="sxs-lookup"><span data-stu-id="2ad41-141">String</span></span>|<span data-ttu-id="2ad41-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2ad41-142">Key of the entity.</span></span> <span data-ttu-id="2ad41-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-144">version</span><span class="sxs-lookup"><span data-stu-id="2ad41-144">version</span></span>|<span data-ttu-id="2ad41-145">String</span><span class="sxs-lookup"><span data-stu-id="2ad41-145">String</span></span>|<span data-ttu-id="2ad41-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2ad41-146">Version of the entity.</span></span> <span data-ttu-id="2ad41-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad41-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2ad41-148">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2ad41-148">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="2ad41-149">持续时间</span><span class="sxs-lookup"><span data-stu-id="2ad41-149">Duration</span></span>|<span data-ttu-id="2ad41-150">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="2ad41-150">The period after which access is checked when the device is not connected to the internet.</span></span>|
|<span data-ttu-id="2ad41-151">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="2ad41-151">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="2ad41-152">持续时间</span><span class="sxs-lookup"><span data-stu-id="2ad41-152">Duration</span></span>|<span data-ttu-id="2ad41-153">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="2ad41-153">The period after which access is checked when the device is connected to the internet.</span></span>|
|<span data-ttu-id="2ad41-154">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="2ad41-154">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="2ad41-155">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="2ad41-155">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="2ad41-156">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="2ad41-156">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="2ad41-157">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="2ad41-157">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2ad41-158">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="2ad41-158">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="2ad41-159">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="2ad41-159">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="2ad41-160">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="2ad41-160">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="2ad41-161">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="2ad41-161">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="2ad41-162">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="2ad41-162">organizationalCredentialsRequired</span></span>|<span data-ttu-id="2ad41-163">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-163">Boolean</span></span>|<span data-ttu-id="2ad41-164">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="2ad41-164">Indicates whether organizational credentials are required for app use.</span></span>|
|<span data-ttu-id="2ad41-165">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2ad41-165">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="2ad41-166">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2ad41-166">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="2ad41-167">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="2ad41-167">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="2ad41-168">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="2ad41-168">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="2ad41-169">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-169">dataBackupBlocked</span></span>|<span data-ttu-id="2ad41-170">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-170">Boolean</span></span>|<span data-ttu-id="2ad41-171">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="2ad41-171">Indicates whether the backup of a managed app's data is blocked.</span></span>|
|<span data-ttu-id="2ad41-172">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="2ad41-172">deviceComplianceRequired</span></span>|<span data-ttu-id="2ad41-173">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-173">Boolean</span></span>|<span data-ttu-id="2ad41-174">指示是否需要设备合规性。</span><span class="sxs-lookup"><span data-stu-id="2ad41-174">Indicates whether device compliance is required.</span></span>|
|<span data-ttu-id="2ad41-175">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="2ad41-175">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="2ad41-176">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-176">Boolean</span></span>|<span data-ttu-id="2ad41-177">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="2ad41-177">Indicates whether internet links should be opened in the managed browser app.</span></span>|
|<span data-ttu-id="2ad41-178">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-178">saveAsBlocked</span></span>|<span data-ttu-id="2ad41-179">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-179">Boolean</span></span>|<span data-ttu-id="2ad41-180">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="2ad41-180">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span>|
|<span data-ttu-id="2ad41-181">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="2ad41-181">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="2ad41-182">持续时间</span><span class="sxs-lookup"><span data-stu-id="2ad41-182">Duration</span></span>|<span data-ttu-id="2ad41-183">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="2ad41-183">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span>|
|<span data-ttu-id="2ad41-184">pinRequired</span><span class="sxs-lookup"><span data-stu-id="2ad41-184">pinRequired</span></span>|<span data-ttu-id="2ad41-185">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-185">Boolean</span></span>|<span data-ttu-id="2ad41-186">指示是否需要应用级 pin。</span><span class="sxs-lookup"><span data-stu-id="2ad41-186">Indicates whether an app-level pin is required.</span></span>|
|<span data-ttu-id="2ad41-187">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="2ad41-187">maximumPinRetries</span></span>|<span data-ttu-id="2ad41-188">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad41-188">Int32</span></span>|<span data-ttu-id="2ad41-189">在阻止或擦除托管应用之前, 不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="2ad41-189">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span>|
|<span data-ttu-id="2ad41-190">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-190">simplePinBlocked</span></span>|<span data-ttu-id="2ad41-191">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-191">Boolean</span></span>|<span data-ttu-id="2ad41-192">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="2ad41-192">Indicates whether simplePin is blocked.</span></span>|
|<span data-ttu-id="2ad41-193">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="2ad41-193">minimumPinLength</span></span>|<span data-ttu-id="2ad41-194">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad41-194">Int32</span></span>|<span data-ttu-id="2ad41-195">PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。</span><span class="sxs-lookup"><span data-stu-id="2ad41-195">Minimum pin length required for an app-level pin if PinRequired is set to True</span></span>|
|<span data-ttu-id="2ad41-196">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="2ad41-196">pinCharacterSet</span></span>|[<span data-ttu-id="2ad41-197">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="2ad41-197">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="2ad41-198">PinRequired 设置为 True 时可用于应用级 pin 的字符集。</span><span class="sxs-lookup"><span data-stu-id="2ad41-198">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="2ad41-199">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="2ad41-199">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="2ad41-200">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="2ad41-200">periodBeforePinReset</span></span>|<span data-ttu-id="2ad41-201">Duration</span><span class="sxs-lookup"><span data-stu-id="2ad41-201">Duration</span></span>|<span data-ttu-id="2ad41-202">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。</span><span class="sxs-lookup"><span data-stu-id="2ad41-202">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span>|
|<span data-ttu-id="2ad41-203">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="2ad41-203">allowedDataStorageLocations</span></span>|<span data-ttu-id="2ad41-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ad41-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="2ad41-205">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="2ad41-205">Data storage locations where a user may store managed data.</span></span>|
|<span data-ttu-id="2ad41-206">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-206">contactSyncBlocked</span></span>|<span data-ttu-id="2ad41-207">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-207">Boolean</span></span>|<span data-ttu-id="2ad41-208">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="2ad41-208">Indicates whether contacts can be synced to the user's device.</span></span>|
|<span data-ttu-id="2ad41-209">printBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-209">printBlocked</span></span>|<span data-ttu-id="2ad41-210">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad41-210">Boolean</span></span>|<span data-ttu-id="2ad41-211">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="2ad41-211">Indicates whether printing is allowed from managed apps.</span></span>|
|<span data-ttu-id="2ad41-212">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="2ad41-212">fingerprintBlocked</span></span>|<span data-ttu-id="2ad41-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad41-213">Boolean</span></span>|<span data-ttu-id="2ad41-214">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。</span><span class="sxs-lookup"><span data-stu-id="2ad41-214">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="2ad41-215">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="2ad41-215">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="2ad41-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad41-216">Boolean</span></span>|<span data-ttu-id="2ad41-217">指示如果设置了设备 pin，是否需要使用应用 pin。</span><span class="sxs-lookup"><span data-stu-id="2ad41-217">Indicates whether use of the app pin is required if the device pin is set.</span></span>|
|<span data-ttu-id="2ad41-218">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ad41-218">minimumRequiredOsVersion</span></span>|<span data-ttu-id="2ad41-219">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad41-219">String</span></span>|<span data-ttu-id="2ad41-220">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="2ad41-220">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2ad41-221">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ad41-221">minimumWarningOsVersion</span></span>|<span data-ttu-id="2ad41-222">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad41-222">String</span></span>|<span data-ttu-id="2ad41-223">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="2ad41-223">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2ad41-224">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="2ad41-224">minimumRequiredAppVersion</span></span>|<span data-ttu-id="2ad41-225">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad41-225">String</span></span>|<span data-ttu-id="2ad41-226">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="2ad41-226">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="2ad41-227">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="2ad41-227">minimumWarningAppVersion</span></span>|<span data-ttu-id="2ad41-228">String</span><span class="sxs-lookup"><span data-stu-id="2ad41-228">String</span></span>|<span data-ttu-id="2ad41-229">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="2ad41-229">Versions less than the specified version will result in warning message on the managed app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ad41-230">关系</span><span class="sxs-lookup"><span data-stu-id="2ad41-230">Relationships</span></span>
<span data-ttu-id="2ad41-231">无</span><span class="sxs-lookup"><span data-stu-id="2ad41-231">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ad41-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ad41-232">JSON Representation</span></span>
<span data-ttu-id="2ad41-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ad41-233">Here is a JSON representation of the resource.</span></span>
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

