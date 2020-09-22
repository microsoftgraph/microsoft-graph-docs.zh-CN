---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65aee8185daaf83cb746e4d8652b8e3854e7560f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013158"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="12b89-103">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="12b89-103">Create defaultManagedAppProtection</span></span>

<span data-ttu-id="12b89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12b89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12b89-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12b89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12b89-106">创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12b89-106">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12b89-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12b89-107">Prerequisites</span></span>
<span data-ttu-id="12b89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12b89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12b89-110">Permission type</span></span>|<span data-ttu-id="12b89-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12b89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12b89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12b89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12b89-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b89-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12b89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12b89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12b89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12b89-115">Not supported.</span></span>|
|<span data-ttu-id="12b89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12b89-116">Application</span></span>|<span data-ttu-id="12b89-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b89-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12b89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12b89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="12b89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12b89-119">Request headers</span></span>
|<span data-ttu-id="12b89-120">标头</span><span class="sxs-lookup"><span data-stu-id="12b89-120">Header</span></span>|<span data-ttu-id="12b89-121">值</span><span class="sxs-lookup"><span data-stu-id="12b89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12b89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12b89-122">Authorization</span></span>|<span data-ttu-id="12b89-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12b89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12b89-124">接受</span><span class="sxs-lookup"><span data-stu-id="12b89-124">Accept</span></span>|<span data-ttu-id="12b89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12b89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12b89-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12b89-126">Request body</span></span>
<span data-ttu-id="12b89-127">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12b89-127">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="12b89-128">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12b89-128">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="12b89-129">属性</span><span class="sxs-lookup"><span data-stu-id="12b89-129">Property</span></span>|<span data-ttu-id="12b89-130">类型</span><span class="sxs-lookup"><span data-stu-id="12b89-130">Type</span></span>|<span data-ttu-id="12b89-131">说明</span><span class="sxs-lookup"><span data-stu-id="12b89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b89-132">displayName</span><span class="sxs-lookup"><span data-stu-id="12b89-132">displayName</span></span>|<span data-ttu-id="12b89-133">String</span><span class="sxs-lookup"><span data-stu-id="12b89-133">String</span></span>|<span data-ttu-id="12b89-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="12b89-134">Policy display name.</span></span> <span data-ttu-id="12b89-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-136">description</span><span class="sxs-lookup"><span data-stu-id="12b89-136">description</span></span>|<span data-ttu-id="12b89-137">String</span><span class="sxs-lookup"><span data-stu-id="12b89-137">String</span></span>|<span data-ttu-id="12b89-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="12b89-138">The policy's description.</span></span> <span data-ttu-id="12b89-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12b89-140">createdDateTime</span></span>|<span data-ttu-id="12b89-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12b89-141">DateTimeOffset</span></span>|<span data-ttu-id="12b89-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12b89-142">The date and time the policy was created.</span></span> <span data-ttu-id="12b89-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12b89-144">lastModifiedDateTime</span></span>|<span data-ttu-id="12b89-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12b89-145">DateTimeOffset</span></span>|<span data-ttu-id="12b89-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="12b89-146">Last time the policy was modified.</span></span> <span data-ttu-id="12b89-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-148">id</span><span class="sxs-lookup"><span data-stu-id="12b89-148">id</span></span>|<span data-ttu-id="12b89-149">String</span><span class="sxs-lookup"><span data-stu-id="12b89-149">String</span></span>|<span data-ttu-id="12b89-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12b89-150">Key of the entity.</span></span> <span data-ttu-id="12b89-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-152">version</span><span class="sxs-lookup"><span data-stu-id="12b89-152">version</span></span>|<span data-ttu-id="12b89-153">String</span><span class="sxs-lookup"><span data-stu-id="12b89-153">String</span></span>|<span data-ttu-id="12b89-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="12b89-154">Version of the entity.</span></span> <span data-ttu-id="12b89-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="12b89-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="12b89-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="12b89-157">Duration</span><span class="sxs-lookup"><span data-stu-id="12b89-157">Duration</span></span>|<span data-ttu-id="12b89-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="12b89-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="12b89-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="12b89-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="12b89-161">Duration</span><span class="sxs-lookup"><span data-stu-id="12b89-161">Duration</span></span>|<span data-ttu-id="12b89-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="12b89-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="12b89-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="12b89-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="12b89-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="12b89-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="12b89-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="12b89-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="12b89-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="12b89-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="12b89-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="12b89-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="12b89-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="12b89-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="12b89-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="12b89-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="12b89-172">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="12b89-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="12b89-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="12b89-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="12b89-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-175">Boolean</span></span>|<span data-ttu-id="12b89-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="12b89-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="12b89-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="12b89-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="12b89-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="12b89-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="12b89-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="12b89-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="12b89-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="12b89-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="12b89-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-183">dataBackupBlocked</span></span>|<span data-ttu-id="12b89-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-184">Boolean</span></span>|<span data-ttu-id="12b89-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="12b89-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="12b89-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="12b89-187">deviceComplianceRequired</span></span>|<span data-ttu-id="12b89-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-188">Boolean</span></span>|<span data-ttu-id="12b89-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="12b89-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="12b89-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="12b89-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="12b89-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-192">Boolean</span></span>|<span data-ttu-id="12b89-193">指示是否应在托管浏览器应用程序中打开 internet 链接，或由 CustomBrowserProtocol (为 iOS 指定的任何自定义浏览器) 从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的适用于 Android) 或 CustomBrowserPackageId/CustomBrowserDisplayName (</span><span class="sxs-lookup"><span data-stu-id="12b89-193">Indicates whether internet links should be opened in the managed browser app, or any custom browser specified by CustomBrowserProtocol (for iOS) or CustomBrowserPackageId/CustomBrowserDisplayName (for Android) Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-194">saveAsBlocked</span></span>|<span data-ttu-id="12b89-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-195">Boolean</span></span>|<span data-ttu-id="12b89-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="12b89-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="12b89-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="12b89-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="12b89-199">Duration</span><span class="sxs-lookup"><span data-stu-id="12b89-199">Duration</span></span>|<span data-ttu-id="12b89-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="12b89-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="12b89-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="12b89-202">pinRequired</span></span>|<span data-ttu-id="12b89-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-203">Boolean</span></span>|<span data-ttu-id="12b89-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="12b89-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="12b89-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="12b89-206">maximumPinRetries</span></span>|<span data-ttu-id="12b89-207">Int32</span><span class="sxs-lookup"><span data-stu-id="12b89-207">Int32</span></span>|<span data-ttu-id="12b89-208">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="12b89-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="12b89-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-210">simplePinBlocked</span></span>|<span data-ttu-id="12b89-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-211">Boolean</span></span>|<span data-ttu-id="12b89-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="12b89-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="12b89-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="12b89-214">minimumPinLength</span></span>|<span data-ttu-id="12b89-215">Int32</span><span class="sxs-lookup"><span data-stu-id="12b89-215">Int32</span></span>|<span data-ttu-id="12b89-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="12b89-217">pinCharacterSet</span></span>|[<span data-ttu-id="12b89-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="12b89-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="12b89-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="12b89-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="12b89-220">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="12b89-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="12b89-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="12b89-222">periodBeforePinReset</span></span>|<span data-ttu-id="12b89-223">Duration</span><span class="sxs-lookup"><span data-stu-id="12b89-223">Duration</span></span>|<span data-ttu-id="12b89-224">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="12b89-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="12b89-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="12b89-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="12b89-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12b89-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="12b89-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="12b89-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="12b89-229">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="12b89-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="12b89-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-231">contactSyncBlocked</span></span>|<span data-ttu-id="12b89-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-232">Boolean</span></span>|<span data-ttu-id="12b89-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="12b89-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="12b89-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-235">printBlocked</span></span>|<span data-ttu-id="12b89-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-236">Boolean</span></span>|<span data-ttu-id="12b89-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="12b89-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="12b89-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-239">fingerprintBlocked</span></span>|<span data-ttu-id="12b89-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-240">Boolean</span></span>|<span data-ttu-id="12b89-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="12b89-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="12b89-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="12b89-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="12b89-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-244">Boolean</span></span>|<span data-ttu-id="12b89-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="12b89-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="12b89-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="12b89-248">String</span><span class="sxs-lookup"><span data-stu-id="12b89-248">String</span></span>|<span data-ttu-id="12b89-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="12b89-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="12b89-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="12b89-252">String</span><span class="sxs-lookup"><span data-stu-id="12b89-252">String</span></span>|<span data-ttu-id="12b89-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="12b89-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="12b89-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="12b89-256">String</span><span class="sxs-lookup"><span data-stu-id="12b89-256">String</span></span>|<span data-ttu-id="12b89-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="12b89-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="12b89-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="12b89-260">String</span><span class="sxs-lookup"><span data-stu-id="12b89-260">String</span></span>|<span data-ttu-id="12b89-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="12b89-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="12b89-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="12b89-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="12b89-263">managedBrowser</span><span class="sxs-lookup"><span data-stu-id="12b89-263">managedBrowser</span></span>|[<span data-ttu-id="12b89-264">managedBrowserType</span><span class="sxs-lookup"><span data-stu-id="12b89-264">managedBrowserType</span></span>](../resources/intune-mam-managedbrowsertype.md)|<span data-ttu-id="12b89-265">指示在哪个托管浏览器中 (s) 应打开 internet 链接。</span><span class="sxs-lookup"><span data-stu-id="12b89-265">Indicates in which managed browser(s) that internet links should be opened.</span></span> <span data-ttu-id="12b89-266">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="12b89-266">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span> <span data-ttu-id="12b89-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="12b89-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="12b89-268">可取值为：`notConfigured`、`microsoftEdge`。</span><span class="sxs-lookup"><span data-stu-id="12b89-268">Possible values are: `notConfigured`, `microsoftEdge`.</span></span>|
|<span data-ttu-id="12b89-269">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="12b89-269">appDataEncryptionType</span></span>|[<span data-ttu-id="12b89-270">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="12b89-270">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="12b89-271">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="12b89-271">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="12b89-272">仅 (iOS) 。</span><span class="sxs-lookup"><span data-stu-id="12b89-272">(iOS Only).</span></span> <span data-ttu-id="12b89-273">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="12b89-273">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="12b89-274">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-274">screenCaptureBlocked</span></span>|<span data-ttu-id="12b89-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-275">Boolean</span></span>|<span data-ttu-id="12b89-276">指示是否阻止捕获屏幕。</span><span class="sxs-lookup"><span data-stu-id="12b89-276">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="12b89-277">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="12b89-277">(Android only)</span></span>|
|<span data-ttu-id="12b89-278">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="12b89-278">encryptAppData</span></span>|<span data-ttu-id="12b89-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-279">Boolean</span></span>|<span data-ttu-id="12b89-280">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="12b89-280">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="12b89-281">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="12b89-281">(Android only)</span></span>|
|<span data-ttu-id="12b89-282">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="12b89-282">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="12b89-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-283">Boolean</span></span>|<span data-ttu-id="12b89-284">如果启用此设置，则在启用设备级加密的情况下禁用应用级加密。</span><span class="sxs-lookup"><span data-stu-id="12b89-284">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="12b89-285">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="12b89-285">(Android only)</span></span>|
|<span data-ttu-id="12b89-286">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-286">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="12b89-287">String</span><span class="sxs-lookup"><span data-stu-id="12b89-287">String</span></span>|<span data-ttu-id="12b89-288">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="12b89-288">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="12b89-289">仅 (iOS) </span><span class="sxs-lookup"><span data-stu-id="12b89-289">(iOS Only)</span></span>|
|<span data-ttu-id="12b89-290">customSettings</span><span class="sxs-lookup"><span data-stu-id="12b89-290">customSettings</span></span>|<span data-ttu-id="12b89-291">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12b89-291">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="12b89-292">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="12b89-292">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="12b89-293">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="12b89-293">deployedAppCount</span></span>|<span data-ttu-id="12b89-294">Int32</span><span class="sxs-lookup"><span data-stu-id="12b89-294">Int32</span></span>|<span data-ttu-id="12b89-295">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="12b89-295">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="12b89-296">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-296">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="12b89-297">String</span><span class="sxs-lookup"><span data-stu-id="12b89-297">String</span></span>|<span data-ttu-id="12b89-298">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="12b89-298">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="12b89-299">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="12b89-299">(Android only)</span></span>|
|<span data-ttu-id="12b89-300">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="12b89-300">minimumWarningPatchVersion</span></span>|<span data-ttu-id="12b89-301">String</span><span class="sxs-lookup"><span data-stu-id="12b89-301">String</span></span>|<span data-ttu-id="12b89-302">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="12b89-302">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="12b89-303">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="12b89-303">(Android only)</span></span>|
|<span data-ttu-id="12b89-304">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="12b89-304">faceIdBlocked</span></span>|<span data-ttu-id="12b89-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="12b89-305">Boolean</span></span>|<span data-ttu-id="12b89-306">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="12b89-306">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="12b89-307">仅 (iOS) </span><span class="sxs-lookup"><span data-stu-id="12b89-307">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="12b89-308">响应</span><span class="sxs-lookup"><span data-stu-id="12b89-308">Response</span></span>
<span data-ttu-id="12b89-309">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12b89-309">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12b89-310">示例</span><span class="sxs-lookup"><span data-stu-id="12b89-310">Example</span></span>

### <a name="request"></a><span data-ttu-id="12b89-311">请求</span><span class="sxs-lookup"><span data-stu-id="12b89-311">Request</span></span>
<span data-ttu-id="12b89-312">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12b89-312">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 2009

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
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
  "managedBrowser": "microsoftEdge",
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
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="12b89-313">响应</span><span class="sxs-lookup"><span data-stu-id="12b89-313">Response</span></span>
<span data-ttu-id="12b89-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12b89-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2181

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "managedBrowser": "microsoftEdge",
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
  "faceIdBlocked": true
}
```






