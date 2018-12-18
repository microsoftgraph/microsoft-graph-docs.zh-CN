---
title: 更新 defaultManagedAppProtection
description: 更新 defaultManagedAppProtection 对象的属性。
author: tfitzmac
ms.openlocfilehash: e8e17d8303789c499988e24a4b5e21eb64d0255e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302084"
---
# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="7fe07-103">更新 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7fe07-103">Update defaultManagedAppProtection</span></span>

> <span data-ttu-id="7fe07-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7fe07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fe07-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7fe07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fe07-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7fe07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fe07-107">更新 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7fe07-107">Update the properties of a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fe07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7fe07-108">Prerequisites</span></span>
<span data-ttu-id="7fe07-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7fe07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fe07-111">Permission type</span></span>|<span data-ttu-id="7fe07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7fe07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe07-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe07-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fe07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fe07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fe07-116">Not supported.</span></span>|
|<span data-ttu-id="7fe07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fe07-117">Application</span></span>|<span data-ttu-id="7fe07-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fe07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fe07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="7fe07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fe07-120">Request headers</span></span>
|<span data-ttu-id="7fe07-121">标头</span><span class="sxs-lookup"><span data-stu-id="7fe07-121">Header</span></span>|<span data-ttu-id="7fe07-122">值</span><span class="sxs-lookup"><span data-stu-id="7fe07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe07-123">授权</span><span class="sxs-lookup"><span data-stu-id="7fe07-123">Authorization</span></span>|<span data-ttu-id="7fe07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7fe07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fe07-125">Accept</span></span>|<span data-ttu-id="7fe07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fe07-127">Request body</span></span>
<span data-ttu-id="7fe07-128">在请求正文中，提供 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fe07-128">In the request body, supply a JSON representation for the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="7fe07-129">下表显示创建 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7fe07-129">The following table shows the properties that are required when you create the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

