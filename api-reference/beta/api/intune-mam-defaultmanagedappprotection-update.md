---
title: 更新 defaultManagedAppProtection
description: 更新 defaultManagedAppProtection 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 23833af3ecff100e687be9065617fd13b11479bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401423"
---
# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="6471d-103">更新 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="6471d-103">Update defaultManagedAppProtection</span></span>

> <span data-ttu-id="6471d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6471d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6471d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6471d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6471d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6471d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6471d-107">更新 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6471d-107">Update the properties of a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6471d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6471d-108">Prerequisites</span></span>
<span data-ttu-id="6471d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6471d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6471d-111">Permission type</span></span>|<span data-ttu-id="6471d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6471d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6471d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6471d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6471d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6471d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6471d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6471d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6471d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6471d-116">Not supported.</span></span>|
|<span data-ttu-id="6471d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6471d-117">Application</span></span>|<span data-ttu-id="6471d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6471d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6471d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6471d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="6471d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6471d-120">Request headers</span></span>
|<span data-ttu-id="6471d-121">标头</span><span class="sxs-lookup"><span data-stu-id="6471d-121">Header</span></span>|<span data-ttu-id="6471d-122">值</span><span class="sxs-lookup"><span data-stu-id="6471d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6471d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6471d-123">Authorization</span></span>|<span data-ttu-id="6471d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6471d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6471d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6471d-125">Accept</span></span>|<span data-ttu-id="6471d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6471d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6471d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6471d-127">Request body</span></span>
<span data-ttu-id="6471d-128">在请求正文中，提供 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6471d-128">In the request body, supply a JSON representation for the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="6471d-129">下表显示创建 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6471d-129">The following table shows the properties that are required when you create the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

