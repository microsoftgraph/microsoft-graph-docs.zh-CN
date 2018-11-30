---
title: 创建 windows81GeneralConfiguration
description: 创建新的 windows81GeneralConfiguration 对象。
ms.openlocfilehash: 800b84563d4e092b39a5de66be91b635d55b9983
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044745"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="0b7d0-103">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b7d0-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="0b7d0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b7d0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b7d0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b7d0-107">创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b7d0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b7d0-108">Prerequisites</span></span>
<span data-ttu-id="0b7d0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0b7d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b7d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b7d0-111">Permission type</span></span>|<span data-ttu-id="0b7d0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b7d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b7d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b7d0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b7d0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b7d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b7d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-116">Not supported.</span></span>|
|<span data-ttu-id="0b7d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b7d0-117">Application</span></span>|<span data-ttu-id="0b7d0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b7d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b7d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0b7d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b7d0-120">Request headers</span></span>
|<span data-ttu-id="0b7d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="0b7d0-121">Header</span></span>|<span data-ttu-id="0b7d0-122">值</span><span class="sxs-lookup"><span data-stu-id="0b7d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b7d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b7d0-123">Authorization</span></span>|<span data-ttu-id="0b7d0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b7d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b7d0-125">Accept</span></span>|<span data-ttu-id="0b7d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b7d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b7d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b7d0-127">Request body</span></span>
<span data-ttu-id="0b7d0-128">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="0b7d0-129">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="0b7d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="0b7d0-130">Property</span></span>|<span data-ttu-id="0b7d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="0b7d0-131">Type</span></span>|<span data-ttu-id="0b7d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b7d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b7d0-133">id</span><span class="sxs-lookup"><span data-stu-id="0b7d0-133">id</span></span>|<span data-ttu-id="0b7d0-134">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-134">String</span></span>|<span data-ttu-id="0b7d0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-135">Key of the entity.</span></span> <span data-ttu-id="0b7d0-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b7d0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0b7d0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b7d0-138">DateTimeOffset</span></span>|<span data-ttu-id="0b7d0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0b7d0-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b7d0-141">roleScopeTagIds</span></span>|<span data-ttu-id="0b7d0-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0b7d0-142">String collection</span></span>|<span data-ttu-id="0b7d0-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b7d0-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b7d0-145">supportsScopeTags</span></span>|<span data-ttu-id="0b7d0-146">布尔</span><span class="sxs-lookup"><span data-stu-id="0b7d0-146">Boolean</span></span>|<span data-ttu-id="0b7d0-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b7d0-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b7d0-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b7d0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-150">This property is read-only.</span></span> <span data-ttu-id="0b7d0-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b7d0-152">createdDateTime</span></span>|<span data-ttu-id="0b7d0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b7d0-153">DateTimeOffset</span></span>|<span data-ttu-id="0b7d0-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-154">DateTime the object was created.</span></span> <span data-ttu-id="0b7d0-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-156">description</span><span class="sxs-lookup"><span data-stu-id="0b7d0-156">description</span></span>|<span data-ttu-id="0b7d0-157">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-157">String</span></span>|<span data-ttu-id="0b7d0-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b7d0-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0b7d0-160">displayName</span></span>|<span data-ttu-id="0b7d0-161">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-161">String</span></span>|<span data-ttu-id="0b7d0-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b7d0-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-164">version</span><span class="sxs-lookup"><span data-stu-id="0b7d0-164">version</span></span>|<span data-ttu-id="0b7d0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-165">Int32</span></span>|<span data-ttu-id="0b7d0-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-166">Version of the device configuration.</span></span> <span data-ttu-id="0b7d0-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b7d0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b7d0-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="0b7d0-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="0b7d0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-169">Boolean</span></span>|<span data-ttu-id="0b7d0-170">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="0b7d0-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="0b7d0-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="0b7d0-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-172">Boolean</span></span>|<span data-ttu-id="0b7d0-173">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="0b7d0-174">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-174">This property is read-only.</span></span>|
|<span data-ttu-id="0b7d0-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="0b7d0-175">browserBlockAutofill</span></span>|<span data-ttu-id="0b7d0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-176">Boolean</span></span>|<span data-ttu-id="0b7d0-177">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="0b7d0-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="0b7d0-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="0b7d0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-179">Boolean</span></span>|<span data-ttu-id="0b7d0-180">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="0b7d0-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="0b7d0-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="0b7d0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-182">Boolean</span></span>|<span data-ttu-id="0b7d0-183">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="0b7d0-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="0b7d0-184">browserBlockJavaScript</span></span>|<span data-ttu-id="0b7d0-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-185">Boolean</span></span>|<span data-ttu-id="0b7d0-186">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="0b7d0-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="0b7d0-187">browserBlockPlugins</span></span>|<span data-ttu-id="0b7d0-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-188">Boolean</span></span>|<span data-ttu-id="0b7d0-189">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="0b7d0-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="0b7d0-190">browserBlockPopups</span></span>|<span data-ttu-id="0b7d0-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-191">Boolean</span></span>|<span data-ttu-id="0b7d0-192">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="0b7d0-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="0b7d0-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="0b7d0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-194">Boolean</span></span>|<span data-ttu-id="0b7d0-195">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="0b7d0-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="0b7d0-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="0b7d0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-197">Boolean</span></span>|<span data-ttu-id="0b7d0-198">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="0b7d0-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="0b7d0-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="0b7d0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-200">Boolean</span></span>|<span data-ttu-id="0b7d0-201">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="0b7d0-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="0b7d0-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="0b7d0-203">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-203">String</span></span>|<span data-ttu-id="0b7d0-204">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-204">The enterprise mode site list location.</span></span> <span data-ttu-id="0b7d0-205">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="0b7d0-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="0b7d0-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="0b7d0-208">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-208">The internet security level.</span></span> <span data-ttu-id="0b7d0-209">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0b7d0-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="0b7d0-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="0b7d0-212">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-212">The Intranet security level.</span></span> <span data-ttu-id="0b7d0-213">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0b7d0-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="0b7d0-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="0b7d0-215">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-215">String</span></span>|<span data-ttu-id="0b7d0-216">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-216">The logging report location.</span></span>|
|<span data-ttu-id="0b7d0-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="0b7d0-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="0b7d0-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-218">Boolean</span></span>|<span data-ttu-id="0b7d0-219">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="0b7d0-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="0b7d0-220">browserRequireFirewall</span></span>|<span data-ttu-id="0b7d0-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-221">Boolean</span></span>|<span data-ttu-id="0b7d0-222">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="0b7d0-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="0b7d0-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="0b7d0-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-224">Boolean</span></span>|<span data-ttu-id="0b7d0-225">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="0b7d0-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="0b7d0-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b7d0-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="0b7d0-228">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-228">The trusted sites security level.</span></span> <span data-ttu-id="0b7d0-229">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="0b7d0-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="0b7d0-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="0b7d0-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-231">Boolean</span></span>|<span data-ttu-id="0b7d0-232">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="0b7d0-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="0b7d0-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="0b7d0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-234">Boolean</span></span>|<span data-ttu-id="0b7d0-235">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="0b7d0-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="0b7d0-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="0b7d0-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-237">Boolean</span></span>|<span data-ttu-id="0b7d0-238">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="0b7d0-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0b7d0-239">passwordExpirationDays</span></span>|<span data-ttu-id="0b7d0-240">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-240">Int32</span></span>|<span data-ttu-id="0b7d0-241">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-241">Password expiration in days.</span></span>|
|<span data-ttu-id="0b7d0-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0b7d0-242">passwordMinimumLength</span></span>|<span data-ttu-id="0b7d0-243">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-243">Int32</span></span>|<span data-ttu-id="0b7d0-244">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-244">The minimum password length.</span></span>|
|<span data-ttu-id="0b7d0-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0b7d0-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0b7d0-246">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-246">Int32</span></span>|<span data-ttu-id="0b7d0-247">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0b7d0-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0b7d0-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0b7d0-249">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-249">Int32</span></span>|<span data-ttu-id="0b7d0-250">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0b7d0-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0b7d0-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0b7d0-252">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-252">Int32</span></span>|<span data-ttu-id="0b7d0-253">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0b7d0-254">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="0b7d0-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0b7d0-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0b7d0-255">passwordRequiredType</span></span>|[<span data-ttu-id="0b7d0-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0b7d0-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0b7d0-257">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-257">The required password type.</span></span> <span data-ttu-id="0b7d0-258">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0b7d0-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0b7d0-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0b7d0-260">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7d0-260">Int32</span></span>|<span data-ttu-id="0b7d0-261">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="0b7d0-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="0b7d0-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="0b7d0-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-263">Boolean</span></span>|<span data-ttu-id="0b7d0-264">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="0b7d0-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="0b7d0-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="0b7d0-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="0b7d0-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="0b7d0-267">最小值更新分类自动安装。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="0b7d0-268">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="0b7d0-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="0b7d0-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="0b7d0-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="0b7d0-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="0b7d0-271">最小值更新分类自动安装。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="0b7d0-272">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="0b7d0-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="0b7d0-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="0b7d0-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b7d0-274">Boolean</span></span>|<span data-ttu-id="0b7d0-275">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="0b7d0-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="0b7d0-276">userAccountControlSettings</span></span>|[<span data-ttu-id="0b7d0-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="0b7d0-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="0b7d0-278">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-278">The user account control settings.</span></span> <span data-ttu-id="0b7d0-279">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="0b7d0-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="0b7d0-280">workFoldersUrl</span></span>|<span data-ttu-id="0b7d0-281">String</span><span class="sxs-lookup"><span data-stu-id="0b7d0-281">String</span></span>|<span data-ttu-id="0b7d0-282">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="0b7d0-283">响应</span><span class="sxs-lookup"><span data-stu-id="0b7d0-283">Response</span></span>
<span data-ttu-id="0b7d0-284">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b7d0-285">示例</span><span class="sxs-lookup"><span data-stu-id="0b7d0-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b7d0-286">请求</span><span class="sxs-lookup"><span data-stu-id="0b7d0-286">Request</span></span>
<span data-ttu-id="0b7d0-287">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="0b7d0-288">响应</span><span class="sxs-lookup"><span data-stu-id="0b7d0-288">Response</span></span>
<span data-ttu-id="0b7d0-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b7d0-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





