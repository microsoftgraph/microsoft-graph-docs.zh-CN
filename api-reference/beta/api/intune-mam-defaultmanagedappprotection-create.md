---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0da26a10f0925e3b347d971f303f58aef035b8c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146205"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="b2353-103">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b2353-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="b2353-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2353-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2353-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2353-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2353-106">创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2353-106">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2353-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2353-107">Prerequisites</span></span>
<span data-ttu-id="b2353-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2353-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2353-110">Permission type</span></span>|<span data-ttu-id="b2353-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2353-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2353-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2353-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2353-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2353-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2353-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2353-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2353-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2353-115">Not supported.</span></span>|
|<span data-ttu-id="b2353-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2353-116">Application</span></span>|<span data-ttu-id="b2353-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2353-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2353-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2353-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="b2353-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2353-119">Request headers</span></span>
|<span data-ttu-id="b2353-120">标头</span><span class="sxs-lookup"><span data-stu-id="b2353-120">Header</span></span>|<span data-ttu-id="b2353-121">值</span><span class="sxs-lookup"><span data-stu-id="b2353-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2353-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2353-122">Authorization</span></span>|<span data-ttu-id="b2353-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2353-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2353-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2353-124">Accept</span></span>|<span data-ttu-id="b2353-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2353-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2353-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2353-126">Request body</span></span>
<span data-ttu-id="b2353-127">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2353-127">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="b2353-128">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2353-128">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="b2353-129">属性</span><span class="sxs-lookup"><span data-stu-id="b2353-129">Property</span></span>|<span data-ttu-id="b2353-130">类型</span><span class="sxs-lookup"><span data-stu-id="b2353-130">Type</span></span>|<span data-ttu-id="b2353-131">说明</span><span class="sxs-lookup"><span data-stu-id="b2353-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2353-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b2353-132">displayName</span></span>|<span data-ttu-id="b2353-133">String</span><span class="sxs-lookup"><span data-stu-id="b2353-133">String</span></span>|<span data-ttu-id="b2353-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="b2353-134">Policy display name.</span></span> <span data-ttu-id="b2353-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-136">description</span><span class="sxs-lookup"><span data-stu-id="b2353-136">description</span></span>|<span data-ttu-id="b2353-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-137">String</span></span>|<span data-ttu-id="b2353-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b2353-138">The policy's description.</span></span> <span data-ttu-id="b2353-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2353-140">createdDateTime</span></span>|<span data-ttu-id="b2353-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2353-141">DateTimeOffset</span></span>|<span data-ttu-id="b2353-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b2353-142">The date and time the policy was created.</span></span> <span data-ttu-id="b2353-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2353-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b2353-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2353-145">DateTimeOffset</span></span>|<span data-ttu-id="b2353-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="b2353-146">Last time the policy was modified.</span></span> <span data-ttu-id="b2353-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2353-148">roleScopeTagIds</span></span>|<span data-ttu-id="b2353-149">String collection</span><span class="sxs-lookup"><span data-stu-id="b2353-149">String collection</span></span>|<span data-ttu-id="b2353-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b2353-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2353-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-152">id</span><span class="sxs-lookup"><span data-stu-id="b2353-152">id</span></span>|<span data-ttu-id="b2353-153">字串符号</span><span class="sxs-lookup"><span data-stu-id="b2353-153">String</span></span>|<span data-ttu-id="b2353-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2353-154">Key of the entity.</span></span> <span data-ttu-id="b2353-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-156">version</span><span class="sxs-lookup"><span data-stu-id="b2353-156">version</span></span>|<span data-ttu-id="b2353-157">String</span><span class="sxs-lookup"><span data-stu-id="b2353-157">String</span></span>|<span data-ttu-id="b2353-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b2353-158">Version of the entity.</span></span> <span data-ttu-id="b2353-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b2353-160">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="b2353-160">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="b2353-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="b2353-161">Duration</span></span>|<span data-ttu-id="b2353-162">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="b2353-162">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="b2353-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-164">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="b2353-164">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="b2353-165">Duration</span><span class="sxs-lookup"><span data-stu-id="b2353-165">Duration</span></span>|<span data-ttu-id="b2353-166">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="b2353-166">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="b2353-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-168">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="b2353-168">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="b2353-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="b2353-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="b2353-170">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="b2353-170">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="b2353-171">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-172">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b2353-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="b2353-173">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="b2353-173">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="b2353-174">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="b2353-174">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="b2353-175">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="b2353-175">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="b2353-176">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-177">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b2353-177">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="b2353-178">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="b2353-178">organizationalCredentialsRequired</span></span>|<span data-ttu-id="b2353-179">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-179">Boolean</span></span>|<span data-ttu-id="b2353-180">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="b2353-180">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="b2353-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-182">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b2353-182">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="b2353-183">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="b2353-183">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="b2353-184">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="b2353-184">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="b2353-185">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-186">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="b2353-186">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="b2353-187">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-187">dataBackupBlocked</span></span>|<span data-ttu-id="b2353-188">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-188">Boolean</span></span>|<span data-ttu-id="b2353-189">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-189">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="b2353-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-191">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="b2353-191">deviceComplianceRequired</span></span>|<span data-ttu-id="b2353-192">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-192">Boolean</span></span>|<span data-ttu-id="b2353-193">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="b2353-193">Indicates whether device compliance is required.</span></span> <span data-ttu-id="b2353-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-195">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="b2353-195">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="b2353-196">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-196">Boolean</span></span>|<span data-ttu-id="b2353-197">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="b2353-197">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="b2353-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-199">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-199">saveAsBlocked</span></span>|<span data-ttu-id="b2353-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2353-200">Boolean</span></span>|<span data-ttu-id="b2353-201">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="b2353-201">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="b2353-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-203">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="b2353-203">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="b2353-204">持续时间</span><span class="sxs-lookup"><span data-stu-id="b2353-204">Duration</span></span>|<span data-ttu-id="b2353-205">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="b2353-205">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="b2353-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-207">pinRequired</span><span class="sxs-lookup"><span data-stu-id="b2353-207">pinRequired</span></span>|<span data-ttu-id="b2353-208">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-208">Boolean</span></span>|<span data-ttu-id="b2353-209">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="b2353-209">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="b2353-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-211">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="b2353-211">maximumPinRetries</span></span>|<span data-ttu-id="b2353-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b2353-212">Int32</span></span>|<span data-ttu-id="b2353-213">在阻止或擦除托管应用之前, 不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="b2353-213">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="b2353-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-215">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-215">simplePinBlocked</span></span>|<span data-ttu-id="b2353-216">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-216">Boolean</span></span>|<span data-ttu-id="b2353-217">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="b2353-217">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="b2353-218">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-218">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-219">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="b2353-219">minimumPinLength</span></span>|<span data-ttu-id="b2353-220">Int32</span><span class="sxs-lookup"><span data-stu-id="b2353-220">Int32</span></span>|<span data-ttu-id="b2353-221">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-221">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-222">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="b2353-222">pinCharacterSet</span></span>|[<span data-ttu-id="b2353-223">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="b2353-223">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="b2353-224">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="b2353-224">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="b2353-225">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-226">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="b2353-226">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="b2353-227">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="b2353-227">periodBeforePinReset</span></span>|<span data-ttu-id="b2353-228">Duration</span><span class="sxs-lookup"><span data-stu-id="b2353-228">Duration</span></span>|<span data-ttu-id="b2353-229">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="b2353-229">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="b2353-230">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-231">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="b2353-231">allowedDataStorageLocations</span></span>|<span data-ttu-id="b2353-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="b2353-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="b2353-233">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="b2353-233">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="b2353-234">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-235">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="b2353-235">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="b2353-236">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-236">contactSyncBlocked</span></span>|<span data-ttu-id="b2353-237">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-237">Boolean</span></span>|<span data-ttu-id="b2353-238">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="b2353-238">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="b2353-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-240">printBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-240">printBlocked</span></span>|<span data-ttu-id="b2353-241">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-241">Boolean</span></span>|<span data-ttu-id="b2353-242">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="b2353-242">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="b2353-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-244">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-244">fingerprintBlocked</span></span>|<span data-ttu-id="b2353-245">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-245">Boolean</span></span>|<span data-ttu-id="b2353-246">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="b2353-246">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="b2353-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-248">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="b2353-248">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="b2353-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2353-249">Boolean</span></span>|<span data-ttu-id="b2353-250">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="b2353-250">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="b2353-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-252">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-252">minimumRequiredOsVersion</span></span>|<span data-ttu-id="b2353-253">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-253">String</span></span>|<span data-ttu-id="b2353-254">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-254">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="b2353-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-256">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-256">minimumWarningOsVersion</span></span>|<span data-ttu-id="b2353-257">String</span><span class="sxs-lookup"><span data-stu-id="b2353-257">String</span></span>|<span data-ttu-id="b2353-258">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="b2353-258">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="b2353-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-260">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-260">minimumRequiredAppVersion</span></span>|<span data-ttu-id="b2353-261">String</span><span class="sxs-lookup"><span data-stu-id="b2353-261">String</span></span>|<span data-ttu-id="b2353-262">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-262">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="b2353-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-264">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-264">minimumWarningAppVersion</span></span>|<span data-ttu-id="b2353-265">String</span><span class="sxs-lookup"><span data-stu-id="b2353-265">String</span></span>|<span data-ttu-id="b2353-266">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="b2353-266">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="b2353-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-268">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-268">minimumWipeOsVersion</span></span>|<span data-ttu-id="b2353-269">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-269">String</span></span>|<span data-ttu-id="b2353-270">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-270">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="b2353-271">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-271">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-272">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-272">minimumWipeAppVersion</span></span>|<span data-ttu-id="b2353-273">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-273">String</span></span>|<span data-ttu-id="b2353-274">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-274">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="b2353-275">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="b2353-275">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-276">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="b2353-276">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="b2353-277">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="b2353-277">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="b2353-278">如果将 DeviceComplianceRequired 设置为 true, 则定义在设备为根或已越狱时的托管应用行为 (阻止或擦除)。</span><span class="sxs-lookup"><span data-stu-id="b2353-278">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="b2353-279">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-279">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-280">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="b2353-280">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="b2353-281">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="b2353-281">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="b2353-282">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="b2353-282">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="b2353-283">根据最大错误 pin 重试次数定义托管应用行为, 即阻止或擦除。</span><span class="sxs-lookup"><span data-stu-id="b2353-283">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="b2353-284">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="b2353-284">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="b2353-285">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="b2353-285">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="b2353-286">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="b2353-286">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="b2353-287">持续时间</span><span class="sxs-lookup"><span data-stu-id="b2353-287">Duration</span></span>|<span data-ttu-id="b2353-288">以分钟为单位的应用程序 pin (而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)继承的无生物特征密码) 超时</span><span class="sxs-lookup"><span data-stu-id="b2353-288">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="b2353-289">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="b2353-289">appDataEncryptionType</span></span>|[<span data-ttu-id="b2353-290">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="b2353-290">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="b2353-291">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="b2353-291">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="b2353-292">(仅限 iOS)。</span><span class="sxs-lookup"><span data-stu-id="b2353-292">(iOS Only).</span></span> <span data-ttu-id="b2353-293">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="b2353-293">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="b2353-294">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-294">screenCaptureBlocked</span></span>|<span data-ttu-id="b2353-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2353-295">Boolean</span></span>|<span data-ttu-id="b2353-296">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b2353-296">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="b2353-297">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-297">(Android only)</span></span>|
|<span data-ttu-id="b2353-298">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="b2353-298">encryptAppData</span></span>|<span data-ttu-id="b2353-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2353-299">Boolean</span></span>|<span data-ttu-id="b2353-300">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-300">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="b2353-301">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-301">(Android only)</span></span>|
|<span data-ttu-id="b2353-302">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="b2353-302">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="b2353-303">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-303">Boolean</span></span>|<span data-ttu-id="b2353-304">如果启用此设置, 则在启用设备级加密的情况下禁用应用级加密。</span><span class="sxs-lookup"><span data-stu-id="b2353-304">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="b2353-305">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-305">(Android only)</span></span>|
|<span data-ttu-id="b2353-306">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-306">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="b2353-307">String</span><span class="sxs-lookup"><span data-stu-id="b2353-307">String</span></span>|<span data-ttu-id="b2353-308">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-308">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="b2353-309">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-309">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-310">customSettings</span><span class="sxs-lookup"><span data-stu-id="b2353-310">customSettings</span></span>|<span data-ttu-id="b2353-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2353-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b2353-312">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="b2353-312">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="b2353-313">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="b2353-313">deployedAppCount</span></span>|<span data-ttu-id="b2353-314">Int32</span><span class="sxs-lookup"><span data-stu-id="b2353-314">Int32</span></span>|<span data-ttu-id="b2353-315">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="b2353-315">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="b2353-316">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-316">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="b2353-317">String</span><span class="sxs-lookup"><span data-stu-id="b2353-317">String</span></span>|<span data-ttu-id="b2353-318">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="b2353-318">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="b2353-319">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-319">(Android only)</span></span>|
|<span data-ttu-id="b2353-320">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-320">minimumWarningPatchVersion</span></span>|<span data-ttu-id="b2353-321">String</span><span class="sxs-lookup"><span data-stu-id="b2353-321">String</span></span>|<span data-ttu-id="b2353-322">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="b2353-322">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="b2353-323">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-323">(Android only)</span></span>|
|<span data-ttu-id="b2353-324">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="b2353-324">exemptedAppProtocols</span></span>|<span data-ttu-id="b2353-325">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2353-325">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b2353-326">此列表中的 iOS 应用程序将不受策略的阻止, 并且将能够从托管应用接收数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-326">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="b2353-327">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-327">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-328">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="b2353-328">exemptedAppPackages</span></span>|<span data-ttu-id="b2353-329">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2353-329">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b2353-330">此列表中的 Android 应用程序包将从该策略中排除, 并且将能够从托管应用接收数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-330">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="b2353-331">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-331">(Android only)</span></span>|
|<span data-ttu-id="b2353-332">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-332">faceIdBlocked</span></span>|<span data-ttu-id="b2353-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2353-333">Boolean</span></span>|<span data-ttu-id="b2353-334">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。</span><span class="sxs-lookup"><span data-stu-id="b2353-334">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="b2353-335">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-335">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-336">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-336">minimumWipeSdkVersion</span></span>|<span data-ttu-id="b2353-337">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-337">String</span></span>|<span data-ttu-id="b2353-338">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-338">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="b2353-339">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="b2353-339">minimumWipePatchVersion</span></span>|<span data-ttu-id="b2353-340">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-340">String</span></span>|<span data-ttu-id="b2353-341">Android 安全修补程序级别小于或等于指定值将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-341">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="b2353-342">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-342">(Android only)</span></span>|
|<span data-ttu-id="b2353-343">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="b2353-343">allowedIosDeviceModels</span></span>|<span data-ttu-id="b2353-344">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-344">String</span></span>|<span data-ttu-id="b2353-345">允许托管应用使用的设备模型的以分号分隔的列表 (以字符串形式)。</span><span class="sxs-lookup"><span data-stu-id="b2353-345">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="b2353-346">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-346">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-347">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="b2353-347">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="b2353-348">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="b2353-348">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="b2353-349">定义托管应用程序行为, 如果不允许指定的设备模型, 则要么阻止, 也可以擦除。</span><span class="sxs-lookup"><span data-stu-id="b2353-349">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="b2353-350">(仅限 iOS)。</span><span class="sxs-lookup"><span data-stu-id="b2353-350">(iOS Only).</span></span> <span data-ttu-id="b2353-351">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="b2353-351">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="b2353-352">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="b2353-352">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="b2353-353">字符串</span><span class="sxs-lookup"><span data-stu-id="b2353-353">String</span></span>|<span data-ttu-id="b2353-354">允许托管应用使用的设备制造商以分号分隔的列表, 以字符串形式提供。</span><span class="sxs-lookup"><span data-stu-id="b2353-354">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="b2353-355">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="b2353-355">(Android only)</span></span>|
|<span data-ttu-id="b2353-356">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="b2353-356">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="b2353-357">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="b2353-357">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="b2353-358">如果不允许指定的设备制造商, 则定义托管应用行为 (无论是阻止还是擦除)。</span><span class="sxs-lookup"><span data-stu-id="b2353-358">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="b2353-359">(仅限 Android)。</span><span class="sxs-lookup"><span data-stu-id="b2353-359">(Android only).</span></span> <span data-ttu-id="b2353-360">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="b2353-360">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="b2353-361">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="b2353-361">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="b2353-362">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-362">Boolean</span></span>|<span data-ttu-id="b2353-363">定义在访问托管应用程序时是否允许使用第三方键盘。</span><span class="sxs-lookup"><span data-stu-id="b2353-363">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="b2353-364">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-364">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-365">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="b2353-365">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="b2353-366">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-366">Boolean</span></span>|<span data-ttu-id="b2353-367">定义是否支持从受管理的应用程序到所选的可共享位置的打开入点操作。</span><span class="sxs-lookup"><span data-stu-id="b2353-367">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="b2353-368">此设置仅适用于将 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 和 DisableProtectionOfManagedOutboundOpenInData 设置为 False 的情况。</span><span class="sxs-lookup"><span data-stu-id="b2353-368">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="b2353-369">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-369">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-370">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="b2353-370">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="b2353-371">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-371">Boolean</span></span>|<span data-ttu-id="b2353-372">禁用通过 IOS OpenIn 选项传输到其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="b2353-372">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="b2353-373">仅当 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 时, 此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="b2353-373">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="b2353-374">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-374">(iOS Only)</span></span>|
|<span data-ttu-id="b2353-375">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b2353-375">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="b2353-376">布尔</span><span class="sxs-lookup"><span data-stu-id="b2353-376">Boolean</span></span>|<span data-ttu-id="b2353-377">保护来自未知源的传入数据。</span><span class="sxs-lookup"><span data-stu-id="b2353-377">Protect incoming data from unknown source.</span></span> <span data-ttu-id="b2353-378">仅当 AllowedInboundDataTransferSources 设置为 AllApps 时, 此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="b2353-378">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="b2353-379">(仅限 iOS)</span><span class="sxs-lookup"><span data-stu-id="b2353-379">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="b2353-380">响应</span><span class="sxs-lookup"><span data-stu-id="b2353-380">Response</span></span>
<span data-ttu-id="b2353-381">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2353-381">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2353-382">示例</span><span class="sxs-lookup"><span data-stu-id="b2353-382">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2353-383">请求</span><span class="sxs-lookup"><span data-stu-id="b2353-383">Request</span></span>
<span data-ttu-id="b2353-384">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2353-384">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 3217

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="b2353-385">响应</span><span class="sxs-lookup"><span data-stu-id="b2353-385">Response</span></span>
<span data-ttu-id="b2353-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2353-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3389

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```




