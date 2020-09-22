---
title: 创建 iosManagedAppProtection
description: 创建新的 iosManagedAppProtection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ec4434824482ffc8719545d647db10fb8900c36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031954"
---
# <a name="create-iosmanagedappprotection"></a><span data-ttu-id="f820a-103">创建 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="f820a-103">Create iosManagedAppProtection</span></span>

<span data-ttu-id="f820a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f820a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f820a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f820a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f820a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f820a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f820a-107">创建新的 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f820a-107">Create a new [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f820a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f820a-108">Prerequisites</span></span>
<span data-ttu-id="f820a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f820a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f820a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f820a-111">Permission type</span></span>|<span data-ttu-id="f820a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f820a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f820a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f820a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f820a-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f820a-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f820a-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f820a-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f820a-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f820a-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f820a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f820a-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f820a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f820a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f820a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f820a-119">Not supported.</span></span>|
|<span data-ttu-id="f820a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f820a-120">Application</span></span>||
| <span data-ttu-id="f820a-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f820a-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f820a-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f820a-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f820a-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f820a-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f820a-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f820a-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f820a-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f820a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="f820a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f820a-126">Request headers</span></span>
|<span data-ttu-id="f820a-127">标头</span><span class="sxs-lookup"><span data-stu-id="f820a-127">Header</span></span>|<span data-ttu-id="f820a-128">值</span><span class="sxs-lookup"><span data-stu-id="f820a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f820a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f820a-129">Authorization</span></span>|<span data-ttu-id="f820a-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f820a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f820a-131">接受</span><span class="sxs-lookup"><span data-stu-id="f820a-131">Accept</span></span>|<span data-ttu-id="f820a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f820a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f820a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f820a-133">Request body</span></span>
<span data-ttu-id="f820a-134">在请求正文中，提供 iosManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f820a-134">In the request body, supply a JSON representation for the iosManagedAppProtection object.</span></span>

<span data-ttu-id="f820a-135">下表显示创建 iosManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f820a-135">The following table shows the properties that are required when you create the iosManagedAppProtection.</span></span>

