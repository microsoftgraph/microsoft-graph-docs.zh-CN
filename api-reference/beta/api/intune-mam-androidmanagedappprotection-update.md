---
title: 更新 androidManagedAppProtection
description: 更新 androidManagedAppProtection 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9382d7ff13860db626acca32a23e6602b54ae58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157475"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="5056b-103">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="5056b-103">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="5056b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5056b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5056b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5056b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5056b-106">更新 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5056b-106">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5056b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5056b-107">Prerequisites</span></span>
<span data-ttu-id="5056b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5056b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5056b-110">Permission type</span></span>|<span data-ttu-id="5056b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5056b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5056b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5056b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5056b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5056b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5056b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5056b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5056b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5056b-115">Not supported.</span></span>|
|<span data-ttu-id="5056b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5056b-116">Application</span></span>|<span data-ttu-id="5056b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5056b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5056b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5056b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="5056b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5056b-119">Request headers</span></span>
|<span data-ttu-id="5056b-120">标头</span><span class="sxs-lookup"><span data-stu-id="5056b-120">Header</span></span>|<span data-ttu-id="5056b-121">值</span><span class="sxs-lookup"><span data-stu-id="5056b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5056b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5056b-122">Authorization</span></span>|<span data-ttu-id="5056b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5056b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5056b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5056b-124">Accept</span></span>|<span data-ttu-id="5056b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5056b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5056b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5056b-126">Request body</span></span>
<span data-ttu-id="5056b-127">在请求正文中，提供 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5056b-127">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="5056b-128">下表显示了创建 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5056b-128">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="5056b-129">属性</span><span class="sxs-lookup"><span data-stu-id="5056b-129">Property</span></span>|<span data-ttu-id="5056b-130">类型</span><span class="sxs-lookup"><span data-stu-id="5056b-130">Type</span></span>|<span data-ttu-id="5056b-131">说明</span><span class="sxs-lookup"><span data-stu-id="5056b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5056b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5056b-132">displayName</span></span>|<span data-ttu-id="5056b-133">String</span><span class="sxs-lookup"><span data-stu-id="5056b-133">String</span></span>|<span data-ttu-id="5056b-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="5056b-134">Policy display name.</span></span> <span data-ttu-id="5056b-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-136">description</span><span class="sxs-lookup"><span data-stu-id="5056b-136">description</span></span>|<span data-ttu-id="5056b-137">String</span><span class="sxs-lookup"><span data-stu-id="5056b-137">String</span></span>|<span data-ttu-id="5056b-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="5056b-138">The policy's description.</span></span> <span data-ttu-id="5056b-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5056b-140">createdDateTime</span></span>|<span data-ttu-id="5056b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5056b-141">DateTimeOffset</span></span>|<span data-ttu-id="5056b-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5056b-142">The date and time the policy was created.</span></span> <span data-ttu-id="5056b-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5056b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5056b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5056b-145">DateTimeOffset</span></span>|<span data-ttu-id="5056b-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="5056b-146">Last time the policy was modified.</span></span> <span data-ttu-id="5056b-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5056b-148">roleScopeTagIds</span></span>|<span data-ttu-id="5056b-149">String collection</span><span class="sxs-lookup"><span data-stu-id="5056b-149">String collection</span></span>|<span data-ttu-id="5056b-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5056b-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5056b-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-152">id</span><span class="sxs-lookup"><span data-stu-id="5056b-152">id</span></span>|<span data-ttu-id="5056b-153">字符串</span><span class="sxs-lookup"><span data-stu-id="5056b-153">String</span></span>|<span data-ttu-id="5056b-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5056b-154">Key of the entity.</span></span> <span data-ttu-id="5056b-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-156">version</span><span class="sxs-lookup"><span data-stu-id="5056b-156">version</span></span>|<span data-ttu-id="5056b-157">String</span><span class="sxs-lookup"><span data-stu-id="5056b-157">String</span></span>|<span data-ttu-id="5056b-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5056b-158">Version of the entity.</span></span> <span data-ttu-id="5056b-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5056b-160">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="5056b-160">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="5056b-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="5056b-161">Duration</span></span>|<span data-ttu-id="5056b-162">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="5056b-162">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="5056b-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-164">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="5056b-164">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="5056b-165">Duration</span><span class="sxs-lookup"><span data-stu-id="5056b-165">Duration</span></span>|<span data-ttu-id="5056b-166">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="5056b-166">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="5056b-167">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-168">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="5056b-168">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="5056b-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="5056b-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="5056b-170">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="5056b-170">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="5056b-171">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-172">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="5056b-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="5056b-173">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="5056b-173">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="5056b-174">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="5056b-174">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="5056b-175">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="5056b-175">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="5056b-176">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-177">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="5056b-177">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="5056b-178">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="5056b-178">organizationalCredentialsRequired</span></span>|<span data-ttu-id="5056b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-179">Boolean</span></span>|<span data-ttu-id="5056b-180">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="5056b-180">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="5056b-181">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-182">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="5056b-182">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="5056b-183">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="5056b-183">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="5056b-184">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="5056b-184">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="5056b-185">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-186">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="5056b-186">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="5056b-187">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-187">dataBackupBlocked</span></span>|<span data-ttu-id="5056b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-188">Boolean</span></span>|<span data-ttu-id="5056b-189">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-189">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="5056b-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-191">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="5056b-191">deviceComplianceRequired</span></span>|<span data-ttu-id="5056b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-192">Boolean</span></span>|<span data-ttu-id="5056b-193">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="5056b-193">Indicates whether device compliance is required.</span></span> <span data-ttu-id="5056b-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-195">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="5056b-195">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="5056b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-196">Boolean</span></span>|<span data-ttu-id="5056b-197">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="5056b-197">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="5056b-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-199">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-199">saveAsBlocked</span></span>|<span data-ttu-id="5056b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-200">Boolean</span></span>|<span data-ttu-id="5056b-201">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="5056b-201">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="5056b-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-203">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="5056b-203">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="5056b-204">持续时间</span><span class="sxs-lookup"><span data-stu-id="5056b-204">Duration</span></span>|<span data-ttu-id="5056b-205">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="5056b-205">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="5056b-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-207">pinRequired</span><span class="sxs-lookup"><span data-stu-id="5056b-207">pinRequired</span></span>|<span data-ttu-id="5056b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-208">Boolean</span></span>|<span data-ttu-id="5056b-209">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="5056b-209">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="5056b-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-211">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="5056b-211">maximumPinRetries</span></span>|<span data-ttu-id="5056b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="5056b-212">Int32</span></span>|<span data-ttu-id="5056b-213">在阻止或擦除托管应用之前, 不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="5056b-213">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="5056b-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-215">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-215">simplePinBlocked</span></span>|<span data-ttu-id="5056b-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-216">Boolean</span></span>|<span data-ttu-id="5056b-217">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="5056b-217">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="5056b-218">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-218">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-219">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="5056b-219">minimumPinLength</span></span>|<span data-ttu-id="5056b-220">Int32</span><span class="sxs-lookup"><span data-stu-id="5056b-220">Int32</span></span>|<span data-ttu-id="5056b-221">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-221">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-222">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="5056b-222">pinCharacterSet</span></span>|[<span data-ttu-id="5056b-223">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="5056b-223">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="5056b-224">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="5056b-224">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="5056b-225">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-226">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="5056b-226">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="5056b-227">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="5056b-227">periodBeforePinReset</span></span>|<span data-ttu-id="5056b-228">Duration</span><span class="sxs-lookup"><span data-stu-id="5056b-228">Duration</span></span>|<span data-ttu-id="5056b-229">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="5056b-229">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="5056b-230">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-231">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="5056b-231">allowedDataStorageLocations</span></span>|<span data-ttu-id="5056b-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="5056b-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="5056b-233">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="5056b-233">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="5056b-234">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-235">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="5056b-235">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="5056b-236">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-236">contactSyncBlocked</span></span>|<span data-ttu-id="5056b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-237">Boolean</span></span>|<span data-ttu-id="5056b-238">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="5056b-238">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="5056b-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-240">printBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-240">printBlocked</span></span>|<span data-ttu-id="5056b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-241">Boolean</span></span>|<span data-ttu-id="5056b-242">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="5056b-242">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="5056b-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-244">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-244">fingerprintBlocked</span></span>|<span data-ttu-id="5056b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-245">Boolean</span></span>|<span data-ttu-id="5056b-246">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="5056b-246">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="5056b-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-248">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="5056b-248">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="5056b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-249">Boolean</span></span>|<span data-ttu-id="5056b-250">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="5056b-250">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="5056b-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-252">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-252">minimumRequiredOsVersion</span></span>|<span data-ttu-id="5056b-253">String</span><span class="sxs-lookup"><span data-stu-id="5056b-253">String</span></span>|<span data-ttu-id="5056b-254">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-254">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="5056b-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-256">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-256">minimumWarningOsVersion</span></span>|<span data-ttu-id="5056b-257">String</span><span class="sxs-lookup"><span data-stu-id="5056b-257">String</span></span>|<span data-ttu-id="5056b-258">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="5056b-258">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="5056b-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-260">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-260">minimumRequiredAppVersion</span></span>|<span data-ttu-id="5056b-261">String</span><span class="sxs-lookup"><span data-stu-id="5056b-261">String</span></span>|<span data-ttu-id="5056b-262">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-262">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="5056b-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-264">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-264">minimumWarningAppVersion</span></span>|<span data-ttu-id="5056b-265">String</span><span class="sxs-lookup"><span data-stu-id="5056b-265">String</span></span>|<span data-ttu-id="5056b-266">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="5056b-266">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="5056b-267">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-268">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-268">minimumWipeOsVersion</span></span>|<span data-ttu-id="5056b-269">String</span><span class="sxs-lookup"><span data-stu-id="5056b-269">String</span></span>|<span data-ttu-id="5056b-270">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-270">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="5056b-271">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-271">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-272">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-272">minimumWipeAppVersion</span></span>|<span data-ttu-id="5056b-273">String</span><span class="sxs-lookup"><span data-stu-id="5056b-273">String</span></span>|<span data-ttu-id="5056b-274">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-274">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="5056b-275">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-275">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-276">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="5056b-276">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="5056b-277">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="5056b-277">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="5056b-278">如果将 DeviceComplianceRequired 设置为 true, 则定义在设备为根或已越狱时的托管应用行为 (阻止或擦除)。</span><span class="sxs-lookup"><span data-stu-id="5056b-278">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="5056b-279">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-279">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-280">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="5056b-280">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="5056b-281">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="5056b-281">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="5056b-282">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="5056b-282">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="5056b-283">根据最大错误 pin 重试次数定义托管应用行为, 即阻止或擦除。</span><span class="sxs-lookup"><span data-stu-id="5056b-283">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="5056b-284">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="5056b-284">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="5056b-285">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="5056b-285">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="5056b-286">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="5056b-286">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="5056b-287">持续时间</span><span class="sxs-lookup"><span data-stu-id="5056b-287">Duration</span></span>|<span data-ttu-id="5056b-288">以分钟为单位的应用程序 pin (而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)继承的无生物特征密码) 超时</span><span class="sxs-lookup"><span data-stu-id="5056b-288">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-289">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5056b-289">isAssigned</span></span>|<span data-ttu-id="5056b-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-290">Boolean</span></span>|<span data-ttu-id="5056b-291">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="5056b-291">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="5056b-292">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-292">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="5056b-293">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="5056b-293">targetedAppManagementLevels</span></span>|[<span data-ttu-id="5056b-294">appManagementLevel</span><span class="sxs-lookup"><span data-stu-id="5056b-294">appManagementLevel</span></span>](../resources/intune-mam-appmanagementlevel.md)|<span data-ttu-id="5056b-295">此策略继承自[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)的预期应用管理级别。</span><span class="sxs-lookup"><span data-stu-id="5056b-295">The intended app management levels for this policy Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span></span> <span data-ttu-id="5056b-296">可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="5056b-296">Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.</span></span>|
|<span data-ttu-id="5056b-297">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5056b-297">screenCaptureBlocked</span></span>|<span data-ttu-id="5056b-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-298">Boolean</span></span>|<span data-ttu-id="5056b-299">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="5056b-299">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="5056b-300">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="5056b-300">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="5056b-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-301">Boolean</span></span>|<span data-ttu-id="5056b-302">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="5056b-302">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="5056b-303">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="5056b-303">encryptAppData</span></span>|<span data-ttu-id="5056b-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="5056b-304">Boolean</span></span>|<span data-ttu-id="5056b-305">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="5056b-305">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="5056b-306">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="5056b-306">deployedAppCount</span></span>|<span data-ttu-id="5056b-307">Int32</span><span class="sxs-lookup"><span data-stu-id="5056b-307">Int32</span></span>|<span data-ttu-id="5056b-308">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="5056b-308">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="5056b-309">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-309">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="5056b-310">String</span><span class="sxs-lookup"><span data-stu-id="5056b-310">String</span></span>|<span data-ttu-id="5056b-311">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="5056b-311">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="5056b-312">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-312">minimumWarningPatchVersion</span></span>|<span data-ttu-id="5056b-313">String</span><span class="sxs-lookup"><span data-stu-id="5056b-313">String</span></span>|<span data-ttu-id="5056b-314">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="5056b-314">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="5056b-315">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="5056b-315">exemptedAppPackages</span></span>|<span data-ttu-id="5056b-316">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5056b-316">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5056b-317">此列表中的应用程序包将从该策略中排除, 并且将能够从托管应用接收数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-317">App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span>|
|<span data-ttu-id="5056b-318">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="5056b-318">minimumWipePatchVersion</span></span>|<span data-ttu-id="5056b-319">String</span><span class="sxs-lookup"><span data-stu-id="5056b-319">String</span></span>|<span data-ttu-id="5056b-320">Android 安全修补程序级别小于或等于指定值将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="5056b-320">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span>|
|<span data-ttu-id="5056b-321">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="5056b-321">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="5056b-322">String</span><span class="sxs-lookup"><span data-stu-id="5056b-322">String</span></span>|<span data-ttu-id="5056b-323">允许托管应用使用的设备制造商以分号分隔的列表, 以字符串形式提供。</span><span class="sxs-lookup"><span data-stu-id="5056b-323">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span>|
|<span data-ttu-id="5056b-324">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="5056b-324">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="5056b-325">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="5056b-325">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="5056b-326">如果不允许指定的设备制造商, 则定义托管应用行为 (无论是阻止还是擦除)。</span><span class="sxs-lookup"><span data-stu-id="5056b-326">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="5056b-327">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="5056b-327">Possible values are: `block`, `wipe`, `warn`.</span></span>|



## <a name="response"></a><span data-ttu-id="5056b-328">响应</span><span class="sxs-lookup"><span data-stu-id="5056b-328">Response</span></span>
<span data-ttu-id="5056b-329">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5056b-329">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5056b-330">示例</span><span class="sxs-lookup"><span data-stu-id="5056b-330">Example</span></span>

### <a name="request"></a><span data-ttu-id="5056b-331">请求</span><span class="sxs-lookup"><span data-stu-id="5056b-331">Request</span></span>
<span data-ttu-id="5056b-332">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5056b-332">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 2460

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```

### <a name="response"></a><span data-ttu-id="5056b-333">响应</span><span class="sxs-lookup"><span data-stu-id="5056b-333">Response</span></span>
<span data-ttu-id="5056b-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5056b-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2632

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```




