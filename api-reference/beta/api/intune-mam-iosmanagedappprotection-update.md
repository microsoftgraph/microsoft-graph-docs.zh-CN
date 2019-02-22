---
title: 更新 iosManagedAppProtection
description: 更新 iosManagedAppProtection 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a528b5e7b2fb986ef65fbf1e15ff57386b96d44e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174226"
---
# <a name="update-iosmanagedappprotection"></a><span data-ttu-id="15173-103">更新 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="15173-103">Update iosManagedAppProtection</span></span>

> <span data-ttu-id="15173-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15173-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15173-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15173-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15173-106">更新 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15173-106">Update the properties of a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15173-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="15173-107">Prerequisites</span></span>
<span data-ttu-id="15173-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15173-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="15173-110">Permission type</span></span>|<span data-ttu-id="15173-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="15173-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15173-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15173-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15173-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15173-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15173-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15173-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15173-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="15173-115">Not supported.</span></span>|
|<span data-ttu-id="15173-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="15173-116">Application</span></span>|<span data-ttu-id="15173-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="15173-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15173-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15173-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="15173-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="15173-119">Request headers</span></span>
|<span data-ttu-id="15173-120">标头</span><span class="sxs-lookup"><span data-stu-id="15173-120">Header</span></span>|<span data-ttu-id="15173-121">值</span><span class="sxs-lookup"><span data-stu-id="15173-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15173-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15173-122">Authorization</span></span>|<span data-ttu-id="15173-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="15173-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15173-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15173-124">Accept</span></span>|<span data-ttu-id="15173-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15173-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15173-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="15173-126">Request body</span></span>
<span data-ttu-id="15173-127">在请求正文中，提供 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15173-127">In the request body, supply a JSON representation for the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

<span data-ttu-id="15173-128">下表显示创建 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="15173-128">The following table shows the properties that are required when you create the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span></span>

