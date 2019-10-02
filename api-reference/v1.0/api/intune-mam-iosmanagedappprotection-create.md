---
title: 创建 iosManagedAppProtection
description: 创建新的 iosManagedAppProtection 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcbf582bb7150adb3f412a8055f17fc6e77e5898
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363834"
---
# <a name="create-iosmanagedappprotection"></a><span data-ttu-id="c0d1e-103">创建 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c0d1e-103">Create iosManagedAppProtection</span></span>

> <span data-ttu-id="c0d1e-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0d1e-105">创建新的 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-105">Create a new [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0d1e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0d1e-106">Prerequisites</span></span>
<span data-ttu-id="c0d1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d1e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0d1e-109">Permission type</span></span>|<span data-ttu-id="c0d1e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0d1e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0d1e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0d1e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0d1e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d1e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0d1e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0d1e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0d1e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-114">Not supported.</span></span>|
|<span data-ttu-id="c0d1e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0d1e-115">Application</span></span>|<span data-ttu-id="c0d1e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0d1e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0d1e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="c0d1e-118">请求头</span><span class="sxs-lookup"><span data-stu-id="c0d1e-118">Request headers</span></span>
|<span data-ttu-id="c0d1e-119">标头</span><span class="sxs-lookup"><span data-stu-id="c0d1e-119">Header</span></span>|<span data-ttu-id="c0d1e-120">值</span><span class="sxs-lookup"><span data-stu-id="c0d1e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0d1e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d1e-121">Authorization</span></span>|<span data-ttu-id="c0d1e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0d1e-123">接受</span><span class="sxs-lookup"><span data-stu-id="c0d1e-123">Accept</span></span>|<span data-ttu-id="c0d1e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c0d1e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d1e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0d1e-125">Request body</span></span>
<span data-ttu-id="c0d1e-126">在请求正文中，提供 iosManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-126">In the request body, supply a JSON representation for the iosManagedAppProtection object.</span></span>

<span data-ttu-id="c0d1e-127">下表显示创建 iosManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-127">The following table shows the properties that are required when you create the iosManagedAppProtection.</span></span>

