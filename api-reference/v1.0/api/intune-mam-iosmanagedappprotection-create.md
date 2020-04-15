---
title: 创建 iosManagedAppProtection
description: 创建新的 iosManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c6a102544394e5db97dd3977dfb7c2529cb9549
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399288"
---
# <a name="create-iosmanagedappprotection"></a><span data-ttu-id="a65b2-103">创建 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a65b2-103">Create iosManagedAppProtection</span></span>

<span data-ttu-id="a65b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a65b2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a65b2-106">创建新的 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a65b2-106">Create a new [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a65b2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a65b2-107">Prerequisites</span></span>
<span data-ttu-id="a65b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65b2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a65b2-110">Permission type</span></span>|<span data-ttu-id="a65b2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a65b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a65b2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a65b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a65b2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65b2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a65b2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a65b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a65b2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a65b2-115">Not supported.</span></span>|
|<span data-ttu-id="a65b2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a65b2-116">Application</span></span>|<span data-ttu-id="a65b2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a65b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a65b2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a65b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="a65b2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a65b2-119">Request headers</span></span>
|<span data-ttu-id="a65b2-120">标头</span><span class="sxs-lookup"><span data-stu-id="a65b2-120">Header</span></span>|<span data-ttu-id="a65b2-121">值</span><span class="sxs-lookup"><span data-stu-id="a65b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a65b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a65b2-122">Authorization</span></span>|<span data-ttu-id="a65b2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a65b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a65b2-124">接受</span><span class="sxs-lookup"><span data-stu-id="a65b2-124">Accept</span></span>|<span data-ttu-id="a65b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a65b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65b2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a65b2-126">Request body</span></span>
<span data-ttu-id="a65b2-127">在请求正文中，提供 iosManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a65b2-127">In the request body, supply a JSON representation for the iosManagedAppProtection object.</span></span>

<span data-ttu-id="a65b2-128">下表显示创建 iosManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a65b2-128">The following table shows the properties that are required when you create the iosManagedAppProtection.</span></span>

