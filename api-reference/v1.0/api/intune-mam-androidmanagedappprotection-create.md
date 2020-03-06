---
title: 创建 androidManagedAppProtection
description: 创建新的 androidManagedAppProtection 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f86da9b3ff95f8a385bfd238621eb7aca94af4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513348"
---
# <a name="create-androidmanagedappprotection"></a><span data-ttu-id="3c87e-103">创建 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="3c87e-103">Create androidManagedAppProtection</span></span>

<span data-ttu-id="3c87e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c87e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c87e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c87e-106">创建新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c87e-106">Create a new [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c87e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c87e-107">Prerequisites</span></span>
<span data-ttu-id="3c87e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c87e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c87e-110">Permission type</span></span>|<span data-ttu-id="3c87e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c87e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c87e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c87e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c87e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c87e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c87e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c87e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c87e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c87e-115">Not supported.</span></span>|
|<span data-ttu-id="3c87e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c87e-116">Application</span></span>|<span data-ttu-id="3c87e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c87e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c87e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c87e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="3c87e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c87e-119">Request headers</span></span>
|<span data-ttu-id="3c87e-120">标头</span><span class="sxs-lookup"><span data-stu-id="3c87e-120">Header</span></span>|<span data-ttu-id="3c87e-121">值</span><span class="sxs-lookup"><span data-stu-id="3c87e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c87e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c87e-122">Authorization</span></span>|<span data-ttu-id="3c87e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c87e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c87e-124">接受</span><span class="sxs-lookup"><span data-stu-id="3c87e-124">Accept</span></span>|<span data-ttu-id="3c87e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c87e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c87e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c87e-126">Request body</span></span>
<span data-ttu-id="3c87e-127">在请求正文中，提供 androidManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c87e-127">In the request body, supply a JSON representation for the androidManagedAppProtection object.</span></span>

<span data-ttu-id="3c87e-128">下表显示了创建 androidManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c87e-128">The following table shows the properties that are required when you create the androidManagedAppProtection.</span></span>

