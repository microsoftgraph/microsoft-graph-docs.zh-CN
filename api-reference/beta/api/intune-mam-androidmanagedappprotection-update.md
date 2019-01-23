---
title: 更新 androidManagedAppProtection
description: 更新 androidManagedAppProtection 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b405c114cf0a6c70f5f6bc0312158d2b231bf7b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412434"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="a335b-103">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a335b-103">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="a335b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a335b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a335b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a335b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a335b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a335b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a335b-107">更新 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a335b-107">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a335b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a335b-108">Prerequisites</span></span>
<span data-ttu-id="a335b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a335b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a335b-111">Permission type</span></span>|<span data-ttu-id="a335b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a335b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a335b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a335b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a335b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a335b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a335b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a335b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a335b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a335b-116">Not supported.</span></span>|
|<span data-ttu-id="a335b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a335b-117">Application</span></span>|<span data-ttu-id="a335b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a335b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a335b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a335b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="a335b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a335b-120">Request headers</span></span>
|<span data-ttu-id="a335b-121">标头</span><span class="sxs-lookup"><span data-stu-id="a335b-121">Header</span></span>|<span data-ttu-id="a335b-122">值</span><span class="sxs-lookup"><span data-stu-id="a335b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a335b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a335b-123">Authorization</span></span>|<span data-ttu-id="a335b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a335b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a335b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a335b-125">Accept</span></span>|<span data-ttu-id="a335b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a335b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a335b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a335b-127">Request body</span></span>
<span data-ttu-id="a335b-128">在请求正文中，提供 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a335b-128">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="a335b-129">下表显示了创建 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a335b-129">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="a335b-130">属性</span><span class="sxs-lookup"><span data-stu-id="a335b-130">Property</span></span>|<span data-ttu-id="a335b-131">类型</span><span class="sxs-lookup"><span data-stu-id="a335b-131">Type</span></span>|<span data-ttu-id="a335b-132">说明</span><span class="sxs-lookup"><span data-stu-id="a335b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a335b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a335b-133">displayName</span></span>|<span data-ttu-id="a335b-134">String</span><span class="sxs-lookup"><span data-stu-id="a335b-134">String</span></span>|<span data-ttu-id="a335b-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a335b-135">Policy display name.</span></span> <span data-ttu-id="a335b-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-137">description</span><span class="sxs-lookup"><span data-stu-id="a335b-137">description</span></span>|<span data-ttu-id="a335b-138">String</span><span class="sxs-lookup"><span data-stu-id="a335b-138">String</span></span>|<span data-ttu-id="a335b-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a335b-139">The policy's description.</span></span> <span data-ttu-id="a335b-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a335b-141">createdDateTime</span></span>|<span data-ttu-id="a335b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a335b-142">DateTimeOffset</span></span>|<span data-ttu-id="a335b-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a335b-143">The date and time the policy was created.</span></span> <span data-ttu-id="a335b-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a335b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="a335b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a335b-146">DateTimeOffset</span></span>|<span data-ttu-id="a335b-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="a335b-147">Last time the policy was modified.</span></span> <span data-ttu-id="a335b-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a335b-149">roleScopeTagIds</span></span>|<span data-ttu-id="a335b-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="a335b-150">String collection</span></span>|<span data-ttu-id="a335b-151">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a335b-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a335b-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-153">id</span><span class="sxs-lookup"><span data-stu-id="a335b-153">id</span></span>|<span data-ttu-id="a335b-154">String</span><span class="sxs-lookup"><span data-stu-id="a335b-154">String</span></span>|<span data-ttu-id="a335b-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a335b-155">Key of the entity.</span></span> <span data-ttu-id="a335b-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-157">version</span><span class="sxs-lookup"><span data-stu-id="a335b-157">version</span></span>|<span data-ttu-id="a335b-158">String</span><span class="sxs-lookup"><span data-stu-id="a335b-158">String</span></span>|<span data-ttu-id="a335b-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a335b-159">Version of the entity.</span></span> <span data-ttu-id="a335b-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a335b-161">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="a335b-161">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="a335b-162">Duration</span><span class="sxs-lookup"><span data-stu-id="a335b-162">Duration</span></span>|<span data-ttu-id="a335b-163">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="a335b-163">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="a335b-164">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-165">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="a335b-165">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="a335b-166">Duration</span><span class="sxs-lookup"><span data-stu-id="a335b-166">Duration</span></span>|<span data-ttu-id="a335b-167">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="a335b-167">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="a335b-168">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-169">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="a335b-169">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="a335b-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="a335b-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="a335b-171">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="a335b-171">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="a335b-172">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-173">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="a335b-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="a335b-174">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="a335b-174">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="a335b-175">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="a335b-175">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="a335b-176">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="a335b-176">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="a335b-177">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-178">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="a335b-178">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="a335b-179">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="a335b-179">organizationalCredentialsRequired</span></span>|<span data-ttu-id="a335b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-180">Boolean</span></span>|<span data-ttu-id="a335b-181">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="a335b-181">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="a335b-182">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-183">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="a335b-183">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="a335b-184">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="a335b-184">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="a335b-185">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="a335b-185">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="a335b-186">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-187">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a335b-187">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="a335b-188">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-188">dataBackupBlocked</span></span>|<span data-ttu-id="a335b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-189">Boolean</span></span>|<span data-ttu-id="a335b-190">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="a335b-190">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="a335b-191">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-192">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="a335b-192">deviceComplianceRequired</span></span>|<span data-ttu-id="a335b-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-193">Boolean</span></span>|<span data-ttu-id="a335b-194">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="a335b-194">Indicates whether device compliance is required.</span></span> <span data-ttu-id="a335b-195">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-196">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="a335b-196">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="a335b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-197">Boolean</span></span>|<span data-ttu-id="a335b-198">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="a335b-198">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="a335b-199">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-200">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-200">saveAsBlocked</span></span>|<span data-ttu-id="a335b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-201">Boolean</span></span>|<span data-ttu-id="a335b-202">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="a335b-202">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="a335b-203">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-204">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="a335b-204">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="a335b-205">Duration</span><span class="sxs-lookup"><span data-stu-id="a335b-205">Duration</span></span>|<span data-ttu-id="a335b-206">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="a335b-206">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="a335b-207">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-208">pinRequired</span><span class="sxs-lookup"><span data-stu-id="a335b-208">pinRequired</span></span>|<span data-ttu-id="a335b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-209">Boolean</span></span>|<span data-ttu-id="a335b-210">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="a335b-210">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="a335b-211">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-212">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="a335b-212">maximumPinRetries</span></span>|<span data-ttu-id="a335b-213">Int32</span><span class="sxs-lookup"><span data-stu-id="a335b-213">Int32</span></span>|<span data-ttu-id="a335b-214">最大不正确的 pin 重试次数之前阻止或之前托管的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a335b-214">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="a335b-215">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-216">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-216">simplePinBlocked</span></span>|<span data-ttu-id="a335b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-217">Boolean</span></span>|<span data-ttu-id="a335b-218">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="a335b-218">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="a335b-219">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-219">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-220">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="a335b-220">minimumPinLength</span></span>|<span data-ttu-id="a335b-221">Int32</span><span class="sxs-lookup"><span data-stu-id="a335b-221">Int32</span></span>|<span data-ttu-id="a335b-222">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-222">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-223">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="a335b-223">pinCharacterSet</span></span>|[<span data-ttu-id="a335b-224">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="a335b-224">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="a335b-225">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="a335b-225">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="a335b-226">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-227">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="a335b-227">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="a335b-228">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="a335b-228">periodBeforePinReset</span></span>|<span data-ttu-id="a335b-229">Duration</span><span class="sxs-lookup"><span data-stu-id="a335b-229">Duration</span></span>|<span data-ttu-id="a335b-230">PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
</span><span class="sxs-lookup"><span data-stu-id="a335b-230">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="a335b-231">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-232">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="a335b-232">allowedDataStorageLocations</span></span>|<span data-ttu-id="a335b-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)集合</span><span class="sxs-lookup"><span data-stu-id="a335b-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="a335b-234">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="a335b-234">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="a335b-235">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-236">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="a335b-236">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="a335b-237">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-237">contactSyncBlocked</span></span>|<span data-ttu-id="a335b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-238">Boolean</span></span>|<span data-ttu-id="a335b-239">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="a335b-239">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="a335b-240">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-241">printBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-241">printBlocked</span></span>|<span data-ttu-id="a335b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-242">Boolean</span></span>|<span data-ttu-id="a335b-243">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="a335b-243">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="a335b-244">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-245">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-245">fingerprintBlocked</span></span>|<span data-ttu-id="a335b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-246">Boolean</span></span>|<span data-ttu-id="a335b-247">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="a335b-247">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="a335b-248">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-249">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="a335b-249">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="a335b-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-250">Boolean</span></span>|<span data-ttu-id="a335b-251">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="a335b-251">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="a335b-252">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-253">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-253">minimumRequiredOsVersion</span></span>|<span data-ttu-id="a335b-254">String</span><span class="sxs-lookup"><span data-stu-id="a335b-254">String</span></span>|<span data-ttu-id="a335b-255">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="a335b-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="a335b-256">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-257">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-257">minimumWarningOsVersion</span></span>|<span data-ttu-id="a335b-258">String</span><span class="sxs-lookup"><span data-stu-id="a335b-258">String</span></span>|<span data-ttu-id="a335b-259">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="a335b-259">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="a335b-260">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-261">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-261">minimumRequiredAppVersion</span></span>|<span data-ttu-id="a335b-262">String</span><span class="sxs-lookup"><span data-stu-id="a335b-262">String</span></span>|<span data-ttu-id="a335b-263">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="a335b-263">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="a335b-264">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-265">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-265">minimumWarningAppVersion</span></span>|<span data-ttu-id="a335b-266">String</span><span class="sxs-lookup"><span data-stu-id="a335b-266">String</span></span>|<span data-ttu-id="a335b-267">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="a335b-267">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="a335b-268">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-269">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-269">minimumWipeOsVersion</span></span>|<span data-ttu-id="a335b-270">String</span><span class="sxs-lookup"><span data-stu-id="a335b-270">String</span></span>|<span data-ttu-id="a335b-271">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="a335b-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="a335b-272">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-273">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-273">minimumWipeAppVersion</span></span>|<span data-ttu-id="a335b-274">String</span><span class="sxs-lookup"><span data-stu-id="a335b-274">String</span></span>|<span data-ttu-id="a335b-275">小于或等于指定的版本将擦除托管应用程序和关联的公司数据的版本。</span><span class="sxs-lookup"><span data-stu-id="a335b-275">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="a335b-276">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-277">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="a335b-277">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="a335b-278">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="a335b-278">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="a335b-279">定义托管的应用程序行为，阻止或擦除时也根设备, 或 jailbroken，如果 DeviceComplianceRequired 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="a335b-279">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="a335b-280">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-280">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-281">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="a335b-281">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="a335b-282">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="a335b-282">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="a335b-283">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="a335b-283">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="a335b-284">定义托管的应用程序行为，或者是阻止或擦除，基于最大数量的不正确的 pin 重试次数。</span><span class="sxs-lookup"><span data-stu-id="a335b-284">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="a335b-285">继承自[managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="a335b-285">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="a335b-286">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="a335b-286">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="a335b-287">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="a335b-287">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="a335b-288">持续时间</span><span class="sxs-lookup"><span data-stu-id="a335b-288">Duration</span></span>|<span data-ttu-id="a335b-289">以分钟为单位的而不是从[managedAppProtection](../resources/intune-mam-managedappprotection.md)非生物密码继承应用程序 pin 超时</span><span class="sxs-lookup"><span data-stu-id="a335b-289">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-290">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a335b-290">isAssigned</span></span>|<span data-ttu-id="a335b-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-291">Boolean</span></span>|<span data-ttu-id="a335b-292">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="a335b-292">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a335b-293">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a335b-293">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="a335b-294">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="a335b-294">targetedAppManagementLevels</span></span>|[<span data-ttu-id="a335b-295">appManagementLevel</span><span class="sxs-lookup"><span data-stu-id="a335b-295">appManagementLevel</span></span>](../resources/intune-mam-appmanagementlevel.md)|<span data-ttu-id="a335b-296">从[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)此策略继承目标应用程序管理级别。</span><span class="sxs-lookup"><span data-stu-id="a335b-296">The intended app management levels for this policy Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span></span> <span data-ttu-id="a335b-297">可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="a335b-297">Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.</span></span>|
|<span data-ttu-id="a335b-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a335b-298">screenCaptureBlocked</span></span>|<span data-ttu-id="a335b-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-299">Boolean</span></span>|<span data-ttu-id="a335b-300">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="a335b-300">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="a335b-301">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="a335b-301">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="a335b-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-302">Boolean</span></span>|<span data-ttu-id="a335b-303">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="a335b-303">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="a335b-304">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="a335b-304">encryptAppData</span></span>|<span data-ttu-id="a335b-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="a335b-305">Boolean</span></span>|<span data-ttu-id="a335b-306">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="a335b-306">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="a335b-307">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="a335b-307">deployedAppCount</span></span>|<span data-ttu-id="a335b-308">Int32</span><span class="sxs-lookup"><span data-stu-id="a335b-308">Int32</span></span>|<span data-ttu-id="a335b-309">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="a335b-309">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="a335b-310">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-310">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="a335b-311">String</span><span class="sxs-lookup"><span data-stu-id="a335b-311">String</span></span>|<span data-ttu-id="a335b-312">定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
</span><span class="sxs-lookup"><span data-stu-id="a335b-312">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="a335b-313">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-313">minimumWarningPatchVersion</span></span>|<span data-ttu-id="a335b-314">String</span><span class="sxs-lookup"><span data-stu-id="a335b-314">String</span></span>|<span data-ttu-id="a335b-315">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="a335b-315">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|
|<span data-ttu-id="a335b-316">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="a335b-316">exemptedAppPackages</span></span>|<span data-ttu-id="a335b-317">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a335b-317">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a335b-318">此列表中的应用程序包将从策略中排除并且能够接收从托管的应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="a335b-318">App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span>|
|<span data-ttu-id="a335b-319">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="a335b-319">minimumWipePatchVersion</span></span>|<span data-ttu-id="a335b-320">String</span><span class="sxs-lookup"><span data-stu-id="a335b-320">String</span></span>|<span data-ttu-id="a335b-321">托管的应用程序和关联的公司数据，将擦除 android 安全修补程序级别小于或等于指定值。</span><span class="sxs-lookup"><span data-stu-id="a335b-321">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span>|
|<span data-ttu-id="a335b-322">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="a335b-322">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="a335b-323">String</span><span class="sxs-lookup"><span data-stu-id="a335b-323">String</span></span>|<span data-ttu-id="a335b-324">作为字符串的托管的应用程序，以允许的设备制造商的分号分隔列表。</span><span class="sxs-lookup"><span data-stu-id="a335b-324">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span>|
|<span data-ttu-id="a335b-325">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="a335b-325">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="a335b-326">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="a335b-326">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="a335b-327">定义托管的应用程序行为，阻止或擦除，如果不允许指定的设备制造商。</span><span class="sxs-lookup"><span data-stu-id="a335b-327">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="a335b-328">可取值为：`block`、`wipe`。</span><span class="sxs-lookup"><span data-stu-id="a335b-328">Possible values are: `block`, `wipe`.</span></span>|



## <a name="response"></a><span data-ttu-id="a335b-329">响应</span><span class="sxs-lookup"><span data-stu-id="a335b-329">Response</span></span>
<span data-ttu-id="a335b-330">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a335b-330">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a335b-331">示例</span><span class="sxs-lookup"><span data-stu-id="a335b-331">Example</span></span>

### <a name="request"></a><span data-ttu-id="a335b-332">请求</span><span class="sxs-lookup"><span data-stu-id="a335b-332">Request</span></span>
<span data-ttu-id="a335b-333">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a335b-333">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a335b-334">响应</span><span class="sxs-lookup"><span data-stu-id="a335b-334">Response</span></span>
<span data-ttu-id="a335b-p142">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a335b-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




