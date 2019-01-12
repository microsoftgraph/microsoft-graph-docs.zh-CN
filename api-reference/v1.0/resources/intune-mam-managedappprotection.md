---
title: managedAppProtection 资源类型
description: 用于为指定的一组应用配置详细管理设置的策略
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad18cf543fa34dc4e44e6afe747bd2da9bcc487a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939880"
---
# <a name="managedappprotection-resource-type"></a><span data-ttu-id="9f0f7-103">managedAppProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f0f7-103">managedAppProtection resource type</span></span>

> <span data-ttu-id="9f0f7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f0f7-105">用于为指定的一组应用配置详细管理设置的策略</span><span class="sxs-lookup"><span data-stu-id="9f0f7-105">Policy used to configure detailed management settings for a specified set of apps</span></span>

<span data-ttu-id="9f0f7-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9f0f7-107">方法</span><span class="sxs-lookup"><span data-stu-id="9f0f7-107">Methods</span></span>
|<span data-ttu-id="9f0f7-108">方法</span><span class="sxs-lookup"><span data-stu-id="9f0f7-108">Method</span></span>|<span data-ttu-id="9f0f7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f0f7-109">Return Type</span></span>|<span data-ttu-id="9f0f7-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f0f7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f0f7-111">List managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="9f0f7-111">List managedAppProtections</span></span>](../api/intune-mam-managedappprotection-list.md)|<span data-ttu-id="9f0f7-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f0f7-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) collection</span></span>|<span data-ttu-id="9f0f7-113">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-113">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="9f0f7-114">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="9f0f7-114">Get managedAppProtection</span></span>](../api/intune-mam-managedappprotection-get.md)|[<span data-ttu-id="9f0f7-115">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="9f0f7-115">managedAppProtection</span></span>](../resources/intune-mam-managedappprotection.md)|<span data-ttu-id="9f0f7-116">读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-116">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>|
|[<span data-ttu-id="9f0f7-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="9f0f7-117">targetApps action</span></span>](../api/intune-mam-managedappprotection-targetapps.md)|<span data-ttu-id="9f0f7-118">无</span><span class="sxs-lookup"><span data-stu-id="9f0f7-118">None</span></span>|<span data-ttu-id="9f0f7-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9f0f7-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9f0f7-120">属性</span><span class="sxs-lookup"><span data-stu-id="9f0f7-120">Properties</span></span>
|<span data-ttu-id="9f0f7-121">属性</span><span class="sxs-lookup"><span data-stu-id="9f0f7-121">Property</span></span>|<span data-ttu-id="9f0f7-122">类型</span><span class="sxs-lookup"><span data-stu-id="9f0f7-122">Type</span></span>|<span data-ttu-id="9f0f7-123">说明</span><span class="sxs-lookup"><span data-stu-id="9f0f7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f0f7-124">displayName</span><span class="sxs-lookup"><span data-stu-id="9f0f7-124">displayName</span></span>|<span data-ttu-id="9f0f7-125">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-125">String</span></span>|<span data-ttu-id="9f0f7-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-126">Policy display name.</span></span> <span data-ttu-id="9f0f7-127">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-128">description</span><span class="sxs-lookup"><span data-stu-id="9f0f7-128">description</span></span>|<span data-ttu-id="9f0f7-129">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-129">String</span></span>|<span data-ttu-id="9f0f7-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-130">The policy's description.</span></span> <span data-ttu-id="9f0f7-131">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f0f7-132">createdDateTime</span></span>|<span data-ttu-id="9f0f7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f0f7-133">DateTimeOffset</span></span>|<span data-ttu-id="9f0f7-134">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-134">The date and time the policy was created.</span></span> <span data-ttu-id="9f0f7-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f0f7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9f0f7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f0f7-137">DateTimeOffset</span></span>|<span data-ttu-id="9f0f7-138">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-138">Last time the policy was modified.</span></span> <span data-ttu-id="9f0f7-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-140">id</span><span class="sxs-lookup"><span data-stu-id="9f0f7-140">id</span></span>|<span data-ttu-id="9f0f7-141">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-141">String</span></span>|<span data-ttu-id="9f0f7-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-142">Key of the entity.</span></span> <span data-ttu-id="9f0f7-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-144">version</span><span class="sxs-lookup"><span data-stu-id="9f0f7-144">version</span></span>|<span data-ttu-id="9f0f7-145">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-145">String</span></span>|<span data-ttu-id="9f0f7-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-146">Version of the entity.</span></span> <span data-ttu-id="9f0f7-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f0f7-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f0f7-148">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="9f0f7-148">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="9f0f7-149">Duration</span><span class="sxs-lookup"><span data-stu-id="9f0f7-149">Duration</span></span>|<span data-ttu-id="9f0f7-150">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-150">The period after which access is checked when the device is not connected to the internet.</span></span>|
|<span data-ttu-id="9f0f7-151">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="9f0f7-151">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="9f0f7-152">Duration</span><span class="sxs-lookup"><span data-stu-id="9f0f7-152">Duration</span></span>|<span data-ttu-id="9f0f7-153">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-153">The period after which access is checked when the device is connected to the internet.</span></span>|
|<span data-ttu-id="9f0f7-154">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="9f0f7-154">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="9f0f7-155">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="9f0f7-155">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="9f0f7-156">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-156">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="9f0f7-157">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-157">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="9f0f7-158">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="9f0f7-158">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="9f0f7-159">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="9f0f7-159">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="9f0f7-160">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-160">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="9f0f7-161">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-161">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="9f0f7-162">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="9f0f7-162">organizationalCredentialsRequired</span></span>|<span data-ttu-id="9f0f7-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-163">Boolean</span></span>|<span data-ttu-id="9f0f7-164">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-164">Indicates whether organizational credentials are required for app use.</span></span>|
|<span data-ttu-id="9f0f7-165">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="9f0f7-165">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="9f0f7-166">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="9f0f7-166">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="9f0f7-167">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-167">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="9f0f7-168">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-168">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="9f0f7-169">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-169">dataBackupBlocked</span></span>|<span data-ttu-id="9f0f7-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-170">Boolean</span></span>|<span data-ttu-id="9f0f7-171">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-171">Indicates whether the backup of a managed app's data is blocked.</span></span>|
|<span data-ttu-id="9f0f7-172">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="9f0f7-172">deviceComplianceRequired</span></span>|<span data-ttu-id="9f0f7-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-173">Boolean</span></span>|<span data-ttu-id="9f0f7-174">指示是否需要设备合规性。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-174">Indicates whether device compliance is required.</span></span>|
|<span data-ttu-id="9f0f7-175">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="9f0f7-175">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="9f0f7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-176">Boolean</span></span>|<span data-ttu-id="9f0f7-177">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-177">Indicates whether internet links should be opened in the managed browser app.</span></span>|
|<span data-ttu-id="9f0f7-178">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-178">saveAsBlocked</span></span>|<span data-ttu-id="9f0f7-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-179">Boolean</span></span>|<span data-ttu-id="9f0f7-180">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-180">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span>|
|<span data-ttu-id="9f0f7-181">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="9f0f7-181">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="9f0f7-182">Duration</span><span class="sxs-lookup"><span data-stu-id="9f0f7-182">Duration</span></span>|<span data-ttu-id="9f0f7-183">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-183">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span>|
|<span data-ttu-id="9f0f7-184">pinRequired</span><span class="sxs-lookup"><span data-stu-id="9f0f7-184">pinRequired</span></span>|<span data-ttu-id="9f0f7-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-185">Boolean</span></span>|<span data-ttu-id="9f0f7-186">指示是否需要应用级 pin。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-186">Indicates whether an app-level pin is required.</span></span>|
|<span data-ttu-id="9f0f7-187">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="9f0f7-187">maximumPinRetries</span></span>|<span data-ttu-id="9f0f7-188">Int32</span><span class="sxs-lookup"><span data-stu-id="9f0f7-188">Int32</span></span>|<span data-ttu-id="9f0f7-189">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-189">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span>|
|<span data-ttu-id="9f0f7-190">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-190">simplePinBlocked</span></span>|<span data-ttu-id="9f0f7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-191">Boolean</span></span>|<span data-ttu-id="9f0f7-192">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-192">Indicates whether simplePin is blocked.</span></span>|
|<span data-ttu-id="9f0f7-193">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="9f0f7-193">minimumPinLength</span></span>|<span data-ttu-id="9f0f7-194">Int32</span><span class="sxs-lookup"><span data-stu-id="9f0f7-194">Int32</span></span>|<span data-ttu-id="9f0f7-195">PinRequired 设置为 True 时应用级 pin 所需的最小 pin 长度。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-195">Minimum pin length required for an app-level pin if PinRequired is set to True</span></span>|
|<span data-ttu-id="9f0f7-196">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="9f0f7-196">pinCharacterSet</span></span>|[<span data-ttu-id="9f0f7-197">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="9f0f7-197">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="9f0f7-198">PinRequired 设置为 True 时可用于应用级 pin 的字符集。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-198">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="9f0f7-199">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-199">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="9f0f7-200">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="9f0f7-200">periodBeforePinReset</span></span>|<span data-ttu-id="9f0f7-201">Duration</span><span class="sxs-lookup"><span data-stu-id="9f0f7-201">Duration</span></span>|<span data-ttu-id="9f0f7-202">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 pin。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-202">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span>|
|<span data-ttu-id="9f0f7-203">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="9f0f7-203">allowedDataStorageLocations</span></span>|<span data-ttu-id="9f0f7-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="9f0f7-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="9f0f7-205">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-205">Data storage locations where a user may store managed data.</span></span>|
|<span data-ttu-id="9f0f7-206">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-206">contactSyncBlocked</span></span>|<span data-ttu-id="9f0f7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-207">Boolean</span></span>|<span data-ttu-id="9f0f7-208">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-208">Indicates whether contacts can be synced to the user's device.</span></span>|
|<span data-ttu-id="9f0f7-209">printBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-209">printBlocked</span></span>|<span data-ttu-id="9f0f7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-210">Boolean</span></span>|<span data-ttu-id="9f0f7-211">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-211">Indicates whether printing is allowed from managed apps.</span></span>|
|<span data-ttu-id="9f0f7-212">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="9f0f7-212">fingerprintBlocked</span></span>|<span data-ttu-id="9f0f7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-213">Boolean</span></span>|<span data-ttu-id="9f0f7-214">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 pin。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-214">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="9f0f7-215">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="9f0f7-215">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="9f0f7-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f0f7-216">Boolean</span></span>|<span data-ttu-id="9f0f7-217">指示如果设置了设备 pin，是否需要使用应用 pin。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-217">Indicates whether use of the app pin is required if the device pin is set.</span></span>|
|<span data-ttu-id="9f0f7-218">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f0f7-218">minimumRequiredOsVersion</span></span>|<span data-ttu-id="9f0f7-219">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-219">String</span></span>|<span data-ttu-id="9f0f7-220">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-220">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="9f0f7-221">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f0f7-221">minimumWarningOsVersion</span></span>|<span data-ttu-id="9f0f7-222">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-222">String</span></span>|<span data-ttu-id="9f0f7-223">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-223">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span>|
|<span data-ttu-id="9f0f7-224">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="9f0f7-224">minimumRequiredAppVersion</span></span>|<span data-ttu-id="9f0f7-225">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-225">String</span></span>|<span data-ttu-id="9f0f7-226">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-226">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="9f0f7-227">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="9f0f7-227">minimumWarningAppVersion</span></span>|<span data-ttu-id="9f0f7-228">String</span><span class="sxs-lookup"><span data-stu-id="9f0f7-228">String</span></span>|<span data-ttu-id="9f0f7-229">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-229">Versions less than the specified version will result in warning message on the managed app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f0f7-230">关系</span><span class="sxs-lookup"><span data-stu-id="9f0f7-230">Relationships</span></span>
<span data-ttu-id="9f0f7-231">无</span><span class="sxs-lookup"><span data-stu-id="9f0f7-231">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f0f7-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f0f7-232">JSON Representation</span></span>
<span data-ttu-id="9f0f7-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f0f7-233">Here is a JSON representation of the resource.</span></span>
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