|<span data-ttu-id="15173-129">属性</span><span class="sxs-lookup"><span data-stu-id="15173-129">Property</span></span>|<span data-ttu-id="15173-130">类型</span><span class="sxs-lookup"><span data-stu-id="15173-130">Type</span></span>|<span data-ttu-id="15173-131">说明</span><span class="sxs-lookup"><span data-stu-id="15173-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15173-132">displayName</span><span class="sxs-lookup"><span data-stu-id="15173-132">displayName</span></span>|<span data-ttu-id="15173-133">String</span><span class="sxs-lookup"><span data-stu-id="15173-133">String</span></span>|<span data-ttu-id="15173-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="15173-134">Policy display name.</span></span> <span data-ttu-id="15173-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-136">description</span><span class="sxs-lookup"><span data-stu-id="15173-136">description</span></span>|<span data-ttu-id="15173-137">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-137">String</span></span>|<span data-ttu-id="15173-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="15173-138">The policy's description.</span></span> <span data-ttu-id="15173-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15173-140">createdDateTime</span></span>|<span data-ttu-id="15173-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15173-141">DateTimeOffset</span></span>|<span data-ttu-id="15173-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="15173-142">The date and time the policy was created.</span></span> <span data-ttu-id="15173-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15173-144">lastModifiedDateTime</span></span>|<span data-ttu-id="15173-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15173-145">DateTimeOffset</span></span>|<span data-ttu-id="15173-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="15173-146">Last time the policy was modified.</span></span> <span data-ttu-id="15173-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15173-148">roleScopeTagIds</span></span>|<span data-ttu-id="15173-149">String collection</span><span class="sxs-lookup"><span data-stu-id="15173-149">String collection</span></span>|<span data-ttu-id="15173-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="15173-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15173-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-152">id</span><span class="sxs-lookup"><span data-stu-id="15173-152">id</span></span>|<span data-ttu-id="15173-153">字串符号</span><span class="sxs-lookup"><span data-stu-id="15173-153">String</span></span>|<span data-ttu-id="15173-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="15173-154">Key of the entity.</span></span> <span data-ttu-id="15173-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-156">version</span><span class="sxs-lookup"><span data-stu-id="15173-156">version</span></span>|<span data-ttu-id="15173-157">String</span><span class="sxs-lookup"><span data-stu-id="15173-157">String</span></span>|<span data-ttu-id="15173-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="15173-158">Version of the entity.</span></span> <span data-ttu-id="15173-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15173-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="15173-160">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="15173-160">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="15173-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="15173-161">Duration</span></span>|<span data-ttu-id="15173-162">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="15173-162">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="15173-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-164">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="15173-164">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="15173-165">Duration</span><span class="sxs-lookup"><span data-stu-id="15173-165">Duration</span></span>|<span data-ttu-id="15173-166">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="15173-166">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="15173-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-168">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="15173-168">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="15173-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="15173-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="15173-170">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="15173-170">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="15173-171">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-172">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="15173-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="15173-173">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="15173-173">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="15173-174">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="15173-174">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="15173-175">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="15173-175">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="15173-176">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-177">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="15173-177">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="15173-178">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="15173-178">organizationalCredentialsRequired</span></span>|<span data-ttu-id="15173-179">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-179">Boolean</span></span>|<span data-ttu-id="15173-180">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="15173-180">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="15173-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-182">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="15173-182">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="15173-183">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="15173-183">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="15173-184">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="15173-184">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="15173-185">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-186">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="15173-186">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="15173-187">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-187">dataBackupBlocked</span></span>|<span data-ttu-id="15173-188">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-188">Boolean</span></span>|<span data-ttu-id="15173-189">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="15173-189">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="15173-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-191">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="15173-191">deviceComplianceRequired</span></span>|<span data-ttu-id="15173-192">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-192">Boolean</span></span>|<span data-ttu-id="15173-193">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="15173-193">Indicates whether device compliance is required.</span></span> <span data-ttu-id="15173-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-195">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="15173-195">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="15173-196">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-196">Boolean</span></span>|<span data-ttu-id="15173-197">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="15173-197">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="15173-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-199">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-199">saveAsBlocked</span></span>|<span data-ttu-id="15173-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="15173-200">Boolean</span></span>|<span data-ttu-id="15173-201">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="15173-201">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="15173-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-203">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="15173-203">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="15173-204">持续时间</span><span class="sxs-lookup"><span data-stu-id="15173-204">Duration</span></span>|<span data-ttu-id="15173-205">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="15173-205">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="15173-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-207">pinRequired</span><span class="sxs-lookup"><span data-stu-id="15173-207">pinRequired</span></span>|<span data-ttu-id="15173-208">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-208">Boolean</span></span>|<span data-ttu-id="15173-209">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="15173-209">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="15173-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-211">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="15173-211">maximumPinRetries</span></span>|<span data-ttu-id="15173-212">Int32</span><span class="sxs-lookup"><span data-stu-id="15173-212">Int32</span></span>|<span data-ttu-id="15173-213">在阻止或擦除托管应用之前, 不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="15173-213">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="15173-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-215">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-215">simplePinBlocked</span></span>|<span data-ttu-id="15173-216">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-216">Boolean</span></span>|<span data-ttu-id="15173-217">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="15173-217">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="15173-218">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-218">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-219">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="15173-219">minimumPinLength</span></span>|<span data-ttu-id="15173-220">Int32</span><span class="sxs-lookup"><span data-stu-id="15173-220">Int32</span></span>|<span data-ttu-id="15173-221">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-221">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-222">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="15173-222">pinCharacterSet</span></span>|[<span data-ttu-id="15173-223">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="15173-223">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="15173-224">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="15173-224">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="15173-225">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-226">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="15173-226">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="15173-227">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="15173-227">periodBeforePinReset</span></span>|<span data-ttu-id="15173-228">Duration</span><span class="sxs-lookup"><span data-stu-id="15173-228">Duration</span></span>|<span data-ttu-id="15173-229">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="15173-229">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="15173-230">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-231">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="15173-231">allowedDataStorageLocations</span></span>|<span data-ttu-id="15173-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="15173-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="15173-233">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="15173-233">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="15173-234">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-235">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="15173-235">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="15173-236">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-236">contactSyncBlocked</span></span>|<span data-ttu-id="15173-237">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-237">Boolean</span></span>|<span data-ttu-id="15173-238">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="15173-238">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="15173-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-240">printBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-240">printBlocked</span></span>|<span data-ttu-id="15173-241">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-241">Boolean</span></span>|<span data-ttu-id="15173-242">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="15173-242">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="15173-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-244">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-244">fingerprintBlocked</span></span>|<span data-ttu-id="15173-245">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-245">Boolean</span></span>|<span data-ttu-id="15173-246">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="15173-246">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="15173-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-248">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="15173-248">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="15173-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="15173-249">Boolean</span></span>|<span data-ttu-id="15173-250">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="15173-250">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="15173-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-252">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="15173-252">minimumRequiredOsVersion</span></span>|<span data-ttu-id="15173-253">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-253">String</span></span>|<span data-ttu-id="15173-254">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-254">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="15173-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-256">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="15173-256">minimumWarningOsVersion</span></span>|<span data-ttu-id="15173-257">String</span><span class="sxs-lookup"><span data-stu-id="15173-257">String</span></span>|<span data-ttu-id="15173-258">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="15173-258">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="15173-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-260">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="15173-260">minimumRequiredAppVersion</span></span>|<span data-ttu-id="15173-261">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-261">String</span></span>|<span data-ttu-id="15173-262">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-262">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="15173-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-264">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="15173-264">minimumWarningAppVersion</span></span>|<span data-ttu-id="15173-265">String</span><span class="sxs-lookup"><span data-stu-id="15173-265">String</span></span>|<span data-ttu-id="15173-266">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="15173-266">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="15173-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-268">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="15173-268">minimumWipeOsVersion</span></span>|<span data-ttu-id="15173-269">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-269">String</span></span>|<span data-ttu-id="15173-270">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-270">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="15173-271">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-271">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-272">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="15173-272">minimumWipeAppVersion</span></span>|<span data-ttu-id="15173-273">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-273">String</span></span>|<span data-ttu-id="15173-274">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-274">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="15173-275">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-275">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-276">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="15173-276">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="15173-277">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="15173-277">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="15173-278">如果将 DeviceComplianceRequired 设置为 true, 则定义在设备为根或已越狱时的托管应用行为 (阻止或擦除)。</span><span class="sxs-lookup"><span data-stu-id="15173-278">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="15173-279">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-279">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-280">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="15173-280">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="15173-281">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="15173-281">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="15173-282">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="15173-282">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="15173-283">根据最大错误 pin 重试次数定义托管应用行为, 即阻止或擦除。</span><span class="sxs-lookup"><span data-stu-id="15173-283">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="15173-284">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="15173-284">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="15173-285">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="15173-285">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="15173-286">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="15173-286">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="15173-287">持续时间</span><span class="sxs-lookup"><span data-stu-id="15173-287">Duration</span></span>|<span data-ttu-id="15173-288">以分钟为单位的应用程序 pin (而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)继承的无生物特征密码) 超时</span><span class="sxs-lookup"><span data-stu-id="15173-288">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="15173-289">isAssigned</span><span class="sxs-lookup"><span data-stu-id="15173-289">isAssigned</span></span>|<span data-ttu-id="15173-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="15173-290">Boolean</span></span>|<span data-ttu-id="15173-291">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="15173-291">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="15173-292">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="15173-292">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="15173-293">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="15173-293">targetedAppManagementLevels</span></span>|[<span data-ttu-id="15173-294">appManagementLevel</span><span class="sxs-lookup"><span data-stu-id="15173-294">appManagementLevel</span></span>](../resources/intune-mam-appmanagementlevel.md)|<span data-ttu-id="15173-295">此策略继承自[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)的预期应用管理级别。</span><span class="sxs-lookup"><span data-stu-id="15173-295">The intended app management levels for this policy Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span></span> <span data-ttu-id="15173-296">可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="15173-296">Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.</span></span>|
|<span data-ttu-id="15173-297">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="15173-297">appDataEncryptionType</span></span>|[<span data-ttu-id="15173-298">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="15173-298">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="15173-299">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="15173-299">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="15173-300">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="15173-300">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="15173-301">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="15173-301">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="15173-302">String</span><span class="sxs-lookup"><span data-stu-id="15173-302">String</span></span>|<span data-ttu-id="15173-303">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-303">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="15173-304">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="15173-304">deployedAppCount</span></span>|<span data-ttu-id="15173-305">Int32</span><span class="sxs-lookup"><span data-stu-id="15173-305">Int32</span></span>|<span data-ttu-id="15173-306">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="15173-306">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="15173-307">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-307">faceIdBlocked</span></span>|<span data-ttu-id="15173-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="15173-308">Boolean</span></span>|<span data-ttu-id="15173-309">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。</span><span class="sxs-lookup"><span data-stu-id="15173-309">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="15173-310">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="15173-310">exemptedAppProtocols</span></span>|<span data-ttu-id="15173-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15173-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="15173-312">此列表中的应用程序将从策略中排除, 并将能够从托管应用接收数据。</span><span class="sxs-lookup"><span data-stu-id="15173-312">Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span>|
|<span data-ttu-id="15173-313">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="15173-313">minimumWipeSdkVersion</span></span>|<span data-ttu-id="15173-314">String</span><span class="sxs-lookup"><span data-stu-id="15173-314">String</span></span>|<span data-ttu-id="15173-315">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="15173-315">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="15173-316">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="15173-316">allowedIosDeviceModels</span></span>|<span data-ttu-id="15173-317">字符串</span><span class="sxs-lookup"><span data-stu-id="15173-317">String</span></span>|<span data-ttu-id="15173-318">允许托管应用使用的设备模型的以分号分隔的列表 (以字符串形式)。</span><span class="sxs-lookup"><span data-stu-id="15173-318">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span>|
|<span data-ttu-id="15173-319">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="15173-319">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="15173-320">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="15173-320">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="15173-321">定义托管应用程序行为, 如果不允许指定的设备模型, 则要么阻止, 也可以擦除。</span><span class="sxs-lookup"><span data-stu-id="15173-321">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="15173-322">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="15173-322">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="15173-323">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="15173-323">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="15173-324">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-324">Boolean</span></span>|<span data-ttu-id="15173-325">定义在访问托管应用程序时是否允许使用第三方键盘</span><span class="sxs-lookup"><span data-stu-id="15173-325">Defines if third party keyboards are allowed while accessing a managed app</span></span>|
|<span data-ttu-id="15173-326">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="15173-326">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="15173-327">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-327">Boolean</span></span>|<span data-ttu-id="15173-328">定义是否支持从受管理的应用程序到所选的可共享位置的打开入点操作。</span><span class="sxs-lookup"><span data-stu-id="15173-328">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="15173-329">此设置仅适用于将 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 和 DisableProtectionOfManagedOutboundOpenInData 设置为 False 的情况。</span><span class="sxs-lookup"><span data-stu-id="15173-329">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span>|
|<span data-ttu-id="15173-330">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="15173-330">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="15173-331">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-331">Boolean</span></span>|<span data-ttu-id="15173-332">禁用通过 IOS OpenIn 选项传输到其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="15173-332">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="15173-333">仅当 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 时, 此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="15173-333">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span>|
|<span data-ttu-id="15173-334">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="15173-334">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="15173-335">布尔</span><span class="sxs-lookup"><span data-stu-id="15173-335">Boolean</span></span>|<span data-ttu-id="15173-336">保护来自未知源的传入数据。</span><span class="sxs-lookup"><span data-stu-id="15173-336">Protect incoming data from unknown source.</span></span> <span data-ttu-id="15173-337">仅当 AllowedInboundDataTransferSources 设置为 AllApps 时, 此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="15173-337">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span>|



## <a name="response"></a><span data-ttu-id="15173-338">响应</span><span class="sxs-lookup"><span data-stu-id="15173-338">Response</span></span>
<span data-ttu-id="15173-339">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="15173-339">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15173-340">示例</span><span class="sxs-lookup"><span data-stu-id="15173-340">Example</span></span>

### <a name="request"></a><span data-ttu-id="15173-341">请求</span><span class="sxs-lookup"><span data-stu-id="15173-341">Request</span></span>
<span data-ttu-id="15173-342">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15173-342">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
Content-type: application/json
Content-length: 2487

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="15173-343">响应</span><span class="sxs-lookup"><span data-stu-id="15173-343">Response</span></span>
<span data-ttu-id="15173-p145">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="15173-p145">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2659

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```




