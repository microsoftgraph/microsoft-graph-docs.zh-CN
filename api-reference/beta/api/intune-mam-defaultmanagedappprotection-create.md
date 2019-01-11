---
title: 创建 defaultManagedAppProtection
description: 创建新的 defaultManagedAppProtection 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d479fa5dcb1df66bb67cd6e1d7ae550ff408fd43
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890410"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="d9dd7-103">创建 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d9dd7-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="d9dd7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9dd7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9dd7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9dd7-107">创建新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-107">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9dd7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9dd7-108">Prerequisites</span></span>
<span data-ttu-id="d9dd7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d9dd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9dd7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9dd7-111">Permission type</span></span>|<span data-ttu-id="d9dd7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9dd7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9dd7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9dd7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9dd7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9dd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-116">Not supported.</span></span>|
|<span data-ttu-id="d9dd7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9dd7-117">Application</span></span>|<span data-ttu-id="d9dd7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9dd7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9dd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="d9dd7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9dd7-120">Request headers</span></span>
|<span data-ttu-id="d9dd7-121">标头</span><span class="sxs-lookup"><span data-stu-id="d9dd7-121">Header</span></span>|<span data-ttu-id="d9dd7-122">值</span><span class="sxs-lookup"><span data-stu-id="d9dd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9dd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9dd7-123">Authorization</span></span>|<span data-ttu-id="d9dd7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9dd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9dd7-125">Accept</span></span>|<span data-ttu-id="d9dd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9dd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9dd7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9dd7-127">Request body</span></span>
<span data-ttu-id="d9dd7-128">在请求正文中，提供 defaultManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-128">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="d9dd7-129">下表显示创建 defaultManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-129">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="d9dd7-130">属性</span><span class="sxs-lookup"><span data-stu-id="d9dd7-130">Property</span></span>|<span data-ttu-id="d9dd7-131">类型</span><span class="sxs-lookup"><span data-stu-id="d9dd7-131">Type</span></span>|<span data-ttu-id="d9dd7-132">说明</span><span class="sxs-lookup"><span data-stu-id="d9dd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9dd7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d9dd7-133">displayName</span></span>|<span data-ttu-id="d9dd7-134">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-134">String</span></span>|<span data-ttu-id="d9dd7-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-135">Policy display name.</span></span> <span data-ttu-id="d9dd7-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-137">description</span><span class="sxs-lookup"><span data-stu-id="d9dd7-137">description</span></span>|<span data-ttu-id="d9dd7-138">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-138">String</span></span>|<span data-ttu-id="d9dd7-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-139">The policy's description.</span></span> <span data-ttu-id="d9dd7-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9dd7-141">createdDateTime</span></span>|<span data-ttu-id="d9dd7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9dd7-142">DateTimeOffset</span></span>|<span data-ttu-id="d9dd7-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-143">The date and time the policy was created.</span></span> <span data-ttu-id="d9dd7-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9dd7-145">lastModifiedDateTime</span></span>|<span data-ttu-id="d9dd7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9dd7-146">DateTimeOffset</span></span>|<span data-ttu-id="d9dd7-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-147">Last time the policy was modified.</span></span> <span data-ttu-id="d9dd7-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-149">id</span><span class="sxs-lookup"><span data-stu-id="d9dd7-149">id</span></span>|<span data-ttu-id="d9dd7-150">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-150">String</span></span>|<span data-ttu-id="d9dd7-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-151">Key of the entity.</span></span> <span data-ttu-id="d9dd7-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-153">version</span><span class="sxs-lookup"><span data-stu-id="d9dd7-153">version</span></span>|<span data-ttu-id="d9dd7-154">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-154">String</span></span>|<span data-ttu-id="d9dd7-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-155">Version of the entity.</span></span> <span data-ttu-id="d9dd7-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d9dd7-157">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d9dd7-157">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="d9dd7-158">Duration</span><span class="sxs-lookup"><span data-stu-id="d9dd7-158">Duration</span></span>|<span data-ttu-id="d9dd7-159">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-159">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="d9dd7-160">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-160">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-161">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="d9dd7-161">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="d9dd7-162">Duration</span><span class="sxs-lookup"><span data-stu-id="d9dd7-162">Duration</span></span>|<span data-ttu-id="d9dd7-163">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-163">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="d9dd7-164">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-165">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="d9dd7-165">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="d9dd7-166">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d9dd7-166">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="d9dd7-167">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-167">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="d9dd7-168">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-169">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-169">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d9dd7-170">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="d9dd7-170">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="d9dd7-171">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="d9dd7-171">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="d9dd7-172">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-172">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="d9dd7-173">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-173">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-174">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-174">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="d9dd7-175">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="d9dd7-175">organizationalCredentialsRequired</span></span>|<span data-ttu-id="d9dd7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-176">Boolean</span></span>|<span data-ttu-id="d9dd7-177">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-177">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="d9dd7-178">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-178">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-179">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d9dd7-179">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="d9dd7-180">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="d9dd7-180">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="d9dd7-181">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-181">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="d9dd7-182">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-183">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-183">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="d9dd7-184">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-184">dataBackupBlocked</span></span>|<span data-ttu-id="d9dd7-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-185">Boolean</span></span>|<span data-ttu-id="d9dd7-186">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-186">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="d9dd7-187">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-187">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-188">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="d9dd7-188">deviceComplianceRequired</span></span>|<span data-ttu-id="d9dd7-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-189">Boolean</span></span>|<span data-ttu-id="d9dd7-190">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-190">Indicates whether device compliance is required.</span></span> <span data-ttu-id="d9dd7-191">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-192">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="d9dd7-192">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="d9dd7-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-193">Boolean</span></span>|<span data-ttu-id="d9dd7-194">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-194">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="d9dd7-195">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-196">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-196">saveAsBlocked</span></span>|<span data-ttu-id="d9dd7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-197">Boolean</span></span>|<span data-ttu-id="d9dd7-198">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-198">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="d9dd7-199">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-200">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="d9dd7-200">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="d9dd7-201">Duration</span><span class="sxs-lookup"><span data-stu-id="d9dd7-201">Duration</span></span>|<span data-ttu-id="d9dd7-202">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-202">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="d9dd7-203">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-204">pinRequired</span><span class="sxs-lookup"><span data-stu-id="d9dd7-204">pinRequired</span></span>|<span data-ttu-id="d9dd7-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-205">Boolean</span></span>|<span data-ttu-id="d9dd7-206">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-206">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="d9dd7-207">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-208">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="d9dd7-208">maximumPinRetries</span></span>|<span data-ttu-id="d9dd7-209">Int32</span><span class="sxs-lookup"><span data-stu-id="d9dd7-209">Int32</span></span>|<span data-ttu-id="d9dd7-210">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-210">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="d9dd7-211">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-212">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-212">simplePinBlocked</span></span>|<span data-ttu-id="d9dd7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-213">Boolean</span></span>|<span data-ttu-id="d9dd7-214">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-214">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="d9dd7-215">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-216">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="d9dd7-216">minimumPinLength</span></span>|<span data-ttu-id="d9dd7-217">Int32</span><span class="sxs-lookup"><span data-stu-id="d9dd7-217">Int32</span></span>|<span data-ttu-id="d9dd7-218">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-218">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-219">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d9dd7-219">pinCharacterSet</span></span>|[<span data-ttu-id="d9dd7-220">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="d9dd7-220">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="d9dd7-221">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-221">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="d9dd7-222">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-222">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-223">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-223">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="d9dd7-224">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="d9dd7-224">periodBeforePinReset</span></span>|<span data-ttu-id="d9dd7-225">Duration</span><span class="sxs-lookup"><span data-stu-id="d9dd7-225">Duration</span></span>|<span data-ttu-id="d9dd7-226">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="d9dd7-226">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="d9dd7-227">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-227">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-228">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="d9dd7-228">allowedDataStorageLocations</span></span>|<span data-ttu-id="d9dd7-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9dd7-229">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="d9dd7-230">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-230">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="d9dd7-231">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-232">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-232">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="d9dd7-233">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-233">contactSyncBlocked</span></span>|<span data-ttu-id="d9dd7-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-234">Boolean</span></span>|<span data-ttu-id="d9dd7-235">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-235">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="d9dd7-236">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-236">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-237">printBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-237">printBlocked</span></span>|<span data-ttu-id="d9dd7-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-238">Boolean</span></span>|<span data-ttu-id="d9dd7-239">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-239">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="d9dd7-240">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-241">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-241">fingerprintBlocked</span></span>|<span data-ttu-id="d9dd7-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-242">Boolean</span></span>|<span data-ttu-id="d9dd7-243">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-243">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="d9dd7-244">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-245">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="d9dd7-245">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="d9dd7-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-246">Boolean</span></span>|<span data-ttu-id="d9dd7-247">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-247">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="d9dd7-248">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-249">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-249">minimumRequiredOsVersion</span></span>|<span data-ttu-id="d9dd7-250">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-250">String</span></span>|<span data-ttu-id="d9dd7-251">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-251">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d9dd7-252">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-253">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-253">minimumWarningOsVersion</span></span>|<span data-ttu-id="d9dd7-254">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-254">String</span></span>|<span data-ttu-id="d9dd7-255">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-255">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="d9dd7-256">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-257">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-257">minimumRequiredAppVersion</span></span>|<span data-ttu-id="d9dd7-258">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-258">String</span></span>|<span data-ttu-id="d9dd7-259">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-259">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d9dd7-260">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-261">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-261">minimumWarningAppVersion</span></span>|<span data-ttu-id="d9dd7-262">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-262">String</span></span>|<span data-ttu-id="d9dd7-263">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-263">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="d9dd7-264">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-265">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-265">minimumWipeOsVersion</span></span>|<span data-ttu-id="d9dd7-266">字符串</span><span class="sxs-lookup"><span data-stu-id="d9dd7-266">String</span></span>|<span data-ttu-id="d9dd7-267">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-267">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="d9dd7-268">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-269">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-269">minimumWipeAppVersion</span></span>|<span data-ttu-id="d9dd7-270">字符串</span><span class="sxs-lookup"><span data-stu-id="d9dd7-270">String</span></span>|<span data-ttu-id="d9dd7-271">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="d9dd7-272">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-273">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="d9dd7-273">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="d9dd7-274">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="d9dd7-274">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="d9dd7-275">定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-275">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="d9dd7-276">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-277">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-277">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="d9dd7-278">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="d9dd7-278">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="d9dd7-279">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="d9dd7-279">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="d9dd7-280">定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-280">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="d9dd7-281">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-281">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="d9dd7-282">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-282">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="d9dd7-283">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="d9dd7-283">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="d9dd7-284">Duration</span><span class="sxs-lookup"><span data-stu-id="d9dd7-284">Duration</span></span>|<span data-ttu-id="d9dd7-285">以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时</span><span class="sxs-lookup"><span data-stu-id="d9dd7-285">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="d9dd7-286">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="d9dd7-286">appDataEncryptionType</span></span>|[<span data-ttu-id="d9dd7-287">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="d9dd7-287">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="d9dd7-288">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-288">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="d9dd7-289">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-289">(iOS Only).</span></span> <span data-ttu-id="d9dd7-290">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-290">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="d9dd7-291">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-291">screenCaptureBlocked</span></span>|<span data-ttu-id="d9dd7-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-292">Boolean</span></span>|<span data-ttu-id="d9dd7-293">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-293">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="d9dd7-294">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-294">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-295">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="d9dd7-295">encryptAppData</span></span>|<span data-ttu-id="d9dd7-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-296">Boolean</span></span>|<span data-ttu-id="d9dd7-297">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-297">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="d9dd7-298">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-298">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-299">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="d9dd7-299">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="d9dd7-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-300">Boolean</span></span>|<span data-ttu-id="d9dd7-301">启用此设置后，如果启用设备加密，则禁用应用程序级别的加密。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-301">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="d9dd7-302">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-302">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-303">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-303">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="d9dd7-304">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-304">String</span></span>|<span data-ttu-id="d9dd7-305">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-305">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="d9dd7-306">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-306">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-307">customSettings</span><span class="sxs-lookup"><span data-stu-id="d9dd7-307">customSettings</span></span>|<span data-ttu-id="d9dd7-308">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9dd7-308">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d9dd7-309">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="d9dd7-309">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="d9dd7-310">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="d9dd7-310">deployedAppCount</span></span>|<span data-ttu-id="d9dd7-311">Int32</span><span class="sxs-lookup"><span data-stu-id="d9dd7-311">Int32</span></span>|<span data-ttu-id="d9dd7-312">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-312">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="d9dd7-313">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-313">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="d9dd7-314">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-314">String</span></span>|<span data-ttu-id="d9dd7-315">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="d9dd7-315">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="d9dd7-316">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-316">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-317">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-317">minimumWarningPatchVersion</span></span>|<span data-ttu-id="d9dd7-318">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-318">String</span></span>|<span data-ttu-id="d9dd7-319">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-319">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="d9dd7-320">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-320">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-321">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="d9dd7-321">exemptedAppProtocols</span></span>|<span data-ttu-id="d9dd7-322">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9dd7-322">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d9dd7-323">此列表中的 iOS 应用程序将从策略中排除和都将能够从托管的应用程序接收数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-323">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="d9dd7-324">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-324">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-325">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="d9dd7-325">exemptedAppPackages</span></span>|<span data-ttu-id="d9dd7-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9dd7-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d9dd7-327">此列表中的 android 应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-327">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="d9dd7-328">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-328">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-329">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-329">faceIdBlocked</span></span>|<span data-ttu-id="d9dd7-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9dd7-330">Boolean</span></span>|<span data-ttu-id="d9dd7-331">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-331">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="d9dd7-332">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-332">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-333">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-333">minimumWipeSdkVersion</span></span>|<span data-ttu-id="d9dd7-334">String</span><span class="sxs-lookup"><span data-stu-id="d9dd7-334">String</span></span>|<span data-ttu-id="d9dd7-335">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-335">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="d9dd7-336">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="d9dd7-336">minimumWipePatchVersion</span></span>|<span data-ttu-id="d9dd7-337">字符串</span><span class="sxs-lookup"><span data-stu-id="d9dd7-337">String</span></span>|<span data-ttu-id="d9dd7-338">托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-338">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="d9dd7-339">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-339">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-340">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="d9dd7-340">allowedIosDeviceModels</span></span>|<span data-ttu-id="d9dd7-341">字符串</span><span class="sxs-lookup"><span data-stu-id="d9dd7-341">String</span></span>|<span data-ttu-id="d9dd7-342">作为字符串的托管的应用程序，以允许的设备模型的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-342">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="d9dd7-343">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-343">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-344">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="d9dd7-344">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="d9dd7-345">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="d9dd7-345">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="d9dd7-346">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备模型。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-346">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="d9dd7-347">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-347">(iOS Only).</span></span> <span data-ttu-id="d9dd7-348">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-348">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="d9dd7-349">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="d9dd7-349">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="d9dd7-350">字符串</span><span class="sxs-lookup"><span data-stu-id="d9dd7-350">String</span></span>|<span data-ttu-id="d9dd7-351">作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-351">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="d9dd7-352">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="d9dd7-352">(Android only)</span></span>|
|<span data-ttu-id="d9dd7-353">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="d9dd7-353">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="d9dd7-354">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="d9dd7-354">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="d9dd7-355">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-355">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="d9dd7-356">(仅 android)。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-356">(Android only).</span></span> <span data-ttu-id="d9dd7-357">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-357">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="d9dd7-358">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9dd7-358">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="d9dd7-359">布尔</span><span class="sxs-lookup"><span data-stu-id="d9dd7-359">Boolean</span></span>|<span data-ttu-id="d9dd7-360">如果第三方键盘允许访问托管的应用程序时，定义。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-360">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="d9dd7-361">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-361">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-362">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="d9dd7-362">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="d9dd7-363">布尔</span><span class="sxs-lookup"><span data-stu-id="d9dd7-363">Boolean</span></span>|<span data-ttu-id="d9dd7-364">如果到所选的文件共享位置从托管的应用程序支持打开项操作，定义。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-364">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="d9dd7-365">此设置仅适用于 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 并且 DisableProtectionOfManagedOutboundOpenInData 设置为 False。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-365">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="d9dd7-366">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-366">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-367">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="d9dd7-367">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="d9dd7-368">布尔</span><span class="sxs-lookup"><span data-stu-id="d9dd7-368">Boolean</span></span>|<span data-ttu-id="d9dd7-369">禁用传输到 IOS OpenIn 选项通过其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-369">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="d9dd7-370">此设置只允许为 True 时 AllowedOutboundDataTransferDestinations 设置为 ManagedApps。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-370">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="d9dd7-371">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-371">(iOS Only)</span></span>|
|<span data-ttu-id="d9dd7-372">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="d9dd7-372">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="d9dd7-373">布尔</span><span class="sxs-lookup"><span data-stu-id="d9dd7-373">Boolean</span></span>|<span data-ttu-id="d9dd7-374">从未知源保护传入的数据。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-374">Protect incoming data from unknown source.</span></span> <span data-ttu-id="d9dd7-375">此设置只允许为 True 时 AllowedInboundDataTransferSources 设置为 AllApps。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-375">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="d9dd7-376">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="d9dd7-376">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="d9dd7-377">响应</span><span class="sxs-lookup"><span data-stu-id="d9dd7-377">Response</span></span>
<span data-ttu-id="d9dd7-378">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-378">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9dd7-379">示例</span><span class="sxs-lookup"><span data-stu-id="d9dd7-379">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9dd7-380">请求</span><span class="sxs-lookup"><span data-stu-id="d9dd7-380">Request</span></span>
<span data-ttu-id="d9dd7-381">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-381">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 3219

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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

### <a name="response"></a><span data-ttu-id="d9dd7-382">响应</span><span class="sxs-lookup"><span data-stu-id="d9dd7-382">Response</span></span>
<span data-ttu-id="d9dd7-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9dd7-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





