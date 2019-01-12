---
title: 更新 androidManagedAppProtection
description: 更新 androidManagedAppProtection 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af739f624fbc2ea5f38232a6e4a41fdc1ba68b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914673"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="eea77-103">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="eea77-103">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="eea77-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eea77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eea77-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eea77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eea77-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eea77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eea77-107">更新 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eea77-107">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eea77-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eea77-108">Prerequisites</span></span>
<span data-ttu-id="eea77-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eea77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea77-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eea77-111">Permission type</span></span>|<span data-ttu-id="eea77-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eea77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eea77-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eea77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eea77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eea77-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eea77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea77-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eea77-116">Not supported.</span></span>|
|<span data-ttu-id="eea77-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eea77-117">Application</span></span>|<span data-ttu-id="eea77-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eea77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eea77-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eea77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="eea77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eea77-120">Request headers</span></span>
|<span data-ttu-id="eea77-121">标头</span><span class="sxs-lookup"><span data-stu-id="eea77-121">Header</span></span>|<span data-ttu-id="eea77-122">值</span><span class="sxs-lookup"><span data-stu-id="eea77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eea77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eea77-123">Authorization</span></span>|<span data-ttu-id="eea77-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eea77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eea77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eea77-125">Accept</span></span>|<span data-ttu-id="eea77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eea77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea77-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eea77-127">Request body</span></span>
<span data-ttu-id="eea77-128">在请求正文中，提供 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eea77-128">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="eea77-129">下表显示了创建 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eea77-129">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="eea77-130">属性</span><span class="sxs-lookup"><span data-stu-id="eea77-130">Property</span></span>|<span data-ttu-id="eea77-131">类型</span><span class="sxs-lookup"><span data-stu-id="eea77-131">Type</span></span>|<span data-ttu-id="eea77-132">说明</span><span class="sxs-lookup"><span data-stu-id="eea77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea77-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eea77-133">displayName</span></span>|<span data-ttu-id="eea77-134">String</span><span class="sxs-lookup"><span data-stu-id="eea77-134">String</span></span>|<span data-ttu-id="eea77-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="eea77-135">Policy display name.</span></span> <span data-ttu-id="eea77-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-137">description</span><span class="sxs-lookup"><span data-stu-id="eea77-137">description</span></span>|<span data-ttu-id="eea77-138">String</span><span class="sxs-lookup"><span data-stu-id="eea77-138">String</span></span>|<span data-ttu-id="eea77-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="eea77-139">The policy's description.</span></span> <span data-ttu-id="eea77-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eea77-141">createdDateTime</span></span>|<span data-ttu-id="eea77-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea77-142">DateTimeOffset</span></span>|<span data-ttu-id="eea77-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eea77-143">The date and time the policy was created.</span></span> <span data-ttu-id="eea77-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eea77-145">lastModifiedDateTime</span></span>|<span data-ttu-id="eea77-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea77-146">DateTimeOffset</span></span>|<span data-ttu-id="eea77-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="eea77-147">Last time the policy was modified.</span></span> <span data-ttu-id="eea77-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-149">id</span><span class="sxs-lookup"><span data-stu-id="eea77-149">id</span></span>|<span data-ttu-id="eea77-150">String</span><span class="sxs-lookup"><span data-stu-id="eea77-150">String</span></span>|<span data-ttu-id="eea77-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eea77-151">Key of the entity.</span></span> <span data-ttu-id="eea77-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-153">version</span><span class="sxs-lookup"><span data-stu-id="eea77-153">version</span></span>|<span data-ttu-id="eea77-154">String</span><span class="sxs-lookup"><span data-stu-id="eea77-154">String</span></span>|<span data-ttu-id="eea77-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="eea77-155">Version of the entity.</span></span> <span data-ttu-id="eea77-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="eea77-157">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="eea77-157">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="eea77-158">Duration</span><span class="sxs-lookup"><span data-stu-id="eea77-158">Duration</span></span>|<span data-ttu-id="eea77-159">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="eea77-159">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="eea77-160">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-160">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-161">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="eea77-161">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="eea77-162">Duration</span><span class="sxs-lookup"><span data-stu-id="eea77-162">Duration</span></span>|<span data-ttu-id="eea77-163">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="eea77-163">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="eea77-164">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-165">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="eea77-165">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="eea77-166">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="eea77-166">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="eea77-167">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="eea77-167">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="eea77-168">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-169">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="eea77-169">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="eea77-170">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="eea77-170">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="eea77-171">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="eea77-171">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="eea77-172">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="eea77-172">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="eea77-173">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-173">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-174">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="eea77-174">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="eea77-175">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="eea77-175">organizationalCredentialsRequired</span></span>|<span data-ttu-id="eea77-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-176">Boolean</span></span>|<span data-ttu-id="eea77-177">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="eea77-177">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="eea77-178">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-178">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-179">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="eea77-179">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="eea77-180">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="eea77-180">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="eea77-181">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="eea77-181">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="eea77-182">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-183">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="eea77-183">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="eea77-184">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-184">dataBackupBlocked</span></span>|<span data-ttu-id="eea77-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-185">Boolean</span></span>|<span data-ttu-id="eea77-186">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="eea77-186">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="eea77-187">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-187">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-188">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="eea77-188">deviceComplianceRequired</span></span>|<span data-ttu-id="eea77-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-189">Boolean</span></span>|<span data-ttu-id="eea77-190">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="eea77-190">Indicates whether device compliance is required.</span></span> <span data-ttu-id="eea77-191">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-192">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="eea77-192">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="eea77-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-193">Boolean</span></span>|<span data-ttu-id="eea77-194">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="eea77-194">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="eea77-195">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-196">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-196">saveAsBlocked</span></span>|<span data-ttu-id="eea77-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-197">Boolean</span></span>|<span data-ttu-id="eea77-198">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="eea77-198">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="eea77-199">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-200">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="eea77-200">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="eea77-201">Duration</span><span class="sxs-lookup"><span data-stu-id="eea77-201">Duration</span></span>|<span data-ttu-id="eea77-202">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="eea77-202">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="eea77-203">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-204">pinRequired</span><span class="sxs-lookup"><span data-stu-id="eea77-204">pinRequired</span></span>|<span data-ttu-id="eea77-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-205">Boolean</span></span>|<span data-ttu-id="eea77-206">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="eea77-206">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="eea77-207">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-208">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="eea77-208">maximumPinRetries</span></span>|<span data-ttu-id="eea77-209">Int32</span><span class="sxs-lookup"><span data-stu-id="eea77-209">Int32</span></span>|<span data-ttu-id="eea77-210">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="eea77-210">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="eea77-211">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-212">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-212">simplePinBlocked</span></span>|<span data-ttu-id="eea77-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-213">Boolean</span></span>|<span data-ttu-id="eea77-214">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="eea77-214">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="eea77-215">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-216">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="eea77-216">minimumPinLength</span></span>|<span data-ttu-id="eea77-217">Int32</span><span class="sxs-lookup"><span data-stu-id="eea77-217">Int32</span></span>|<span data-ttu-id="eea77-218">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-218">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-219">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="eea77-219">pinCharacterSet</span></span>|[<span data-ttu-id="eea77-220">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="eea77-220">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="eea77-221">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="eea77-221">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="eea77-222">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-222">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-223">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="eea77-223">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="eea77-224">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="eea77-224">periodBeforePinReset</span></span>|<span data-ttu-id="eea77-225">Duration</span><span class="sxs-lookup"><span data-stu-id="eea77-225">Duration</span></span>|<span data-ttu-id="eea77-226">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="eea77-226">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="eea77-227">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-227">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-228">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="eea77-228">allowedDataStorageLocations</span></span>|<span data-ttu-id="eea77-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="eea77-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="eea77-230">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="eea77-230">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="eea77-231">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-232">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="eea77-232">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="eea77-233">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-233">contactSyncBlocked</span></span>|<span data-ttu-id="eea77-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-234">Boolean</span></span>|<span data-ttu-id="eea77-235">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="eea77-235">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="eea77-236">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-236">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-237">printBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-237">printBlocked</span></span>|<span data-ttu-id="eea77-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-238">Boolean</span></span>|<span data-ttu-id="eea77-239">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="eea77-239">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="eea77-240">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-241">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-241">fingerprintBlocked</span></span>|<span data-ttu-id="eea77-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-242">Boolean</span></span>|<span data-ttu-id="eea77-243">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="eea77-243">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="eea77-244">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-245">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="eea77-245">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="eea77-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-246">Boolean</span></span>|<span data-ttu-id="eea77-247">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="eea77-247">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="eea77-248">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-249">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-249">minimumRequiredOsVersion</span></span>|<span data-ttu-id="eea77-250">String</span><span class="sxs-lookup"><span data-stu-id="eea77-250">String</span></span>|<span data-ttu-id="eea77-251">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="eea77-251">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="eea77-252">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-253">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-253">minimumWarningOsVersion</span></span>|<span data-ttu-id="eea77-254">String</span><span class="sxs-lookup"><span data-stu-id="eea77-254">String</span></span>|<span data-ttu-id="eea77-255">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="eea77-255">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="eea77-256">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-257">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-257">minimumRequiredAppVersion</span></span>|<span data-ttu-id="eea77-258">String</span><span class="sxs-lookup"><span data-stu-id="eea77-258">String</span></span>|<span data-ttu-id="eea77-259">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="eea77-259">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="eea77-260">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-261">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-261">minimumWarningAppVersion</span></span>|<span data-ttu-id="eea77-262">String</span><span class="sxs-lookup"><span data-stu-id="eea77-262">String</span></span>|<span data-ttu-id="eea77-263">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="eea77-263">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="eea77-264">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-265">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-265">minimumWipeOsVersion</span></span>|<span data-ttu-id="eea77-266">字符串</span><span class="sxs-lookup"><span data-stu-id="eea77-266">String</span></span>|<span data-ttu-id="eea77-267">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="eea77-267">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="eea77-268">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-269">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-269">minimumWipeAppVersion</span></span>|<span data-ttu-id="eea77-270">字符串</span><span class="sxs-lookup"><span data-stu-id="eea77-270">String</span></span>|<span data-ttu-id="eea77-271">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="eea77-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="eea77-272">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-273">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="eea77-273">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="eea77-274">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="eea77-274">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="eea77-275">定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="eea77-275">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="eea77-276">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-277">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="eea77-277">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="eea77-278">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="eea77-278">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="eea77-279">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="eea77-279">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="eea77-280">定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。</span><span class="sxs-lookup"><span data-stu-id="eea77-280">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="eea77-281">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="eea77-281">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="eea77-282">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="eea77-282">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="eea77-283">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="eea77-283">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="eea77-284">Duration</span><span class="sxs-lookup"><span data-stu-id="eea77-284">Duration</span></span>|<span data-ttu-id="eea77-285">以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时</span><span class="sxs-lookup"><span data-stu-id="eea77-285">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-286">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eea77-286">isAssigned</span></span>|<span data-ttu-id="eea77-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-287">Boolean</span></span>|<span data-ttu-id="eea77-288">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="eea77-288">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="eea77-289">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="eea77-289">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="eea77-290">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="eea77-290">targetedAppManagementLevels</span></span>|[<span data-ttu-id="eea77-291">appManagementLevel</span><span class="sxs-lookup"><span data-stu-id="eea77-291">appManagementLevel</span></span>](../resources/intune-mam-appmanagementlevel.md)|<span data-ttu-id="eea77-292">从[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)此策略继承目标应用程序管理级别。</span><span class="sxs-lookup"><span data-stu-id="eea77-292">The intended app management levels for this policy Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span></span> <span data-ttu-id="eea77-293">可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="eea77-293">Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.</span></span>|
|<span data-ttu-id="eea77-294">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="eea77-294">screenCaptureBlocked</span></span>|<span data-ttu-id="eea77-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-295">Boolean</span></span>|<span data-ttu-id="eea77-296">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="eea77-296">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="eea77-297">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="eea77-297">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="eea77-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-298">Boolean</span></span>|<span data-ttu-id="eea77-299">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="eea77-299">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="eea77-300">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="eea77-300">encryptAppData</span></span>|<span data-ttu-id="eea77-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="eea77-301">Boolean</span></span>|<span data-ttu-id="eea77-302">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="eea77-302">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="eea77-303">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="eea77-303">deployedAppCount</span></span>|<span data-ttu-id="eea77-304">Int32</span><span class="sxs-lookup"><span data-stu-id="eea77-304">Int32</span></span>|<span data-ttu-id="eea77-305">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="eea77-305">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="eea77-306">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-306">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="eea77-307">String</span><span class="sxs-lookup"><span data-stu-id="eea77-307">String</span></span>|<span data-ttu-id="eea77-308">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="eea77-308">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="eea77-309">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-309">minimumWarningPatchVersion</span></span>|<span data-ttu-id="eea77-310">String</span><span class="sxs-lookup"><span data-stu-id="eea77-310">String</span></span>|<span data-ttu-id="eea77-311">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="eea77-311">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="eea77-312">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="eea77-312">exemptedAppPackages</span></span>|<span data-ttu-id="eea77-313">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eea77-313">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="eea77-314">此列表中的应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="eea77-314">App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span>|
|<span data-ttu-id="eea77-315">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="eea77-315">minimumWipePatchVersion</span></span>|<span data-ttu-id="eea77-316">字符串</span><span class="sxs-lookup"><span data-stu-id="eea77-316">String</span></span>|<span data-ttu-id="eea77-317">托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。</span><span class="sxs-lookup"><span data-stu-id="eea77-317">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span>|
|<span data-ttu-id="eea77-318">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="eea77-318">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="eea77-319">字符串</span><span class="sxs-lookup"><span data-stu-id="eea77-319">String</span></span>|<span data-ttu-id="eea77-320">作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="eea77-320">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span>|
|<span data-ttu-id="eea77-321">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="eea77-321">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="eea77-322">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="eea77-322">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="eea77-323">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。</span><span class="sxs-lookup"><span data-stu-id="eea77-323">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="eea77-324">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="eea77-324">Possible values are: `block`, `wipe`.</span></span>|



## <a name="response"></a><span data-ttu-id="eea77-325">响应</span><span class="sxs-lookup"><span data-stu-id="eea77-325">Response</span></span>
<span data-ttu-id="eea77-326">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eea77-326">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eea77-327">示例</span><span class="sxs-lookup"><span data-stu-id="eea77-327">Example</span></span>
### <a name="request"></a><span data-ttu-id="eea77-328">请求</span><span class="sxs-lookup"><span data-stu-id="eea77-328">Request</span></span>
<span data-ttu-id="eea77-329">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eea77-329">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 2396

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

### <a name="response"></a><span data-ttu-id="eea77-330">响应</span><span class="sxs-lookup"><span data-stu-id="eea77-330">Response</span></span>
<span data-ttu-id="eea77-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eea77-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2570

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