|<span data-ttu-id="c0d1e-128">属性</span><span class="sxs-lookup"><span data-stu-id="c0d1e-128">Property</span></span>|<span data-ttu-id="c0d1e-129">类型</span><span class="sxs-lookup"><span data-stu-id="c0d1e-129">Type</span></span>|<span data-ttu-id="c0d1e-130">说明</span><span class="sxs-lookup"><span data-stu-id="c0d1e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0d1e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c0d1e-131">displayName</span></span>|<span data-ttu-id="c0d1e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c0d1e-132">String</span></span>|<span data-ttu-id="c0d1e-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-133">Policy display name.</span></span> <span data-ttu-id="c0d1e-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-135">说明</span><span class="sxs-lookup"><span data-stu-id="c0d1e-135">description</span></span>|<span data-ttu-id="c0d1e-136">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-136">String</span></span>|<span data-ttu-id="c0d1e-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-137">The policy's description.</span></span> <span data-ttu-id="c0d1e-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0d1e-139">createdDateTime</span></span>|<span data-ttu-id="c0d1e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0d1e-140">DateTimeOffset</span></span>|<span data-ttu-id="c0d1e-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-141">The date and time the policy was created.</span></span> <span data-ttu-id="c0d1e-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0d1e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="c0d1e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0d1e-144">DateTimeOffset</span></span>|<span data-ttu-id="c0d1e-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-145">Last time the policy was modified.</span></span> <span data-ttu-id="c0d1e-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-147">id</span><span class="sxs-lookup"><span data-stu-id="c0d1e-147">id</span></span>|<span data-ttu-id="c0d1e-148">字符串</span><span class="sxs-lookup"><span data-stu-id="c0d1e-148">String</span></span>|<span data-ttu-id="c0d1e-149">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-149">Key of the entity.</span></span> <span data-ttu-id="c0d1e-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-151">version</span><span class="sxs-lookup"><span data-stu-id="c0d1e-151">version</span></span>|<span data-ttu-id="c0d1e-152">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-152">String</span></span>|<span data-ttu-id="c0d1e-153">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-153">Version of the entity.</span></span> <span data-ttu-id="c0d1e-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c0d1e-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c0d1e-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="c0d1e-156">持续时间</span><span class="sxs-lookup"><span data-stu-id="c0d1e-156">Duration</span></span>|<span data-ttu-id="c0d1e-157">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="c0d1e-158">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c0d1e-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="c0d1e-160">持续时间</span><span class="sxs-lookup"><span data-stu-id="c0d1e-160">Duration</span></span>|<span data-ttu-id="c0d1e-161">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="c0d1e-162">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="c0d1e-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="c0d1e-164">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c0d1e-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c0d1e-165">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="c0d1e-166">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c0d1e-167">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c0d1e-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="c0d1e-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="c0d1e-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="c0d1e-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c0d1e-170">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="c0d1e-171">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c0d1e-172">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c0d1e-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="c0d1e-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="c0d1e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-174">Boolean</span></span>|<span data-ttu-id="c0d1e-175">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="c0d1e-176">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c0d1e-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="c0d1e-178">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c0d1e-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="c0d1e-179">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="c0d1e-180">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c0d1e-181">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="c0d1e-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-182">dataBackupBlocked</span></span>|<span data-ttu-id="c0d1e-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-183">Boolean</span></span>|<span data-ttu-id="c0d1e-184">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="c0d1e-185">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="c0d1e-186">deviceComplianceRequired</span></span>|<span data-ttu-id="c0d1e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-187">Boolean</span></span>|<span data-ttu-id="c0d1e-188">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="c0d1e-189">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="c0d1e-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="c0d1e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-191">Boolean</span></span>|<span data-ttu-id="c0d1e-192">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="c0d1e-193">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-194">saveAsBlocked</span></span>|<span data-ttu-id="c0d1e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-195">Boolean</span></span>|<span data-ttu-id="c0d1e-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="c0d1e-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="c0d1e-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="c0d1e-199">持续时间</span><span class="sxs-lookup"><span data-stu-id="c0d1e-199">Duration</span></span>|<span data-ttu-id="c0d1e-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="c0d1e-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="c0d1e-202">pinRequired</span></span>|<span data-ttu-id="c0d1e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-203">Boolean</span></span>|<span data-ttu-id="c0d1e-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="c0d1e-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="c0d1e-206">maximumPinRetries</span></span>|<span data-ttu-id="c0d1e-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d1e-207">Int32</span></span>|<span data-ttu-id="c0d1e-208">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="c0d1e-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-210">simplePinBlocked</span></span>|<span data-ttu-id="c0d1e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-211">Boolean</span></span>|<span data-ttu-id="c0d1e-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="c0d1e-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="c0d1e-214">minimumPinLength</span></span>|<span data-ttu-id="c0d1e-215">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d1e-215">Int32</span></span>|<span data-ttu-id="c0d1e-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c0d1e-217">pinCharacterSet</span></span>|[<span data-ttu-id="c0d1e-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c0d1e-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="c0d1e-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="c0d1e-220">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c0d1e-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="c0d1e-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="c0d1e-222">periodBeforePinReset</span></span>|<span data-ttu-id="c0d1e-223">Duration</span><span class="sxs-lookup"><span data-stu-id="c0d1e-223">Duration</span></span>|<span data-ttu-id="c0d1e-224">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="c0d1e-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="c0d1e-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="c0d1e-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0d1e-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="c0d1e-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="c0d1e-229">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="c0d1e-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="c0d1e-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-231">contactSyncBlocked</span></span>|<span data-ttu-id="c0d1e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-232">Boolean</span></span>|<span data-ttu-id="c0d1e-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="c0d1e-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-235">printBlocked</span></span>|<span data-ttu-id="c0d1e-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-236">Boolean</span></span>|<span data-ttu-id="c0d1e-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="c0d1e-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-239">fingerprintBlocked</span></span>|<span data-ttu-id="c0d1e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-240">Boolean</span></span>|<span data-ttu-id="c0d1e-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="c0d1e-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="c0d1e-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="c0d1e-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-244">Boolean</span></span>|<span data-ttu-id="c0d1e-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="c0d1e-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0d1e-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="c0d1e-248">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-248">String</span></span>|<span data-ttu-id="c0d1e-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c0d1e-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0d1e-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="c0d1e-252">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-252">String</span></span>|<span data-ttu-id="c0d1e-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="c0d1e-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="c0d1e-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="c0d1e-256">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-256">String</span></span>|<span data-ttu-id="c0d1e-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="c0d1e-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="c0d1e-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="c0d1e-260">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-260">String</span></span>|<span data-ttu-id="c0d1e-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="c0d1e-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-263">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c0d1e-263">isAssigned</span></span>|<span data-ttu-id="c0d1e-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-264">Boolean</span></span>|<span data-ttu-id="c0d1e-265">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-265">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="c0d1e-266">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1e-266">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="c0d1e-267">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c0d1e-267">appDataEncryptionType</span></span>|[<span data-ttu-id="c0d1e-268">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="c0d1e-268">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="c0d1e-269">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-269">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="c0d1e-270">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-270">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="c0d1e-271">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c0d1e-271">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="c0d1e-272">String</span><span class="sxs-lookup"><span data-stu-id="c0d1e-272">String</span></span>|<span data-ttu-id="c0d1e-273">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-273">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="c0d1e-274">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c0d1e-274">deployedAppCount</span></span>|<span data-ttu-id="c0d1e-275">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d1e-275">Int32</span></span>|<span data-ttu-id="c0d1e-276">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-276">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c0d1e-277">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="c0d1e-277">faceIdBlocked</span></span>|<span data-ttu-id="c0d1e-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0d1e-278">Boolean</span></span>|<span data-ttu-id="c0d1e-279">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-279">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|



## <a name="response"></a><span data-ttu-id="c0d1e-280">响应</span><span class="sxs-lookup"><span data-stu-id="c0d1e-280">Response</span></span>
<span data-ttu-id="c0d1e-281">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-281">If successful, this method returns a `201 Created` response code and a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0d1e-282">示例</span><span class="sxs-lookup"><span data-stu-id="c0d1e-282">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0d1e-283">请求</span><span class="sxs-lookup"><span data-stu-id="c0d1e-283">Request</span></span>
<span data-ttu-id="c0d1e-284">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-284">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
Content-type: application/json
Content-length: 1568

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
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="c0d1e-285">响应</span><span class="sxs-lookup"><span data-stu-id="c0d1e-285">Response</span></span>
<span data-ttu-id="c0d1e-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0d1e-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1740

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
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```




