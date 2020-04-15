---
title: 更新 defaultManagedAppProtection
description: 更新 defaultManagedAppProtection 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d7de635f32e252fa87726a79451cea50ae8844d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463887"
---
# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="dbb20-103">更新 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="dbb20-103">Update defaultManagedAppProtection</span></span>

<span data-ttu-id="dbb20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbb20-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbb20-106">更新 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dbb20-106">Update the properties of a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbb20-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dbb20-107">Prerequisites</span></span>
<span data-ttu-id="dbb20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb20-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbb20-110">Permission type</span></span>|<span data-ttu-id="dbb20-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dbb20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbb20-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbb20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbb20-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb20-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbb20-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbb20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbb20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbb20-115">Not supported.</span></span>|
|<span data-ttu-id="dbb20-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbb20-116">Application</span></span>|<span data-ttu-id="dbb20-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbb20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbb20-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbb20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="dbb20-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbb20-119">Request headers</span></span>
|<span data-ttu-id="dbb20-120">标头</span><span class="sxs-lookup"><span data-stu-id="dbb20-120">Header</span></span>|<span data-ttu-id="dbb20-121">值</span><span class="sxs-lookup"><span data-stu-id="dbb20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbb20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbb20-122">Authorization</span></span>|<span data-ttu-id="dbb20-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dbb20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbb20-124">接受</span><span class="sxs-lookup"><span data-stu-id="dbb20-124">Accept</span></span>|<span data-ttu-id="dbb20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbb20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb20-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbb20-126">Request body</span></span>
<span data-ttu-id="dbb20-127">在请求正文中，提供 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbb20-127">In the request body, supply a JSON representation for the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="dbb20-128">下表显示创建 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dbb20-128">The following table shows the properties that are required when you create the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