|<span data-ttu-id="6471d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6471d-130">Property</span></span>|<span data-ttu-id="6471d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6471d-131">Type</span></span>|<span data-ttu-id="6471d-132">说明</span><span class="sxs-lookup"><span data-stu-id="6471d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6471d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6471d-133">displayName</span></span>|<span data-ttu-id="6471d-134">String</span><span class="sxs-lookup"><span data-stu-id="6471d-134">String</span></span>|<span data-ttu-id="6471d-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="6471d-135">Policy display name.</span></span> <span data-ttu-id="6471d-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-137">description</span><span class="sxs-lookup"><span data-stu-id="6471d-137">description</span></span>|<span data-ttu-id="6471d-138">String</span><span class="sxs-lookup"><span data-stu-id="6471d-138">String</span></span>|<span data-ttu-id="6471d-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="6471d-139">The policy's description.</span></span> <span data-ttu-id="6471d-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6471d-141">createdDateTime</span></span>|<span data-ttu-id="6471d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6471d-142">DateTimeOffset</span></span>|<span data-ttu-id="6471d-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6471d-143">The date and time the policy was created.</span></span> <span data-ttu-id="6471d-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6471d-145">lastModifiedDateTime</span></span>|<span data-ttu-id="6471d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6471d-146">DateTimeOffset</span></span>|<span data-ttu-id="6471d-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="6471d-147">Last time the policy was modified.</span></span> <span data-ttu-id="6471d-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6471d-149">roleScopeTagIds</span></span>|<span data-ttu-id="6471d-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="6471d-150">String collection</span></span>|<span data-ttu-id="6471d-151">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6471d-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6471d-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-153">id</span><span class="sxs-lookup"><span data-stu-id="6471d-153">id</span></span>|<span data-ttu-id="6471d-154">String</span><span class="sxs-lookup"><span data-stu-id="6471d-154">String</span></span>|<span data-ttu-id="6471d-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6471d-155">Key of the entity.</span></span> <span data-ttu-id="6471d-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-157">version</span><span class="sxs-lookup"><span data-stu-id="6471d-157">version</span></span>|<span data-ttu-id="6471d-158">String</span><span class="sxs-lookup"><span data-stu-id="6471d-158">String</span></span>|<span data-ttu-id="6471d-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6471d-159">Version of the entity.</span></span> <span data-ttu-id="6471d-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6471d-161">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="6471d-161">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="6471d-162">Duration</span><span class="sxs-lookup"><span data-stu-id="6471d-162">Duration</span></span>|<span data-ttu-id="6471d-163">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="6471d-163">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="6471d-164">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-165">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="6471d-165">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="6471d-166">Duration</span><span class="sxs-lookup"><span data-stu-id="6471d-166">Duration</span></span>|<span data-ttu-id="6471d-167">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="6471d-167">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="6471d-168">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-169">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="6471d-169">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="6471d-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="6471d-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="6471d-171">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="6471d-171">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="6471d-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="6471d-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="6471d-174">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="6471d-174">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="6471d-175">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="6471d-175">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="6471d-176">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="6471d-176">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="6471d-177">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-178">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="6471d-178">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="6471d-179">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="6471d-179">organizationalCredentialsRequired</span></span>|<span data-ttu-id="6471d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-180">Boolean</span></span>|<span data-ttu-id="6471d-181">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="6471d-181">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="6471d-182">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-183">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="6471d-183">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="6471d-184">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="6471d-184">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="6471d-185">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="6471d-185">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="6471d-186">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-187">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="6471d-187">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="6471d-188">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-188">dataBackupBlocked</span></span>|<span data-ttu-id="6471d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-189">Boolean</span></span>|<span data-ttu-id="6471d-190">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-190">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="6471d-191">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-192">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="6471d-192">deviceComplianceRequired</span></span>|<span data-ttu-id="6471d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-193">Boolean</span></span>|<span data-ttu-id="6471d-194">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="6471d-194">Indicates whether device compliance is required.</span></span> <span data-ttu-id="6471d-195">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-196">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="6471d-196">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="6471d-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-197">Boolean</span></span>|<span data-ttu-id="6471d-198">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="6471d-198">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="6471d-199">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-200">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-200">saveAsBlocked</span></span>|<span data-ttu-id="6471d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-201">Boolean</span></span>|<span data-ttu-id="6471d-202">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="6471d-202">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="6471d-203">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-204">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="6471d-204">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="6471d-205">Duration</span><span class="sxs-lookup"><span data-stu-id="6471d-205">Duration</span></span>|<span data-ttu-id="6471d-206">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="6471d-206">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="6471d-207">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-208">pinRequired</span><span class="sxs-lookup"><span data-stu-id="6471d-208">pinRequired</span></span>|<span data-ttu-id="6471d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-209">Boolean</span></span>|<span data-ttu-id="6471d-210">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="6471d-210">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="6471d-211">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-212">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="6471d-212">maximumPinRetries</span></span>|<span data-ttu-id="6471d-213">Int32</span><span class="sxs-lookup"><span data-stu-id="6471d-213">Int32</span></span>|<span data-ttu-id="6471d-214">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6471d-214">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="6471d-215">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-216">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-216">simplePinBlocked</span></span>|<span data-ttu-id="6471d-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-217">Boolean</span></span>|<span data-ttu-id="6471d-218">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="6471d-218">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="6471d-219">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-219">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-220">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="6471d-220">minimumPinLength</span></span>|<span data-ttu-id="6471d-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6471d-221">Int32</span></span>|<span data-ttu-id="6471d-222">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-222">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-223">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="6471d-223">pinCharacterSet</span></span>|[<span data-ttu-id="6471d-224">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="6471d-224">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="6471d-225">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="6471d-225">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="6471d-226">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-227">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="6471d-227">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="6471d-228">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="6471d-228">periodBeforePinReset</span></span>|<span data-ttu-id="6471d-229">Duration</span><span class="sxs-lookup"><span data-stu-id="6471d-229">Duration</span></span>|<span data-ttu-id="6471d-230">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="6471d-230">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="6471d-231">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-232">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="6471d-232">allowedDataStorageLocations</span></span>|<span data-ttu-id="6471d-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="6471d-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="6471d-234">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="6471d-234">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="6471d-235">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-236">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="6471d-236">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="6471d-237">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-237">contactSyncBlocked</span></span>|<span data-ttu-id="6471d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-238">Boolean</span></span>|<span data-ttu-id="6471d-239">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="6471d-239">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="6471d-240">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-241">printBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-241">printBlocked</span></span>|<span data-ttu-id="6471d-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-242">Boolean</span></span>|<span data-ttu-id="6471d-243">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="6471d-243">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="6471d-244">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-245">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-245">fingerprintBlocked</span></span>|<span data-ttu-id="6471d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-246">Boolean</span></span>|<span data-ttu-id="6471d-247">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="6471d-247">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="6471d-248">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-249">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="6471d-249">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="6471d-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-250">Boolean</span></span>|<span data-ttu-id="6471d-251">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="6471d-251">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="6471d-252">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-253">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-253">minimumRequiredOsVersion</span></span>|<span data-ttu-id="6471d-254">String</span><span class="sxs-lookup"><span data-stu-id="6471d-254">String</span></span>|<span data-ttu-id="6471d-255">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6471d-256">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-257">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-257">minimumWarningOsVersion</span></span>|<span data-ttu-id="6471d-258">String</span><span class="sxs-lookup"><span data-stu-id="6471d-258">String</span></span>|<span data-ttu-id="6471d-259">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="6471d-259">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="6471d-260">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-261">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-261">minimumRequiredAppVersion</span></span>|<span data-ttu-id="6471d-262">String</span><span class="sxs-lookup"><span data-stu-id="6471d-262">String</span></span>|<span data-ttu-id="6471d-263">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-263">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6471d-264">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-265">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-265">minimumWarningAppVersion</span></span>|<span data-ttu-id="6471d-266">String</span><span class="sxs-lookup"><span data-stu-id="6471d-266">String</span></span>|<span data-ttu-id="6471d-267">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="6471d-267">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="6471d-268">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-269">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-269">minimumWipeOsVersion</span></span>|<span data-ttu-id="6471d-270">String</span><span class="sxs-lookup"><span data-stu-id="6471d-270">String</span></span>|<span data-ttu-id="6471d-271">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="6471d-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="6471d-272">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-273">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-273">minimumWipeAppVersion</span></span>|<span data-ttu-id="6471d-274">String</span><span class="sxs-lookup"><span data-stu-id="6471d-274">String</span></span>|<span data-ttu-id="6471d-275">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="6471d-275">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="6471d-276">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6471d-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-277">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="6471d-277">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="6471d-278">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="6471d-278">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="6471d-279">定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="6471d-279">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="6471d-280">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-280">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-281">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="6471d-281">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="6471d-282">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="6471d-282">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="6471d-283">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="6471d-283">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="6471d-284">定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。</span><span class="sxs-lookup"><span data-stu-id="6471d-284">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="6471d-285">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="6471d-285">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6471d-286">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="6471d-286">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="6471d-287">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="6471d-287">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="6471d-288">持续时间</span><span class="sxs-lookup"><span data-stu-id="6471d-288">Duration</span></span>|<span data-ttu-id="6471d-289">以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时</span><span class="sxs-lookup"><span data-stu-id="6471d-289">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6471d-290">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="6471d-290">appDataEncryptionType</span></span>|[<span data-ttu-id="6471d-291">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="6471d-291">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="6471d-292">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="6471d-292">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="6471d-293">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="6471d-293">(iOS Only).</span></span> <span data-ttu-id="6471d-294">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="6471d-294">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="6471d-295">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-295">screenCaptureBlocked</span></span>|<span data-ttu-id="6471d-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-296">Boolean</span></span>|<span data-ttu-id="6471d-297">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="6471d-297">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="6471d-298">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-298">(Android only)</span></span>|
|<span data-ttu-id="6471d-299">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="6471d-299">encryptAppData</span></span>|<span data-ttu-id="6471d-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-300">Boolean</span></span>|<span data-ttu-id="6471d-301">指示是否应加密托管应用数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-301">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="6471d-302">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-302">(Android only)</span></span>|
|<span data-ttu-id="6471d-303">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="6471d-303">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="6471d-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-304">Boolean</span></span>|<span data-ttu-id="6471d-305">启用此设置后，如果启用设备加密，则禁用应用程序级别的加密。</span><span class="sxs-lookup"><span data-stu-id="6471d-305">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="6471d-306">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-306">(Android only)</span></span>|
|<span data-ttu-id="6471d-307">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-307">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="6471d-308">String</span><span class="sxs-lookup"><span data-stu-id="6471d-308">String</span></span>|<span data-ttu-id="6471d-309">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-309">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6471d-310">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-310">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-311">customSettings</span><span class="sxs-lookup"><span data-stu-id="6471d-311">customSettings</span></span>|<span data-ttu-id="6471d-312">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6471d-312">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6471d-313">要发送给受影响用户的一组字符串键和字符串值对，不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="6471d-313">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="6471d-314">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="6471d-314">deployedAppCount</span></span>|<span data-ttu-id="6471d-315">Int32</span><span class="sxs-lookup"><span data-stu-id="6471d-315">Int32</span></span>|<span data-ttu-id="6471d-316">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="6471d-316">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="6471d-317">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-317">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="6471d-318">String</span><span class="sxs-lookup"><span data-stu-id="6471d-318">String</span></span>|<span data-ttu-id="6471d-319">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="6471d-319">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="6471d-320">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-320">(Android only)</span></span>|
|<span data-ttu-id="6471d-321">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-321">minimumWarningPatchVersion</span></span>|<span data-ttu-id="6471d-322">String</span><span class="sxs-lookup"><span data-stu-id="6471d-322">String</span></span>|<span data-ttu-id="6471d-323">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="6471d-323">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="6471d-324">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-324">(Android only)</span></span>|
|<span data-ttu-id="6471d-325">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="6471d-325">exemptedAppProtocols</span></span>|<span data-ttu-id="6471d-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6471d-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6471d-327">此列表中的 iOS 应用程序将从策略中排除和都将能够从托管的应用程序接收数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-327">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="6471d-328">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-328">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-329">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="6471d-329">exemptedAppPackages</span></span>|<span data-ttu-id="6471d-330">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6471d-330">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6471d-331">此列表中的 android 应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-331">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="6471d-332">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-332">(Android only)</span></span>|
|<span data-ttu-id="6471d-333">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-333">faceIdBlocked</span></span>|<span data-ttu-id="6471d-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-334">Boolean</span></span>|<span data-ttu-id="6471d-335">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 pin。</span><span class="sxs-lookup"><span data-stu-id="6471d-335">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="6471d-336">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-336">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-337">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-337">minimumWipeSdkVersion</span></span>|<span data-ttu-id="6471d-338">String</span><span class="sxs-lookup"><span data-stu-id="6471d-338">String</span></span>|<span data-ttu-id="6471d-339">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-339">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="6471d-340">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="6471d-340">minimumWipePatchVersion</span></span>|<span data-ttu-id="6471d-341">String</span><span class="sxs-lookup"><span data-stu-id="6471d-341">String</span></span>|<span data-ttu-id="6471d-342">托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。</span><span class="sxs-lookup"><span data-stu-id="6471d-342">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="6471d-343">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-343">(Android only)</span></span>|
|<span data-ttu-id="6471d-344">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="6471d-344">allowedIosDeviceModels</span></span>|<span data-ttu-id="6471d-345">String</span><span class="sxs-lookup"><span data-stu-id="6471d-345">String</span></span>|<span data-ttu-id="6471d-346">作为字符串的托管的应用程序，以允许的设备模型的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="6471d-346">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="6471d-347">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-347">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-348">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="6471d-348">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="6471d-349">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="6471d-349">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="6471d-350">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备模型。</span><span class="sxs-lookup"><span data-stu-id="6471d-350">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="6471d-351">(仅 iOS)。</span><span class="sxs-lookup"><span data-stu-id="6471d-351">(iOS Only).</span></span> <span data-ttu-id="6471d-352">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="6471d-352">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="6471d-353">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="6471d-353">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="6471d-354">String</span><span class="sxs-lookup"><span data-stu-id="6471d-354">String</span></span>|<span data-ttu-id="6471d-355">作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="6471d-355">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="6471d-356">（仅限 Android）</span><span class="sxs-lookup"><span data-stu-id="6471d-356">(Android only)</span></span>|
|<span data-ttu-id="6471d-357">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="6471d-357">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="6471d-358">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="6471d-358">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="6471d-359">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。</span><span class="sxs-lookup"><span data-stu-id="6471d-359">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="6471d-360">(仅 android)。</span><span class="sxs-lookup"><span data-stu-id="6471d-360">(Android only).</span></span> <span data-ttu-id="6471d-361">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="6471d-361">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="6471d-362">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="6471d-362">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="6471d-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-363">Boolean</span></span>|<span data-ttu-id="6471d-364">如果第三方键盘允许访问托管的应用程序时，定义。</span><span class="sxs-lookup"><span data-stu-id="6471d-364">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="6471d-365">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-365">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-366">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="6471d-366">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="6471d-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-367">Boolean</span></span>|<span data-ttu-id="6471d-368">如果到所选的文件共享位置从托管的应用程序支持打开项操作，定义。</span><span class="sxs-lookup"><span data-stu-id="6471d-368">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="6471d-369">此设置仅适用于 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 并且 DisableProtectionOfManagedOutboundOpenInData 设置为 False。</span><span class="sxs-lookup"><span data-stu-id="6471d-369">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="6471d-370">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-370">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-371">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="6471d-371">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="6471d-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-372">Boolean</span></span>|<span data-ttu-id="6471d-373">禁用传输到 IOS OpenIn 选项通过其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="6471d-373">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="6471d-374">此设置只允许为 True 时 AllowedOutboundDataTransferDestinations 设置为 ManagedApps。</span><span class="sxs-lookup"><span data-stu-id="6471d-374">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="6471d-375">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-375">(iOS Only)</span></span>|
|<span data-ttu-id="6471d-376">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6471d-376">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="6471d-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471d-377">Boolean</span></span>|<span data-ttu-id="6471d-378">从未知源保护传入的数据。</span><span class="sxs-lookup"><span data-stu-id="6471d-378">Protect incoming data from unknown source.</span></span> <span data-ttu-id="6471d-379">此设置只允许为 True 时 AllowedInboundDataTransferSources 设置为 AllApps。</span><span class="sxs-lookup"><span data-stu-id="6471d-379">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="6471d-380">(仅适用于 iOS)</span><span class="sxs-lookup"><span data-stu-id="6471d-380">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="6471d-381">响应</span><span class="sxs-lookup"><span data-stu-id="6471d-381">Response</span></span>
<span data-ttu-id="6471d-382">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6471d-382">If successful, this method returns a `200 OK` response code and an updated [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6471d-383">示例</span><span class="sxs-lookup"><span data-stu-id="6471d-383">Example</span></span>

### <a name="request"></a><span data-ttu-id="6471d-384">请求</span><span class="sxs-lookup"><span data-stu-id="6471d-384">Request</span></span>
<span data-ttu-id="6471d-385">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6471d-385">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 3217

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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

### <a name="response"></a><span data-ttu-id="6471d-386">响应</span><span class="sxs-lookup"><span data-stu-id="6471d-386">Response</span></span>
<span data-ttu-id="6471d-p158">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6471d-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3389

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




