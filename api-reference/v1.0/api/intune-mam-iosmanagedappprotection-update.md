---
title: 更新 iosManagedAppProtection
description: 更新 iosManagedAppProtection 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bbea9438e265e60ff1a4f519f1726227d5d2621
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048692"
---
# <a name="update-iosmanagedappprotection"></a><span data-ttu-id="c18cd-103">更新 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c18cd-103">Update iosManagedAppProtection</span></span>

<span data-ttu-id="c18cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c18cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c18cd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18cd-106">更新 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c18cd-106">Update the properties of a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c18cd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c18cd-107">Prerequisites</span></span>
<span data-ttu-id="c18cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c18cd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c18cd-110">Permission type</span></span>|<span data-ttu-id="c18cd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c18cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c18cd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c18cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c18cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c18cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c18cd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c18cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c18cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c18cd-115">Not supported.</span></span>|
|<span data-ttu-id="c18cd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c18cd-116">Application</span></span>|<span data-ttu-id="c18cd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c18cd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c18cd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c18cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="c18cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c18cd-119">Request headers</span></span>
|<span data-ttu-id="c18cd-120">标头</span><span class="sxs-lookup"><span data-stu-id="c18cd-120">Header</span></span>|<span data-ttu-id="c18cd-121">值</span><span class="sxs-lookup"><span data-stu-id="c18cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c18cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c18cd-122">Authorization</span></span>|<span data-ttu-id="c18cd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c18cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c18cd-124">接受</span><span class="sxs-lookup"><span data-stu-id="c18cd-124">Accept</span></span>|<span data-ttu-id="c18cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c18cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c18cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c18cd-126">Request body</span></span>
<span data-ttu-id="c18cd-127">在请求正文中，提供 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c18cd-127">In the request body, supply a JSON representation for the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

<span data-ttu-id="c18cd-128">下表显示创建 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c18cd-128">The following table shows the properties that are required when you create the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span></span>