|<span data-ttu-id="dbb20-129">属性</span><span class="sxs-lookup"><span data-stu-id="dbb20-129">Property</span></span>|<span data-ttu-id="dbb20-130">类型</span><span class="sxs-lookup"><span data-stu-id="dbb20-130">Type</span></span>|<span data-ttu-id="dbb20-131">说明</span><span class="sxs-lookup"><span data-stu-id="dbb20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb20-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dbb20-132">displayName</span></span>|<span data-ttu-id="dbb20-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dbb20-133">String</span></span>|<span data-ttu-id="dbb20-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="dbb20-134">Policy display name.</span></span> <span data-ttu-id="dbb20-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-136">description</span><span class="sxs-lookup"><span data-stu-id="dbb20-136">description</span></span>|<span data-ttu-id="dbb20-137">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-137">String</span></span>|<span data-ttu-id="dbb20-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dbb20-138">The policy's description.</span></span> <span data-ttu-id="dbb20-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbb20-140">createdDateTime</span></span>|<span data-ttu-id="dbb20-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb20-141">DateTimeOffset</span></span>|<span data-ttu-id="dbb20-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dbb20-142">The date and time the policy was created.</span></span> <span data-ttu-id="dbb20-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbb20-144">lastModifiedDateTime</span></span>|<span data-ttu-id="dbb20-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb20-145">DateTimeOffset</span></span>|<span data-ttu-id="dbb20-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="dbb20-146">Last time the policy was modified.</span></span> <span data-ttu-id="dbb20-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-148">id</span><span class="sxs-lookup"><span data-stu-id="dbb20-148">id</span></span>|<span data-ttu-id="dbb20-149">字符串</span><span class="sxs-lookup"><span data-stu-id="dbb20-149">String</span></span>|<span data-ttu-id="dbb20-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dbb20-150">Key of the entity.</span></span> <span data-ttu-id="dbb20-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-152">version</span><span class="sxs-lookup"><span data-stu-id="dbb20-152">version</span></span>|<span data-ttu-id="dbb20-153">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-153">String</span></span>|<span data-ttu-id="dbb20-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="dbb20-154">Version of the entity.</span></span> <span data-ttu-id="dbb20-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dbb20-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="dbb20-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="dbb20-157">持续时间</span><span class="sxs-lookup"><span data-stu-id="dbb20-157">Duration</span></span>|<span data-ttu-id="dbb20-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="dbb20-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="dbb20-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="dbb20-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="dbb20-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="dbb20-161">Duration</span></span>|<span data-ttu-id="dbb20-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="dbb20-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="dbb20-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="dbb20-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="dbb20-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="dbb20-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="dbb20-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="dbb20-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="dbb20-167">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="dbb20-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="dbb20-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="dbb20-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="dbb20-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="dbb20-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="dbb20-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="dbb20-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="dbb20-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="dbb20-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="dbb20-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="dbb20-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="dbb20-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-175">Boolean</span></span>|<span data-ttu-id="dbb20-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="dbb20-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="dbb20-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="dbb20-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="dbb20-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="dbb20-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="dbb20-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="dbb20-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="dbb20-181">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="dbb20-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="dbb20-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-183">dataBackupBlocked</span></span>|<span data-ttu-id="dbb20-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-184">Boolean</span></span>|<span data-ttu-id="dbb20-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="dbb20-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="dbb20-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="dbb20-187">deviceComplianceRequired</span></span>|<span data-ttu-id="dbb20-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-188">Boolean</span></span>|<span data-ttu-id="dbb20-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="dbb20-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="dbb20-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="dbb20-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="dbb20-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-192">Boolean</span></span>|<span data-ttu-id="dbb20-193">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="dbb20-193">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="dbb20-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-195">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-195">saveAsBlocked</span></span>|<span data-ttu-id="dbb20-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-196">Boolean</span></span>|<span data-ttu-id="dbb20-197">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="dbb20-197">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="dbb20-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-199">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="dbb20-199">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="dbb20-200">持续时间</span><span class="sxs-lookup"><span data-stu-id="dbb20-200">Duration</span></span>|<span data-ttu-id="dbb20-201">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="dbb20-201">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="dbb20-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-203">pinRequired</span><span class="sxs-lookup"><span data-stu-id="dbb20-203">pinRequired</span></span>|<span data-ttu-id="dbb20-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-204">Boolean</span></span>|<span data-ttu-id="dbb20-205">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="dbb20-205">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="dbb20-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-207">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="dbb20-207">maximumPinRetries</span></span>|<span data-ttu-id="dbb20-208">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb20-208">Int32</span></span>|<span data-ttu-id="dbb20-209">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="dbb20-209">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="dbb20-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-211">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-211">simplePinBlocked</span></span>|<span data-ttu-id="dbb20-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-212">Boolean</span></span>|<span data-ttu-id="dbb20-213">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="dbb20-213">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="dbb20-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-215">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="dbb20-215">minimumPinLength</span></span>|<span data-ttu-id="dbb20-216">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb20-216">Int32</span></span>|<span data-ttu-id="dbb20-217">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-217">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-218">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="dbb20-218">pinCharacterSet</span></span>|[<span data-ttu-id="dbb20-219">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="dbb20-219">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="dbb20-220">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="dbb20-220">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="dbb20-221">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-221">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="dbb20-222">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-222">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="dbb20-223">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="dbb20-223">periodBeforePinReset</span></span>|<span data-ttu-id="dbb20-224">Duration</span><span class="sxs-lookup"><span data-stu-id="dbb20-224">Duration</span></span>|<span data-ttu-id="dbb20-225">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="dbb20-225">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="dbb20-226">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-227">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="dbb20-227">allowedDataStorageLocations</span></span>|<span data-ttu-id="dbb20-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbb20-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="dbb20-229">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="dbb20-229">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="dbb20-230">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="dbb20-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="dbb20-231">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-231">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="dbb20-232">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-232">contactSyncBlocked</span></span>|<span data-ttu-id="dbb20-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-233">Boolean</span></span>|<span data-ttu-id="dbb20-234">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="dbb20-234">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="dbb20-235">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-236">printBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-236">printBlocked</span></span>|<span data-ttu-id="dbb20-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-237">Boolean</span></span>|<span data-ttu-id="dbb20-238">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="dbb20-238">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="dbb20-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-240">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-240">fingerprintBlocked</span></span>|<span data-ttu-id="dbb20-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-241">Boolean</span></span>|<span data-ttu-id="dbb20-242">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="dbb20-242">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="dbb20-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-244">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="dbb20-244">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="dbb20-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-245">Boolean</span></span>|<span data-ttu-id="dbb20-246">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="dbb20-246">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="dbb20-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-248">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-248">minimumRequiredOsVersion</span></span>|<span data-ttu-id="dbb20-249">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-249">String</span></span>|<span data-ttu-id="dbb20-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="dbb20-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="dbb20-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-252">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-252">minimumWarningOsVersion</span></span>|<span data-ttu-id="dbb20-253">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-253">String</span></span>|<span data-ttu-id="dbb20-254">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="dbb20-254">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="dbb20-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-256">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-256">minimumRequiredAppVersion</span></span>|<span data-ttu-id="dbb20-257">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-257">String</span></span>|<span data-ttu-id="dbb20-258">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="dbb20-258">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="dbb20-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-260">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-260">minimumWarningAppVersion</span></span>|<span data-ttu-id="dbb20-261">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-261">String</span></span>|<span data-ttu-id="dbb20-262">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="dbb20-262">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="dbb20-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="dbb20-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="dbb20-264">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="dbb20-264">appDataEncryptionType</span></span>|[<span data-ttu-id="dbb20-265">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="dbb20-265">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="dbb20-266">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="dbb20-266">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="dbb20-267">（仅限 iOS）。</span><span class="sxs-lookup"><span data-stu-id="dbb20-267">(iOS Only).</span></span> <span data-ttu-id="dbb20-268">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="dbb20-268">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="dbb20-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-269">screenCaptureBlocked</span></span>|<span data-ttu-id="dbb20-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-270">Boolean</span></span>|<span data-ttu-id="dbb20-271">指示是否阻止捕获屏幕。</span><span class="sxs-lookup"><span data-stu-id="dbb20-271">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="dbb20-272">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="dbb20-272">(Android only)</span></span>|
|<span data-ttu-id="dbb20-273">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="dbb20-273">encryptAppData</span></span>|<span data-ttu-id="dbb20-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-274">Boolean</span></span>|<span data-ttu-id="dbb20-275">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="dbb20-275">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="dbb20-276">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="dbb20-276">(Android only)</span></span>|
|<span data-ttu-id="dbb20-277">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="dbb20-277">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="dbb20-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-278">Boolean</span></span>|<span data-ttu-id="dbb20-279">如果启用此设置，则在启用设备级加密的情况下禁用应用级加密。</span><span class="sxs-lookup"><span data-stu-id="dbb20-279">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="dbb20-280">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="dbb20-280">(Android only)</span></span>|
|<span data-ttu-id="dbb20-281">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-281">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="dbb20-282">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-282">String</span></span>|<span data-ttu-id="dbb20-283">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="dbb20-283">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="dbb20-284">（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="dbb20-284">(iOS Only)</span></span>|
|<span data-ttu-id="dbb20-285">customSettings</span><span class="sxs-lookup"><span data-stu-id="dbb20-285">customSettings</span></span>|<span data-ttu-id="dbb20-286">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dbb20-286">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="dbb20-287">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="dbb20-287">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="dbb20-288">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="dbb20-288">deployedAppCount</span></span>|<span data-ttu-id="dbb20-289">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb20-289">Int32</span></span>|<span data-ttu-id="dbb20-290">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="dbb20-290">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="dbb20-291">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-291">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="dbb20-292">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-292">String</span></span>|<span data-ttu-id="dbb20-293">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="dbb20-293">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="dbb20-294">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="dbb20-294">(Android only)</span></span>|
|<span data-ttu-id="dbb20-295">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="dbb20-295">minimumWarningPatchVersion</span></span>|<span data-ttu-id="dbb20-296">String</span><span class="sxs-lookup"><span data-stu-id="dbb20-296">String</span></span>|<span data-ttu-id="dbb20-297">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="dbb20-297">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="dbb20-298">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="dbb20-298">(Android only)</span></span>|
|<span data-ttu-id="dbb20-299">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="dbb20-299">faceIdBlocked</span></span>|<span data-ttu-id="dbb20-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbb20-300">Boolean</span></span>|<span data-ttu-id="dbb20-301">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="dbb20-301">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="dbb20-302">（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="dbb20-302">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="dbb20-303">响应</span><span class="sxs-lookup"><span data-stu-id="dbb20-303">Response</span></span>
<span data-ttu-id="dbb20-304">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbb20-304">If successful, this method returns a `200 OK` response code and an updated [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbb20-305">示例</span><span class="sxs-lookup"><span data-stu-id="dbb20-305">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbb20-306">请求</span><span class="sxs-lookup"><span data-stu-id="dbb20-306">Request</span></span>
<span data-ttu-id="dbb20-307">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbb20-307">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 1971

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

### <a name="response"></a><span data-ttu-id="dbb20-308">响应</span><span class="sxs-lookup"><span data-stu-id="dbb20-308">Response</span></span>
<span data-ttu-id="dbb20-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbb20-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2143

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






