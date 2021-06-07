---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f58139d5f037818a0f054966b110316bc59d64b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758134"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="c3684-103">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c3684-103">Create defaultManagedAppProtection</span></span>

<span data-ttu-id="c3684-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3684-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3684-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3684-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3684-106">创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3684-106">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3684-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3684-107">Prerequisites</span></span>
<span data-ttu-id="c3684-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3684-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3684-110">Permission type</span></span>|<span data-ttu-id="c3684-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3684-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3684-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3684-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3684-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3684-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3684-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3684-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3684-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3684-115">Not supported.</span></span>|
|<span data-ttu-id="c3684-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3684-116">Application</span></span>|<span data-ttu-id="c3684-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3684-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3684-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3684-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="c3684-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3684-119">Request headers</span></span>
|<span data-ttu-id="c3684-120">标头</span><span class="sxs-lookup"><span data-stu-id="c3684-120">Header</span></span>|<span data-ttu-id="c3684-121">值</span><span class="sxs-lookup"><span data-stu-id="c3684-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3684-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3684-122">Authorization</span></span>|<span data-ttu-id="c3684-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3684-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3684-124">接受</span><span class="sxs-lookup"><span data-stu-id="c3684-124">Accept</span></span>|<span data-ttu-id="c3684-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3684-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3684-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3684-126">Request body</span></span>
<span data-ttu-id="c3684-127">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3684-127">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="c3684-128">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3684-128">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="c3684-129">属性</span><span class="sxs-lookup"><span data-stu-id="c3684-129">Property</span></span>|<span data-ttu-id="c3684-130">类型</span><span class="sxs-lookup"><span data-stu-id="c3684-130">Type</span></span>|<span data-ttu-id="c3684-131">说明</span><span class="sxs-lookup"><span data-stu-id="c3684-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3684-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c3684-132">displayName</span></span>|<span data-ttu-id="c3684-133">String</span><span class="sxs-lookup"><span data-stu-id="c3684-133">String</span></span>|<span data-ttu-id="c3684-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3684-134">Policy display name.</span></span> <span data-ttu-id="c3684-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-136">description</span><span class="sxs-lookup"><span data-stu-id="c3684-136">description</span></span>|<span data-ttu-id="c3684-137">String</span><span class="sxs-lookup"><span data-stu-id="c3684-137">String</span></span>|<span data-ttu-id="c3684-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c3684-138">The policy's description.</span></span> <span data-ttu-id="c3684-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3684-140">createdDateTime</span></span>|<span data-ttu-id="c3684-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3684-141">DateTimeOffset</span></span>|<span data-ttu-id="c3684-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3684-142">The date and time the policy was created.</span></span> <span data-ttu-id="c3684-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3684-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c3684-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3684-145">DateTimeOffset</span></span>|<span data-ttu-id="c3684-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c3684-146">Last time the policy was modified.</span></span> <span data-ttu-id="c3684-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-148">id</span><span class="sxs-lookup"><span data-stu-id="c3684-148">id</span></span>|<span data-ttu-id="c3684-149">String</span><span class="sxs-lookup"><span data-stu-id="c3684-149">String</span></span>|<span data-ttu-id="c3684-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3684-150">Key of the entity.</span></span> <span data-ttu-id="c3684-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-152">version</span><span class="sxs-lookup"><span data-stu-id="c3684-152">version</span></span>|<span data-ttu-id="c3684-153">String</span><span class="sxs-lookup"><span data-stu-id="c3684-153">String</span></span>|<span data-ttu-id="c3684-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c3684-154">Version of the entity.</span></span> <span data-ttu-id="c3684-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3684-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c3684-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="c3684-157">Duration</span><span class="sxs-lookup"><span data-stu-id="c3684-157">Duration</span></span>|<span data-ttu-id="c3684-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c3684-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="c3684-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c3684-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="c3684-161">Duration</span><span class="sxs-lookup"><span data-stu-id="c3684-161">Duration</span></span>|<span data-ttu-id="c3684-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c3684-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="c3684-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="c3684-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="c3684-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c3684-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c3684-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="c3684-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="c3684-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c3684-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c3684-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="c3684-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="c3684-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c3684-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c3684-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="c3684-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="c3684-172">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c3684-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c3684-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="c3684-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="c3684-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-175">Boolean</span></span>|<span data-ttu-id="c3684-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="c3684-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="c3684-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c3684-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="c3684-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c3684-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="c3684-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="c3684-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="c3684-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c3684-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="c3684-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-183">dataBackupBlocked</span></span>|<span data-ttu-id="c3684-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-184">Boolean</span></span>|<span data-ttu-id="c3684-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="c3684-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="c3684-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="c3684-187">deviceComplianceRequired</span></span>|<span data-ttu-id="c3684-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-188">Boolean</span></span>|<span data-ttu-id="c3684-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="c3684-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="c3684-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="c3684-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="c3684-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-192">Boolean</span></span>|<span data-ttu-id="c3684-193">指示是应在托管浏览器应用中打开 Internet 链接，还是应在由 CustomBrowserProtocol (for iOS) 或 CustomBrowserPackageId/CustomBrowserDisplayName (for Android) 指定的任何自定义浏览器继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-193">Indicates whether internet links should be opened in the managed browser app, or any custom browser specified by CustomBrowserProtocol (for iOS) or CustomBrowserPackageId/CustomBrowserDisplayName (for Android) Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-194">saveAsBlocked</span></span>|<span data-ttu-id="c3684-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-195">Boolean</span></span>|<span data-ttu-id="c3684-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="c3684-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="c3684-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="c3684-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="c3684-199">Duration</span><span class="sxs-lookup"><span data-stu-id="c3684-199">Duration</span></span>|<span data-ttu-id="c3684-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="c3684-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="c3684-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="c3684-202">pinRequired</span></span>|<span data-ttu-id="c3684-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-203">Boolean</span></span>|<span data-ttu-id="c3684-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="c3684-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="c3684-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="c3684-206">maximumPinRetries</span></span>|<span data-ttu-id="c3684-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c3684-207">Int32</span></span>|<span data-ttu-id="c3684-208">阻止或擦除托管应用之前的最大错误引脚重试次数。</span><span class="sxs-lookup"><span data-stu-id="c3684-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="c3684-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-210">simplePinBlocked</span></span>|<span data-ttu-id="c3684-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-211">Boolean</span></span>|<span data-ttu-id="c3684-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="c3684-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="c3684-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="c3684-214">minimumPinLength</span></span>|<span data-ttu-id="c3684-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c3684-215">Int32</span></span>|<span data-ttu-id="c3684-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c3684-217">pinCharacterSet</span></span>|[<span data-ttu-id="c3684-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c3684-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="c3684-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="c3684-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="c3684-220">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="c3684-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="c3684-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="c3684-222">periodBeforePinReset</span></span>|<span data-ttu-id="c3684-223">Duration</span><span class="sxs-lookup"><span data-stu-id="c3684-223">Duration</span></span>|<span data-ttu-id="c3684-224">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="c3684-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="c3684-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="c3684-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="c3684-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3684-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="c3684-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="c3684-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="c3684-229">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`box`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="c3684-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `box`, `localStorage`.</span></span>|
|<span data-ttu-id="c3684-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-231">contactSyncBlocked</span></span>|<span data-ttu-id="c3684-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-232">Boolean</span></span>|<span data-ttu-id="c3684-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="c3684-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="c3684-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-235">printBlocked</span></span>|<span data-ttu-id="c3684-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-236">Boolean</span></span>|<span data-ttu-id="c3684-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="c3684-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="c3684-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-239">fingerprintBlocked</span></span>|<span data-ttu-id="c3684-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-240">Boolean</span></span>|<span data-ttu-id="c3684-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c3684-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="c3684-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="c3684-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="c3684-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-244">Boolean</span></span>|<span data-ttu-id="c3684-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="c3684-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="c3684-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="c3684-248">String</span><span class="sxs-lookup"><span data-stu-id="c3684-248">String</span></span>|<span data-ttu-id="c3684-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c3684-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c3684-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="c3684-252">String</span><span class="sxs-lookup"><span data-stu-id="c3684-252">String</span></span>|<span data-ttu-id="c3684-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c3684-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="c3684-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="c3684-256">String</span><span class="sxs-lookup"><span data-stu-id="c3684-256">String</span></span>|<span data-ttu-id="c3684-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c3684-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c3684-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="c3684-260">String</span><span class="sxs-lookup"><span data-stu-id="c3684-260">String</span></span>|<span data-ttu-id="c3684-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c3684-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="c3684-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c3684-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c3684-263">managedBrowser</span><span class="sxs-lookup"><span data-stu-id="c3684-263">managedBrowser</span></span>|[<span data-ttu-id="c3684-264">managedBrowserType</span><span class="sxs-lookup"><span data-stu-id="c3684-264">managedBrowserType</span></span>](../resources/intune-mam-managedbrowsertype.md)|<span data-ttu-id="c3684-265">指示应在哪个托管 (浏览器) 打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="c3684-265">Indicates in which managed browser(s) that internet links should be opened.</span></span> <span data-ttu-id="c3684-266">配置此属性时，ManagedBrowserToOpenLinksRequired 应为 true。</span><span class="sxs-lookup"><span data-stu-id="c3684-266">When this property is configured, ManagedBrowserToOpenLinksRequired should be true.</span></span> <span data-ttu-id="c3684-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c3684-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c3684-268">可取值为：`notConfigured`、`microsoftEdge`。</span><span class="sxs-lookup"><span data-stu-id="c3684-268">Possible values are: `notConfigured`, `microsoftEdge`.</span></span>|
|<span data-ttu-id="c3684-269">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c3684-269">appDataEncryptionType</span></span>|[<span data-ttu-id="c3684-270">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c3684-270">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="c3684-271">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="c3684-271">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="c3684-272"> (仅 iOS) 。</span><span class="sxs-lookup"><span data-stu-id="c3684-272">(iOS Only).</span></span> <span data-ttu-id="c3684-273">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="c3684-273">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="c3684-274">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-274">screenCaptureBlocked</span></span>|<span data-ttu-id="c3684-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-275">Boolean</span></span>|<span data-ttu-id="c3684-276">指示是否阻止捕获屏幕。</span><span class="sxs-lookup"><span data-stu-id="c3684-276">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="c3684-277">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="c3684-277">(Android only)</span></span>|
|<span data-ttu-id="c3684-278">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="c3684-278">encryptAppData</span></span>|<span data-ttu-id="c3684-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-279">Boolean</span></span>|<span data-ttu-id="c3684-280">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="c3684-280">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="c3684-281">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="c3684-281">(Android only)</span></span>|
|<span data-ttu-id="c3684-282">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="c3684-282">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="c3684-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-283">Boolean</span></span>|<span data-ttu-id="c3684-284">启用此设置后，如果启用了设备级别加密，则应用级别加密将被禁用。</span><span class="sxs-lookup"><span data-stu-id="c3684-284">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="c3684-285">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="c3684-285">(Android only)</span></span>|
|<span data-ttu-id="c3684-286">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-286">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="c3684-287">String</span><span class="sxs-lookup"><span data-stu-id="c3684-287">String</span></span>|<span data-ttu-id="c3684-288">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c3684-288">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c3684-289"> (仅 iOS) </span><span class="sxs-lookup"><span data-stu-id="c3684-289">(iOS Only)</span></span>|
|<span data-ttu-id="c3684-290">customSettings</span><span class="sxs-lookup"><span data-stu-id="c3684-290">customSettings</span></span>|<span data-ttu-id="c3684-291">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3684-291">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c3684-292">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="c3684-292">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="c3684-293">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c3684-293">deployedAppCount</span></span>|<span data-ttu-id="c3684-294">Int32</span><span class="sxs-lookup"><span data-stu-id="c3684-294">Int32</span></span>|<span data-ttu-id="c3684-295">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="c3684-295">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c3684-296">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-296">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="c3684-297">String</span><span class="sxs-lookup"><span data-stu-id="c3684-297">String</span></span>|<span data-ttu-id="c3684-298">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="c3684-298">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="c3684-299">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="c3684-299">(Android only)</span></span>|
|<span data-ttu-id="c3684-300">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="c3684-300">minimumWarningPatchVersion</span></span>|<span data-ttu-id="c3684-301">String</span><span class="sxs-lookup"><span data-stu-id="c3684-301">String</span></span>|<span data-ttu-id="c3684-302">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="c3684-302">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="c3684-303">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="c3684-303">(Android only)</span></span>|
|<span data-ttu-id="c3684-304">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="c3684-304">faceIdBlocked</span></span>|<span data-ttu-id="c3684-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3684-305">Boolean</span></span>|<span data-ttu-id="c3684-306">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c3684-306">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="c3684-307"> (仅 iOS) </span><span class="sxs-lookup"><span data-stu-id="c3684-307">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="c3684-308">响应</span><span class="sxs-lookup"><span data-stu-id="c3684-308">Response</span></span>
<span data-ttu-id="c3684-309">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3684-309">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3684-310">示例</span><span class="sxs-lookup"><span data-stu-id="c3684-310">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3684-311">请求</span><span class="sxs-lookup"><span data-stu-id="c3684-311">Request</span></span>
<span data-ttu-id="c3684-312">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3684-312">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3684-313">响应</span><span class="sxs-lookup"><span data-stu-id="c3684-313">Response</span></span>
<span data-ttu-id="c3684-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3684-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




