---
title: 更新 androidManagedAppProtection
description: 更新 androidManagedAppProtection 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96e819e3cb8c9ba14974a31e6765c407a7c33f78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015979"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="d24bc-103">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d24bc-103">Update androidManagedAppProtection</span></span>

<span data-ttu-id="d24bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d24bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d24bc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d24bc-106">更新 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d24bc-106">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d24bc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d24bc-107">Prerequisites</span></span>
<span data-ttu-id="d24bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d24bc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d24bc-110">Permission type</span></span>|<span data-ttu-id="d24bc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d24bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d24bc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d24bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d24bc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d24bc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d24bc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d24bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d24bc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d24bc-115">Not supported.</span></span>|
|<span data-ttu-id="d24bc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d24bc-116">Application</span></span>|<span data-ttu-id="d24bc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d24bc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d24bc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d24bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="d24bc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d24bc-119">Request headers</span></span>
|<span data-ttu-id="d24bc-120">标头</span><span class="sxs-lookup"><span data-stu-id="d24bc-120">Header</span></span>|<span data-ttu-id="d24bc-121">值</span><span class="sxs-lookup"><span data-stu-id="d24bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d24bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d24bc-122">Authorization</span></span>|<span data-ttu-id="d24bc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d24bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d24bc-124">接受</span><span class="sxs-lookup"><span data-stu-id="d24bc-124">Accept</span></span>|<span data-ttu-id="d24bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d24bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d24bc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d24bc-126">Request body</span></span>
<span data-ttu-id="d24bc-127">在请求正文中，提供 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d24bc-127">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="d24bc-128">下表显示了创建 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d24bc-128">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="d24bc-129">属性</span><span class="sxs-lookup"><span data-stu-id="d24bc-129">Property</span></span>|<span data-ttu-id="d24bc-130">类型</span><span class="sxs-lookup"><span data-stu-id="d24bc-130">Type</span></span>|<span data-ttu-id="d24bc-131">说明</span><span class="sxs-lookup"><span data-stu-id="d24bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d24bc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d24bc-132">displayName</span></span>|<span data-ttu-id="d24bc-133">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-133">String</span></span>|<span data-ttu-id="d24bc-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d24bc-134">Policy display name.</span></span> <span data-ttu-id="d24bc-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-136">description</span><span class="sxs-lookup"><span data-stu-id="d24bc-136">description</span></span>|<span data-ttu-id="d24bc-137">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-137">String</span></span>|<span data-ttu-id="d24bc-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d24bc-138">The policy's description.</span></span> <span data-ttu-id="d24bc-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d24bc-140">createdDateTime</span></span>|<span data-ttu-id="d24bc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d24bc-141">DateTimeOffset</span></span>|<span data-ttu-id="d24bc-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d24bc-142">The date and time the policy was created.</span></span> <span data-ttu-id="d24bc-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d24bc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d24bc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d24bc-145">DateTimeOffset</span></span>|<span data-ttu-id="d24bc-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d24bc-146">Last time the policy was modified.</span></span> <span data-ttu-id="d24bc-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-148">id</span><span class="sxs-lookup"><span data-stu-id="d24bc-148">id</span></span>|<span data-ttu-id="d24bc-149">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-149">String</span></span>|<span data-ttu-id="d24bc-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d24bc-150">Key of the entity.</span></span> <span data-ttu-id="d24bc-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-152">version</span><span class="sxs-lookup"><span data-stu-id="d24bc-152">version</span></span>|<span data-ttu-id="d24bc-153">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-153">String</span></span>|<span data-ttu-id="d24bc-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d24bc-154">Version of the entity.</span></span> <span data-ttu-id="d24bc-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d24bc-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d24bc-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="d24bc-157">Duration</span><span class="sxs-lookup"><span data-stu-id="d24bc-157">Duration</span></span>|<span data-ttu-id="d24bc-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d24bc-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="d24bc-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d24bc-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="d24bc-161">Duration</span><span class="sxs-lookup"><span data-stu-id="d24bc-161">Duration</span></span>|<span data-ttu-id="d24bc-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d24bc-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="d24bc-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="d24bc-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="d24bc-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d24bc-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="d24bc-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="d24bc-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="d24bc-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d24bc-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="d24bc-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="d24bc-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d24bc-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="d24bc-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="d24bc-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="d24bc-172">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d24bc-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="d24bc-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="d24bc-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-175">Boolean</span></span>|<span data-ttu-id="d24bc-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="d24bc-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="d24bc-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d24bc-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="d24bc-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d24bc-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="d24bc-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="d24bc-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="d24bc-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="d24bc-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-183">dataBackupBlocked</span></span>|<span data-ttu-id="d24bc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-184">Boolean</span></span>|<span data-ttu-id="d24bc-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="d24bc-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="d24bc-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="d24bc-187">deviceComplianceRequired</span></span>|<span data-ttu-id="d24bc-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-188">Boolean</span></span>|<span data-ttu-id="d24bc-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="d24bc-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="d24bc-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="d24bc-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="d24bc-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-192">Boolean</span></span>|<span data-ttu-id="d24bc-193">指示是否应在托管浏览器应用程序中打开 internet 链接，或由 CustomBrowserProtocol (为 iOS 指定的任何自定义浏览器) 从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的适用于 Android) 或 CustomBrowserPackageId/CustomBrowserDisplayName (</span><span class="sxs-lookup"><span data-stu-id="d24bc-193">Indicates whether internet links should be opened in the managed browser app, or any custom browser specified by CustomBrowserProtocol (for iOS) or CustomBrowserPackageId/CustomBrowserDisplayName (for Android) Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-194">saveAsBlocked</span></span>|<span data-ttu-id="d24bc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-195">Boolean</span></span>|<span data-ttu-id="d24bc-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="d24bc-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="d24bc-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="d24bc-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="d24bc-199">Duration</span><span class="sxs-lookup"><span data-stu-id="d24bc-199">Duration</span></span>|<span data-ttu-id="d24bc-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="d24bc-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="d24bc-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="d24bc-202">pinRequired</span></span>|<span data-ttu-id="d24bc-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-203">Boolean</span></span>|<span data-ttu-id="d24bc-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="d24bc-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="d24bc-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="d24bc-206">maximumPinRetries</span></span>|<span data-ttu-id="d24bc-207">Int32</span><span class="sxs-lookup"><span data-stu-id="d24bc-207">Int32</span></span>|<span data-ttu-id="d24bc-208">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="d24bc-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="d24bc-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-210">simplePinBlocked</span></span>|<span data-ttu-id="d24bc-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-211">Boolean</span></span>|<span data-ttu-id="d24bc-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="d24bc-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="d24bc-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="d24bc-214">minimumPinLength</span></span>|<span data-ttu-id="d24bc-215">Int32</span><span class="sxs-lookup"><span data-stu-id="d24bc-215">Int32</span></span>|<span data-ttu-id="d24bc-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d24bc-217">pinCharacterSet</span></span>|[<span data-ttu-id="d24bc-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d24bc-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="d24bc-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="d24bc-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="d24bc-220">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="d24bc-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="d24bc-222">periodBeforePinReset</span></span>|<span data-ttu-id="d24bc-223">Duration</span><span class="sxs-lookup"><span data-stu-id="d24bc-223">Duration</span></span>|<span data-ttu-id="d24bc-224">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="d24bc-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="d24bc-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="d24bc-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="d24bc-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d24bc-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="d24bc-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="d24bc-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="d24bc-229">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="d24bc-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-231">contactSyncBlocked</span></span>|<span data-ttu-id="d24bc-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-232">Boolean</span></span>|<span data-ttu-id="d24bc-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="d24bc-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="d24bc-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-235">printBlocked</span></span>|<span data-ttu-id="d24bc-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-236">Boolean</span></span>|<span data-ttu-id="d24bc-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="d24bc-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="d24bc-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-239">fingerprintBlocked</span></span>|<span data-ttu-id="d24bc-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-240">Boolean</span></span>|<span data-ttu-id="d24bc-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="d24bc-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="d24bc-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="d24bc-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="d24bc-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-244">Boolean</span></span>|<span data-ttu-id="d24bc-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="d24bc-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="d24bc-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="d24bc-248">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-248">String</span></span>|<span data-ttu-id="d24bc-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d24bc-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d24bc-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="d24bc-252">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-252">String</span></span>|<span data-ttu-id="d24bc-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d24bc-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="d24bc-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="d24bc-256">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-256">String</span></span>|<span data-ttu-id="d24bc-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d24bc-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d24bc-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="d24bc-260">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-260">String</span></span>|<span data-ttu-id="d24bc-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d24bc-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="d24bc-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-263">managedBrowser</span><span class="sxs-lookup"><span data-stu-id="d24bc-263">managedBrowser</span></span>|[<span data-ttu-id="d24bc-264">managedBrowserType</span><span class="sxs-lookup"><span data-stu-id="d24bc-264">managedBrowserType</span></span>](../resources/intune-mam-managedbrowsertype.md)|<span data-ttu-id="d24bc-265">指示在哪个托管浏览器中 (s) 应打开 internet 链接。</span><span class="sxs-lookup"><span data-stu-id="d24bc-265">Indicates in which managed browser(s) that internet links should be opened.</span></span> <span data-ttu-id="d24bc-266">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="d24bc-266">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span> <span data-ttu-id="d24bc-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d24bc-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d24bc-268">可取值为：`notConfigured`、`microsoftEdge`。</span><span class="sxs-lookup"><span data-stu-id="d24bc-268">Possible values are: `notConfigured`, `microsoftEdge`.</span></span>|
|<span data-ttu-id="d24bc-269">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d24bc-269">isAssigned</span></span>|<span data-ttu-id="d24bc-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-270">Boolean</span></span>|<span data-ttu-id="d24bc-271">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="d24bc-271">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d24bc-272">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d24bc-272">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="d24bc-273">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d24bc-273">screenCaptureBlocked</span></span>|<span data-ttu-id="d24bc-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-274">Boolean</span></span>|<span data-ttu-id="d24bc-275">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="d24bc-275">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="d24bc-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="d24bc-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="d24bc-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-277">Boolean</span></span>|<span data-ttu-id="d24bc-278">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="d24bc-278">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="d24bc-279">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="d24bc-279">encryptAppData</span></span>|<span data-ttu-id="d24bc-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="d24bc-280">Boolean</span></span>|<span data-ttu-id="d24bc-281">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="d24bc-281">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="d24bc-282">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="d24bc-282">deployedAppCount</span></span>|<span data-ttu-id="d24bc-283">Int32</span><span class="sxs-lookup"><span data-stu-id="d24bc-283">Int32</span></span>|<span data-ttu-id="d24bc-284">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="d24bc-284">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="d24bc-285">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-285">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="d24bc-286">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-286">String</span></span>|<span data-ttu-id="d24bc-287">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="d24bc-287">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="d24bc-288">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d24bc-288">minimumWarningPatchVersion</span></span>|<span data-ttu-id="d24bc-289">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-289">String</span></span>|<span data-ttu-id="d24bc-290">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="d24bc-290">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="d24bc-291">customBrowserPackageId</span><span class="sxs-lookup"><span data-stu-id="d24bc-291">customBrowserPackageId</span></span>|<span data-ttu-id="d24bc-292">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-292">String</span></span>|<span data-ttu-id="d24bc-293">在 Android 上打开 weblink 的首选自定义浏览器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d24bc-293">Unique identifier of the preferred custom browser to open weblink on Android.</span></span> <span data-ttu-id="d24bc-294">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="d24bc-294">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span>|
|<span data-ttu-id="d24bc-295">customBrowserDisplayName</span><span class="sxs-lookup"><span data-stu-id="d24bc-295">customBrowserDisplayName</span></span>|<span data-ttu-id="d24bc-296">String</span><span class="sxs-lookup"><span data-stu-id="d24bc-296">String</span></span>|<span data-ttu-id="d24bc-297">首选自定义浏览器的友好名称，以在 Android 上打开 weblink。</span><span class="sxs-lookup"><span data-stu-id="d24bc-297">Friendly name of the preferred custom browser to open weblink on Android.</span></span> <span data-ttu-id="d24bc-298">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="d24bc-298">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span>|



## <a name="response"></a><span data-ttu-id="d24bc-299">响应</span><span class="sxs-lookup"><span data-stu-id="d24bc-299">Response</span></span>
<span data-ttu-id="d24bc-300">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d24bc-300">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d24bc-301">示例</span><span class="sxs-lookup"><span data-stu-id="d24bc-301">Example</span></span>

### <a name="request"></a><span data-ttu-id="d24bc-302">请求</span><span class="sxs-lookup"><span data-stu-id="d24bc-302">Request</span></span>
<span data-ttu-id="d24bc-303">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d24bc-303">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 1862

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d24bc-304">响应</span><span class="sxs-lookup"><span data-stu-id="d24bc-304">Response</span></span>
<span data-ttu-id="d24bc-p136">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d24bc-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2034

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value"
}
```






