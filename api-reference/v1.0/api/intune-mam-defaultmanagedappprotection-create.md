---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7aad221854091952806247f8f901593ae8489eb7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513292"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="7f3ea-103">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7f3ea-103">Create defaultManagedAppProtection</span></span>

<span data-ttu-id="7f3ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f3ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f3ea-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f3ea-106">创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-106">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f3ea-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f3ea-107">Prerequisites</span></span>
<span data-ttu-id="7f3ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f3ea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f3ea-110">Permission type</span></span>|<span data-ttu-id="7f3ea-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f3ea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f3ea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f3ea-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f3ea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f3ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-115">Not supported.</span></span>|
|<span data-ttu-id="7f3ea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f3ea-116">Application</span></span>|<span data-ttu-id="7f3ea-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f3ea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f3ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="7f3ea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f3ea-119">Request headers</span></span>
|<span data-ttu-id="7f3ea-120">标头</span><span class="sxs-lookup"><span data-stu-id="7f3ea-120">Header</span></span>|<span data-ttu-id="7f3ea-121">值</span><span class="sxs-lookup"><span data-stu-id="7f3ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f3ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f3ea-122">Authorization</span></span>|<span data-ttu-id="7f3ea-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f3ea-124">接受</span><span class="sxs-lookup"><span data-stu-id="7f3ea-124">Accept</span></span>|<span data-ttu-id="7f3ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f3ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f3ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f3ea-126">Request body</span></span>
<span data-ttu-id="7f3ea-127">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-127">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="7f3ea-128">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-128">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="7f3ea-129">属性</span><span class="sxs-lookup"><span data-stu-id="7f3ea-129">Property</span></span>|<span data-ttu-id="7f3ea-130">类型</span><span class="sxs-lookup"><span data-stu-id="7f3ea-130">Type</span></span>|<span data-ttu-id="7f3ea-131">说明</span><span class="sxs-lookup"><span data-stu-id="7f3ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f3ea-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7f3ea-132">displayName</span></span>|<span data-ttu-id="7f3ea-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-133">String</span></span>|<span data-ttu-id="7f3ea-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-134">Policy display name.</span></span> <span data-ttu-id="7f3ea-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-136">说明</span><span class="sxs-lookup"><span data-stu-id="7f3ea-136">description</span></span>|<span data-ttu-id="7f3ea-137">String</span><span class="sxs-lookup"><span data-stu-id="7f3ea-137">String</span></span>|<span data-ttu-id="7f3ea-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-138">The policy's description.</span></span> <span data-ttu-id="7f3ea-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3ea-140">createdDateTime</span></span>|<span data-ttu-id="7f3ea-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3ea-141">DateTimeOffset</span></span>|<span data-ttu-id="7f3ea-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-142">The date and time the policy was created.</span></span> <span data-ttu-id="7f3ea-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3ea-144">lastModifiedDateTime</span></span>|<span data-ttu-id="7f3ea-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3ea-145">DateTimeOffset</span></span>|<span data-ttu-id="7f3ea-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-146">Last time the policy was modified.</span></span> <span data-ttu-id="7f3ea-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-148">id</span><span class="sxs-lookup"><span data-stu-id="7f3ea-148">id</span></span>|<span data-ttu-id="7f3ea-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-149">String</span></span>|<span data-ttu-id="7f3ea-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-150">Key of the entity.</span></span> <span data-ttu-id="7f3ea-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-152">version</span><span class="sxs-lookup"><span data-stu-id="7f3ea-152">version</span></span>|<span data-ttu-id="7f3ea-153">String</span><span class="sxs-lookup"><span data-stu-id="7f3ea-153">String</span></span>|<span data-ttu-id="7f3ea-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-154">Version of the entity.</span></span> <span data-ttu-id="7f3ea-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7f3ea-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="7f3ea-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="7f3ea-157">持续时间</span><span class="sxs-lookup"><span data-stu-id="7f3ea-157">Duration</span></span>|<span data-ttu-id="7f3ea-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="7f3ea-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="7f3ea-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="7f3ea-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="7f3ea-161">Duration</span></span>|<span data-ttu-id="7f3ea-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="7f3ea-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="7f3ea-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="7f3ea-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="7f3ea-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="7f3ea-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="7f3ea-167">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7f3ea-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="7f3ea-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="7f3ea-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="7f3ea-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="7f3ea-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="7f3ea-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="7f3ea-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7f3ea-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="7f3ea-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="7f3ea-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="7f3ea-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-175">Boolean</span></span>|<span data-ttu-id="7f3ea-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="7f3ea-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="7f3ea-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="7f3ea-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="7f3ea-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="7f3ea-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="7f3ea-181">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7f3ea-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="7f3ea-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-183">dataBackupBlocked</span></span>|<span data-ttu-id="7f3ea-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-184">Boolean</span></span>|<span data-ttu-id="7f3ea-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="7f3ea-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="7f3ea-187">deviceComplianceRequired</span></span>|<span data-ttu-id="7f3ea-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-188">Boolean</span></span>|<span data-ttu-id="7f3ea-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="7f3ea-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="7f3ea-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="7f3ea-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-192">Boolean</span></span>|<span data-ttu-id="7f3ea-193">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-193">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="7f3ea-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-195">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-195">saveAsBlocked</span></span>|<span data-ttu-id="7f3ea-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-196">Boolean</span></span>|<span data-ttu-id="7f3ea-197">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-197">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="7f3ea-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-199">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="7f3ea-199">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="7f3ea-200">持续时间</span><span class="sxs-lookup"><span data-stu-id="7f3ea-200">Duration</span></span>|<span data-ttu-id="7f3ea-201">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-201">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="7f3ea-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-203">pinRequired</span><span class="sxs-lookup"><span data-stu-id="7f3ea-203">pinRequired</span></span>|<span data-ttu-id="7f3ea-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-204">Boolean</span></span>|<span data-ttu-id="7f3ea-205">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-205">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="7f3ea-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-207">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="7f3ea-207">maximumPinRetries</span></span>|<span data-ttu-id="7f3ea-208">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3ea-208">Int32</span></span>|<span data-ttu-id="7f3ea-209">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-209">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="7f3ea-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-211">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-211">simplePinBlocked</span></span>|<span data-ttu-id="7f3ea-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-212">Boolean</span></span>|<span data-ttu-id="7f3ea-213">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-213">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="7f3ea-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-215">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="7f3ea-215">minimumPinLength</span></span>|<span data-ttu-id="7f3ea-216">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3ea-216">Int32</span></span>|<span data-ttu-id="7f3ea-217">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-217">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-218">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="7f3ea-218">pinCharacterSet</span></span>|[<span data-ttu-id="7f3ea-219">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="7f3ea-219">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="7f3ea-220">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-220">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="7f3ea-221">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-221">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7f3ea-222">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-222">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="7f3ea-223">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="7f3ea-223">periodBeforePinReset</span></span>|<span data-ttu-id="7f3ea-224">Duration</span><span class="sxs-lookup"><span data-stu-id="7f3ea-224">Duration</span></span>|<span data-ttu-id="7f3ea-225">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-225">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="7f3ea-226">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-227">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="7f3ea-227">allowedDataStorageLocations</span></span>|<span data-ttu-id="7f3ea-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f3ea-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="7f3ea-229">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-229">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="7f3ea-230">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7f3ea-231">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-231">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="7f3ea-232">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-232">contactSyncBlocked</span></span>|<span data-ttu-id="7f3ea-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-233">Boolean</span></span>|<span data-ttu-id="7f3ea-234">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-234">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="7f3ea-235">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-236">printBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-236">printBlocked</span></span>|<span data-ttu-id="7f3ea-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-237">Boolean</span></span>|<span data-ttu-id="7f3ea-238">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-238">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="7f3ea-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-240">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-240">fingerprintBlocked</span></span>|<span data-ttu-id="7f3ea-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-241">Boolean</span></span>|<span data-ttu-id="7f3ea-242">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-242">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="7f3ea-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-244">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="7f3ea-244">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="7f3ea-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-245">Boolean</span></span>|<span data-ttu-id="7f3ea-246">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-246">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="7f3ea-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-248">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-248">minimumRequiredOsVersion</span></span>|<span data-ttu-id="7f3ea-249">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-249">String</span></span>|<span data-ttu-id="7f3ea-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7f3ea-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-252">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-252">minimumWarningOsVersion</span></span>|<span data-ttu-id="7f3ea-253">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-253">String</span></span>|<span data-ttu-id="7f3ea-254">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-254">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="7f3ea-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-256">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-256">minimumRequiredAppVersion</span></span>|<span data-ttu-id="7f3ea-257">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-257">String</span></span>|<span data-ttu-id="7f3ea-258">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-258">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7f3ea-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-260">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-260">minimumWarningAppVersion</span></span>|<span data-ttu-id="7f3ea-261">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-261">String</span></span>|<span data-ttu-id="7f3ea-262">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-262">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="7f3ea-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7f3ea-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7f3ea-264">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="7f3ea-264">appDataEncryptionType</span></span>|[<span data-ttu-id="7f3ea-265">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="7f3ea-265">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="7f3ea-266">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-266">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="7f3ea-267">（仅限 iOS）。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-267">(iOS Only).</span></span> <span data-ttu-id="7f3ea-268">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-268">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="7f3ea-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-269">screenCaptureBlocked</span></span>|<span data-ttu-id="7f3ea-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-270">Boolean</span></span>|<span data-ttu-id="7f3ea-271">指示是否阻止捕获屏幕。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-271">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="7f3ea-272">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-272">(Android only)</span></span>|
|<span data-ttu-id="7f3ea-273">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="7f3ea-273">encryptAppData</span></span>|<span data-ttu-id="7f3ea-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-274">Boolean</span></span>|<span data-ttu-id="7f3ea-275">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-275">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="7f3ea-276">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-276">(Android only)</span></span>|
|<span data-ttu-id="7f3ea-277">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="7f3ea-277">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="7f3ea-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-278">Boolean</span></span>|<span data-ttu-id="7f3ea-279">如果启用此设置，则在启用设备级加密的情况下禁用应用级加密。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-279">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="7f3ea-280">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-280">(Android only)</span></span>|
|<span data-ttu-id="7f3ea-281">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-281">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="7f3ea-282">String</span><span class="sxs-lookup"><span data-stu-id="7f3ea-282">String</span></span>|<span data-ttu-id="7f3ea-283">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-283">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7f3ea-284">（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-284">(iOS Only)</span></span>|
|<span data-ttu-id="7f3ea-285">customSettings</span><span class="sxs-lookup"><span data-stu-id="7f3ea-285">customSettings</span></span>|<span data-ttu-id="7f3ea-286">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f3ea-286">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7f3ea-287">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="7f3ea-287">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="7f3ea-288">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="7f3ea-288">deployedAppCount</span></span>|<span data-ttu-id="7f3ea-289">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3ea-289">Int32</span></span>|<span data-ttu-id="7f3ea-290">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-290">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="7f3ea-291">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-291">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="7f3ea-292">字符串</span><span class="sxs-lookup"><span data-stu-id="7f3ea-292">String</span></span>|<span data-ttu-id="7f3ea-293">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-293">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="7f3ea-294">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-294">(Android only)</span></span>|
|<span data-ttu-id="7f3ea-295">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="7f3ea-295">minimumWarningPatchVersion</span></span>|<span data-ttu-id="7f3ea-296">String</span><span class="sxs-lookup"><span data-stu-id="7f3ea-296">String</span></span>|<span data-ttu-id="7f3ea-297">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-297">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="7f3ea-298">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-298">(Android only)</span></span>|
|<span data-ttu-id="7f3ea-299">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="7f3ea-299">faceIdBlocked</span></span>|<span data-ttu-id="7f3ea-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3ea-300">Boolean</span></span>|<span data-ttu-id="7f3ea-301">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-301">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="7f3ea-302">（仅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="7f3ea-302">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="7f3ea-303">响应</span><span class="sxs-lookup"><span data-stu-id="7f3ea-303">Response</span></span>
<span data-ttu-id="7f3ea-304">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-304">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f3ea-305">示例</span><span class="sxs-lookup"><span data-stu-id="7f3ea-305">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f3ea-306">请求</span><span class="sxs-lookup"><span data-stu-id="7f3ea-306">Request</span></span>
<span data-ttu-id="7f3ea-307">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-307">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
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

### <a name="response"></a><span data-ttu-id="7f3ea-308">响应</span><span class="sxs-lookup"><span data-stu-id="7f3ea-308">Response</span></span>
<span data-ttu-id="7f3ea-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f3ea-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




