---
title: 更新 androidManagedAppProtection
description: 更新 androidManagedAppProtection 对象的属性。
ms.openlocfilehash: 1fa95bddbd69f6f51a92869de9c39c37e03d6447
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011412"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="8d6f0-103">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="8d6f0-103">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="8d6f0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d6f0-105">更新 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-105">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d6f0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d6f0-106">Prerequisites</span></span>
<span data-ttu-id="8d6f0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8d6f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d6f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d6f0-109">Permission type</span></span>|<span data-ttu-id="8d6f0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d6f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d6f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d6f0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6f0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d6f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d6f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-114">Not supported.</span></span>|
|<span data-ttu-id="8d6f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d6f0-115">Application</span></span>|<span data-ttu-id="8d6f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d6f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d6f0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="8d6f0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d6f0-118">Request headers</span></span>
|<span data-ttu-id="8d6f0-119">标头</span><span class="sxs-lookup"><span data-stu-id="8d6f0-119">Header</span></span>|<span data-ttu-id="8d6f0-120">值</span><span class="sxs-lookup"><span data-stu-id="8d6f0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d6f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d6f0-121">Authorization</span></span>|<span data-ttu-id="8d6f0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d6f0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8d6f0-123">Accept</span></span>|<span data-ttu-id="8d6f0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d6f0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d6f0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d6f0-125">Request body</span></span>
<span data-ttu-id="8d6f0-126">在请求正文中，提供 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-126">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="8d6f0-127">下表显示了创建 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-127">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="8d6f0-128">属性</span><span class="sxs-lookup"><span data-stu-id="8d6f0-128">Property</span></span>|<span data-ttu-id="8d6f0-129">类型</span><span class="sxs-lookup"><span data-stu-id="8d6f0-129">Type</span></span>|<span data-ttu-id="8d6f0-130">说明</span><span class="sxs-lookup"><span data-stu-id="8d6f0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d6f0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="8d6f0-131">displayName</span></span>|<span data-ttu-id="8d6f0-132">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-132">String</span></span>|<span data-ttu-id="8d6f0-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-133">Policy display name.</span></span> <span data-ttu-id="8d6f0-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-135">description</span><span class="sxs-lookup"><span data-stu-id="8d6f0-135">description</span></span>|<span data-ttu-id="8d6f0-136">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-136">String</span></span>|<span data-ttu-id="8d6f0-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-137">The policy's description.</span></span> <span data-ttu-id="8d6f0-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d6f0-139">createdDateTime</span></span>|<span data-ttu-id="8d6f0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d6f0-140">DateTimeOffset</span></span>|<span data-ttu-id="8d6f0-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-141">The date and time the policy was created.</span></span> <span data-ttu-id="8d6f0-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d6f0-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8d6f0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d6f0-144">DateTimeOffset</span></span>|<span data-ttu-id="8d6f0-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-145">Last time the policy was modified.</span></span> <span data-ttu-id="8d6f0-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-147">id</span><span class="sxs-lookup"><span data-stu-id="8d6f0-147">id</span></span>|<span data-ttu-id="8d6f0-148">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-148">String</span></span>|<span data-ttu-id="8d6f0-149">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-149">Key of the entity.</span></span> <span data-ttu-id="8d6f0-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-151">version</span><span class="sxs-lookup"><span data-stu-id="8d6f0-151">version</span></span>|<span data-ttu-id="8d6f0-152">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-152">String</span></span>|<span data-ttu-id="8d6f0-153">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-153">Version of the entity.</span></span> <span data-ttu-id="8d6f0-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8d6f0-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="8d6f0-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="8d6f0-156">Duration</span><span class="sxs-lookup"><span data-stu-id="8d6f0-156">Duration</span></span>|<span data-ttu-id="8d6f0-157">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="8d6f0-158">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="8d6f0-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="8d6f0-160">Duration</span><span class="sxs-lookup"><span data-stu-id="8d6f0-160">Duration</span></span>|<span data-ttu-id="8d6f0-161">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="8d6f0-162">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="8d6f0-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="8d6f0-164">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="8d6f0-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="8d6f0-165">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="8d6f0-166">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="8d6f0-167">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="8d6f0-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="8d6f0-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="8d6f0-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="8d6f0-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="8d6f0-170">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="8d6f0-171">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="8d6f0-172">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="8d6f0-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="8d6f0-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="8d6f0-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-174">Boolean</span></span>|<span data-ttu-id="8d6f0-175">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="8d6f0-176">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="8d6f0-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="8d6f0-178">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="8d6f0-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="8d6f0-179">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="8d6f0-180">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="8d6f0-181">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="8d6f0-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-182">dataBackupBlocked</span></span>|<span data-ttu-id="8d6f0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-183">Boolean</span></span>|<span data-ttu-id="8d6f0-184">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="8d6f0-185">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="8d6f0-186">deviceComplianceRequired</span></span>|<span data-ttu-id="8d6f0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-187">Boolean</span></span>|<span data-ttu-id="8d6f0-188">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="8d6f0-189">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="8d6f0-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="8d6f0-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-191">Boolean</span></span>|<span data-ttu-id="8d6f0-192">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="8d6f0-193">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-194">saveAsBlocked</span></span>|<span data-ttu-id="8d6f0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-195">Boolean</span></span>|<span data-ttu-id="8d6f0-196">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="8d6f0-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="8d6f0-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="8d6f0-199">Duration</span><span class="sxs-lookup"><span data-stu-id="8d6f0-199">Duration</span></span>|<span data-ttu-id="8d6f0-200">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="8d6f0-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="8d6f0-202">pinRequired</span></span>|<span data-ttu-id="8d6f0-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-203">Boolean</span></span>|<span data-ttu-id="8d6f0-204">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="8d6f0-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="8d6f0-206">maximumPinRetries</span></span>|<span data-ttu-id="8d6f0-207">Int32</span><span class="sxs-lookup"><span data-stu-id="8d6f0-207">Int32</span></span>|<span data-ttu-id="8d6f0-208">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="8d6f0-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-210">simplePinBlocked</span></span>|<span data-ttu-id="8d6f0-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-211">Boolean</span></span>|<span data-ttu-id="8d6f0-212">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="8d6f0-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="8d6f0-214">minimumPinLength</span></span>|<span data-ttu-id="8d6f0-215">Int32</span><span class="sxs-lookup"><span data-stu-id="8d6f0-215">Int32</span></span>|<span data-ttu-id="8d6f0-216">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="8d6f0-217">pinCharacterSet</span></span>|[<span data-ttu-id="8d6f0-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="8d6f0-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="8d6f0-219">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="8d6f0-220">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="8d6f0-221">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="8d6f0-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="8d6f0-222">periodBeforePinReset</span></span>|<span data-ttu-id="8d6f0-223">Duration</span><span class="sxs-lookup"><span data-stu-id="8d6f0-223">Duration</span></span>|<span data-ttu-id="8d6f0-224">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="8d6f0-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="8d6f0-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="8d6f0-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="8d6f0-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d6f0-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="8d6f0-228">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="8d6f0-229">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="8d6f0-230">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="8d6f0-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-231">contactSyncBlocked</span></span>|<span data-ttu-id="8d6f0-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-232">Boolean</span></span>|<span data-ttu-id="8d6f0-233">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="8d6f0-234">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-235">printBlocked</span></span>|<span data-ttu-id="8d6f0-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-236">Boolean</span></span>|<span data-ttu-id="8d6f0-237">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="8d6f0-238">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-239">fingerprintBlocked</span></span>|<span data-ttu-id="8d6f0-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-240">Boolean</span></span>|<span data-ttu-id="8d6f0-241">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="8d6f0-242">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="8d6f0-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="8d6f0-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-244">Boolean</span></span>|<span data-ttu-id="8d6f0-245">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="8d6f0-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="8d6f0-248">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-248">String</span></span>|<span data-ttu-id="8d6f0-249">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="8d6f0-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="8d6f0-252">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-252">String</span></span>|<span data-ttu-id="8d6f0-253">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="8d6f0-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="8d6f0-256">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-256">String</span></span>|<span data-ttu-id="8d6f0-257">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="8d6f0-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="8d6f0-260">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-260">String</span></span>|<span data-ttu-id="8d6f0-261">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="8d6f0-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-263">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8d6f0-263">isAssigned</span></span>|<span data-ttu-id="8d6f0-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-264">Boolean</span></span>|<span data-ttu-id="8d6f0-265">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-265">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="8d6f0-266">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f0-266">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="8d6f0-267">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8d6f0-267">screenCaptureBlocked</span></span>|<span data-ttu-id="8d6f0-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-268">Boolean</span></span>|<span data-ttu-id="8d6f0-269">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="8d6f0-269">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="8d6f0-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="8d6f0-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="8d6f0-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-271">Boolean</span></span>|<span data-ttu-id="8d6f0-272">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="8d6f0-272">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="8d6f0-273">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="8d6f0-273">encryptAppData</span></span>|<span data-ttu-id="8d6f0-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6f0-274">Boolean</span></span>|<span data-ttu-id="8d6f0-275">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="8d6f0-275">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="8d6f0-276">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="8d6f0-276">deployedAppCount</span></span>|<span data-ttu-id="8d6f0-277">Int32</span><span class="sxs-lookup"><span data-stu-id="8d6f0-277">Int32</span></span>|<span data-ttu-id="8d6f0-278">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-278">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="8d6f0-279">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-279">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="8d6f0-280">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-280">String</span></span>|<span data-ttu-id="8d6f0-281">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="8d6f0-281">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="8d6f0-282">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="8d6f0-282">minimumWarningPatchVersion</span></span>|<span data-ttu-id="8d6f0-283">String</span><span class="sxs-lookup"><span data-stu-id="8d6f0-283">String</span></span>|<span data-ttu-id="8d6f0-284">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-284">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|



## <a name="response"></a><span data-ttu-id="8d6f0-285">响应</span><span class="sxs-lookup"><span data-stu-id="8d6f0-285">Response</span></span>
<span data-ttu-id="8d6f0-286">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-286">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d6f0-287">示例</span><span class="sxs-lookup"><span data-stu-id="8d6f0-287">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d6f0-288">请求</span><span class="sxs-lookup"><span data-stu-id="8d6f0-288">Request</span></span>
<span data-ttu-id="8d6f0-289">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 1692

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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="8d6f0-290">响应</span><span class="sxs-lookup"><span data-stu-id="8d6f0-290">Response</span></span>
<span data-ttu-id="8d6f0-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d6f0-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1864

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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```