|<span data-ttu-id="f820a-136">属性</span><span class="sxs-lookup"><span data-stu-id="f820a-136">Property</span></span>|<span data-ttu-id="f820a-137">类型</span><span class="sxs-lookup"><span data-stu-id="f820a-137">Type</span></span>|<span data-ttu-id="f820a-138">说明</span><span class="sxs-lookup"><span data-stu-id="f820a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f820a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f820a-139">displayName</span></span>|<span data-ttu-id="f820a-140">String</span><span class="sxs-lookup"><span data-stu-id="f820a-140">String</span></span>|<span data-ttu-id="f820a-141">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="f820a-141">Policy display name.</span></span> <span data-ttu-id="f820a-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-143">description</span><span class="sxs-lookup"><span data-stu-id="f820a-143">description</span></span>|<span data-ttu-id="f820a-144">String</span><span class="sxs-lookup"><span data-stu-id="f820a-144">String</span></span>|<span data-ttu-id="f820a-145">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="f820a-145">The policy's description.</span></span> <span data-ttu-id="f820a-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f820a-147">createdDateTime</span></span>|<span data-ttu-id="f820a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f820a-148">DateTimeOffset</span></span>|<span data-ttu-id="f820a-149">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f820a-149">The date and time the policy was created.</span></span> <span data-ttu-id="f820a-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f820a-151">lastModifiedDateTime</span></span>|<span data-ttu-id="f820a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f820a-152">DateTimeOffset</span></span>|<span data-ttu-id="f820a-153">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="f820a-153">Last time the policy was modified.</span></span> <span data-ttu-id="f820a-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f820a-155">roleScopeTagIds</span></span>|<span data-ttu-id="f820a-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="f820a-156">String collection</span></span>|<span data-ttu-id="f820a-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f820a-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f820a-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-159">id</span><span class="sxs-lookup"><span data-stu-id="f820a-159">id</span></span>|<span data-ttu-id="f820a-160">String</span><span class="sxs-lookup"><span data-stu-id="f820a-160">String</span></span>|<span data-ttu-id="f820a-161">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f820a-161">Key of the entity.</span></span> <span data-ttu-id="f820a-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-163">version</span><span class="sxs-lookup"><span data-stu-id="f820a-163">version</span></span>|<span data-ttu-id="f820a-164">String</span><span class="sxs-lookup"><span data-stu-id="f820a-164">String</span></span>|<span data-ttu-id="f820a-165">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f820a-165">Version of the entity.</span></span> <span data-ttu-id="f820a-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f820a-167">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="f820a-167">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="f820a-168">Duration</span><span class="sxs-lookup"><span data-stu-id="f820a-168">Duration</span></span>|<span data-ttu-id="f820a-169">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="f820a-169">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="f820a-170">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-170">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-171">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="f820a-171">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="f820a-172">Duration</span><span class="sxs-lookup"><span data-stu-id="f820a-172">Duration</span></span>|<span data-ttu-id="f820a-173">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="f820a-173">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="f820a-174">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-174">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-175">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="f820a-175">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="f820a-176">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="f820a-176">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="f820a-177">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="f820a-177">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="f820a-178">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-178">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-179">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="f820a-179">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="f820a-180">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="f820a-180">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="f820a-181">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="f820a-181">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="f820a-182">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="f820a-182">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="f820a-183">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-183">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-184">可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="f820a-184">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="f820a-185">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="f820a-185">organizationalCredentialsRequired</span></span>|<span data-ttu-id="f820a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-186">Boolean</span></span>|<span data-ttu-id="f820a-187">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="f820a-187">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="f820a-188">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-188">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-189">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="f820a-189">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="f820a-190">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="f820a-190">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="f820a-191">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="f820a-191">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="f820a-192">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-192">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-193">可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="f820a-193">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="f820a-194">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-194">dataBackupBlocked</span></span>|<span data-ttu-id="f820a-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-195">Boolean</span></span>|<span data-ttu-id="f820a-196">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-196">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="f820a-197">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-198">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="f820a-198">deviceComplianceRequired</span></span>|<span data-ttu-id="f820a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-199">Boolean</span></span>|<span data-ttu-id="f820a-200">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="f820a-200">Indicates whether device compliance is required.</span></span> <span data-ttu-id="f820a-201">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-202">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="f820a-202">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="f820a-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-203">Boolean</span></span>|<span data-ttu-id="f820a-204">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="f820a-204">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="f820a-205">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-206">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-206">saveAsBlocked</span></span>|<span data-ttu-id="f820a-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-207">Boolean</span></span>|<span data-ttu-id="f820a-208">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="f820a-208">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="f820a-209">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-210">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="f820a-210">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="f820a-211">Duration</span><span class="sxs-lookup"><span data-stu-id="f820a-211">Duration</span></span>|<span data-ttu-id="f820a-212">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="f820a-212">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="f820a-213">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-214">pinRequired</span><span class="sxs-lookup"><span data-stu-id="f820a-214">pinRequired</span></span>|<span data-ttu-id="f820a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-215">Boolean</span></span>|<span data-ttu-id="f820a-216">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="f820a-216">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="f820a-217">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-217">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-218">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="f820a-218">maximumPinRetries</span></span>|<span data-ttu-id="f820a-219">Int32</span><span class="sxs-lookup"><span data-stu-id="f820a-219">Int32</span></span>|<span data-ttu-id="f820a-220">在阻止或擦除托管应用之前，不正确 pin 重试的最大次数。</span><span class="sxs-lookup"><span data-stu-id="f820a-220">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="f820a-221">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-221">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-222">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-222">simplePinBlocked</span></span>|<span data-ttu-id="f820a-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-223">Boolean</span></span>|<span data-ttu-id="f820a-224">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="f820a-224">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="f820a-225">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-226">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="f820a-226">minimumPinLength</span></span>|<span data-ttu-id="f820a-227">Int32</span><span class="sxs-lookup"><span data-stu-id="f820a-227">Int32</span></span>|<span data-ttu-id="f820a-228">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-228">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-229">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="f820a-229">pinCharacterSet</span></span>|[<span data-ttu-id="f820a-230">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="f820a-230">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="f820a-231">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="f820a-231">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="f820a-232">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-232">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-233">可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="f820a-233">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="f820a-234">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="f820a-234">periodBeforePinReset</span></span>|<span data-ttu-id="f820a-235">Duration</span><span class="sxs-lookup"><span data-stu-id="f820a-235">Duration</span></span>|<span data-ttu-id="f820a-236">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="f820a-236">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="f820a-237">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-237">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-238">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="f820a-238">allowedDataStorageLocations</span></span>|<span data-ttu-id="f820a-239">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f820a-239">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="f820a-240">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="f820a-240">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="f820a-241">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-241">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-242">可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="f820a-242">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="f820a-243">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-243">contactSyncBlocked</span></span>|<span data-ttu-id="f820a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-244">Boolean</span></span>|<span data-ttu-id="f820a-245">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="f820a-245">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="f820a-246">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-247">printBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-247">printBlocked</span></span>|<span data-ttu-id="f820a-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-248">Boolean</span></span>|<span data-ttu-id="f820a-249">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="f820a-249">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="f820a-250">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-251">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-251">fingerprintBlocked</span></span>|<span data-ttu-id="f820a-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-252">Boolean</span></span>|<span data-ttu-id="f820a-253">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="f820a-253">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="f820a-254">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-255">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="f820a-255">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="f820a-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-256">Boolean</span></span>|<span data-ttu-id="f820a-257">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="f820a-257">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="f820a-258">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-259">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-259">minimumRequiredOsVersion</span></span>|<span data-ttu-id="f820a-260">String</span><span class="sxs-lookup"><span data-stu-id="f820a-260">String</span></span>|<span data-ttu-id="f820a-261">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-261">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="f820a-262">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-263">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-263">minimumWarningOsVersion</span></span>|<span data-ttu-id="f820a-264">String</span><span class="sxs-lookup"><span data-stu-id="f820a-264">String</span></span>|<span data-ttu-id="f820a-265">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="f820a-265">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="f820a-266">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-266">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-267">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-267">minimumRequiredAppVersion</span></span>|<span data-ttu-id="f820a-268">String</span><span class="sxs-lookup"><span data-stu-id="f820a-268">String</span></span>|<span data-ttu-id="f820a-269">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-269">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="f820a-270">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-270">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-271">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-271">minimumWarningAppVersion</span></span>|<span data-ttu-id="f820a-272">String</span><span class="sxs-lookup"><span data-stu-id="f820a-272">String</span></span>|<span data-ttu-id="f820a-273">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="f820a-273">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="f820a-274">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-274">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-275">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-275">minimumWipeOsVersion</span></span>|<span data-ttu-id="f820a-276">String</span><span class="sxs-lookup"><span data-stu-id="f820a-276">String</span></span>|<span data-ttu-id="f820a-277">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-277">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="f820a-278">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-278">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-279">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-279">minimumWipeAppVersion</span></span>|<span data-ttu-id="f820a-280">String</span><span class="sxs-lookup"><span data-stu-id="f820a-280">String</span></span>|<span data-ttu-id="f820a-281">小于或等于指定版本的版本将擦除托管应用和关联的公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-281">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="f820a-282">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-282">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-283">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="f820a-283">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="f820a-284">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="f820a-284">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="f820a-285">如果将 DeviceComplianceRequired 设置为 true，则定义在设备为根或已越狱时的托管应用行为（阻止或擦除）。</span><span class="sxs-lookup"><span data-stu-id="f820a-285">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="f820a-286">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-286">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-287">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="f820a-287">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="f820a-288">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="f820a-288">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="f820a-289">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="f820a-289">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="f820a-290">根据最大错误 pin 重试次数定义托管应用行为，即阻止或擦除。</span><span class="sxs-lookup"><span data-stu-id="f820a-290">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="f820a-291">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)。</span><span class="sxs-lookup"><span data-stu-id="f820a-291">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-292">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="f820a-292">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="f820a-293">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="f820a-293">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="f820a-294">持续时间</span><span class="sxs-lookup"><span data-stu-id="f820a-294">Duration</span></span>|<span data-ttu-id="f820a-295">以分钟为单位的应用程序 pin （而不是从[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的无生物特征密码）超时</span><span class="sxs-lookup"><span data-stu-id="f820a-295">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-296">allowedOutboundClipboardSharingExceptionLength</span><span class="sxs-lookup"><span data-stu-id="f820a-296">allowedOutboundClipboardSharingExceptionLength</span></span>|<span data-ttu-id="f820a-297">Int32</span><span class="sxs-lookup"><span data-stu-id="f820a-297">Int32</span></span>|<span data-ttu-id="f820a-298">指定可以从组织数据和帐户中剪切或复制到任何应用程序的字符数。</span><span class="sxs-lookup"><span data-stu-id="f820a-298">Specify the number of characters that may be cut or copied from Org data and accounts to any application.</span></span> <span data-ttu-id="f820a-299">此设置将覆盖 AllowedOutboundClipboardSharingLevel 限制。</span><span class="sxs-lookup"><span data-stu-id="f820a-299">This setting overrides the AllowedOutboundClipboardSharingLevel restriction.</span></span> <span data-ttu-id="f820a-300">默认值为 "0" 表示不允许异常。</span><span class="sxs-lookup"><span data-stu-id="f820a-300">Default value of '0' means no exception is allowed.</span></span> <span data-ttu-id="f820a-301">继承自 [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-301">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-302">notificationRestriction</span><span class="sxs-lookup"><span data-stu-id="f820a-302">notificationRestriction</span></span>|[<span data-ttu-id="f820a-303">managedAppNotificationRestriction</span><span class="sxs-lookup"><span data-stu-id="f820a-303">managedAppNotificationRestriction</span></span>](../resources/intune-mam-managedappnotificationrestriction.md)|<span data-ttu-id="f820a-304">指定从 [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)继承的应用程序通知限制。</span><span class="sxs-lookup"><span data-stu-id="f820a-304">Specify app notification restriction Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="f820a-305">可取值为：`allow`、`blockOrganizationalData`、`block`。</span><span class="sxs-lookup"><span data-stu-id="f820a-305">Possible values are: `allow`, `blockOrganizationalData`, `block`.</span></span>|
|<span data-ttu-id="f820a-306">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f820a-306">isAssigned</span></span>|<span data-ttu-id="f820a-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-307">Boolean</span></span>|<span data-ttu-id="f820a-308">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="f820a-308">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="f820a-309">继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="f820a-309">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="f820a-310">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="f820a-310">targetedAppManagementLevels</span></span>|[<span data-ttu-id="f820a-311">appManagementLevel</span><span class="sxs-lookup"><span data-stu-id="f820a-311">appManagementLevel</span></span>](../resources/intune-mam-appmanagementlevel.md)|<span data-ttu-id="f820a-312">此策略继承自 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)的预期应用管理级别。</span><span class="sxs-lookup"><span data-stu-id="f820a-312">The intended app management levels for this policy Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span></span> <span data-ttu-id="f820a-313">可取值为：`unspecified`、`unmanaged`、`mdm`、`androidEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="f820a-313">Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.</span></span>|
|<span data-ttu-id="f820a-314">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="f820a-314">appDataEncryptionType</span></span>|[<span data-ttu-id="f820a-315">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="f820a-315">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="f820a-316">应该用于托管应用中的数据的加密类型。</span><span class="sxs-lookup"><span data-stu-id="f820a-316">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="f820a-317">可取值为：`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked`。</span><span class="sxs-lookup"><span data-stu-id="f820a-317">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="f820a-318">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-318">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="f820a-319">String</span><span class="sxs-lookup"><span data-stu-id="f820a-319">String</span></span>|<span data-ttu-id="f820a-320">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-320">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="f820a-321">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="f820a-321">deployedAppCount</span></span>|<span data-ttu-id="f820a-322">Int32</span><span class="sxs-lookup"><span data-stu-id="f820a-322">Int32</span></span>|<span data-ttu-id="f820a-323">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="f820a-323">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="f820a-324">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="f820a-324">faceIdBlocked</span></span>|<span data-ttu-id="f820a-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-325">Boolean</span></span>|<span data-ttu-id="f820a-326">指示如果 PinRequired 设置为 True，是否允许使用 FaceID 代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="f820a-326">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="f820a-327">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="f820a-327">exemptedAppProtocols</span></span>|<span data-ttu-id="f820a-328">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f820a-328">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f820a-329">此列表中的应用程序将从策略中排除，并将能够从托管应用接收数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-329">Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span>|
|<span data-ttu-id="f820a-330">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f820a-330">minimumWipeSdkVersion</span></span>|<span data-ttu-id="f820a-331">String</span><span class="sxs-lookup"><span data-stu-id="f820a-331">String</span></span>|<span data-ttu-id="f820a-332">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-332">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="f820a-333">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="f820a-333">allowedIosDeviceModels</span></span>|<span data-ttu-id="f820a-334">String</span><span class="sxs-lookup"><span data-stu-id="f820a-334">String</span></span>|<span data-ttu-id="f820a-335">允许托管应用使用的设备模型的以分号分隔的列表（以字符串形式）。</span><span class="sxs-lookup"><span data-stu-id="f820a-335">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span>|
|<span data-ttu-id="f820a-336">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="f820a-336">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="f820a-337">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="f820a-337">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="f820a-338">定义托管应用程序行为，如果不允许指定的设备模型，则要么阻止，也可以擦除。</span><span class="sxs-lookup"><span data-stu-id="f820a-338">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="f820a-339">可取值为：`block`、`wipe`、`warn`。</span><span class="sxs-lookup"><span data-stu-id="f820a-339">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="f820a-340">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="f820a-340">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="f820a-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-341">Boolean</span></span>|<span data-ttu-id="f820a-342">定义是否支持从受管理的应用程序到所选的可共享位置的打开入点操作。</span><span class="sxs-lookup"><span data-stu-id="f820a-342">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="f820a-343">此设置仅适用于将 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 和 DisableProtectionOfManagedOutboundOpenInData 设置为 False 的情况。</span><span class="sxs-lookup"><span data-stu-id="f820a-343">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span>|
|<span data-ttu-id="f820a-344">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="f820a-344">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="f820a-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-345">Boolean</span></span>|<span data-ttu-id="f820a-346">禁用通过 IOS OpenIn 选项传输到其他应用程序的数据保护。</span><span class="sxs-lookup"><span data-stu-id="f820a-346">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="f820a-347">仅当 AllowedOutboundDataTransferDestinations 设置为 ManagedApps 时，此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="f820a-347">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span>|
|<span data-ttu-id="f820a-348">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f820a-348">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="f820a-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="f820a-349">Boolean</span></span>|<span data-ttu-id="f820a-350">保护来自未知源的传入数据。</span><span class="sxs-lookup"><span data-stu-id="f820a-350">Protect incoming data from unknown source.</span></span> <span data-ttu-id="f820a-351">仅当 AllowedInboundDataTransferSources 设置为 AllApps 时，此设置才允许为 True。</span><span class="sxs-lookup"><span data-stu-id="f820a-351">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span>|
|<span data-ttu-id="f820a-352">customBrowserProtocol</span><span class="sxs-lookup"><span data-stu-id="f820a-352">customBrowserProtocol</span></span>|<span data-ttu-id="f820a-353">String</span><span class="sxs-lookup"><span data-stu-id="f820a-353">String</span></span>|<span data-ttu-id="f820a-354">用于在 iOS 上打开 weblink 的自定义浏览器协议。</span><span class="sxs-lookup"><span data-stu-id="f820a-354">A custom browser protocol to open weblink on iOS.</span></span>|



## <a name="response"></a><span data-ttu-id="f820a-355">响应</span><span class="sxs-lookup"><span data-stu-id="f820a-355">Response</span></span>
<span data-ttu-id="f820a-356">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f820a-356">If successful, this method returns a `201 Created` response code and a [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f820a-357">示例</span><span class="sxs-lookup"><span data-stu-id="f820a-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="f820a-358">请求</span><span class="sxs-lookup"><span data-stu-id="f820a-358">Request</span></span>
<span data-ttu-id="f820a-359">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f820a-359">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
Content-type: application/json
Content-length: 2623

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```

### <a name="response"></a><span data-ttu-id="f820a-360">响应</span><span class="sxs-lookup"><span data-stu-id="f820a-360">Response</span></span>
<span data-ttu-id="f820a-p147">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f820a-p147">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2795

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```