|<span data-ttu-id="3c87e-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c87e-129">Property</span></span>|<span data-ttu-id="3c87e-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c87e-130">Type</span></span>|<span data-ttu-id="3c87e-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c87e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c87e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3c87e-132">displayName</span></span>|<span data-ttu-id="3c87e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-133">String</span></span>|<span data-ttu-id="3c87e-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="3c87e-134">Policy display name.</span></span> <span data-ttu-id="3c87e-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-136">说明</span><span class="sxs-lookup"><span data-stu-id="3c87e-136">description</span></span>|<span data-ttu-id="3c87e-137">String</span><span class="sxs-lookup"><span data-stu-id="3c87e-137">String</span></span>|<span data-ttu-id="3c87e-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3c87e-138">The policy's description.</span></span> <span data-ttu-id="3c87e-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c87e-140">createdDateTime</span></span>|<span data-ttu-id="3c87e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c87e-141">DateTimeOffset</span></span>|<span data-ttu-id="3c87e-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3c87e-142">The date and time the policy was created.</span></span> <span data-ttu-id="3c87e-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c87e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3c87e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c87e-145">DateTimeOffset</span></span>|<span data-ttu-id="3c87e-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="3c87e-146">Last time the policy was modified.</span></span> <span data-ttu-id="3c87e-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-148">id</span><span class="sxs-lookup"><span data-stu-id="3c87e-148">id</span></span>|<span data-ttu-id="3c87e-149">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-149">String</span></span>|<span data-ttu-id="3c87e-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c87e-150">Key of the entity.</span></span> <span data-ttu-id="3c87e-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-152">version</span><span class="sxs-lookup"><span data-stu-id="3c87e-152">version</span></span>|<span data-ttu-id="3c87e-153">String</span><span class="sxs-lookup"><span data-stu-id="3c87e-153">String</span></span>|<span data-ttu-id="3c87e-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="3c87e-154">Version of the entity.</span></span> <span data-ttu-id="3c87e-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3c87e-156">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="3c87e-156">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="3c87e-157">持续时间</span><span class="sxs-lookup"><span data-stu-id="3c87e-157">Duration</span></span>|<span data-ttu-id="3c87e-158">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="3c87e-158">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="3c87e-159">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-159">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-160">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="3c87e-160">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="3c87e-161">持续时间</span><span class="sxs-lookup"><span data-stu-id="3c87e-161">Duration</span></span>|<span data-ttu-id="3c87e-162">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="3c87e-162">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="3c87e-163">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-164">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="3c87e-164">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="3c87e-165">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="3c87e-165">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="3c87e-166">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="3c87e-166">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="3c87e-167">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="3c87e-168">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="3c87e-168">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="3c87e-169">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="3c87e-169">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="3c87e-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="3c87e-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="3c87e-171">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="3c87e-171">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="3c87e-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="3c87e-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="3c87e-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="3c87e-174">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="3c87e-174">organizationalCredentialsRequired</span></span>|<span data-ttu-id="3c87e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-175">Boolean</span></span>|<span data-ttu-id="3c87e-176">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="3c87e-176">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="3c87e-177">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-178">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="3c87e-178">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="3c87e-179">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="3c87e-179">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="3c87e-180">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="3c87e-180">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="3c87e-181">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="3c87e-182">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="3c87e-182">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="3c87e-183">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-183">dataBackupBlocked</span></span>|<span data-ttu-id="3c87e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-184">Boolean</span></span>|<span data-ttu-id="3c87e-185">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="3c87e-185">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="3c87e-186">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-187">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="3c87e-187">deviceComplianceRequired</span></span>|<span data-ttu-id="3c87e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-188">Boolean</span></span>|<span data-ttu-id="3c87e-189">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="3c87e-189">Indicates whether device compliance is required.</span></span> <span data-ttu-id="3c87e-190">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-191">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="3c87e-191">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="3c87e-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-192">Boolean</span></span>|<span data-ttu-id="3c87e-193">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="3c87e-193">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="3c87e-194">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-195">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-195">saveAsBlocked</span></span>|<span data-ttu-id="3c87e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-196">Boolean</span></span>|<span data-ttu-id="3c87e-197">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="3c87e-197">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="3c87e-198">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-199">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="3c87e-199">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="3c87e-200">持续时间</span><span class="sxs-lookup"><span data-stu-id="3c87e-200">Duration</span></span>|<span data-ttu-id="3c87e-201">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="3c87e-201">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="3c87e-202">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-203">pinRequired</span><span class="sxs-lookup"><span data-stu-id="3c87e-203">pinRequired</span></span>|<span data-ttu-id="3c87e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-204">Boolean</span></span>|<span data-ttu-id="3c87e-205">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="3c87e-205">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="3c87e-206">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-207">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="3c87e-207">maximumPinRetries</span></span>|<span data-ttu-id="3c87e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3c87e-208">Int32</span></span>|<span data-ttu-id="3c87e-209">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="3c87e-209">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="3c87e-210">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-211">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-211">simplePinBlocked</span></span>|<span data-ttu-id="3c87e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-212">Boolean</span></span>|<span data-ttu-id="3c87e-213">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="3c87e-213">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="3c87e-214">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-215">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="3c87e-215">minimumPinLength</span></span>|<span data-ttu-id="3c87e-216">Int32</span><span class="sxs-lookup"><span data-stu-id="3c87e-216">Int32</span></span>|<span data-ttu-id="3c87e-217">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-217">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-218">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="3c87e-218">pinCharacterSet</span></span>|[<span data-ttu-id="3c87e-219">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="3c87e-219">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="3c87e-220">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="3c87e-220">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="3c87e-221">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-221">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="3c87e-222">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="3c87e-222">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="3c87e-223">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="3c87e-223">periodBeforePinReset</span></span>|<span data-ttu-id="3c87e-224">Duration</span><span class="sxs-lookup"><span data-stu-id="3c87e-224">Duration</span></span>|<span data-ttu-id="3c87e-225">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="3c87e-225">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="3c87e-226">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-227">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="3c87e-227">allowedDataStorageLocations</span></span>|<span data-ttu-id="3c87e-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c87e-228">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="3c87e-229">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="3c87e-229">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="3c87e-230">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="3c87e-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="3c87e-231">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="3c87e-231">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="3c87e-232">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-232">contactSyncBlocked</span></span>|<span data-ttu-id="3c87e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-233">Boolean</span></span>|<span data-ttu-id="3c87e-234">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="3c87e-234">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="3c87e-235">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-236">printBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-236">printBlocked</span></span>|<span data-ttu-id="3c87e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-237">Boolean</span></span>|<span data-ttu-id="3c87e-238">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="3c87e-238">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="3c87e-239">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-240">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-240">fingerprintBlocked</span></span>|<span data-ttu-id="3c87e-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-241">Boolean</span></span>|<span data-ttu-id="3c87e-242">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="3c87e-242">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="3c87e-243">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-244">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="3c87e-244">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="3c87e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-245">Boolean</span></span>|<span data-ttu-id="3c87e-246">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="3c87e-246">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="3c87e-247">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-248">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-248">minimumRequiredOsVersion</span></span>|<span data-ttu-id="3c87e-249">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-249">String</span></span>|<span data-ttu-id="3c87e-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="3c87e-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="3c87e-251">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-252">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-252">minimumWarningOsVersion</span></span>|<span data-ttu-id="3c87e-253">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-253">String</span></span>|<span data-ttu-id="3c87e-254">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="3c87e-254">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="3c87e-255">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-256">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-256">minimumRequiredAppVersion</span></span>|<span data-ttu-id="3c87e-257">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-257">String</span></span>|<span data-ttu-id="3c87e-258">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="3c87e-258">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="3c87e-259">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-260">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-260">minimumWarningAppVersion</span></span>|<span data-ttu-id="3c87e-261">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-261">String</span></span>|<span data-ttu-id="3c87e-262">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="3c87e-262">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="3c87e-263">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-264">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3c87e-264">isAssigned</span></span>|<span data-ttu-id="3c87e-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-265">Boolean</span></span>|<span data-ttu-id="3c87e-266">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="3c87e-266">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="3c87e-267">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="3c87e-267">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="3c87e-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3c87e-268">screenCaptureBlocked</span></span>|<span data-ttu-id="3c87e-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-269">Boolean</span></span>|<span data-ttu-id="3c87e-270">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="3c87e-270">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="3c87e-271">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="3c87e-271">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="3c87e-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-272">Boolean</span></span>|<span data-ttu-id="3c87e-273">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="3c87e-273">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="3c87e-274">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="3c87e-274">encryptAppData</span></span>|<span data-ttu-id="3c87e-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c87e-275">Boolean</span></span>|<span data-ttu-id="3c87e-276">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="3c87e-276">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="3c87e-277">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="3c87e-277">deployedAppCount</span></span>|<span data-ttu-id="3c87e-278">Int32</span><span class="sxs-lookup"><span data-stu-id="3c87e-278">Int32</span></span>|<span data-ttu-id="3c87e-279">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="3c87e-279">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="3c87e-280">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-280">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="3c87e-281">字符串</span><span class="sxs-lookup"><span data-stu-id="3c87e-281">String</span></span>|<span data-ttu-id="3c87e-282">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="3c87e-282">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="3c87e-283">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="3c87e-283">minimumWarningPatchVersion</span></span>|<span data-ttu-id="3c87e-284">String</span><span class="sxs-lookup"><span data-stu-id="3c87e-284">String</span></span>|<span data-ttu-id="3c87e-285">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="3c87e-285">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|



## <a name="response"></a><span data-ttu-id="3c87e-286">响应</span><span class="sxs-lookup"><span data-stu-id="3c87e-286">Response</span></span>
<span data-ttu-id="3c87e-287">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c87e-287">If successful, this method returns a `201 Created` response code and a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c87e-288">示例</span><span class="sxs-lookup"><span data-stu-id="3c87e-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c87e-289">请求</span><span class="sxs-lookup"><span data-stu-id="3c87e-289">Request</span></span>
<span data-ttu-id="3c87e-290">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c87e-290">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
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

### <a name="response"></a><span data-ttu-id="3c87e-291">响应</span><span class="sxs-lookup"><span data-stu-id="3c87e-291">Response</span></span>
<span data-ttu-id="3c87e-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c87e-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