|<span data-ttu-id="a65b2-129">属性</span><span class="sxs-lookup"><span data-stu-id="a65b2-129">Property</span></span>|<span data-ttu-id="a65b2-130">类型</span><span class="sxs-lookup"><span data-stu-id="a65b2-130">Type</span></span>|<span data-ttu-id="a65b2-131">说明</span><span class="sxs-lookup"><span data-stu-id="a65b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a65b2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a65b2-132">displayName</span></span>|<span data-ttu-id="a65b2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a65b2-133">String</span></span>|<span data-ttu-id="a65b2-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a65b2-134">Policy display name.</span></span> <span data-ttu-id="a65b2-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-136">description</span><span class="sxs-lookup"><span data-stu-id="a65b2-136">description</span></span>|<span data-ttu-id="a65b2-137">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-137">String</span></span>|<span data-ttu-id="a65b2-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a65b2-138">The policy's description.</span></span> <span data-ttu-id="a65b2-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a65b2-140">createdDateTime</span></span>|<span data-ttu-id="a65b2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65b2-141">DateTimeOffset</span></span>|<span data-ttu-id="a65b2-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a65b2-142">The date and time the policy was created.</span></span> <span data-ttu-id="a65b2-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a65b2-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a65b2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65b2-145">DateTimeOffset</span></span>|<span data-ttu-id="a65b2-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="a65b2-146">Last time the policy was modified.</span></span> <span data-ttu-id="a65b2-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-148">id</span><span class="sxs-lookup"><span data-stu-id="a65b2-148">id</span></span>|<span data-ttu-id="a65b2-149">字符串</span><span class="sxs-lookup"><span data-stu-id="a65b2-149">String</span></span>|<span data-ttu-id="a65b2-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a65b2-150">Key of the entity.</span></span> <span data-ttu-id="a65b2-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-152">version</span><span class="sxs-lookup"><span data-stu-id="a65b2-152">version</span></span>|<span data-ttu-id="a65b2-153">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-153">String</span></span>|<span data-ttu-id="a65b2-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a65b2-154">Version of the entity.</span></span> <span data-ttu-id="a65b2-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a65b2-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="a65b2-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="a65b2-157">持续时间</span><span class="sxs-lookup"><span data-stu-id="a65b2-157">Duration</span></span>|<span data-ttu-id="a65b2-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="a65b2-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="a65b2-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="a65b2-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="a65b2-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="a65b2-161">Duration</span></span>|<span data-ttu-id="a65b2-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="a65b2-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="a65b2-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="a65b2-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="a65b2-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="a65b2-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="a65b2-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="a65b2-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="a65b2-167">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a65b2-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="a65b2-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="a65b2-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="a65b2-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="a65b2-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="a65b2-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="a65b2-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="a65b2-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a65b2-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="a65b2-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="a65b2-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="a65b2-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-175">Boolean</span></span>|<span data-ttu-id="a65b2-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="a65b2-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="a65b2-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="a65b2-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="a65b2-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="a65b2-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="a65b2-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="a65b2-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="a65b2-181">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a65b2-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="a65b2-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-183">dataBackupBlocked</span></span>|<span data-ttu-id="a65b2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-184">Boolean</span></span>|<span data-ttu-id="a65b2-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="a65b2-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="a65b2-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="a65b2-187">deviceComplianceRequired</span></span>|<span data-ttu-id="a65b2-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-188">Boolean</span></span>|<span data-ttu-id="a65b2-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="a65b2-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="a65b2-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="a65b2-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="a65b2-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-192">Boolean</span></span>|<span data-ttu-id="a65b2-193">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="a65b2-193">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="a65b2-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-195">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-195">saveAsBlocked</span></span>|<span data-ttu-id="a65b2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-196">Boolean</span></span>|<span data-ttu-id="a65b2-197">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="a65b2-197">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="a65b2-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-199">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="a65b2-199">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="a65b2-200">持续时间</span><span class="sxs-lookup"><span data-stu-id="a65b2-200">Duration</span></span>|<span data-ttu-id="a65b2-201">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="a65b2-201">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="a65b2-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-203">pinRequired</span><span class="sxs-lookup"><span data-stu-id="a65b2-203">pinRequired</span></span>|<span data-ttu-id="a65b2-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-204">Boolean</span></span>|<span data-ttu-id="a65b2-205">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="a65b2-205">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="a65b2-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-207">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="a65b2-207">maximumPinRetries</span></span>|<span data-ttu-id="a65b2-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a65b2-208">Int32</span></span>|<span data-ttu-id="a65b2-209">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="a65b2-209">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="a65b2-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-211">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-211">simplePinBlocked</span></span>|<span data-ttu-id="a65b2-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-212">Boolean</span></span>|<span data-ttu-id="a65b2-213">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="a65b2-213">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="a65b2-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-215">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="a65b2-215">minimumPinLength</span></span>|<span data-ttu-id="a65b2-216">Int32</span><span class="sxs-lookup"><span data-stu-id="a65b2-216">Int32</span></span>|<span data-ttu-id="a65b2-217">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-217">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-218">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="a65b2-218">pinCharacterSet</span></span>|[<span data-ttu-id="a65b2-219">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="a65b2-219">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="a65b2-220">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="a65b2-220">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="a65b2-221">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-221">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a65b2-222">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-222">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="a65b2-223">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="a65b2-223">periodBeforePinReset</span></span>|<span data-ttu-id="a65b2-224">Duration</span><span class="sxs-lookup"><span data-stu-id="a65b2-224">Duration</span></span>|<span data-ttu-id="a65b2-225">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="a65b2-225">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="a65b2-226">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-227">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="a65b2-227">allowedDataStorageLocations</span></span>|<span data-ttu-id="a65b2-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="a65b2-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="a65b2-229">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="a65b2-229">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="a65b2-230">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a65b2-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a65b2-231">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-231">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="a65b2-232">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-232">contactSyncBlocked</span></span>|<span data-ttu-id="a65b2-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-233">Boolean</span></span>|<span data-ttu-id="a65b2-234">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="a65b2-234">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="a65b2-235">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-236">printBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-236">printBlocked</span></span>|<span data-ttu-id="a65b2-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-237">Boolean</span></span>|<span data-ttu-id="a65b2-238">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="a65b2-238">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="a65b2-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-240">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-240">fingerprintBlocked</span></span>|<span data-ttu-id="a65b2-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-241">Boolean</span></span>|<span data-ttu-id="a65b2-242">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="a65b2-242">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="a65b2-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-244">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="a65b2-244">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="a65b2-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-245">Boolean</span></span>|<span data-ttu-id="a65b2-246">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="a65b2-246">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="a65b2-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-248">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="a65b2-248">minimumRequiredOsVersion</span></span>|<span data-ttu-id="a65b2-249">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-249">String</span></span>|<span data-ttu-id="a65b2-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="a65b2-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="a65b2-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-252">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="a65b2-252">minimumWarningOsVersion</span></span>|<span data-ttu-id="a65b2-253">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-253">String</span></span>|<span data-ttu-id="a65b2-254">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="a65b2-254">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="a65b2-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-256">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="a65b2-256">minimumRequiredAppVersion</span></span>|<span data-ttu-id="a65b2-257">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-257">String</span></span>|<span data-ttu-id="a65b2-258">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="a65b2-258">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="a65b2-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-260">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="a65b2-260">minimumWarningAppVersion</span></span>|<span data-ttu-id="a65b2-261">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-261">String</span></span>|<span data-ttu-id="a65b2-262">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="a65b2-262">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="a65b2-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-264">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a65b2-264">isAssigned</span></span>|<span data-ttu-id="a65b2-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-265">Boolean</span></span>|<span data-ttu-id="a65b2-266">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="a65b2-266">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a65b2-267">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a65b2-267">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="a65b2-268">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="a65b2-268">appDataEncryptionType</span></span>|[<span data-ttu-id="a65b2-269">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="a65b2-269">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="a65b2-270">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="a65b2-270">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="a65b2-271">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="a65b2-271">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="a65b2-272">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="a65b2-272">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="a65b2-273">String</span><span class="sxs-lookup"><span data-stu-id="a65b2-273">String</span></span>|<span data-ttu-id="a65b2-274">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="a65b2-274">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="a65b2-275">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="a65b2-275">deployedAppCount</span></span>|<span data-ttu-id="a65b2-276">Int32</span><span class="sxs-lookup"><span data-stu-id="a65b2-276">Int32</span></span>|<span data-ttu-id="a65b2-277">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="a65b2-277">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="a65b2-278">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="a65b2-278">faceIdBlocked</span></span>|<span data-ttu-id="a65b2-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65b2-279">Boolean</span></span>|<span data-ttu-id="a65b2-280">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="a65b2-280">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|



## <a name="response"></a><span data-ttu-id="a65b2-281">响应</span><span class="sxs-lookup"><span data-stu-id="a65b2-281">Response</span></span>
<span data-ttu-id="a65b2-282">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a65b2-282">If successful, this method returns a `201 Created` response code and a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a65b2-283">示例</span><span class="sxs-lookup"><span data-stu-id="a65b2-283">Example</span></span>

### <a name="request"></a><span data-ttu-id="a65b2-284">请求</span><span class="sxs-lookup"><span data-stu-id="a65b2-284">Request</span></span>
<span data-ttu-id="a65b2-285">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a65b2-285">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a65b2-286">响应</span><span class="sxs-lookup"><span data-stu-id="a65b2-286">Response</span></span>
<span data-ttu-id="a65b2-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a65b2-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