|<span data-ttu-id="7fe07-130">属性</span><span class="sxs-lookup"><span data-stu-id="7fe07-130">Property</span></span>|<span data-ttu-id="7fe07-131">类型</span><span class="sxs-lookup"><span data-stu-id="7fe07-131">Type</span></span>|<span data-ttu-id="7fe07-132">说明</span><span class="sxs-lookup"><span data-stu-id="7fe07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe07-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7fe07-133">displayName</span></span>|<span data-ttu-id="7fe07-134">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-134">String</span></span>|<span data-ttu-id="7fe07-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="7fe07-135">Policy display name.</span></span> <span data-ttu-id="7fe07-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-137">description</span><span class="sxs-lookup"><span data-stu-id="7fe07-137">description</span></span>|<span data-ttu-id="7fe07-138">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-138">String</span></span>|<span data-ttu-id="7fe07-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="7fe07-139">The policy's description.</span></span> <span data-ttu-id="7fe07-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fe07-141">createdDateTime</span></span>|<span data-ttu-id="7fe07-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fe07-142">DateTimeOffset</span></span>|<span data-ttu-id="7fe07-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7fe07-143">The date and time the policy was created.</span></span> <span data-ttu-id="7fe07-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fe07-145">lastModifiedDateTime</span></span>|<span data-ttu-id="7fe07-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fe07-146">DateTimeOffset</span></span>|<span data-ttu-id="7fe07-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="7fe07-147">Last time the policy was modified.</span></span> <span data-ttu-id="7fe07-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-149">id</span><span class="sxs-lookup"><span data-stu-id="7fe07-149">id</span></span>|<span data-ttu-id="7fe07-150">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-150">String</span></span>|<span data-ttu-id="7fe07-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fe07-151">Key of the entity.</span></span> <span data-ttu-id="7fe07-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-153">version</span><span class="sxs-lookup"><span data-stu-id="7fe07-153">version</span></span>|<span data-ttu-id="7fe07-154">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-154">String</span></span>|<span data-ttu-id="7fe07-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="7fe07-155">Version of the entity.</span></span> <span data-ttu-id="7fe07-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7fe07-157">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="7fe07-157">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="7fe07-158">Duration</span><span class="sxs-lookup"><span data-stu-id="7fe07-158">Duration</span></span>|<span data-ttu-id="7fe07-159">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="7fe07-159">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="7fe07-160">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-160">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-161">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="7fe07-161">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="7fe07-162">Duration</span><span class="sxs-lookup"><span data-stu-id="7fe07-162">Duration</span></span>|<span data-ttu-id="7fe07-163">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="7fe07-163">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="7fe07-164">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-165">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="7fe07-165">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="7fe07-166">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="7fe07-166">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="7fe07-167">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="7fe07-167">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="7fe07-168">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-169">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-169">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="7fe07-170">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="7fe07-170">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="7fe07-171">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="7fe07-171">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="7fe07-172">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="7fe07-172">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="7fe07-173">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-173">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-174">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-174">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="7fe07-175">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="7fe07-175">organizationalCredentialsRequired</span></span>|<span data-ttu-id="7fe07-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-176">Boolean</span></span>|<span data-ttu-id="7fe07-177">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="7fe07-177">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="7fe07-178">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-178">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-179">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="7fe07-179">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="7fe07-180">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="7fe07-180">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="7fe07-181">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="7fe07-181">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="7fe07-182">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-183">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-183">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="7fe07-184">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-184">dataBackupBlocked</span></span>|<span data-ttu-id="7fe07-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-185">Boolean</span></span>|<span data-ttu-id="7fe07-186">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-186">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="7fe07-187">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-187">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-188">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="7fe07-188">deviceComplianceRequired</span></span>|<span data-ttu-id="7fe07-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-189">Boolean</span></span>|<span data-ttu-id="7fe07-190">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="7fe07-190">Indicates whether device compliance is required.</span></span> <span data-ttu-id="7fe07-191">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-192">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="7fe07-192">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="7fe07-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-193">Boolean</span></span>|<span data-ttu-id="7fe07-194">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="7fe07-194">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="7fe07-195">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-196">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-196">saveAsBlocked</span></span>|<span data-ttu-id="7fe07-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-197">Boolean</span></span>|<span data-ttu-id="7fe07-198">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="7fe07-198">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="7fe07-199">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-200">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="7fe07-200">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="7fe07-201">Duration</span><span class="sxs-lookup"><span data-stu-id="7fe07-201">Duration</span></span>|<span data-ttu-id="7fe07-202">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="7fe07-202">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="7fe07-203">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-204">pinRequired</span><span class="sxs-lookup"><span data-stu-id="7fe07-204">pinRequired</span></span>|<span data-ttu-id="7fe07-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-205">Boolean</span></span>|<span data-ttu-id="7fe07-206">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="7fe07-206">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="7fe07-207">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-208">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="7fe07-208">maximumPinRetries</span></span>|<span data-ttu-id="7fe07-209">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe07-209">Int32</span></span>|<span data-ttu-id="7fe07-210">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7fe07-210">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="7fe07-211">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-212">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-212">simplePinBlocked</span></span>|<span data-ttu-id="7fe07-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-213">Boolean</span></span>|<span data-ttu-id="7fe07-214">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="7fe07-214">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="7fe07-215">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-216">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="7fe07-216">minimumPinLength</span></span>|<span data-ttu-id="7fe07-217">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe07-217">Int32</span></span>|<span data-ttu-id="7fe07-218">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-218">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-219">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="7fe07-219">pinCharacterSet</span></span>|[<span data-ttu-id="7fe07-220">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="7fe07-220">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="7fe07-221">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="7fe07-221">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="7fe07-222">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-222">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-223">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-223">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="7fe07-224">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="7fe07-224">periodBeforePinReset</span></span>|<span data-ttu-id="7fe07-225">Duration</span><span class="sxs-lookup"><span data-stu-id="7fe07-225">Duration</span></span>|<span data-ttu-id="7fe07-226">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="7fe07-226">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="7fe07-227">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-227">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-228">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="7fe07-228">allowedDataStorageLocations</span></span>|<span data-ttu-id="7fe07-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="7fe07-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="7fe07-230">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="7fe07-230">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="7fe07-231">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-232">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-232">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="7fe07-233">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-233">contactSyncBlocked</span></span>|<span data-ttu-id="7fe07-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-234">Boolean</span></span>|<span data-ttu-id="7fe07-235">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="7fe07-235">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="7fe07-236">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-236">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-237">printBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-237">printBlocked</span></span>|<span data-ttu-id="7fe07-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-238">Boolean</span></span>|<span data-ttu-id="7fe07-239">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="7fe07-239">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="7fe07-240">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-241">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-241">fingerprintBlocked</span></span>|<span data-ttu-id="7fe07-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-242">Boolean</span></span>|<span data-ttu-id="7fe07-243">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="7fe07-243">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="7fe07-244">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-245">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="7fe07-245">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="7fe07-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-246">Boolean</span></span>|<span data-ttu-id="7fe07-247">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="7fe07-247">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="7fe07-248">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-249">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-249">minimumRequiredOsVersion</span></span>|<span data-ttu-id="7fe07-250">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-250">String</span></span>|<span data-ttu-id="7fe07-251">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-251">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7fe07-252">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-253">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-253">minimumWarningOsVersion</span></span>|<span data-ttu-id="7fe07-254">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-254">String</span></span>|<span data-ttu-id="7fe07-255">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="7fe07-255">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="7fe07-256">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-257">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-257">minimumRequiredAppVersion</span></span>|<span data-ttu-id="7fe07-258">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-258">String</span></span>|<span data-ttu-id="7fe07-259">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-259">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7fe07-260">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-261">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-261">minimumWarningAppVersion</span></span>|<span data-ttu-id="7fe07-262">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-262">String</span></span>|<span data-ttu-id="7fe07-263">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="7fe07-263">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="7fe07-264">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-265">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-265">minimumWipeOsVersion</span></span>|<span data-ttu-id="7fe07-266">字符串</span><span class="sxs-lookup"><span data-stu-id="7fe07-266">String</span></span>|<span data-ttu-id="7fe07-267">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="7fe07-267">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="7fe07-268">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-269">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-269">minimumWipeAppVersion</span></span>|<span data-ttu-id="7fe07-270">字符串</span><span class="sxs-lookup"><span data-stu-id="7fe07-270">String</span></span>|<span data-ttu-id="7fe07-271">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="7fe07-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="7fe07-272">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="7fe07-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-273">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="7fe07-273">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="7fe07-274">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="7fe07-274">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="7fe07-275">定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="7fe07-275">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="7fe07-276">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-277">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-277">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="7fe07-278">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="7fe07-278">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="7fe07-279">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="7fe07-279">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="7fe07-280">定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。</span><span class="sxs-lookup"><span data-stu-id="7fe07-280">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="7fe07-281">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-281">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="7fe07-282">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-282">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="7fe07-283">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="7fe07-283">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="7fe07-284">Duration</span><span class="sxs-lookup"><span data-stu-id="7fe07-284">Duration</span></span>|<span data-ttu-id="7fe07-285">以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时</span><span class="sxs-lookup"><span data-stu-id="7fe07-285">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="7fe07-286">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="7fe07-286">appDataEncryptionType</span></span>|[<span data-ttu-id="7fe07-287">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="7fe07-287">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="7fe07-288">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="7fe07-288">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="7fe07-289">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-289">(iOS Only).</span></span> <span data-ttu-id="7fe07-290">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-290">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="7fe07-291">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-291">screenCaptureBlocked</span></span>|<span data-ttu-id="7fe07-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-292">Boolean</span></span>|<span data-ttu-id="7fe07-293">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="7fe07-293">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="7fe07-294">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-294">(Android only)</span></span>|
|<span data-ttu-id="7fe07-295">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="7fe07-295">encryptAppData</span></span>|<span data-ttu-id="7fe07-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-296">Boolean</span></span>|<span data-ttu-id="7fe07-297">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-297">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="7fe07-298">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-298">(Android only)</span></span>|
|<span data-ttu-id="7fe07-299">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="7fe07-299">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="7fe07-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-300">Boolean</span></span>|<span data-ttu-id="7fe07-301">启用此设置后，如果启用设备加密，则禁用应用程序级别的加密。</span><span class="sxs-lookup"><span data-stu-id="7fe07-301">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="7fe07-302">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-302">(Android only)</span></span>|
|<span data-ttu-id="7fe07-303">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-303">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="7fe07-304">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-304">String</span></span>|<span data-ttu-id="7fe07-305">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-305">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="7fe07-306">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-306">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-307">customSettings</span><span class="sxs-lookup"><span data-stu-id="7fe07-307">customSettings</span></span>|<span data-ttu-id="7fe07-308">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fe07-308">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fe07-309">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="7fe07-309">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="7fe07-310">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="7fe07-310">deployedAppCount</span></span>|<span data-ttu-id="7fe07-311">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe07-311">Int32</span></span>|<span data-ttu-id="7fe07-312">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="7fe07-312">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="7fe07-313">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-313">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="7fe07-314">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-314">String</span></span>|<span data-ttu-id="7fe07-315">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="7fe07-315">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="7fe07-316">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-316">(Android only)</span></span>|
|<span data-ttu-id="7fe07-317">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-317">minimumWarningPatchVersion</span></span>|<span data-ttu-id="7fe07-318">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-318">String</span></span>|<span data-ttu-id="7fe07-319">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="7fe07-319">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="7fe07-320">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-320">(Android only)</span></span>|
|<span data-ttu-id="7fe07-321">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="7fe07-321">exemptedAppProtocols</span></span>|<span data-ttu-id="7fe07-322">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fe07-322">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fe07-323">此列表中的 iOS 应用程序将从策略中排除和都将能够从托管的应用程序接收数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-323">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="7fe07-324">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-324">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-325">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="7fe07-325">exemptedAppPackages</span></span>|<span data-ttu-id="7fe07-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7fe07-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fe07-327">此列表中的 android 应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-327">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="7fe07-328">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-328">(Android only)</span></span>|
|<span data-ttu-id="7fe07-329">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-329">faceIdBlocked</span></span>|<span data-ttu-id="7fe07-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-330">Boolean</span></span>|<span data-ttu-id="7fe07-331">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。</span><span class="sxs-lookup"><span data-stu-id="7fe07-331">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="7fe07-332">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-332">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-333">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-333">minimumWipeSdkVersion</span></span>|<span data-ttu-id="7fe07-334">String</span><span class="sxs-lookup"><span data-stu-id="7fe07-334">String</span></span>|<span data-ttu-id="7fe07-335">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-335">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="7fe07-336">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="7fe07-336">minimumWipePatchVersion</span></span>|<span data-ttu-id="7fe07-337">字符串</span><span class="sxs-lookup"><span data-stu-id="7fe07-337">String</span></span>|<span data-ttu-id="7fe07-338">托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。</span><span class="sxs-lookup"><span data-stu-id="7fe07-338">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="7fe07-339">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-339">(Android only)</span></span>|
|<span data-ttu-id="7fe07-340">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="7fe07-340">allowedIosDeviceModels</span></span>|<span data-ttu-id="7fe07-341">字符串</span><span class="sxs-lookup"><span data-stu-id="7fe07-341">String</span></span>|<span data-ttu-id="7fe07-342">作为字符串的托管的应用程序，以允许的设备模型的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="7fe07-342">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="7fe07-343">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-343">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-344">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="7fe07-344">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="7fe07-345">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="7fe07-345">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="7fe07-346">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备模型。</span><span class="sxs-lookup"><span data-stu-id="7fe07-346">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="7fe07-347">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-347">(iOS Only).</span></span> <span data-ttu-id="7fe07-348">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-348">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="7fe07-349">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="7fe07-349">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="7fe07-350">字符串</span><span class="sxs-lookup"><span data-stu-id="7fe07-350">String</span></span>|<span data-ttu-id="7fe07-351">作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="7fe07-351">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="7fe07-352">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="7fe07-352">(Android only)</span></span>|
|<span data-ttu-id="7fe07-353">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="7fe07-353">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="7fe07-354">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="7fe07-354">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="7fe07-355">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。</span><span class="sxs-lookup"><span data-stu-id="7fe07-355">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="7fe07-356">(仅 android)。</span><span class="sxs-lookup"><span data-stu-id="7fe07-356">(Android only).</span></span> <span data-ttu-id="7fe07-357">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="7fe07-357">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="7fe07-358">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="7fe07-358">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="7fe07-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-359">Boolean</span></span>|<span data-ttu-id="7fe07-360">如果第三方键盘允许访问托管的应用程序时，定义。</span><span class="sxs-lookup"><span data-stu-id="7fe07-360">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="7fe07-361">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-361">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-362">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="7fe07-362">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="7fe07-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-363">Boolean</span></span>|<span data-ttu-id="7fe07-364">如果到所选的文件共享位置从托管的应用程序支持打开项操作，定义。</span><span class="sxs-lookup"><span data-stu-id="7fe07-364">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="7fe07-365">此设置仅适用于 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 并且 DisableProtectionOfManagedOutboundOpenInData 设置为 False。</span><span class="sxs-lookup"><span data-stu-id="7fe07-365">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="7fe07-366">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-366">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-367">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="7fe07-367">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="7fe07-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-368">Boolean</span></span>|<span data-ttu-id="7fe07-369">禁用传输到 IOS OpenIn 选项通过其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="7fe07-369">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="7fe07-370">此设置只允许为 True 时 AllowedOutboundDataTransferDestinations 设置为 ManagedApps。</span><span class="sxs-lookup"><span data-stu-id="7fe07-370">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="7fe07-371">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-371">(iOS Only)</span></span>|
|<span data-ttu-id="7fe07-372">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="7fe07-372">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="7fe07-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fe07-373">Boolean</span></span>|<span data-ttu-id="7fe07-374">从未知源保护传入的数据。</span><span class="sxs-lookup"><span data-stu-id="7fe07-374">Protect incoming data from unknown source.</span></span> <span data-ttu-id="7fe07-375">此设置只允许为 True 时 AllowedInboundDataTransferSources 设置为 AllApps。</span><span class="sxs-lookup"><span data-stu-id="7fe07-375">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="7fe07-376">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="7fe07-376">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="7fe07-377">响应</span><span class="sxs-lookup"><span data-stu-id="7fe07-377">Response</span></span>
<span data-ttu-id="7fe07-378">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7fe07-378">If successful, this method returns a `200 OK` response code and an updated [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe07-379">示例</span><span class="sxs-lookup"><span data-stu-id="7fe07-379">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fe07-380">请求</span><span class="sxs-lookup"><span data-stu-id="7fe07-380">Request</span></span>
<span data-ttu-id="7fe07-381">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fe07-381">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 3153

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="7fe07-382">响应</span><span class="sxs-lookup"><span data-stu-id="7fe07-382">Response</span></span>
<span data-ttu-id="7fe07-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fe07-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3327

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
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
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
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```