|<span data-ttu-id="c18cd-129">属性</span><span class="sxs-lookup"><span data-stu-id="c18cd-129">Property</span></span>|<span data-ttu-id="c18cd-130">类型</span><span class="sxs-lookup"><span data-stu-id="c18cd-130">Type</span></span>|<span data-ttu-id="c18cd-131">说明</span><span class="sxs-lookup"><span data-stu-id="c18cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18cd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c18cd-132">displayName</span></span>|<span data-ttu-id="c18cd-133">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-133">String</span></span>|<span data-ttu-id="c18cd-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c18cd-134">Policy display name.</span></span> <span data-ttu-id="c18cd-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-136">description</span><span class="sxs-lookup"><span data-stu-id="c18cd-136">description</span></span>|<span data-ttu-id="c18cd-137">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-137">String</span></span>|<span data-ttu-id="c18cd-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c18cd-138">The policy's description.</span></span> <span data-ttu-id="c18cd-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c18cd-140">createdDateTime</span></span>|<span data-ttu-id="c18cd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c18cd-141">DateTimeOffset</span></span>|<span data-ttu-id="c18cd-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c18cd-142">The date and time the policy was created.</span></span> <span data-ttu-id="c18cd-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c18cd-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c18cd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c18cd-145">DateTimeOffset</span></span>|<span data-ttu-id="c18cd-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c18cd-146">Last time the policy was modified.</span></span> <span data-ttu-id="c18cd-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-148">id</span><span class="sxs-lookup"><span data-stu-id="c18cd-148">id</span></span>|<span data-ttu-id="c18cd-149">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-149">String</span></span>|<span data-ttu-id="c18cd-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c18cd-150">Key of the entity.</span></span> <span data-ttu-id="c18cd-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-152">version</span><span class="sxs-lookup"><span data-stu-id="c18cd-152">version</span></span>|<span data-ttu-id="c18cd-153">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-153">String</span></span>|<span data-ttu-id="c18cd-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c18cd-154">Version of the entity.</span></span> <span data-ttu-id="c18cd-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c18cd-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c18cd-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="c18cd-157">Duration</span><span class="sxs-lookup"><span data-stu-id="c18cd-157">Duration</span></span>|<span data-ttu-id="c18cd-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c18cd-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="c18cd-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c18cd-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="c18cd-161">Duration</span><span class="sxs-lookup"><span data-stu-id="c18cd-161">Duration</span></span>|<span data-ttu-id="c18cd-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c18cd-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="c18cd-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="c18cd-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="c18cd-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c18cd-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c18cd-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="c18cd-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="c18cd-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c18cd-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="c18cd-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="c18cd-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c18cd-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c18cd-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="c18cd-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="c18cd-172">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c18cd-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="c18cd-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="c18cd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-175">Boolean</span></span>|<span data-ttu-id="c18cd-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="c18cd-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="c18cd-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c18cd-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="c18cd-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c18cd-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="c18cd-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="c18cd-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="c18cd-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="c18cd-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-183">dataBackupBlocked</span></span>|<span data-ttu-id="c18cd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-184">Boolean</span></span>|<span data-ttu-id="c18cd-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="c18cd-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="c18cd-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="c18cd-187">deviceComplianceRequired</span></span>|<span data-ttu-id="c18cd-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-188">Boolean</span></span>|<span data-ttu-id="c18cd-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="c18cd-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="c18cd-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="c18cd-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="c18cd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-192">Boolean</span></span>|<span data-ttu-id="c18cd-193">指示是否应在托管浏览器应用程序中打开 internet 链接，或由 CustomBrowserProtocol (为 iOS 指定的任何自定义浏览器) 从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的适用于 Android) 或 CustomBrowserPackageId/CustomBrowserDisplayName (</span><span class="sxs-lookup"><span data-stu-id="c18cd-193">Indicates whether internet links should be opened in the managed browser app, or any custom browser specified by CustomBrowserProtocol (for iOS) or CustomBrowserPackageId/CustomBrowserDisplayName (for Android) Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-194">saveAsBlocked</span></span>|<span data-ttu-id="c18cd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-195">Boolean</span></span>|<span data-ttu-id="c18cd-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="c18cd-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="c18cd-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="c18cd-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="c18cd-199">Duration</span><span class="sxs-lookup"><span data-stu-id="c18cd-199">Duration</span></span>|<span data-ttu-id="c18cd-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="c18cd-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="c18cd-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="c18cd-202">pinRequired</span></span>|<span data-ttu-id="c18cd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-203">Boolean</span></span>|<span data-ttu-id="c18cd-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="c18cd-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="c18cd-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="c18cd-206">maximumPinRetries</span></span>|<span data-ttu-id="c18cd-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c18cd-207">Int32</span></span>|<span data-ttu-id="c18cd-208">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="c18cd-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="c18cd-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-210">simplePinBlocked</span></span>|<span data-ttu-id="c18cd-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-211">Boolean</span></span>|<span data-ttu-id="c18cd-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="c18cd-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="c18cd-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="c18cd-214">minimumPinLength</span></span>|<span data-ttu-id="c18cd-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c18cd-215">Int32</span></span>|<span data-ttu-id="c18cd-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c18cd-217">pinCharacterSet</span></span>|[<span data-ttu-id="c18cd-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c18cd-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="c18cd-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="c18cd-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="c18cd-220">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="c18cd-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="c18cd-222">periodBeforePinReset</span></span>|<span data-ttu-id="c18cd-223">Duration</span><span class="sxs-lookup"><span data-stu-id="c18cd-223">Duration</span></span>|<span data-ttu-id="c18cd-224">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="c18cd-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="c18cd-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="c18cd-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="c18cd-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c18cd-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="c18cd-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="c18cd-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="c18cd-229">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="c18cd-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-231">contactSyncBlocked</span></span>|<span data-ttu-id="c18cd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-232">Boolean</span></span>|<span data-ttu-id="c18cd-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="c18cd-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="c18cd-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-235">printBlocked</span></span>|<span data-ttu-id="c18cd-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-236">Boolean</span></span>|<span data-ttu-id="c18cd-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="c18cd-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="c18cd-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-239">fingerprintBlocked</span></span>|<span data-ttu-id="c18cd-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-240">Boolean</span></span>|<span data-ttu-id="c18cd-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c18cd-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="c18cd-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="c18cd-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="c18cd-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-244">Boolean</span></span>|<span data-ttu-id="c18cd-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="c18cd-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="c18cd-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="c18cd-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="c18cd-248">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-248">String</span></span>|<span data-ttu-id="c18cd-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c18cd-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c18cd-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="c18cd-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="c18cd-252">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-252">String</span></span>|<span data-ttu-id="c18cd-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c18cd-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="c18cd-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="c18cd-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="c18cd-256">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-256">String</span></span>|<span data-ttu-id="c18cd-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c18cd-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c18cd-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="c18cd-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="c18cd-260">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-260">String</span></span>|<span data-ttu-id="c18cd-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c18cd-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="c18cd-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-263">managedBrowser</span><span class="sxs-lookup"><span data-stu-id="c18cd-263">managedBrowser</span></span>|[<span data-ttu-id="c18cd-264">managedBrowserType</span><span class="sxs-lookup"><span data-stu-id="c18cd-264">managedBrowserType</span></span>](../resources/intune-mam-managedbrowsertype.md)|<span data-ttu-id="c18cd-265">指示在哪个托管浏览器中 (s) 应打开 internet 链接。</span><span class="sxs-lookup"><span data-stu-id="c18cd-265">Indicates in which managed browser(s) that internet links should be opened.</span></span> <span data-ttu-id="c18cd-266">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="c18cd-266">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span> <span data-ttu-id="c18cd-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c18cd-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c18cd-268">可取值为：`notConfigured`、`microsoftEdge`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-268">Possible values are: `notConfigured`, `microsoftEdge`.</span></span>|
|<span data-ttu-id="c18cd-269">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c18cd-269">isAssigned</span></span>|<span data-ttu-id="c18cd-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-270">Boolean</span></span>|<span data-ttu-id="c18cd-271">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="c18cd-271">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="c18cd-272">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c18cd-272">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="c18cd-273">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c18cd-273">appDataEncryptionType</span></span>|[<span data-ttu-id="c18cd-274">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c18cd-274">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="c18cd-275">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="c18cd-275">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="c18cd-276">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="c18cd-276">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="c18cd-277">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c18cd-277">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="c18cd-278">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-278">String</span></span>|<span data-ttu-id="c18cd-279">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c18cd-279">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="c18cd-280">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c18cd-280">deployedAppCount</span></span>|<span data-ttu-id="c18cd-281">Int32</span><span class="sxs-lookup"><span data-stu-id="c18cd-281">Int32</span></span>|<span data-ttu-id="c18cd-282">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="c18cd-282">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c18cd-283">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="c18cd-283">faceIdBlocked</span></span>|<span data-ttu-id="c18cd-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="c18cd-284">Boolean</span></span>|<span data-ttu-id="c18cd-285">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c18cd-285">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="c18cd-286">customBrowserProtocol</span><span class="sxs-lookup"><span data-stu-id="c18cd-286">customBrowserProtocol</span></span>|<span data-ttu-id="c18cd-287">String</span><span class="sxs-lookup"><span data-stu-id="c18cd-287">String</span></span>|<span data-ttu-id="c18cd-288">用于在 iOS 上打开 weblink 的自定义浏览器协议。</span><span class="sxs-lookup"><span data-stu-id="c18cd-288">A custom browser protocol to open weblink on iOS.</span></span> <span data-ttu-id="c18cd-289">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="c18cd-289">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span>|



## <a name="response"></a><span data-ttu-id="c18cd-290">响应</span><span class="sxs-lookup"><span data-stu-id="c18cd-290">Response</span></span>
<span data-ttu-id="c18cd-291">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c18cd-291">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c18cd-292">示例</span><span class="sxs-lookup"><span data-stu-id="c18cd-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="c18cd-293">请求</span><span class="sxs-lookup"><span data-stu-id="c18cd-293">Request</span></span>
<span data-ttu-id="c18cd-294">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c18cd-294">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
Content-type: application/json
Content-length: 1667

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```

### <a name="response"></a><span data-ttu-id="c18cd-295">响应</span><span class="sxs-lookup"><span data-stu-id="c18cd-295">Response</span></span>
<span data-ttu-id="c18cd-p136">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c18cd-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "managedBrowser": "microsoftEdge",
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```






